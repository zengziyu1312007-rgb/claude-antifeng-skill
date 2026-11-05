# Claude 账号防风控 Skill

> 一套合规、可落地的 Claude（Anthropic）账号使用方法，帮你降低被误风控 / 误封的风险，并在异常时知道怎么自查和申诉。

## 为什么需要这个

Claude 账号被风控，绝大多数时候不是"做错了什么大事"，而是日常使用习惯偏离了正常用户画像：

- 网络环境频繁切换，IP 到处跳；
- 一天之内多地登录、多设备并发；
- 调用频率远超订阅档位的正常范围；
- 内容触到 Usage Policy 的灰区；
- 注册时身份 / 支付信息不一致。

这个 Skill 把这些坑整理成 **可执行** 的清单，而不是玄学。

## ⚠️ 合规声明

本仓库 **只覆盖合规使用建议**，包括：

- ✅ 真实身份注册与合规支付
- ✅ 稳定网络环境配置
- ✅ 合理使用频率
- ✅ 内容合规边界
- ✅ 账号异常自查与官方申诉

**不包含**，也 **不会包含**：

- ❌ 绕过 Anthropic 安全审核 / 内容过滤
- ❌ 规模化共享、倒卖、出租账号
- ❌ 伪造身份、盗用支付信息
- ❌ 任何违反 [Anthropic Consumer Terms](https://www.anthropic.com/legal/consumer-terms) 与 [Usage Policy](https://www.anthropic.com/legal/aup) 的内容

如果你要找的是上面这类东西，这里没有，也不应该有。

## 目录结构

```
claude-antifeng-skill/
├── SKILL.md                          # Skill 入口（带 frontmatter）
├── README.md                         # 你正在看的这个
├── LICENSE
├── docs/
│   ├── 01-账号注册合规.md
│   ├── 02-网络环境管理.md
│   ├── 03-使用规范.md
│   ├── 04-内容合规边界.md
│   ├── 05-异常自查清单.md
│   ├── 06-申诉与恢复.md
│   └── 07-多账号合规管理.md
└── checklists/
    ├── 账号健康自查.md
    └── 异常应急流程.md
```

## 怎么用

### 作为阅读材料

直接按 `docs/01` → `07` 顺序读，每篇 5–10 分钟，看完就知道怎么把账号用稳。

### 作为 AI Agent Skill

`SKILL.md` 带标准 frontmatter，可被支持 Agent Skill 加载的工具（如 Claude Code、Claude.ai Agent Skills、兼容的本地 Agent 框架）挂载为技能库。加载后，Agent 在用户提到"Claude 账号风控/被封/异常"时自动调用本指南。

### 作为自查清单

`checklists/` 下的两份清单可以每周跑一次健康自查，或异常时按应急流程逐项排查。

## 适用对象

- Claude Free / Pro / Max 个人订阅用户；
- 通过 Claude API 做个人项目的开发者；
- 团队中需要给同事分享"怎么用 Claude 不会被封"的人。

不适用：想搞账号农场的人（见合规声明）。

## License

MIT，见 [LICENSE](./LICENSE)。

## 贡献

欢迎提 Issue / PR 补充实战经验，但请保持合规边界。涉及绕过审核、共享账号农场类的 PR 会被直接关闭。