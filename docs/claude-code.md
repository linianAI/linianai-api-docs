# Claude Code 配置指南

在 Claude Code 中使用 LinianAPI：

1. 打开配置，将接口地址设置为 `https://api.linianai.com/v1`。
2. 填入你的 API Key（控制台创建的令牌）。
3. 填入模型名（如 `claude-sonnet-5`、`claude-opus-5-5` 等，见价格表）。

关键参数：

- Base URL：`https://api.linianai.com/v1`
- API Key：你的令牌
- Model：按需选择，见 [`docs/pricing-live.md`](pricing-live.md)

如果 Claude Code 通过环境变量配置，可参考设置 `ANTHROPIC_BASE_URL` 与 `ANTHROPIC_AUTH_TOKEN`。
