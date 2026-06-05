<div align="center">

# half-second-skills

**李笑来《半秒》(The Half Second, 2026) 的可执行 AI Skill**

把"想改却改不掉"的下意识反应,翻译成一句能装进口袋的"自我对话",
让大脑里的频率计数器 (System 1) 替它装上新的第一反应。

</div>

---

## 这是什么

不是读书笔记,是一个**可被 AI 反复调用的工具箱**。它把《半秒》一整本书里的
框架、原则、技法、反模式、作者语气,提炼成结构化、可执行的指导。

核心引擎:**把任何"想改却改不掉"的下意识反应,翻译成一句符合 ARISE 五要素
(Action / Reason / Identity / Situation / Emotion)、能在自己声音里朗读的
短句,然后靠频次计数安装到半秒里。**

> 反复念、念到自己都觉得"这有点傻"——那就是计数器在装,别停。

---

## 它由什么组成

双平台分发 —— 同一个台账,两种 frontmatter 物理形态:

```
half-second-skills/
├── cursor/SKILL.md       多行 `>-` 折叠语法: Cursor / Claude Code 直装
└── openclaw/SKILL.md     单行双引号语法:     OpenClaw / Hermes 直装
```

正文(台账 + build 程序)逐字相同。**两者用 frontmatter 物理行数区别**,
非内容差异。OpenClaw / Hermes 的嵌入式解析器只吃单行 frontmatter 键,
所以单独提供一份。

台账结构(共 6 张主表 + 1 张速查):

| 章节 | 作用 |
|---|---|
| 调用纪律 | 3 条必须先遵守的规则(triage / 忠于原书 / 短输出) |
| 0. First move | 临床转介 + Breaking vs Building 分流 |
| 1. Frameworks | 半秒 / 频率计数器 / ARISE / 路由 / 安装 vs 理解 / 键盘等 9 个核心概念 |
| 1.x 易错点速查 | 4 对最常被读反的区分 |
| 2. Principles | 10 条脚本设计硬规则(三铁约束、诚实 scope、行动而非情绪……) |
| 3. Techniques | 10 个具体技法(泛 vs 情境决策、Langer because、四情绪通道……) |
| 4. Anti-patterns | 12 个高失败模式(情绪目标 / 未来时 / 列举情境 / 第 14 天放弃……) |
| 5. Author's voice | 李笑来原话金句(种子句 / 主权口号 / 收尾命令) |
| 6. Build procedure | 7 步写脚本流程 + 4 个书中范例 |
| 7. Ledger | 🟢🟡🟠 核心/中间/边缘的分级使用指南 |

---

## 安装

**Cursor**

```bash
git clone https://github.com/<your-account>/half-second-skills.git \
  ~/.cursor/skills/half-second-skills
cp half-second-skills/cursor/SKILL.md \
   ~/.cursor/skills/half-second-skills/SKILL.md
```

或手动把 `cursor/SKILL.md` 放进 `~/.cursor/skills/half-second-skills/SKILL.md`。

**Claude Code**

```bash
git clone https://github.com/<your-account>/half-second-skills.git \
  ~/.claude/skills/half-second-skills
cp half-second-skills/cursor/SKILL.md \
   ~/.claude/skills/half-second-skills/SKILL.md
```

**OpenClaw / Hermes**

```bash
git clone https://github.com/<your-account>/half-second-skills.git
cp half-second-skills/openclaw/SKILL.md \
   <workspace>/skills/half-second-skills/SKILL.md
# 或: ~/.agents/skills/half-second-skills/SKILL.md
# 或: ~/.openclaw/skills/half-second-skills/SKILL.md
```

---

## 怎么用

装好后正常对话即可被自动召回(读 `description` 命中),或手动喂 SKILL.md。
四大族触发场景,说中任一种就会跳出来:

| 族 | 你会怎么描述 | 它会做什么 |
|---|---|---|
| **戒不掉** | "道理我都懂就是做不到""又破戒了""21 天没用""管不住自己" | 诊断是 Breaking 还是 Building,匹配反模式,给一句能装的短句 |
| **关系里下意识** | "我俩又冷战了""他这么说我怎么回""忍不住跟孩子发火" | 调"刺激 vs 旧反应"分离,写情境脚本("当她开口,先听三秒再回") |
| **钱和冲动** | "又追涨杀跌了""账单都不敢拆""看到就买" | 给"我决定看周不看分"类决策句,装计数器 |
| **内在批判 + 建立新习惯** | "我总觉得自己不够好""写作/运动/冥想坚持不下来" | 先 map the voices,再写"四情绪通道"安装,配 stack 与锚定 |

显式点名也会命中:直接说"想聊聊《半秒》""帮我用 ARISE 写个自我对话"
"System 1 counts it does not check" 即可。

---

## 致谢与边界

- 方法论全部来自李笑来《半秒》(2026)。本仓库是对其方法的**结构化提炼
  与工具化**,所有引述均忠于原著,不编造框架、数字或案例。
- **与 NVC(非暴力沟通)无关**——本 skill 关注的是"自己装自己的第一反应",
  不是"与他人沟通的话术"。如需沟通侧工具,请另寻其他资源(如
  [ayi-nonviolent-communication](https://github.com/ayi-ai/ayi-nonviolent-communication))。
- **临床边界**——创伤/成瘾/精神危机一律转介专业,不在本 skill 能力范围。
- 想深入,请支持购买正版原书。

## License

[MIT](./LICENSE) © 2026
