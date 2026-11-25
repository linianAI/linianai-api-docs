# LinianAPI 价格表（实时抓取）

> 抓取时间：2026-11-25T22:52:30+08:00
> 数据来源：`GET https://api.linianai.com/api/pricing`（pricing_version `a42d372ccf0b5dd13ecf71203521f9d2`）

## 计费公式

按量模型：**人民币价 = 模型系数(model_ratio) × 分组系数(group_ratio) × 14.6**，单位 元 / 100 万 tokens（输入）。输出价格 = 输入价 × completion_ratio（该字段缺失时输入输出同价）。

按次模型（图片/视频）：固定单价，见下表 `model_price` 列，单位 元/次。

## 分组与系数

| 分组 key | 中文名称 | 分组系数 group_ratio |
|---|---|---|
| `default` | 经济档 | 1 |
| `claude-member` | Claude稳定·正价会员 | 3.3333 |
| `claude-maozi` | Claude纯血·Max毛子 | 6.6667 |
| `claude-max` | Claude纯血·Max真签 | 11.1111 |
| `claude-vertex` | Claude纯血·Vertex官方 | 10 |
| `claude-awsb` | Claude纯血·AWS | 27.7778 |
| `gpt-pro-nd` | GPT稳定·Pro不降智 | 1.1429 |
| `gpt-pro` | GPT稳定·Pro | 3 |
| `gpt-ultrafast` | GPT稳定·极速 | 3.5714 |
| `gpt-qiye` | GPT纯血·企业组 | 3.7143 |
| `gpt-fuge` | GPT纯血·官方Key | 5.1429 |
| `guomod-stable` | 国模稳定组 | 1.7778 |
| `guomod-key` | 国模官方Key | 4 |
| `grok-feiyu` | Grok·飞宇线 | 0.381 |

## 按量模型价格（默认分组：经济档）

