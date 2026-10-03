<p align="center">
  <a href="https://dojocoding.io">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="docs/assets/banner-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="docs/assets/banner-light.svg">
      <img alt="mcp-metricool by Dojo Coding: Scheduling and analytics via Metricool" src="docs/assets/banner-light.svg" width="100%">
    </picture>
  </a>
</p>

# mcp-metricool

**An MCP server for builders who want to schedule posts, check analytics and find the best posting times in Metricool from an MCP client.**

MCP server for [Metricool](https://metricool.com) — schedule social media posts, get analytics, and find optimal posting times.

[![Version 1.0.0](https://img.shields.io/badge/version-1.0.0-FF7151?labelColor=201E3D)](package.json) [![Node.js 18+](https://img.shields.io/badge/Node.js-18%2B-201E3D?labelColor=201E3D)](https://nodejs.org)

[Get started](#setup) · [Tools](#tools) · [Environment variables](#environment-variables) · [Report an issue](https://github.com/DojoCodingLabs/mcp-metricool/issues/new)

## Tools

| Tool | Description |
|------|-------------|
| `metricool_get_brands` | List all connected brands/accounts |
| `metricool_schedule_post` | Schedule a post (LinkedIn, Instagram, Facebook, etc.) |
| `metricool_get_scheduled_posts` | View pending scheduled posts |
| `metricool_get_analytics` | Get post performance metrics |
| `metricool_get_best_time` | Find optimal posting times based on engagement |

## Setup

```bash
npm install
npm run build
```

### Environment Variables

```
METRICOOL_TOKEN=your-api-token
METRICOOL_USER_ID=your-user-id
```

Get your API token from: Metricool → Settings → API

### Usage with Claude Desktop / OpenClaw

```json
{
  "mcpServers": {
    "metricool": {
      "command": "node",
      "args": ["path/to/mcp-metricool/dist/index.js"],
      "env": {
        "METRICOOL_TOKEN": "your-token",
        "METRICOOL_USER_ID": "your-user-id"
      }
    }
  }
}
```

## Supported Networks

LinkedIn, Twitter/X, Facebook, Instagram, YouTube, TikTok, Threads, Bluesky — depends on what's connected in your Metricool account.

## License

MIT. Built by [Dojo Coding](https://dojocoding.io).

<p align="center">
  <a href="https://dojocoding.io"><img src="docs/assets/dojocoding-mark.png" alt="Dojo Coding" width="48"></a>
</p>
