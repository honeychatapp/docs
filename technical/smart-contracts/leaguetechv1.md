---
description: League Tech Core
---

# LeagueTechV1

LeagueTechV1

## Roles

Listed below are the roles on LeagueTechV1 and their responsibilities.

<table><thead><tr><th width="278">Role</th><th width="210.56373937677054">Responsibilities</th><th>Methods Accessible</th></tr></thead><tbody><tr><td><code>owner</code></td><td><ul><li>Pause/unpause the contract</li><li>Set protocol addresses</li><li>Set fee percentages</li><li>Set subscription parameters</li><li>Withdraw lost funds </li></ul></td><td><ul><li>setPaused</li><li>setFeeDestination</li><li>setProtocolDev</li><li>setProtocolFeePercent</li><li>setSubjectFeePercent</li><li>setReferralFeePercent</li><li>setSubscriptionPrice</li><li>setSubscriptionDuration</li><li>withdrawFunds</li></ul></td></tr><tr><td><code>protocolDev</code></td><td><ul><li>Pause/unpause the contract</li></ul></td><td><ul><li>setPaused</li></ul></td></tr></tbody></table>

## View Methods

### getPrice

`getPrice(supply, amount)`

Gets the total price of an `amount` of shares with a specified `supply`.

Call Parameters

| Name   | Type    | Description                     |
| ------ | ------- | ------------------------------- |
| supply | uint256 | Current supply of shares        |
| amount | uint256 | Amount of shares to buy or sell |

Return Value

| Type    | Description                              |
| ------- | ---------------------------------------- |
| uint256 | Price for the amount of shares specified |

### getMyShares

`getMyShares(sharesSubject)`

Gets the total amount of shares that the caller owns of `sharesSubject`.

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

| Name          | Type    | Description                                        |
| ------------- | ------- | -------------------------------------------------- |
| sharesSubject | address | Address of the user whose share buy price to check |
| amount        | uint256 | Amount of shares to buy                            |

Return Value

| Type    | Description                                  |
| ------- | -------------------------------------------- |
| uint256 | Buy price for the amount of shares specified |

### getSellPrice

`getSellPrice(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name          | Type    | Description                                         |
| ------------- | ------- | --------------------------------------------------- |
| sharesSubject | address | Address of the user whose share sell price to check |
| amount        | uint256 | Amount of shares to sell                            |

Return Value

| Type    | Description                                   |
| ------- | --------------------------------------------- |
| uint256 | Sell price for the amount of shares specified |

### getBuyPriceAfterFee

`getBuyPriceAfterFee(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name          | Type    | Description                                        |
| ------------- | ------- | -------------------------------------------------- |
| sharesSubject | address | Address of the user whose share buy price to check |
| amount        | uint256 | Amount of shares to buy                            |

Return Value

| Type    | Description                                                         |
| ------- | ------------------------------------------------------------------- |
| uint256 | Total buy price for the amount of shares specified (including fees) |

### getSellPriceAfterFee

`getSellPriceAfterFee(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name          | Type    | Description                                         |
| ------------- | ------- | --------------------------------------------------- |
| sharesSubject | address | Address of the user whose share sell price to check |
| amount        | uint256 | Amount of shares to sell                            |

Return Value

| Type    | Description                                                          |
| ------- | -------------------------------------------------------------------- |
| uint256 | Total sell price for the amount of shares specified (including fees) |

### getSubscriptionPriceAfterFee

`getSubscriptionPriceAfterFee()`

Gets the share supply

Return Value

| Type    | Description                                                      |
| ------- | ---------------------------------------------------------------- |
| uint256 | Total subscription price to subscribe to a user (including fees) |

## Write Methods

### buySharesWithReferrer

`buySharesWithReferrer(sharesSubject, amount, referrer)`

Gets the share supply

Call Parameters

| Name          | Type    | Description                                 |
| ------------- | ------- | ------------------------------------------- |
| sharesSubject | address | Address of the user whose shares to buy     |
| amount        | uint256 | Amount of shares to buy                     |
| referrer      | address | Address of the user who referred the caller |

### buyShares

`buyShares(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name          | Type    | Description                             |
| ------------- | ------- | --------------------------------------- |
| sharesSubject | address | Address of the user whose shares to buy |
| amount        | uint256 | Amount of shares to buy                 |

### sellShares

`sellShares(sharesSubject, amount)`

Gets the share supply

Call Parameters

| Name          | Type    | Description                              |
| ------------- | ------- | ---------------------------------------- |
| sharesSubject | address | Address of the user whose shares to sell |
| amount        | uint256 | Amount of shares to sell                 |

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

| Name                 | Type    | Description                                 |
| -------------------- | ------- | ------------------------------------------- |
| subscriptionsSubject | address | Address of the user to subscribe to         |
| referrer             | address | Address of the user who referred the caller |

### buySubscription

`buySubscription(subscriptionsSubject)`

Gets the share supply

Call Parameters

| Name                 | Type    |                                     |
| -------------------- | ------- | ----------------------------------- |
| subscriptionsSubject | address | Address of the user to subscribe to |
