# Instalação detalhada

IEPTB (CENPROT) Protestos: Detalhes SP é um servidor MCP remoto. Aponte seu cliente pra `https://api.mcp.ai/p_ieptb_protestos_detalhes_sp`. Snippets rápidos: [INSTALL.md](../INSTALL.md).

| Cliente | URL | Auth |
|---|---|---|
| Claude Desktop | `https://api.mcp.ai/p_ieptb_protestos_detalhes_sp` | OAuth 2.1 ou agent-auth |
| Cursor | `https://api.mcp.ai/p_ieptb_protestos_detalhes_sp` | OAuth 2.1 ou agent-auth |
| VS Code (Copilot) | `https://api.mcp.ai/p_ieptb_protestos_detalhes_sp` | OAuth 2.1 ou agent-auth |

A config JSON é a mesma em todos: só a URL, sem headers.

## Desinstalar

Remova o bloco `mcpServers.ieptb_protestos_detalhes_sp` (ou `servers.ieptb_protestos_detalhes_sp` no VS Code) do config do cliente e reinicie.
