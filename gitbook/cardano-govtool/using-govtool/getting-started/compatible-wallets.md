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

# Compatible Wallets

{% hint style="warning" %}
GovTool requires Cardano wallets to have upgraded to CIP-95 to be able to connect and share governance data, thus some existing Cardano wallets might not work.
{% endhint %}

### Mainnet Compatible Wallets (`gov.tools`)

Wallets which are working with GovTool on Mainnet.

| Wallet                  | Download link                                                                                                 | Status                                                                                                                                                                                                   |
| ----------------------- | ------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Eternl**              | [visit site](https://chromewebstore.google.com/detail/eternl/kmhcihpebfmpgmihbkipmjlmmioameka)                | <mark style="color:green;background-color:green;">Online</mark>                                                                                                                                          |
| **Lace**                | [visit site](https://chromewebstore.google.com/detail/lace/gafhhkghbfjjkeiendhlofajokpaflmk)                  | <mark style="color:green;background-color:green;">Online</mark>                                                                                                                                          |
| **NuFi**                | [visit site](https://chromewebstore.google.com/detail/nufi/gpnihlnnodeiiaakbikldcihojploeca)                  | <mark style="color:green;background-color:green;">Online</mark>                                                                                                                                          |
| **Vespr**               | [visit site](https://vespr.xyz/)                                                                              | <mark style="color:green;background-color:green;">Online</mark>                                                                                                                                          |
| **Typhon**              | [visit site](https://chromewebstore.google.com/detail/typhon-wallet/kfdniefadaanbjodldohaedphafoffoh)         | <mark style="color:green;background-color:green;">Online</mark>                                                                                                                                          |
| **Yoroi**               | [visit site](https://chromewebstore.google.com/detail/yoroi/ffnbelfdoeiohenkjibnmadjiehjhajb)                 | <mark style="color:green;background-color:green;">Online</mark>                                                                                                                                          |
| **Ledger (hardware)**   | [visit site](https://www.ledger.com/)                                                                         | <mark style="color:green;background-color:green;">Compatible</mark> <mark style="color:green;background-color:green;"></mark><mark style="color:green;background-color:green;">**\*(see note)**</mark>   |
| **Trezor (hardware)**   | [visit site](https://trezor.io/)                                                                              | <mark style="color:green;background-color:green;">Compatible</mark> <mark style="color:green;background-color:green;"></mark><mark style="color:green;background-color:green;">**\*\*(see note)**</mark> |
| **Keystone (hardware)** | [visit site](https://keyst.one/)                                                                              | <mark style="color:green;background-color:green;">Compatible</mark>                                                                                                                                      |
| **Flint**               | N/A (see [announcement](https://x.com/FlintWallet/status/1828184961960308832?t=0eIBBMnAY5feMTOlojFlSg\&s=19)) | <mark style="color:red;background-color:red;">Will not progress</mark>                                                                                                                                   |

\*Ledger devices support all governance activities via GovTool, except submission of governance actions.

\*\*Trezor devices are limited with their governance functionality, only supporting DRep vote delegation via GovTool.

### Preview Network Compatible Wallets (`preview.gov.tools`)

Wallets which are working with GovTool on Preview testnet.

| Wallet     | Download link                                                                                  | Status                                                           |
| ---------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| **Eternl** | [visit site](https://chromewebstore.google.com/detail/eternl/kmhcihpebfmpgmihbkipmjlmmioameka) | <mark style="color:green;background-color:green;">Online</mark>  |
| **Lace**   | [visit site](https://chromewebstore.google.com/detail/lace/gafhhkghbfjjkeiendhlofajokpaflmk)   | <mark style="color:green;background-color:green;">Online</mark>  |
| **Vespr**  | [visit site](https://vespr.xyz/)                                                               | <mark style="color:green;background-color:green;">Online</mark>  |

### SanchoNet Compatible Wallets (`sanchogov.tools`)

Wallets which are working with GovTool  on SanchoNet.

| Wallet                       | Download link                                                                                                  | Status                                                          |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| **Eternl**                   | [visit site](https://chromewebstore.google.com/detail/eternl/kmhcihpebfmpgmihbkipmjlmmioameka)                 | <mark style="color:green;background-color:green;">Online</mark> |
| **Nufi** _SanchoNet Version_ | [download here](https://assets.nu.fi/extension/sanchonet/nufi-cwe-sanchonet-latest.zip)                        | <mark style="color:green;background-color:green;">Online</mark> |
| **Yoroi (Nightly)**          | [visit site](https://chrome.google.com/webstore/detail/yoroi-nightly/poonlenmfdfbjfeeballhiibknlknepo/related) | <mark style="color:green;background-color:green;">Online</mark> |

### Wallets with in-wallet governance functionality

Some wallets have chosen to add the governance functionality in-wallet. This means that some governance flows are supported without leaving the connecting to GovTool or leaving the wallet.

| Wallet               | Download link                                                                                         | Description                                               |
| -------------------- | ----------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| **Eternl**           | [visit site](https://chromewebstore.google.com/detail/eternl/kmhcihpebfmpgmihbkipmjlmmioameka)        | Supports DRep delegation in wallet.                       |
| **Typhon**           | [visit site](https://chromewebstore.google.com/detail/typhon-wallet/kfdniefadaanbjodldohaedphafoffoh) | Supports DRep delegation in wallet, with a DRep explorer. |
| **Yoroi**            | [visit site](https://chromewebstore.google.com/detail/yoroi/ffnbelfdoeiohenkjibnmadjiehjhajb)         | Supports DRep delegation in wallet.                       |
| Daedalus (full node) | [visit site](https://daedaluswallet.io/)                                                              | Supports DRep delegation in wallet.                       |
