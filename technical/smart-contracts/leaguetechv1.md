---
description: League Tech Core
---

# LeagueTechV1

LeagueTechV1

## Roles

Listed below are the roles on LeagueTechV1 and their responsibilities.

<table><thead><tr><th width="278">Role</th><th width="210.56373937677054">Responsibility</th><th>Methods Accessible</th></tr></thead><tbody><tr><td><code>owner</code></td><td><p>Can:</p><ul><li>Pause/unpause the contract</li><li>Set protocol addresses</li><li>Set fee percentages</li><li>Set subscription parameters</li><li>Withdraw lost funds </li></ul></td><td><ul><li>setPaused</li><li>setFeeDestination</li><li>setProtocolDev</li><li>setProtocolFeePercent</li><li>setSubjectFeePercent</li><li>setReferralFeePercent</li><li>setSubscriptionPrice</li><li>setSubscriptionDuration</li><li>withdrawFunds</li></ul></td></tr><tr><td><code>protocolDev</code></td><td><p>Can:</p><ul><li>Pause/unpause the contract</li></ul></td><td><ul><li>setPaused</li></ul></td></tr></tbody></table>

## View Methods

### getPrice

`getPrice(supply, amount)`

Gets the total price of an `amount` of shares with a specified `supply`

Call Parameters

| Name   | Type    | Description                         |
| ------ | ------- | ----------------------------------- |
| supply | uint256 | The current supply of shares        |
| amount | uint256 | The amount of shares to buy or sell |

Return Value

| Type    | Description                                  |
| ------- | -------------------------------------------- |
| uint256 | The price for the amount of shares specified |

### getMyShares

`getMyShares(sharesSubject)`

Gets the total amount of shares that the caller owns of `sharesSubject`

Call Parameters

| Name          | Type    | Description                                      |
| ------------- | ------- | ------------------------------------------------ |
| sharesSubject | address | Address of the user whose share balance to check |

Return Value

| Type    | Description                                 |
| ------- | ------------------------------------------- |
| uint256 | Total amount of shares that the caller owns |

### getSharesSupply

`getSharesSupply(sharesSubject)`

Gets the share supply

Call Parameters

| Name          | Type    | Description                                     |
| ------------- | ------- | ----------------------------------------------- |
| sharesSubject | address | Address of the user whose share supply to check |

Return Value

| Type    | Description                                      |
| ------- | ------------------------------------------------ |
| uint256 | Total supply of the shares of the specified user |

### getBuyPrice

`getBuyPrice(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name          | Type    | Description |
| ------------- | ------- | ----------- |
| sharesSubject | address |             |
| amount        | uint256 |             |

Return Value

| Type    | Description |
| ------- | ----------- |
| uint256 |             |

### getSellPrice

`getSellPrice(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name          | Type    |   |
| ------------- | ------- | - |
| sharesSubject | address |   |
| amount        | uint256 |   |

Return Value

| Type    | Description |
| ------- | ----------- |
| uint256 |             |

### getBuyPriceAfterFee

`getBuyPriceAfterFee(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name          | Type    | Description |
| ------------- | ------- | ----------- |
| sharesSubject | address |             |
| amount        | uint256 |             |

Return Value

| Type    | Description |
| ------- | ----------- |
| uint256 |             |

### getSellPriceAfterFee

`getSellPriceAfterFee(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name | Type |
| ---- | ---- |
|      |      |
|      |      |
|      |      |

Return Value

| Type    | Description |
| ------- | ----------- |
| uint256 |             |

### getSubscriptionPriceAfterFee

`getSubscriptionPriceAfterFee()`

Gets the share supply

Return Value

| Type    | Description |
| ------- | ----------- |
| uint256 |             |

## Write Methods

### buySharesWithReferrer

`buySharesWithReferrer(sharesSubject, amount, referrer)`

Gets the share supply

Call Parameters

| Name | Type |
| ---- | ---- |
|      |      |
|      |      |
|      |      |

### buyShares

`buyShares(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name | Type |
| ---- | ---- |
|      |      |
|      |      |
|      |      |

### sellShares

`sellShares(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name | Type |
| ---- | ---- |
|      |      |
|      |      |
|      |      |

### enableSubscriptions

`enableSubscriptions()`

Gets the share supply

### disableSubscriptions

`disableSubscriptions()`

Gets the share supply

### buySubscriptionWithReferrer

`buySubscriptionWithReferrer(subscriptionsSubject, referrer)`

Gets the share supply

Call Parameters

| Name | Type |
| ---- | ---- |
|      |      |
|      |      |
|      |      |

### buySubscription

`buySubscription(subscriptionsSubject)`

Gets the share supply

Call Parameters

| Name | Type |
| ---- | ---- |
|      |      |
|      |      |
|      |      |
