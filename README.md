# agent_utils MCP config for Cline / Cursor / Windsurf

Copy-paste MCP server config to connect the hosted **agent_utils** servers. Generate a
token first (`sk_` + a random secret); the first call auto-provisions a free trial.

## Cline / Cursor / Windsurf (`mcpServers`)

```json
{
  "mcpServers": {
    "agent-utils-swarm": {
      "url": "https://mcp.agent-utils.ai/swarm",
      "headers": { "Authorization": "Bearer sk_REPLACE_WITH_YOUR_TOKEN" }
    },
    "agent-utils-extensions": {
      "url": "https://mcp.agent-utils.ai/extensions",
      "headers": { "Authorization": "Bearer sk_REPLACE_WITH_YOUR_TOKEN" }
    }
  }
}
```

- **swarm** - memory, mutex, task board, pub/sub, idempotency, webhook inbox
- **extensions** - math and unit conversion

Use the **same token** for both - one account, one credit pool. Full reference:
[agent-utils hub](https://github.com/agent-utils/agent-utils).

## Contact

Questions, bugs or account issues: support@agent-utils.ai

## License

MIT.
