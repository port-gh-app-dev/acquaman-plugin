# Acquaman Plugin (OpenAI Codex Scaffold)

This repository is scaffolded to support an OpenAI plugin-style integration and local Codex MCP configuration.

## Included Files

- `/.well-known/ai-plugin.json` - Plugin manifest following OpenAI plugin conventions.
- `/openapi.yaml` - Mock OpenAPI contract consumed by the plugin manifest.
- `/.mcp.json` - Local default MCP server configuration using a mock server package.
- `/.mcp.example.json` - Example MCP configurations for HTTP and stdio transports.
- `/mock/mcp-server.js` - Placeholder script for a local stdio MCP server.

## Quick Start

1. Serve repository files from `http://localhost:3333` (or update URLs in `ai-plugin.json`).
2. Customize `openapi.yaml` endpoints for your real plugin API.
3. Replace placeholder values in `.mcp.example.json` and copy it to `.mcp.json` as needed.
4. Implement a real MCP server in `mock/mcp-server.js` or point `.mcp.json` to your actual server command.

## Notes

- This scaffold is intentionally minimal and mock-oriented.
- `contact_email`, `legal_info_url`, API URLs, and auth settings should be updated for production use.
