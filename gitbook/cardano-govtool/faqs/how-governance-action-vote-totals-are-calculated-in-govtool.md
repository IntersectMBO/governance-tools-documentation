# How Governance Action Vote Totals are Calculated in Govtool

[See GovTool's SQL query](https://github.com/IntersectMBO/govtool/blob/develop/govtool/backend/sql/list-proposals.sql) run on DB-Sync.

## DRep Vote Totals

* We are taking the very latest vote from DReps for that governance action, filtering out votes from DReps who have retired\*.
* There are 3 types of votes - `yes`, `no`, `abstain`
* Then, GovTool fetchs the voting power of such DRep and sum all the yes votes voting power, no votes voting power, and abstain (this voting power comes from the [`drep_distr` table of DB-Sync](https://github.com/IntersectMBO/cardano-db-sync/blob/master/doc/schema.md#drep_distr))
* Note that the [`drep_distr`](https://github.com/IntersectMBO/cardano-db-sync/blob/master/doc/schema.md#drep_distr) is only updated once per epoch.
* To the `abstain` vote total we add the voting power of "DRep always abstain" (predefined voting option).
* For the "DRep always no confidence" (predefined voting option), this voting power total is added to the `no` total for all types of governance action except no confidence actions, where this is added to the `yes` total. \*\*
* `NOT VOTED` - is the sum of active DRep voting power minus voting power that has been counted to votes

\*Filtering out votes from retired DReps was spotted during authoring, this will be fixed, unlikely to be affecting current totals.

\*\*The logic applied in GovTool for this is slightly off, unlikely to be affecting current totals, fix to be deployed shortly.

### Example

* So we have some DRep John Doe, who voted `yes` on X governance action
* John Doe has 100k Voting power coming from his own stake and all delegators (we are taking that value directly from db-sync (no calculations on GovTool side))
* We have another DRep - Andre, who has 200k Voting power!
* Andre also likes the governance action and votes `yes`
* As a result - we display the sum of their voting powers, so it would be 300k for `yes` votes
* Important note - John Doe and Andre can change their votes

## SPO Vote Totals

* For SPOs logic is completely the same as the DReps one - the difference is that we are taking the voting power from a different table - dedicated to SPOs (`pool_stat`)
