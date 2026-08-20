# Instalação rápida

IEPTB (CENPROT) Protestos: Detalhes SP é um servidor MCP remoto hospedado em `https://api.mcp.ai/p_ieptb_protestos_detalhes_sp`. Você não baixa nem roda nada localmente — só aponta seu cliente pra essa URL.

A auth acontece em runtime: clientes com **OAuth 2.1** (Claude Desktop, Cursor, VS Code recentes) abrem o browser na 1ª chamada (magic-link). Clientes sem OAuth recebem a tool `authenticate` — abra `https://app.mcp.ai/agent-auth`, faça login, copie o JWT e cole no chat.

---

## Claude (Web e Desktop)

[➕ Abrir no Claude e conectar](https://claude.ai/new?modal=add-custom-connector#settings/customize-connectors)

Manual: [claude.ai/customize/connectors](https://claude.ai/customize/connectors?surface=cowork) → **+** → **Adicionar conector personalizado** → `IEPTB (CENPROT) Protestos: Detalhes SP` / `https://api.mcp.ai/p_ieptb_protestos_detalhes_sp`.

Config file (legado): `~/Library/Application Support/Claude/claude_desktop_config.json` (macOS) ou `%APPDATA%\Claude\claude_desktop_config.json` (Windows):

```json
{ "mcpServers": { "ieptb_protestos_detalhes_sp": { "type": "http", "url": "https://api.mcp.ai/p_ieptb_protestos_detalhes_sp" } } }
```

## Cursor

[➕ Instalar no Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=ieptb_protestos_detalhes_sp&config=eyJ1cmwiOiJodHRwczovL2FwaS5tY3AuYWkvcF9pZXB0Yl9wcm90ZXN0b3NfZGV0YWxoZXNfc3AifQ==)

`.cursor/mcp.json`:
```json
{ "mcpServers": { "ieptb_protestos_detalhes_sp": { "url": "https://api.mcp.ai/p_ieptb_protestos_detalhes_sp" } } }
```

## VS Code (Copilot Chat)

[➕ Instalar no VS Code](vscode:mcp/install?name=ieptb_protestos_detalhes_sp&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fapi.mcp.ai%2Fp_ieptb_protestos_detalhes_sp%22%7D)

`.vscode/mcp.json`:
```json
{ "servers": { "ieptb_protestos_detalhes_sp": { "type": "http", "url": "https://api.mcp.ai/p_ieptb_protestos_detalhes_sp" } } }
```

## Outros clientes MCP

Qualquer cliente com **MCP over HTTP**. URL fixa:

```
https://api.mcp.ai/p_ieptb_protestos_detalhes_sp
```

Dúvidas? [ieptb_protestos_detalhes_sp@mcp.ai](mailto:ieptb_protestos_detalhes_sp@mcp.ai)
