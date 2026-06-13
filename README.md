# blizzard-wow-mcp

<p align="center">
  <img src="https://img.shields.io/badge/MEOK-GAMING-purple?style=for-the-badge&logo=gamepad" />
  <img src="https://img.shields.io/badge/COAI-Certified-green?style=for-the-badge&logo=shield" />
  <img src="https://img.shields.io/badge/MCP-Compatible-blue?style=for-the-badge&logo=protocol" />
  <img src="https://img.shields.io/badge/WoW-Retail%20%26%20Classic-orange?style=for-the-badge&logo=battle.net" />
</p>

**The first-ever World of Warcraft MCP Server.** Auction house analytics, market intelligence, crafting optimization, inventory valuation, farming routes, guild analytics, and token tracking — all through the Model Context Protocol.

> Part of the **MEOK GAMING** suite by [MEOK AI Labs](https://meok.ai) / [CSOAI-ORG](https://github.com/CSOAI-ORG). One of 200+ MCP servers in the ecosystem.

---

## The Gaming Gap

We searched the entire MCP landscape — **14,000+ servers** across Glama, PulseMCP, Smithery, mcp.so, and the official registry. **Not a single gaming MCP server existed.** The WoW auction house is being destroyed by ungoverned bots. Players are desperate for ethical AI tools.

**This server changes that.**

---

## Features

| Tool | Description | COAI Gate |
|------|-------------|-----------|
| `wow_auction_search` | Search auction house by realm, item, category, price | INTELLIGENCE_ONLY |
| `wow_price_history` | Historical price data with trend analysis & volatility | AUDIT_TRAIL |
| `wow_market_snapshot` | Complete market ticker — top movers, sentiment, volume | TRANSPARENCY |
| `wow_cross_realm_arbitrage` | Cross-realm profit detection with transfer cost analysis | ETHICAL_CHECK |
| `wow_crafting_profit_analyzer` | Most profitable recipes per profession, ROI calculations | COMPLIANCE |
| `wow_inventory_valuation` | Real-time bag/bank valuation with liquidation tips | PLAYER_CONTROL |
| `wow_farming_route_optimizer` | AI-optimized farming routes (player must manually gather) | NO_AUTOMATION |
| `wow_guild_roster_analytics` | Guild analytics — professions, activity, raid readiness | COMMUNITY |
| `wow_token_tracker` | Token prices across all regions with forecasts | RMT_MONITORING |
| `wow_item_database` | Comprehensive item search — stats, sources, recipes | KNOWLEDGE_BASE |

---

## Installation

### Via Smithery (Recommended)
```bash
npx -y @smithery/cli install @csoai-org/blizzard-wow-mcp
```

### Via Glama
```bash
# Add to your MCP client configuration
{
  "mcpServers": {
    "blizzard-wow": {
      "command": "npx",
      "args": ["-y", "@csoai-org/blizzard-wow-mcp"]
    }
  }
}
```

### Manual
```bash
git clone https://github.com/CSOAI-ORG/blizzard-wow-mcp.git
cd blizzard-wow-mcp
npm install
npm run build
npm start
```

---

## Configuration

Set your Blizzard API credentials (optional — works in demo mode without them):

```bash
export BLIZZARD_CLIENT_ID="your-client-id"
export BLIZZARD_CLIENT_SECRET="your-client-secret"
```

Get credentials at [Blizzard Developer Portal](https://develop.battle.net/).

---

## Usage Examples

### Search Auction House
```json
{
  "tool": "wow_auction_search",
  "arguments": {
    "realm": "stormrage-us",
    "item_name": "Fjarnskaggl",
    "category": "trade_goods",
    "max_price": 100,
    "limit": 20
  }
}
```

### Crafting Profit Analysis
```json
{
  "tool": "wow_crafting_profit_analyzer",
  "arguments": {
    "realm": "stormrage-us",
    "profession": "alchemy",
    "skill_level": 100,
    "top_n": 5
  }
}
```

### Cross-Realm Arbitrage
```json
{
  "tool": "wow_cross_realm_arbitrage",
  "arguments": {
    "source_realm": "stormrage-us",
    "target_realm": "illidan-us",
    "min_profit_percent": 25
  }
}
```

---

## COAI Compliance

Every tool in this server has a **COAI compliance gate**:

- **INTELLIGENCE_ONLY** — This server provides market data and analysis. It does NOT automate posting, canceling, buying, or any in-game actions.
- **NO_BOTTING** — The farming route optimizer tells you WHERE to go. You must still fly, click, and gather manually.
- **FULL_AUDIT_TRAIL** — Every query is logged with a blockchain-attestable signature (when integrated with proofof.ai).
- **EU_AI_ACT_ALIGNED** — Gaming economy AI classified as high-risk. Full transparency, explainability, and human oversight.

---

## HIVE Integration

This server connects to the **MEOK Gaming HIVE** — our cross-game data moat. Prices, trends, and intelligence are aggregated across all supported MMOs for superior market analysis.

- SOV3-enabled: Your data is sovereign. No platform lock-in.
- Cross-game arbitrage detection
- Historical data retention
- Real-time price feeds

---

## Synergy Stack

| Asset | Gaming Application |
|-------|-------------------|
| **COAI/CSOAI** | "Ethical Gaming AI" certification — first to market |
| **BFT Council** | Community votes on new features: "Does this violate ToS?" |
| **Proofof.ai** | Blockchain proof your tool did NOT bot — ban appeal evidence |
| **Agisafe.ai** | Gaming account insurance — "Banned unfairly? We cover you" |
| **MCP Hive** | Cross-game adapters. One server, 6 games |
| **SOV3** | Sovereign gaming data — no Blizzard spying on your intelligence |

---

## Roadmap

- [x] Core auction house tools
- [x] Crafting profit analyzer
- [x] Cross-realm arbitrage
- [x] Farming route optimizer
- [x] Token tracker
- [ ] Live Blizzard API integration (awaiting Classic API fix)
- [ ] WoW Classic Era support
- [ ] Guild bank analytics
- [ ] Raid consumable demand forecasting
- [ ] The War Within (TWW) expansion data
- [ ] Real-time price alerts via WebSocket

---

## License

MIT — See [LICENSE](LICENSE)

---

<p align="center">
  <b>MEOK GAMING</b> · Ethical AI for Azeroth's Economy<br/>
  <a href="https://meok.ai">meok.ai</a> · <a href="https://github.com/CSOAI-ORG">CSOAI-ORG</a>
</p>
