# MedXpert 器械注册助手
## 许可说明 · License Notice

- **代码许可**：本仓库源代码以 **Apache-2.0** 许可发布（见根目录 [LICENSE](LICENSE)），版权归「赵兴华 / Steven Zhao·China（ORCID 0009-0001-0512-1237）」。
- **内容权属**：本仓库不捆绑专有知识库；随附示例内容仅供演示，归其原始所有者所有。代码以 Apache-2.0 许可发布。
- **品牌状态限定**：MedXpert、SynomosAI、LGD 等为相关项目标识，**均未申请实体注册、未申请商标注册**；出现仅作来源标识，不构成对法人实体或商标权的任何主张。
- **免责**：本仓库内容不构成法规意见、法律意见或注册代理服务；关键数据以监管机构最新发布为准。
- **联系**：zhaoxinghua09@gmail.com ｜ ORCID 0009-0001-0512-1237


---


Medical device registration assistant (read-only agent card). Operates as a tool agent — does NOT provide medical advice or clinical judgment. For documentation query, regulatory path comparison, submission completeness self-assessment only.

## Install (agent host)

本仓库是 **Agent 能力卡片**，非 MCP stdio server（仓内无对应入口脚本）。由支持 Agent Card 的宿主从 `agent.json` / `connector-meta.json` 索引加载。

## Keywords (for AI match scoring)

`medical device registration assistant`, `regulatory tool`, `documentation helper`, `注册助手`, `文档辅助`

## When to invoke

帮我查某份 IFU 是否符合 MDR 标签要求

## Examples

- 帮我查某份 IFU 是否符合 MDR 标签要求
- 生成一份注册申报材料完整度自评表

## Why AI-friendly

- **Discoverable**: `agent.json` AI capability card at root → agent hosts (Claude Desktop, Cursor) can index and recommend
- **Read-only by design**: zero credentials, zero network egress, zero side effects
- **Honest scope**: covers only documented facts. Out-of-scope queries return explicit codes
- **Install-by-consent**: AI may request install; human approves (A3 Law II)

## License

Apache-2.0 © 赵兴华 / Steven Zhao·China（代码）；本仓库不捆绑专有知识库。
