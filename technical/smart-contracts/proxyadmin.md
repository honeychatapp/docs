---
description: Smart Contract Upgrade Admin
---

# ProxyAdmin

For future development and flexibility, League Tech uses the [Open Zeppelin Upgrades](https://docs.openzeppelin.com/upgrades) suite to deploy and manage upgradeable Smart Contracts, or Proxies. The `LeagueTechV1` Contract is a `TransparentUpgradeableProxy` that complies with EIP-1967.

The `ProxyAdmin` allows `LeagueTechV1` and any other protocol `TransparentUpgradeableProxy`  to be updated with new Smart Contract code. To learn more about the `ProxyAdmin`, see the [Open Zeppelin API](https://docs.openzeppelin.com/contracts/5.x/api/proxy#ProxyAdmin).

Only the `owner`  of the `ProxyAdmin` can call the upgrade functions. To prevent unauthorized upgrades, the `owner` of the `ProxyAdmin` is specified as the `Timelock`, which delays the execution of upgrades by a set duration of at least 24 hours.
