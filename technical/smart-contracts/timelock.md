---
description: Timelock Upgrade Controller
---

# Timelock

The `Timelock` is an implementation of the [Open Zeppelin TimelockController](https://docs.openzeppelin.com/contracts/5.x/api/governance#TimelockController). This contract is the `owner` of the `ProxyAdmin`. It adds an additional layer of safety when upgrading, by requiring at least 1 day, represented in the `Timelock` as `86400` seconds, to pass before an upgrade transaction can be executed.



Deployment Parameters

| Parameter | Value                                            | Description                                                                                                         |
| --------- | ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------- |
| minDelay  | 1 day                                            | Minimum seconds that must pass before a proposed transaction can be executed.                                       |
| proposers | <ul><li>Team Multisig</li><li>Deployer</li></ul> | Addresses allowed to propose transactions. Only the Team Multisig and Deployer can propose transactions.            |
| executors | <ul><li>Team Multisig</li></ul>                  | Addresses allowed to execute transactions after the `delayPeriod`. Only the Team Multisig can execute transactions. |
| admin     | <ul><li>Zero Address</li></ul>                   | Addresses allowed to add `proposers` and `executors`. No other additions can be made.                               |
