# Clash & Sing-box 精选分流规则包（AI 专线 + Just My Socks 优化版）

> 本仓库由 [Just My Socks 官方指南组织](https://github.com/justmysocks-guide) 维护，提供专为 **ChatGPT、Claude、Midjourney** 及现代出海网络加速优化的分流规则集，完美适配 **Clash Verge Rev、Mihomo、Sing-box 及 Shadowrocket**。

---

## 🚀 核心特性

- 🎯 **精准 AI 分流**：自动识别 `openai.com`、`claude.ai`、`gemini.google.com` 等主流大模型域名，定向走高纯净度机房节点，告别 Access Denied 报错。
- ⚡️ **无缝融合 Just My Socks**：完美兼容搬瓦工官方运营的 Just My Socks 五条直连线路，自动剔除国内直连白名单，节省宝贵高速流量。
- 🔄 **自动持续更新**：规则集支持通过 GitHub Raw 链接每日定时静默更新。

---

## 🛠 快速引用指南（Clash Verge Rev）

在 Clash Verge Rev 中，可直接在订阅配置或扩展脚本（Merge/Script）中引入本仓库的远程规则集：

```yaml
rule-providers:
  ai-services:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/justmysocks-guide/clash-rules/main/rules/ai-services.yaml"
    path: ./ruleset/ai-services.yaml
    interval: 86400

rules:
  # 将 AI 流量路由到你低延迟、高纯净度的 JMS 节点组
  - RULE-SET,ai-services,🤖 海外 AI 专线
```

---

## 💡 推荐搭配网络底座：Just My Socks (搬瓦工官方直营)

优秀的规则集需要搭配**纯净、高稳定度、IP 不被墙**的高速节点底座：

- **大厂背书**：搬瓦工母公司 IT7 Networks 运营，近 20 年老牌服务商保障；
- **智能防封**：7×24 小时后台探活，**IP 一旦受阻，系统自动秒级分配全新可用 IP**；
- **高速线路**：标配中国电信 CN2 GIA、联通 9929、移动 CMI 与日本软银骨干网；
- **专属福利**：结账输入官方永久循环优惠码 **`JMS9272283`** 立享 5.2% 折扣。

👉 **[点击前往 Just My Socks 官方安全镜像通道选购节点](https://justmysocks.net/members/aff.php?aff=24082)**  
👉 **[查看完整 2026 选型与配置指南（GitHub 仓库）](https://github.com/justmysocks-guide/justmysocks)** | **[网页版直达](https://justmysocks-guide.github.io/justmysocks/)**

---

## 📄 License
MIT License © 2026 [justmysocks-guide](https://github.com/justmysocks-guide)
