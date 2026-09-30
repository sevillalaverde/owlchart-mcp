# OwlChart MCP server

Live, raw market data for any AI assistant. Add one link as a connector and ask about any coin, stock or market:

```
https://owlchart.com/mcp
```

Remote Streamable HTTP server, OAuth 2.1 with dynamic client registration. Trial with no account; PRO with a personal `owl_` key (Bearer). Official MCP Registry name: `com.owlchart/owlchart`.

## Tools (23)

| Tool | What it returns |
|---|---|
| search_markets | Any instrument: crypto spot and perps, stocks, ETFs, forex, futures, commodities |
| get_price_history | OHLCV candles with last price, change, high and low |
| get_liquidity_heatmap | Liquidity magnets above and below, pull direction, whale walls, long/short, measured hit rate |
| get_open_interest | Open interest summed across 13 exchanges, one row per venue |
| get_orderbook_depth | Resting bids and asks across 22+ venues, market-maker books stripped |
| get_owl_score | 0 to 100 market conditions score |
| get_etf_flows | BTC and ETH spot ETF flows fund by fund, BlackRock holdings, verdict |
| get_funding_rates | Perpetual funding by exchange |
| get_liquidations | Realised long and short liquidations |
| scan_patterns | Candlestick and chart patterns with measured win rates |
| get_market_radar | Major coins at a glance |
| get_tokenization_overview | Stablecoins, tokenised treasuries, gold and shares read from the contracts |
| get_crypto_regulation | CLARITY Act, SEC and CFTC tracker |
| show_chart | A live candle chart drawn inside the AI chat (MCP Apps), with liquidity magnets |
| get_money_flows | Stablecoin mints and burns, tokenised gold and treasuries, ETF money, open interest change |
| get_track_record | Public forward-tested record of OwlChart's liquidity model, per coin |
| create_alert / list_alerts / delete_alert / check_alerts | Alerts on open interest, liquidity magnets, funding, ETF verdict flips and price; delivered to the chat or a webhook |
| get_watchlist / add_to_watchlist / remove_from_watchlist | The member's own watchlist with live prices |

## Connect

- Claude: Settings, Connectors, Add custom connector, paste the URL
- ChatGPT: Settings, Apps and Connectors, Create, paste the URL
- Grok: grok.com/connectors, New Connector, Custom
- Cursor: `{ "mcpServers": { "owlchart": { "url": "https://owlchart.com/mcp" } } }`
- VS Code: `{ "servers": { "owlchart": { "type": "http", "url": "https://owlchart.com/mcp" } } }`
- Gemini, Perplexity, Le Chat, Copilot Studio, Claude Code, Codex CLI, Gemini CLI, Windsurf, Cline, Zed, Kiro, DeepSeek, n8n, Make, Pipedream: see https://owlchart.com/connectors.html and llms-install.md

![OwlChart](owlchart-logo-400.png)

Every answer carries the source, the read time and the owlchart.com page it came from. Data and analysis only, never a trade instruction.
