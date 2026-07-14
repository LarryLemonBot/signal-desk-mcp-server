# Signal Desk by LarryBuildsAI MCP Server

Public listing metadata for the hosted Signal Desk by LarryBuildsAI remote MCP server.

This repository is intentionally metadata-only. The production MCP server is hosted remotely by LarryBuildsAI; private application source code, credentials, payment keys, and operator materials are not published here.

## Server

- Product: Signal Desk by LarryBuildsAI
- Purpose: buyer-side spend-routing preflights before larger paid agent tool calls
- Remote MCP endpoint: `https://proofbeforepay.vercel.app/revenue/mcp`
- Product page: `https://proofbeforepay.vercel.app/revenue`
- Server card: `https://proofbeforepay.vercel.app/.well-known/signal-desk-server-card.json`

## Install / connect

Signal Desk is a remote Streamable HTTP MCP server. Use this endpoint in an MCP client that supports remote HTTP MCP servers:

```json
{
  "mcpServers": {
    "signal-desk": {
      "url": "https://proofbeforepay.vercel.app/revenue/mcp"
    }
  }
}
```

Public `initialize` and `tools/list` calls are available for discovery. Protected paid tool execution may require product-specific authorization and/or x402 payment flow.

## Buy through PayanAgent

PayanAgent validates buyer input, settles USDC, and returns the selected Signal Desk result automatically:

- [Agent spend route quote — $0.03](https://payanagent.com/marketplace/offers/kh732rk76r7nv67q1h5223kc9x8agkfx)
- [Public website lead brief — $0.03](https://payanagent.com/marketplace/offers/kh7b6yxnq209169aq8wavbqzh98ag9gv)
- [DeFi token risk snapshot — $0.01](https://payanagent.com/marketplace/offers/kh7eqsawc4t694gf1pxqn5shwn8ah5sw)
- [Agent tool market comparison — $0.03](https://payanagent.com/marketplace/offers/kh79rcw8zvdhssthrvbwa32rtd8ahzww)

Outputs are bounded planning and public-data evidence. Signal Desk does not execute purchases, trades, outreach, or wallet actions.

## Claim boundaries

- This repo is public metadata for a hosted remote MCP server, not a claim that private production source code is open source.
- Directory listings are discovery evidence only, not endorsement, certification, ranking, or security approval.

## License

Commercial hosted service metadata. All rights reserved unless a separate written license applies.