| 模型 | 输入价（元/1M tokens） | 输出价（元/1M tokens） | 可用分组 |
|---|---|---|---|
| codex-auto-review | 0.39 | 4.63 | GPT稳定·Pro不降智, GPT稳定·Pro, GPT稳定·极速, GPT纯血·企业组, GPT纯血·官方Key, 经济档 |
| claude-sonnet-5 | 1.32 | 6.60 | Claude纯血·Vertex官方, Claude纯血·Max真签, Claude纯血·AWS, Claude稳定·正价会员, 经济档, Claude纯血·Max毛子 |
| deepseek-v4.1-flash | 0.40 | 1.58 | 经济档, 国模稳定组, 国模官方Key |
| grok-4.6 | 1.68 | 5.04 | 经济档, Grok·飞宇线 |
| gemini-3-flash-preview | 2.20 | 13.20 | 经济档 |
| gpt-6.1-terra | 0.15 | 0.77 | GPT纯血·企业组, GPT纯血·官方Key, 经济档, GPT稳定·Pro不降智, GPT稳定·Pro, GPT稳定·极速 |
| gpt-5.6-luna | 0.31 | 1.85 | 经济档 |
| gpt-5.6-sol | 0.77 | 4.62 | 经济档, GPT稳定·Pro不降智, GPT稳定·Pro, GPT稳定·极速, GPT纯血·企业组, GPT纯血·官方Key |
| gpt-6-astra | 1.54 | 7.70 | GPT纯血·官方Key, 经济档, GPT稳定·Pro不降智, GPT稳定·Pro, GPT稳定·极速, GPT纯血·企业组 |
| claude-opus-5-5 | 2.64 | 13.20 | Claude纯血·Max真签, Claude纯血·AWS, Claude稳定·正价会员, 经济档, Claude纯血·Max毛子, Claude纯血·Vertex官方 |
| claude-sonnet-4-6 | 0.59 | 2.97 | Claude纯血·Max真签, Claude纯血·AWS, 经济档, Claude稳定·正价会员, Claude纯血·Vertex官方 |
| deepseek-v4-flash-vision-exp | 1.92 | 7.68 | 经济档 |
| glm-5.2 | 7.68 | 26.88 | 经济档 |
| grok-4.7 | 1.68 | 5.04 | 经济档, Grok·飞宇线 |
| gpt-6.2-sol | 0.31 | 1.54 | GPT纯血·企业组, GPT纯血·官方Key, 经济档, GPT稳定·Pro不降智, GPT稳定·Pro, GPT稳定·极速 |
| claude-opus-4-7 | 3.30 | 16.50 | Claude稳定·正价会员, 经济档, Claude纯血·Vertex官方, Claude纯血·Max真签, Claude纯血·AWS |
| claude-haiku-5-5 | 0.07 | 0.33 | Claude稳定·正价会员, 经济档, Claude纯血·Max毛子, Claude纯血·Vertex官方, Claude纯血·Max真签, Claude纯血·AWS |
| kimi-k3.1-pro | 2.57 | 13.46 | 经济档, 国模稳定组, 国模官方Key |
| claude-opus-4-8 | 3.30 | 16.50 | Claude稳定·正价会员, 经济档, Claude纯血·Vertex官方, Claude纯血·Max真签, Claude纯血·AWS |
| claude-opus-5 | 3.30 | 16.50 | Claude纯血·AWS, Claude稳定·正价会员, 经济档, Claude纯血·Max毛子, Claude纯血·Vertex官方, Claude纯血·Max真签 |
| glm-5.3 | 3.17 | 11.09 | 经济档, 国模稳定组, 国模官方Key |
| deepseek-flash | 1.02 | 4.08 | 经济档, 国模官方Key |
| claude-fable-5 | 6.60 | 33.00 | Claude纯血·Max毛子, Claude纯血·Vertex官方, Claude纯血·Max真签, Claude纯血·AWS, Claude稳定·正价会员, 经济档 |
| deepseek-v4-pro | 0.26 | 0.78 | 经济档, 国模稳定组, 国模官方Key |
| mimo-v2.6-pro | 0.86 | 1.72 | 经济档, 国模稳定组 |
| gpt-6.1-sol | 0.31 | 1.54 | GPT稳定·极速, GPT纯血·企业组, GPT纯血·官方Key, 经济档, GPT稳定·Pro不降智, GPT稳定·Pro |
| claude-fable-5-1 | 6.60 | 33.00 | Claude纯血·Vertex官方, Claude纯血·Max真签, Claude纯血·AWS, Claude稳定·正价会员, 经济档, Claude纯血·Max毛子 |
| claude-sonnet-5-5 | 1.32 | 6.60 | Claude稳定·正价会员, 经济档, Claude纯血·Max毛子, Claude纯血·Vertex官方, Claude纯血·Max真签, Claude纯血·AWS |
| deepseek-v4-flash | 1.92 | 7.68 | 经济档 |
| glm-5.3-flash | 0.32 | 1.11 | 经济档, 国模稳定组, 国模官方Key |
| kimi-k3 | 18.40 | 92.00 | 经济档, 国模稳定组, 国模官方Key |
| grok-4.5 | 1.68 | 5.04 | 经济档, Grok·飞宇线 |
| gpt-5.6-terra | 0.31 | 1.85 | GPT稳定·Pro, GPT稳定·极速, GPT纯血·企业组, GPT纯血·官方Key, 经济档, GPT稳定·Pro不降智 |
| gpt-6.2-astra | 1.23 | 6.16 | GPT纯血·企业组, GPT纯血·官方Key, 经济档, GPT稳定·Pro不降智, GPT稳定·Pro, GPT稳定·极速 |
| gpt-6-sol | 0.31 | 1.54 | GPT纯血·官方Key, 经济档, GPT稳定·Pro不降智, GPT稳定·Pro, GPT稳定·极速, GPT纯血·企业组 |

## 按次模型价格（图片/视频）

| 模型 | 单价（元/次） |
|---|---|
| MiniMaxH3-2k | 2.2352 |
| MiniMaxH3-480p | 1.7648 |
| grok-imagine-video-1.5 | 0.6 |
| MiniMaxH3-720p-按次 | 2.5882 |
| seedance-2.0-480p | 0.9 |
| gpt-image-2 | 0.0041 |
| sd2-903-720p | 8.58824 |
| MiniMaxH3-480p-按次 | 1.7648 |
| seedance-2.0-720p | 1.7 |
| seedance-2.0-fast-900-720p | 2.11764 |
| seedance-2.0-mini-900-720p | 1.882352 |
| MiniMaxH3-2k-按次 | 2.53 |
| wan2.2animate-v4-动作迁移 | 0.16 |
| MiniMaxH3-720p | 2.5882 |
