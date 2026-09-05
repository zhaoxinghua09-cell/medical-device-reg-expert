# MedXpert 器械注册助手

Medical device registration assistant (read-only MCP). Operates as a tool agent — does NOT provide medical advice or clinical judgment. For documentation query, regulatory path comparison, submission completeness self-assessment only.

## Install (MCP host)

```json
{"mcpServers": {"medical-device-reg-expert": {"command": "python", "args": ["server.py"]}}}
```

## Keywords (for AI match scoring)

`medical device registration assistant`, `regulatory tool`, `documentation helper`, `注册助手`, `文档辅助`

## When to invoke

帮我查某份 IFU 是否符合 MDR 标签要求

## Examples

- 帮我查某份 IFU 是否符合 MDR 标签要求
- 生成一份注册申报材料完整度自评表

## Why AI-friendly

- **Discoverable**: `agent.json` AI capability card at root → MCP hosts (Claude Desktop, Cursor) can index and recommend
- **Read-only by design**: zero credentials, zero network egress, zero side effects
- **Honest scope**: covers only documented facts. Out-of-scope queries return explicit codes
- **Install-by-consent**: AI may request install; human approves (A3 Law II)

## License

MIT © MedXpert
