# Installing the OwlChart MCP server

OwlChart is a remote MCP server. Nothing is installed locally: add one URL.

- URL: `https://owlchart.com/mcp`
- Transport: Streamable HTTP
- Authentication: none needed (Trial). Optional: `Authorization: Bearer owl_...` personal key for PRO members, from the OwlChart dashboard, AI Connectors box.

## Cline

Open MCP Servers, Remote Servers, and add:

- Server name: `owlchart`
- Server URL: `https://owlchart.com/mcp`
- Transport type: Streamable HTTP

Or in `cline_mcp_settings.json`:

```json
{
  "mcpServers": {
    "owlchart": {
      "type": "streamableHttp",
      "url": "https://owlchart.com/mcp"
    }
  }
}
```

## Check it works

Ask: "What is BTC open interest across all exchanges?" The `get_open_interest` tool should answer with a total and one row per exchange, and a link to owlchart.com.

## Tools

search_markets, get_price_history, show_chart, get_liquidity_heatmap, get_open_interest, get_orderbook_depth, get_owl_score, get_etf_flows, get_funding_rates, get_liquidations, scan_patterns, get_market_radar, get_tokenization_overview, get_crypto_regulation, get_money_flows, get_track_record, create_alert, list_alerts, delete_alert, check_alerts, get_watchlist, add_to_watchlist, remove_from_watchlist.
