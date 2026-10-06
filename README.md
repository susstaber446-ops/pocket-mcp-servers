# Pocket IDE • Central MCP Servers Repository

Welcome to your central repository for **Model Context Protocol (MCP) Servers** in [Pocket IDE](https://github.com/aqibmehedi007/Pocket_IDE).

## How Pocket IDE Discovers this Repo
Pocket IDE's **Pocket Store Hub** automatically detects this repository on your GitHub account (`pocket-mcp-servers`). It reads:
1. `catalog.json` for multi-server specifications and environment variable configurations.
2. The `servers/` directory for individual server modules.

## Available Servers in this Repository

| Server ID | Category | Description | Command |
| :--- | :--- | :--- | :--- |
| **sqlite** | `database` | Direct SQLite database inspection & queries | `npx -y @modelcontextprotocol/server-sqlite` |
| **brave-search** | `search` | Live web search for fresh library docs | `npx -y @modelcontextprotocol/server-brave-search` |
| **github** | `git` | Inspect GitHub repos, issues, and PRs | `npx -y @modelcontextprotocol/server-github` |
| **postgres** | `database` | PostgreSQL database query executor | `npx -y @modelcontextprotocol/server-postgres` |
| **fetch** | `search` | HTTP web page content fetcher & markdown parser | `npx -y @modelcontextprotocol/server-fetch` |
| **memory** | `reasoning` | Persistent knowledge graph & memory | `npx -y @modelcontextprotocol/server-memory` |

## How to Add a New MCP Server
Simply create a new folder under `servers/<your_server_name>/mcp.json` or add an entry to `catalog.json`. Pocket IDE will detect it and provide a **GET** / **UPDATE** button in your mobile IDE!
