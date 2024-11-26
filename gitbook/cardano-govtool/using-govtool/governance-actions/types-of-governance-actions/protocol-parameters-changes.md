---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Protocol Parameters changes

### Any change to **one or more** updatable protocol parameters, excluding changes to major protocol versions ('hard forks')

There are four types of protocol parameter changes, however, changes are not restricted to any groupp. In case where a Governance Action carries updates for multiple parameters from different groups, the maximum threshold of all the groups involved will apply to any given such governance action.

The four types of parameter changes:

The **network group** consists of:

* maximum block body size (`maxBlockBodySize`)
* maximum transaction size (`maxTxSize`)
* maximum block header size (`maxBlockHeaderSize`)
* maximum size of a serialised asset value (`maxValueSize`)
* maximum script execution units in a single transaction (`maxTxExecutionUnits`)
* maximum script execution units in a single block (`maxBlockExecutionUnits`)
* maximum number of collateral inputs (`maxCollateralInputs`)

Ratification threshold for the **network group:**

<table><thead><tr><th width="258">Constitutional Committee</th><th width="210">DReps</th><th>SPOs</th></tr></thead><tbody><tr><td>Pass</td><td>60%</td><td>51%</td></tr></tbody></table>

The **ecomomic group** consists of:

* minimum fee coefficient (`txFeePerByte`)
* minimum fee constant (`txFeeFixed`)
* delegation key Lovelace deposit (`stakeAddressDeposit`)
* pool registration Lovelace deposit (`stakePoolDeposit`)
* monetary expansion (`monetaryExpansion`)
* treasury expansion (`treasuryCut`)
* minimum fixed rewards cut for pools (`minPoolCost`)
* minimum Lovelace deposit per byte of serialized UTxO (`utxoCostPerByte`)
* prices of Plutus execution units (`executionUnitPrices`)

Ratification threshold for the **ecomomic group:**

<table><thead><tr><th width="258">Constitutional Committee</th><th width="210">DReps</th><th>SPOs</th></tr></thead><tbody><tr><td>Pass</td><td>67%</td><td>Doesn't vote</td></tr></tbody></table>

The **technical group** consists of:

* pool pledge influence (`poolPledgeInfluence`)
* pool retirement maximum epoch (`poolRetireMaxEpoch`)
* desired number of pools (`stakePoolTargetNum`)
* Plutus execution cost models (`costModels`)
* proportion of collateral needed for scripts (`collateralPercentage`)

Ratification threshold for the **technical group:**

<table><thead><tr><th width="258">Constitutional Committee</th><th width="210">DReps</th><th>SPOs</th></tr></thead><tbody><tr><td>Pass</td><td>67%</td><td>Doesn't vote</td></tr></tbody></table>

The **governance group** consists of all the new protocol parameters that are introduced in this CIP:

* governance voting thresholds ( P 1 , P 2 a , P 2 b , P 3 , P 4 , P 5 a , P 5 b , P 5 c , P 5 d , P 6 , Q 1 , Q 2 a , Q 2 b , Q 4 , Q 5 )
* governance action maximum lifetime in epochs (`govActionLifetime`)
* governance action deposit (`govActionDeposit`)
* DRep deposit amount (`dRepDeposit`)
* DRep activity period in epochs (`dRepActivity`)
* minimal constitutional committee size (`committeeMinSize`)
* maximum term length (in epochs) for the constitutional committee members (`committeeMaxTermLength`)

Ratification threshold for the **governance group:**

<table><thead><tr><th width="258">Constitutional Committee</th><th width="210">DReps</th><th>SPOs</th></tr></thead><tbody><tr><td>Pass</td><td>67%</td><td>Doesn't vote</td></tr></tbody></table>

These values could be changed via a new Government Action. To see the current values at any time, you can view [https://cardanoscan.io/protocolparams](https://cardanoscan.io/protocolparams).
