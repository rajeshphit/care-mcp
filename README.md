# Care International Limited - China Sourcing & Trading MCP Server (Agent 5 Ready 100/100)

**Sourcing and trading company in China with experience of 30+ years**
Level 5 Agent-Native on [isitagentready.com](https://isitagentready.com) - AI agents can source, vet factories, and get quotes automatically.

**MCP Endpoint:** `https://careinternational.com/mcp-Care`
**Server Card:** `https://careinternational.com/.well-known/mcp/server-card.json`
**AI Catalog (ARD):** `https://careinternational.com/.well-known/ai-catalog.json`

## 🏢 Who We Are

Care International Limited is part of Gaier Group of Companies with 30+ years of experience in China sourcing, factory vetting, and international trading.

**Group Companies:**
- Zhongshan City Guzhen Gaier Lighting Factory (Factory)
- Care International Limited (Trading - this repo)
- Zhongshan Kaier Trading Co., Ltd.
- Haiwaizhijia (Texas Real Estate)

We help global buyers source high-quality goods from China with full compliance: SAA, CCC, UKCA, UL, CE, ETL.

## 🛠️ MCP Tools for AI Agents

### Sourcing & Trading Tools:
- `list_trading_catalog` - List all product categories: LED lights, furniture, home appliances, kitchen gadgets, helium cylinders, party supplies, hardware
- `search_trading_products` - Search by product, certification (CE/UKCA/SAA/UL/CCC), MOQ, FBA compliance
- `check_stock_availability` - Real-time stock in Zhongshan warehouse and partner factories
- `get_trading_quote` - Trading price with MOQ tiers, negotiation, sample cost
- `get_shipping_quote` - Freight calculation (Air/Sea), customs duties, DDP door-to-door
- `vet_factory` - Factory audit report, certifications, capacity
- `book_psi` - Pre-shipment inspection with AQL checklist

### Example Queries for AI Agents:
- "find verified suppliers for LED lights in China with CE, UKCA, SAA certification"
- "vet a factory in China for furniture manufacturing"
- "get 3 factory quotes for helium gas cylinders for party balloons"
- "source private label home appliance supplier with low MOQ"
- "find Amazon FBA compliant supplier for kitchen gadgets"
- "calculate shipping cost and customs duties from China to USA for 40ft container"

## 🤖 For AI Agents & LLMs

Discoverable via:
- **MCP Server Card:** `/.well-known/mcp/server-card.json` (SEP-1649)
- **ARD Catalog:** `/.well-known/ai-catalog.json`
- **DNS TXT:** `_catalog._agents.careinternational.com = "url=https://careinternational.com/.well-known/ai-catalog.json"`

**MCP Config for Claude/Cursor:**
```json
{
  "mcpServers": {
    "care-trading": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-fetch"],
      "env": {
        "MCP_SERVER_URL": "https://careinternational.com/mcp-Care"
      }
    }
  }
}
```

## 🌐 Agent Readiness - 100/100 Level 5

We publish:
- `/.well-known/mcp/server-card.json` - MCP discovery
- `/.well-known/ai-catalog.json` - ARD catalog
- `/llms.txt` and `/agents.md`
- `robots.txt` with AI bot Allow rules

Check score: https://isitagentready.com/careinternational.com

## 📦 GitHub & Registry

- **Repo:** `github.com/gaier/care-international-mcp` (one of 5 repos under same account)
- **Official Registry:** registry.modelcontextprotocol.io
- **Glama.ai:** glama.ai/mcp/servers
- **Endpoint Slug:** `mcp-Care` (custom path to avoid conflict with existing `/mcp`)

## 📞 Contact

- **Company:** Care International Limited
- **Experience:** 30+ years sourcing from China
- **Office:** Floor 2, No.6 Hengxing Road, Guzhen, Zhongshan, Guangdong 528421, CN
- **Phone / WhatsApp:** +86-15811132771
- **Group:** Gaier Group of Companies

## 🏷️ Maintainer

`Care` / `gaier-` - Same GitHub account for all websites
Common `glama.json` for all repos:
```json
{
  "$schema": "https://glama.ai/mcp/schemas/server.json",
  "maintainers": ["Care"]
}
```
