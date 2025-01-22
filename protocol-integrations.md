# Protocol Integrations

## Smart Contracts
```solidity
interface IYieldAggregator {
    function deposit(address token, uint256 amount) external;
    function withdraw(address token, uint256 shares) external;
    function getAPY(address token) external view returns (uint256);
    function getTVL(address token) external view returns (uint256);
}

interface IStrategy {
    function harvest() external;
    function panic() external;
    function pause() external;
    function unpause() external;
}
```

## Supported Protocols
### AMMs
- Uniswap V2/V3
- Curve v1/v2
- Balancer

### Lending
- Aave v2/v3
- Compound v2/v3
- Euler

### Options
- Lyra
- Dopex
- Hegic