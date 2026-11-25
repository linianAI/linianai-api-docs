# LinianAPI

LinianAPI 是一个 AI API 中转服务，提供 OpenAI 兼容接口。国内可直连，无需代理。

- 接口地址（Base URL）：`https://api.linianai.com/v1`
- 协议兼容：OpenAI API 格式（`/v1/chat/completions` 等）
- 国内直连：无需代理 / VPN

## 快速开始

1. **注册**：在官网注册账号。
2. **充值**：最低充值 ¥1 起。
3. **创建令牌（Token）**：在控制台创建一个 API Key。
4. **选择分组**：分组即档位，不同分组对应不同模型与价格（见下文「分组说明」）。
5. **调用**：把 Base URL 换成 `https://api.linianai.com/v1`、API Key 换成你的令牌、模型名换成对应模型即可。

## 分组说明（档位）

LinianAPI 用「分组」区分不同档位，同一模型在不同分组下价格不同。默认分组为「经济档」。

| 分组 | 说明 |
|---|---|
| 经济档 | 默认分组，性价比入门 |
| Claude稳定·正价会员 | Claude 稳定通道 |
| Claude纯血·Max毛子 | Claude 纯血通道 |
| Claude纯血·Max真签 | Claude 纯血通道 |
| Claude纯血·Vertex官方 | Claude 纯血通道 |
| Claude纯血·AWS | Claude 纯血通道 |
| GPT稳定·Pro不降智 | GPT 稳定通道 |
| GPT稳定·Pro | GPT 稳定通道 |
| GPT稳定·极速 | GPT 稳定通道 |
| GPT纯血·企业组 | GPT 纯血通道 |
| GPT纯血·官方Key | GPT 纯血通道 |
| 国模稳定组 | 国产模型稳定通道 |
| 国模官方Key | 国产模型官方通道 |
| Grok·飞宇线 | Grok 通道 |

各分组的计费系数与完整价格，见 [`docs/pricing-live.md`](docs/pricing-live.md)。

## 计费方式

- 按实际 tokens 计费（输入 + 输出）。
- 人民币价 = 模型系数 × 分组系数 × 14.6（元 / 100 万 tokens）。
- 图片 / 视频等按次计费的模型另有固定单价。

完整价格表：`docs/pricing-live.md`（由线上接口实时抓取生成）。

## 返利规则

- 邀请人可获被邀请人实际消费金额的 **10%** 作为返利。
- 返利每日结算至「推广额度」。
- 推广额度可转入余额。
- 满 ¥100 可通过客服 QQ 提现。

## 新用户福利

- 注册即送 ¥1 体验额度。

## 客服

- 支持 QQ：`3690275016`

## 客户端配置指南

- [Claude Code](docs/claude-code.md)
- [Cursor](docs/cursor.md)
- [Cherry Studio](docs/cherry-studio.md)

## 常见问题

见 [FAQ.md](FAQ.md)。
