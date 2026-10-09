# Scout Squad

Cursor plugin for [Scout Squad](https://scoutsquad.app/), a fantasy football scout for Sleeper leagues. It connects Cursor to Scout Squad's remote MCP server. The plugin searches players, reads a league, and checks waiver, start/sit, trade, and lineup decisions. It reads league data and does not change a lineup, submit a waiver claim, or send a trade.

## Install

After the plugin is listed in the Cursor Marketplace:

1. Open **Customize** in the sidebar.
2. Find **Scout Squad**.
3. Select **Install**.

Or run `/add-plugin scout-squad` in chat.

To try it before it is listed, copy this repository into Cursor's local plugins folder as `scout-squad`, reload Cursor, and confirm the Scout Squad MCP server appears in Customize. Local plugin imports must be allowed. The folder layout is in [Test plugins locally](https://cursor.com/docs/plugins#test-plugins-locally).

## First use

The first connection opens Scout Squad's own sign-in. Approve that prompt in the browser. This repository stores no API keys, client secrets, or tokens. Each person authenticates as themselves.

Then connect Sleeper with a username. Do not provide a Sleeper password. Yahoo and ESPN are not supported.

Start/sit and single add/drop checks are on the free account. Trade analysis, full lineup recommendations, and batch add/drop checks require Pro.

## Tools

| Tool | What it does |
| --- | --- |
| `search` | Find Sleeper players by name and return refs for the other tools. |
| `get` | Read a player, league, roster, or saved receipt. |
| `connect_league` | Look up a Sleeper username, choose active leagues, or check import status. |
| `waiver_board` | Rank projected unrostered players in one active league. |
| `gut_check` | Run and save one decision: start/sit, add/drop, trade, or lineup. |
| `batch_gut_check` | Compare up to three unrostered candidates against up to two owned drops. Does not submit a waiver claim. |

The hosted server is the source of truth for tool names and arguments.

## Links

- Product: https://scoutsquad.app/
- Terms: https://scoutsquad.app/terms
- Privacy: https://scoutsquad.app/privacy
- Server: `https://scout-squad-production.fastapicloud.dev/mcp`

## License

MIT. Copyright (c) 2026 Cachetronaut.
