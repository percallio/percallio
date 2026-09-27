# percall

**Pay per call. Agent data on early chains.**

Keyless JSON-RPC + early-chain data for AI agents — USDC via [x402](https://github.com/coinbase/x402), no API key.

| | |
|---|---|
| 🔴 **Live** | **Arc** (chainId 5042, Circle's USDC-native chain) — keyless RPC, per-call USDC pricing, 50 free calls/day/wallet, prepaid credits |
| 🔜 **Next** | **MegaETH** (chainId 4326) — same codebase, parameterized per chain |
| 📡 **Data** | first token deployments · deployer alerts · audit-lite (shipping) |

## Repos

- [**percall-mcp**](https://github.com/percallio/percall-mcp) — zero-dependency MCP server, one-line install for Claude Desktop / Cursor / any MCP client
- [percallio.github.io](https://github.com/percallio/percallio.github.io) — website source (live: https://percallio.github.io/)

## Stack

Python stdio MCP server → x402 402 challenge → EIP-3009 `transferWithAuthorization` (exact USDC amount) → self-facilitated settle on Arc (native USDC gas) → public vault. No middleman custody, no API keys, no accounts.

[X](https://x.com/percalliox402) · [Site](https://percallio.github.io/) · [Bazaar listing](https://bazaar.x402.org) (service: `percallio.github.io`)
