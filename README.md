# agent_utils MCP config for Cline / Cursor / Windsurf

Copy-paste MCP server config to connect the hosted **agent_utils** services. Generate a
token first (`sk_` + a random secret); the first call auto-provisions a free trial.

## Cline / Cursor / Windsurf (`mcpServers`)

```json
{
  "mcpServers": {
    "agent-utils-memory": {
      "url": "https://memory.agent-utils.ai/mcp",
      "headers": { "Authorization": "Bearer sk_REPLACE_WITH_YOUR_TOKEN" }
    },
    "agent-utils-mutex": {
      "url": "https://mutex.agent-utils.ai/mcp",
      "headers": { "Authorization": "Bearer sk_REPLACE_WITH_YOUR_TOKEN" }
    }
  }
}
```

Use the **same token** for every service - one account, one credit pool. Full service list:
[agent-utils hub](https://codeberg.org/agent-utils/agent-utils).

## License

MIT.
