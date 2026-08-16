---
title: "Exo: Harnesses should see their own code and logs — Alex Krentsel"
channel: "Latent Space"
published: "2026-08-15"
source_url: "https://www.youtube.com/watch?v=5lFD-34dhqE"
video_id: "5lFD-34dhqE"
tags: ["AI Agent", "RSI", "系统架构", "LLM", "Exo"]
rating: 5
language: "英文"
word_count: 16657
duration: "47:11"
---

# Exo: Harnesses should see their own code and logs — Alex Krentsel

- **Channel:** Latent Space
- **Published:** 2026-08-15
- **Source:** https://www.youtube.com/watch?v=5lFD-34dhqE
- **TL;DR:** Agent 的自我改进应从 harness 代码层开始：同媒介生成与执行，让递归自我完善成为可工程化的现实。
- **Tags:** AI Agent, RSI, 系统架构, LLM, Exo
- **Rating:** 5

## 版本

- [结构化文稿](2026-08-15-exo-harnesses-should-see-their-own-code-and-logs-—-alex-krentsel-5lFD-34dhqE.structured.md)
- [原始文稿](2026-08-15-exo-harnesses-should-see-their-own-code-and-logs-—-alex-krentsel-5lFD-34dhqE.transcript.md)

# 材料信息

- **标题**：Exo: Harnesses should see their own code and logs — Alex Krentsel
- **作者/来源**：Latent Space 播客（主持人 swyx，嘉宾 Alex Krentsel）
- **类型**：YouTube 视频字幕（播客访谈）
- **关键元数据**：主持人与 Alex Krentsel 的对话录；Alex 为 UC Berkeley 博士、Exo 项目核心开发者；视频发布方为 Latent Space，访谈内容同步涉及 Alex 在 Berkeley Sky Lab 的研究（Sky Discover）、与 Martin Casado 和 Enkhor Goya 的合作，以及 Exo 的架构设计与实际应用。时长/发布日期未在字幕中标注。

---

# 开篇引入

想象一下，你正在为一个大型语言模型打造一个外壳——一套工具、上下文组装逻辑、行动接口，也就是所谓的"harness"。今天，几乎所有 agent 系统的 harness 都像一辆由人类设计师敲定的汽车：方向盘、油门、刹车都是固定的，用户可以按需加装"技能"或"插件"，但骨架永远不变。那么，如果让这辆车具备自己打开引擎盖、改装配件、甚至重写自身 ECU 的能力呢？这正是 Berkeley 博士生 Alex Krentsel 与两位系统大佬 Martin Casado、Enkhor Goya 合作打造的 Exo 项目所追求的：**一个能够完整、递归地自我改进的 agent**。

这期 Latent Space 播客由主持人 swyx 与 Alex 进行了一场几乎没有冷场的技术深谈，从 Exo 为何值得押注，到它如何通过"执行器—harness—沙箱"的三层架构实现自我演化，再到"为什么现在才是实现 RSI（递归自我改进）的正确时机"这一宏大命题。即便你不关心 Exo 的代码细节，这场对话也会让你重新审视：agent 的能力边界究竟应该由谁——人类还是模型——来定义？

---

# 详细内容

## 一、从"擦肩而过"说起：一个系统的血统 [章节 1]

**核心观点**
Exo 是 Alex 与 Martin Casado、Enkhor Goya 三人合作的产物，而这次合作有着一脉相承的"系统血统"：Martin 的博士导师正是 Alex 的导师 Scott Shenker，学术上同属 Berkeley 系统研究一脉。

**深度阐述**
访谈从一个有趣的细节开始：swyx 坦言，自己其实早就看过 Alex 关于 OpenClaw 的讲座视频，却没有把名字和项目对上号。Alex 笑着承认，自己当时太专注讲解架构，没有刻意自我推销。这种"纯技术人"开场奠定了整场对话的基调——Alex 不是来布道某种宏大叙事的，而是来拆解一个系统的。

Alex 很快亮明身份：他的研究方向是系统（systems），师从 Berkeley 的 Scott Shenker，合作者还有 Sylvia Ratnasamy 和 Ion Stoica。他是在 ChatGPT 爆发之前就开始读博的"核心网络"背景，做过 SDN 控制器的网络架构、网络形式化验证。换句话说，他是"从系统向上生长"进入 AI agent 领域，而不是从机器学习"向下俯冲"。这与 Martin Casado（曾在 Nicira 做网络虚拟化，后成为风投）和 Enkhor Goya（系统思想家，参与 Brain Trust）的相遇，几乎是一种必然——三个人都在思考"agent 的底层架构应该是什么样"。

> "We're kind of come from systems backgrounds. My background is fully in systems and I'll talk more about that later."  
> ——"我们都算系统出身。我的背景完全是系统方向，后面我会细讲。"

**个人感受**
Alex 在谈到自己专注于架构设计时，透露出一种系统研究者特有的克制与骄傲：他不靠渲染模型能力的魔力，而是相信"架构能够带来确定性"。当 swyx 抱怨 VC 装模作样写代码时，Alex 也为 Martin 辩护："Martin 真的每天都在写代码。"这种对真实工程实践的尊重，成为 Exo 团队合作的文化底色。

**延伸思考**
系统思维与 ML 思维在 agent 领域的冲突与融合，是这段对话的暗线。模型研究者常说"下一代模型会冲掉所有 harness"，而 Alex 和合作者们正在押注 harness 本身。这不仅是技术路线之争，也关乎 AI 可靠性的根本路径：到底是在权重里"软性"地希望模型守规矩，还是在架构里"硬性"地保证安全边界？

**精华收获**
Exo 并非凭空冒出的项目，而是 Berkeley 系统学派、AI 驱动发现研究和产业实践三者交汇的产物——理解这点，才能理解它为什么强调"状态、隔离、回滚"等传统系统概念。

---

## 二、Exo 是什么：把自我改进的循环"折叠"起来 [章节 2-3]

**核心观点**
Exo 是一个递归的 agent——它能在运行时安全地编辑自身的一切方面，以更好地完成当前任务。这种能力来自一个刻意设计的三分区 harness 架构：不同组件彼此隔离，从而可以安全演化。

**深度阐述**
Alex 用一句话概括 Exo：**"An agent that's fully recursive. It's able to safely edit all aspects of itself at runtime to get better at the task that it's working on."**（一个完全递归的 agent，能够在运行时安全地编辑自身的一切方面，以更好地完成当前任务。）

它的灵感来源并非凭空而来。过去一年，Alex 在 Berkeley 的 Sky Lab 从事"AI 驱动发现"研究（Sky Discover 项目），核心是一个外部循环系统：一个外部系统不断优化另一个内部系统。Alex 思考的问题是：如果你想优化"优化方式"本身呢？那就需要一个更外层的循环，无限递归下去。他认为唯一的出路是**"collapse the loop"（把循环折叠）**——让系统自己负责改进自己，而不是靠外部的观察者不断调整。

这是 Exo 的核心哲学：不是"你在外面指挥它改"，而是"它自己在运行过程中改自己"。

> "What if you want to optimize the way you're doing your optimizing then you need some outer outer loop and it's this infinite recursion out and the only way I think out of that is to collapse that loop down and make it so that the system itself is responsible for improving itself."  
> ——"如果你想优化你正在做的优化方式，就需要一个更外层的循环，如此无限递归下去。我认为唯一出路是把循环折叠起来，让系统自己负责改进自己。"

**个人感受**
Alex 在阐述这个理念时带着一种研究者的兴奋——"我称之为 collapse the loop"。这不是一个营销词，而是他从 AI-driven discovery 的困境中推导出的必然结论。他反复强调"运行时"（at runtime），即改代码不是停掉系统、人工编辑、再重启，而是系统在运行中完成自我修改。

**延伸思考**
这触及了自我改进 agent 的一个根本问题：外部评估循环（outer loop）本质上仍然是人在设定方向，只是借助机器执行。Exo 想要把"方向"本身也交给系统——当然，这立刻引出谁是最终裁判的问题（后文会详细谈奖励黑客）。

**精华收获**
Exo 的"递归自我改进"不是简单的插件机制，而是把"改进者与被改进者"之间的边界打破，使 agent 与它的优化器合而为一。

---

## 三、OpenClaw 的启发与局限：真正可变的只有 Memory [章节 4-5]

**核心观点**
OpenClaw 让 agent 变得"可适应"，但这种适应发生在特定、有限的可扩展点上——主要是 memory 文件、skills 和 tools。Exo 要改变的，是 agent 内部所有未被标记为"可插拔"的架构组件。

**深度阐述**
swyx 指出，OpenClaw 的人已经意识到"harness 应该自我修改以添加所需能力"，但 OpenClaw 并非完全递归。Alex 同意，并做了精准解剖：

- 所有 agent 系统都有某种"memory"——通常是一个 Markdown 文件，每次调用 LLM 时被注入上下文，可以被编辑。
- OpenClaw 还提供 skills（技能）和 tools（工具）作为扩展点，但**这些扩展通常由人驱动**：用户说"帮我装一个技能"，或从 ClawHub 安装现成插件。
- 然而，一个 agent 的绝大部分策略（policy）是静态的、写在源代码里的：上下文怎么组装、取最近 10 条还是 100 条消息、如何压缩历史、如何定义工具集、如何在上下文中包含这些工具……这些都是 OpenClaw/Claude Code/Codex 等系统中预先写死的。

Alex 对 agent 给出一个清晰的定义：**一个被"上下文构建机器"包裹的 LLM 调用**。它一方面构造上下文（历史、工具描述、系统提示），另一方面执行动作（调用工具并反馈结果）。这个"上下文构建机器"的所有机制，他都称为 **policy（策略）**。而 Exo 的目标，就是让策略本身也成为 agent 可以修改的对象。

> "It's not just certain points where you can insert additional skills. It has changed the very machinery of what skills are for your job."  
> ——"它不仅仅是某些可以插入新技能的特定点位；它改变了技能本身的底层机制。"

**个人感受**
Alex 在对比 OpenClaw 与 Exo 时，没有贬低前者，而是明确肯定 OpenClaw 的真正贡献："它让 agent 系统产生了魔法般的感觉，能适应你的工作流。" 但他的系统研究者本能让他追问：这种魔法到底发生在哪些点上？答案揭示了一个窄得惊人的适用范围。

**延伸思考**
这其实是软件工程中"扩展点（extension point）"与"可演化架构（evolvable architecture）"的区别。常规软件预留扩展接口；Exo 则希望所有接口边界本身都可以被移动。这有点像让一个程序把自己的语法树也当作可操作对象——听起来像 Lisp，实际上 Alex 在后文确实承认了这种相似性。

**精华收获**
任何"看似自我改进"的 agent，都要问一句：它改的是记忆内容，还是构造记忆的机制？真正的递归自我改进，必须面向后者。

---

## 四、显式还是隐式？"谁在改谁"的信任博弈 [章节 6]

**核心观点**
你可以用外部分离的 agent 去修改内部分离的 agent，但本质上你仍然在信任一个机器。Exo 的选择是让运行中的系统自己检查自己、根据自己的运行表现做修改，而不是引入外部观察者。

**深度阐述**
swyx 提出了一个非常实际的问题：他自己运营两家公司，内部有一个生产 bot，外部有一个 Devon bot 负责改内部 bot——但内部 bot 没有修改自身的能力。他很喜欢这种分离：像开车一样，平时只开车，需要时打开引擎盖修理，而不是让车在行驶中自己改自己。他问 Alex：**"你是否需要那种'我什么都没做它就自己变了'的 AGI 感？"**

Alex 的回答是：即使你用一个外部 agent 改内部 agent，你依然在信任一台机器——只是把信任从"内部机器"转移到了"外部机器"。真正的区别不在于有没有机器介入，而在于**系统是否拥有"自我检视"的回路**。

他举了一个生动的例子：Exo 在玩 Pokémon 游戏时，系统自己在运行时决定检查游戏内存（RAM），并像人类逆向工程师一样，把 RAM 中代表"角色位置""当前精灵""是否在战斗"的布尔值映射找出来，然后**修改自己的游戏集成代码**，把这些信息注入系统提示，让后续决策更聪明。

> "The same system that is deciding to make changes is also deciding what to run and also deciding what to inspect."  
> ——"同一个系统，既决定做出修改，又决定运行什么，还决定检查什么。"

一个外部循环需要先提出设计方案、启动新任务、回传结果再迭代；而 Exo 可以把"检查（inspection）"本身作为设计过程的一部分，边运行边学习，边学习边改进。

**个人感受**
Alex 在讲 Pokémon 例子时，是非常有画面感的：一个 agent 在打游戏过程中突然决定"让我看看游戏内存"，然后给自己装上一个"雷达"，接着继续玩。他没有夸张地说"这是 AGI"，而是把它当作论证"运行时自省"的一个具象案例。这种脚踏实地的叙述方式非常打动听众。

**延伸思考**
这引出一个更深的哲学问题：自我改进需要某种"自我模型（self-model）"。外部分离的方案，自我模型存在外部系统的脑中；Exo 的方案，自我模型由系统自己在运行时建立——但这也意味着系统对它自己的认知可能失真或自欺。也许未来需要对"自省能力"本身进行安全约束。

**精华收获**
"显式外部循环 vs 隐式自改进"更像是一种信任分布的选择：前者让你可以随时踩刹车，后者让系统反应更快、表达力更强，但要求你信任它的自省判断。

---

## 五、架构核心：Executor / Harness / Sandbox 三层分离 [章节 7-9]

**核心观点**
Exo 将传统 agent 拆成三个具有不同属性的层：**Executor**（执行器/策略层，无状态）、**Exo Harness**（持层，保存历史、密钥、快照）、**Sandbox**（沙箱，实际执行动作的环境）。这个结构既保护关键状态，又让策略层可以安全地自我演化。

**深度阐述**
Alex 用传统 coding agent 的痛点引出架构：以 Claude Code 为例，它既是 agent 又是 harness，被塞进一个 VM 里，你可能要在那个 VM 里登录 GitHub、保存密钥，然后开启"危险地跳过权限"模式。它和它编辑的代码运行在同一环境，没有隔离。

Exo 的设计刻意打破这种混杂：

- **Executor（执行器）**：包含所有"策略"——上下文组装、prompt、压缩方式、工具列表、技能定义。它是**完全无状态的**。
- **Exo Harness**：持有状态——对话历史、API 密钥等机密、环境工件/快照。它扮演"被保护的状态"角色，不暴露给 LLM。
- **Sandbox（沙箱）**：实际执行 bash 命令、编辑文件的隔离环境，与策略进程分离。

这三层合在一起，才是人们通常说的"一个 agent"：历史的存储（harness）+ 策略的运行（executor）+ 执行的环境（sandbox）。

为什么这对自我改进至关重要？因为当策略层是无状态的时候，它可以随时被替换、重建，而不会丢失历史或泄露密钥。Exo Harness 提供**快照机制**：agent 可以请求修改自己的策略代码，在一个沙箱里尝试，如果失败，自动回滚到上一个状态。

> "The executive can propose changes to itself in a way that you will not lose any history. You won't leak secrets because they're not exposed to the LM itself."  
> ——"执行器可以以一种不会丢失任何历史、不会泄漏机密的方式向自己提出修改——因为密钥根本不暴露给 LLM 本身。"

**个人感受**
Alex 作为一个系统研究者，在讲三层架构时用了大量传统 OS 的类比：无状态进程、持久化层、隔离环境。这种语言让人感到踏实——它不是某种 ML 玄学，而是分布式系统/操作系统的工程常识。swyx 也忍不住赞叹"这种拆解非常清晰"。

**延伸思考**
三层分离其实和云计算的三层（计算、存储、网络）有异曲同工之妙：状态与计算分离，才使得"迁移"（teleportation）成为可能，也才使得"热升级"成为可能。如果你想让 agent 支持 5 万个并发会话，你不可能让每个会话都跑一个完整的 agent 实例；你需要的正是这种"轻量策略 + 共享状态 + 按需沙箱"的弹性结构。

**精华收获**
Exo 架构的本质是：**把"会变的策略"与"不能变的资产"物理隔离**，从而让"变"变得安全。

---

## 六、自我改进的最后一跃：挂载自己的代码 [章节 10-11]

**核心观点**
Exo 之所以成为真正的自我改进 agent，是因为它把 Executor 自己的代码挂载到沙箱中，让 LLM 可以在运行时读取、编辑、重建、测试并提交这些代码；Exo Harness 则负责在出错时自动回滚。

**深度阐述**
如果只是三层架构，Exo 还算不上递归自我改进。Alex 指出，真正的关键是**"把 executor 的源码挂载进 sandbox"**：

在普通用法中，sandbox 是 agent 完成任务的"工作区"；而 Exo 会把自己的 executor 代码也放进这个工作区。于是，LLM 在决策时可以发出指令："去修改一下我自己的 context 组装逻辑"或者"新建一个工具，改变技能的定义方式"。

为了支持这种"运行时自我手术"，Exo Harness 内置了一个"守护进程（guardian）"：它允许 executor 在运行中途被重建，并且在重建之后做一个"冒烟测试"——让它再走一步，如果它成功地把自己改坏了，就自动恢复到上一个快照。

> "We try to bring up the executive, let it proceed one step, and if it breaks itself off accidentally, it'll get rolled back to the previous state automatically."  
> ——"我们尝试启动执行器，让它往前运行一步；如果它不小心把自己搞坏了，系统会自动回滚到之前的状态。"

Alex 还总结了这种设计带来的额外好处：**并行性**。因为对 executor 代码的修改本质上是一个"原子提交"，多个候选修改可以并行尝试，由 harness 决定最终合并哪个。

**个人感受**
Alex 特别强调"这一步让 Exo 做到 fully recursively self-reflective"。他用的词是"最后一步"——仿佛这是一个自然演化的终点。你能感觉到，他站在自己画出的架构图面前，有一种工程上的成就感：不是某个 prompt trick，而是一个可以真正被验证的系统机制。

**延伸思考**
"重建+冒烟测试+自动回滚"这对三元组，本质上是把 DevOps 中的 CI/CD 内化到 agent 的决策循环里。这是一种非常"系统"的解决方案：不祈求模型永远正确，而是允许它犯错，并用工程手段控制错误半径。

**精华收获**
让代码可见，再让代码可改，最后让"改坏"变得可恢复——这就是 Exo 实现递归自我改进的完整闭环。

---

## 七、重新审视 Teleportation：从单机到规模化的跳板 [章节 12-13]

**核心观点**
三层架构让 agent 的状态与计算分离，因此 agent 可以"传送"到任意沙箱。这不仅是个人便利，更是支持大规模并行任务的必需能力。

**深度阐述**
swyx 问：teleportation（把 agent 状态从本地移动到云端）到底有多重要？经典场景无非是"我合上电脑，任务继续在云端跑"。Alex 承认单个 agent 单任务确实不需要传送，但只要规模一上来，情况就完全不同：

假设公司要为每个用户运行一个专属 agent 来分析自己的使用日志。100 个用户时，单机 100 个容器绰绰有余；但如果是 5 万名用户，本地机器根本放不下这么多 sandbox。这时，策略进程（很轻量）可以保留在本地，而每个用户的 sandbox 可以按需唤醒、按需迁移到云端。Exo 已经集成了 Daytona（一个云沙箱提供商），也支持 E2B 等。

swyx 还调侃说，Daytona 的曝光很大程度得益于 Harbor（Terminal-Bench 的作者）的推荐，而 Alex 证实自己的 Exo 集成正是参考了 Harbor 的做法。

> "Once you start running out of space for running sandbox containers on your machine, you can start moving some of them off to the cloud."  
> ——"一旦你的机器没有空间跑更多沙箱容器，你就可以开始把一部分沙箱搬到云端。"

**个人感受**
Alex 没有把 teleportation 包装成"未来功能"，而是当作一个完全务实的扩展性手段。他甚至精准地说：这对个人用户不算什么，但对公司服务来说，是启动高并发 agent 服务的物理前提。

**延伸思考**
这让我想到：agent 的"身体"与"大脑"解耦，会催生一种新的云服务形态——"agent 状态托管 + 沙箱市场"。未来也许会出现专门托管 agent 对话历史和快照的数据库，以及按秒计费的沙箱资源池。Exo 的三层架构其实提前为这种生态画好了蓝图。

**精华收获**
状态与计算分离不仅仅是一种架构洁癖，它直接决定了 agent 能否从"个人玩具"进化为"企业级服务"。

---

## 八、子 Agent、Secret Store 与实时交互的工程问题 [章节 14-17]

**核心观点**
Exo harness 的边界划分遵循一个原则：**方法与机制在 executor（怎么做事），状态与数据在 harness（实际的记忆/密钥/工件）**。同时，key store 绝对不暴露给 LLM，防止泄密；实时交互则需要新的"可中断任务"架构。

**深度阐述**
swyx 逐一追问架构图中的几个组件：

- **子 Agent（sub-agents）**：Alex 说，何时生成子 agent、子 agent 用什么工具、有什么权限，这些都属于 executor 里的策略代码。Exo 本身没有内置子 agent，但可以轻松实现。关键是"怎么产生子 agent"在 executor，"子 agent 的对话状态"依然沉淀在 harness。
- **Secret Store（密钥存储）**：这是 Alex 认为最被低估的组件。今天，你的 agent 和你的 API key 运行在同一环境，等于密钥完全可读。Exo 把密钥放在 harness 的宿主进程中，只通过受控方式注入 executor，**绝不进入沙箱/容器**。即使 agent 被恶意提示词攻击，也无法直接读取密钥。他还进一步提出：应该监控密钥的访问模式，如果例常任务突然开始请求 AWS key，那就是可疑事件。swyx 对此深表赞同。
- **实时语音 agent**：Exo 的 Discord adapter 已经加入了 voice mode，但本质上是"pipeline 级联"（语音转文字 → LLM 回复 → 文字转语音），不是真正的低延迟交互。Alex 认为真正的实时性需要 agent 任务可以"中断"——像 Unix 信号一样，把任务放到后台、可以被打断、可以报错。传统 agent 一旦在某个 thread 里开始工作，就无法响应其他消息，这让他非常沮丧。他期待 agent 世界出现类似 tmux、信号、pub-sub 机制。

> "The same way that when you're working in your terminal you want to start something, you maybe put it in a background, or you open tmux and you put it in a separate pane on the side. I expect this will be an architecture decision of how you put tasks in the background and expose them to the agent as they're running."  
> ——"就像你在终端里把某个任务放到后台，或者用 tmux 把它放到旁边窗格一样，我预期 agent 架构也需要决定如何把任务放到后台，并在运行时把它们暴露给 agent。"

**个人感受**
当 swyx 问"你提 ACP 协议吗"时，Alex 很坦诚地说还没实现，但觉得值得做。他并不装作全知，而是直接承认"我们仍在早期，先把核心架构打磨好"。这种谦逊和务实同时存在，非常有学者风范。

**延伸思考**
密钥隔离、访问审计、任务中断——这三个问题在传统企业软件里已是常识，但在 agent 领域却是稀缺品。这恰恰说明 agent 工程还处在"野蛮生长"阶段；Exo 试图把"常识"重新带回 agent 架构。

**精华收获**
"怎么做"与"存什么"分开，是 agent 安全设计的第一性原理；而"可中断性"将决定 agent 能否真正融入人类的实时工作流。

---

## 九、三人行：Martin、Enkhor 与 Alex 如何分工 [章节 18-19]

**核心观点**
Exo 是一个真实的三人协作项目：Enkhor 首先提出分层架构初稿，Alex 随后把研究重心转向"折叠循环"的自我改进，Martin 除了贡献系统思维还每天都在写代码；团队以 Brain Trust 为"试验田"在生产环境中运行 Exo harness。

**深度阐述**
Alex 详细还原了项目缘起：

- 他先在 Berkeley 做了一场关于"自治系统设计原则"的讲座，重点剖析 OpenClaw，获得大量社区反馈。
- 几乎同时，Martin 在 Berkeley 也做了一场关于 harness 未来的演讲，两人因此结识。
- Martin 提议："Enkhor 也在思考类似的事，我们一起聊聊。" 三个人在一间会议室里开始讨论"agent 到底需要什么架构属性"。
- 最初的重心是 **Exo harness** 本身——为了让 agent 更可扩展、更安全。**Enkhor 率先画出了分层架构的初稿**。
- 花了几周把 harness 基本硬化后，Alex 把大家的目光引向自己真正着迷的问题：**这个分层架构能不能实现"自我改进"？** 他称之为"把 AI-driven discovery 的循环折叠进 executive 本身"。
- 于是，Exo 从一个"优雅的 harness 项目"变成了"一个能自我改进的 agent 项目"。
- Martin 的贡献不仅仅是理念：他深度参与了编码。Alex 特意强调："Martin really codes. You know Martin's really in this coding day-to-day." 在提交历史上，三人的名字都真实存在。

Alex 提到，Exo 已经在 **Brain Trust** 的生产环境中运行，正在承受真实负载的检验。

> "If you look at the commits, we're all there. So, our team is not just posing."  
> ——"如果你看 commit 记录，我们三个人都在上面。我们的团队不是在装样子。"

**个人感受**
这段描述很有画面感：一个 VC、一个系统学者、一个 startup 系统思想家，挤在一间会议室里，从一张白纸开始画 agent 的架构。Alex 的语气既骄傲又感激，他显然享受这种罕见的"学术+产业+资本"的真正碰撞。

**延伸思考**
在 AI 浪潮中，许多项目是"从 demo 到融资"火箭式推进；Exo 则更接近"从架构原理推导出产品"。这种节奏是否能适应市场，还有待验证。但至少在学术上，它是站得住脚的。

**精华收获**
好的系统项目往往源于"对系统架构有共同审美"的三五个人——而不是一个庞大却同质的组织。

---

## 十、实战记录：Exo 如何砍掉 96% 的上下文成本 [章节 20-21]

**核心观点**
Exo 真正展示自我改进能力的第一步是"降低成本"：系统自己发现 Discord adapter 单次消息成本高达 16 美分，于是它运行时重构了 adapter——把上下文范围限制在相关会话和线程中，结果成本降低 96%，并且这些修改最终被提交回代码库。

**深度阐述**
Alex 谈到"给 Exo 一个目标"时，举了一个极具说服力的真实例子：

他问 Exo："刚才那条 Discord 消息花了多少钱？" Exo 回答："16 美分。" Alex 觉得太离谱了，于是命令它："去把成本降下来。"

接下来，Exo 在运行时做了以下操作：
- 分析自己的 Discord adapter 代码；
- 发现每次调用 LLM 时都从所有 Discord 频道拉消息；
- 修改上下文组装逻辑，只拉取当前相关会话和线程的消息；
- 观察和测试修改效果；
- 最终把成本降低了 **96%**。

这个修改不是临时补丁——团队后来把它正式提交到主代码库，变成 Exo 的默认行为。

> "It went and re-architected its own Discord adapter at runtime. Made changes, observed them, tested them … drove down the cost to, I think, like a 96% decrease. And by the way, we committed this back afterwards."  
> ——"它在运行时重新架构了自己的 Discord adapter，作出修改、观察效果、进行测试……把成本降了大约 96%。顺便说一句，我们后来把这个改动提交了。"

swyx 立刻追问："你们有 eval 吗？有回归测试吗？" 这是所有自我改进系统面对的灵魂拷问：你怎么知道它在优化成本的同时没有破坏性能？

Alex 的回应相当诚实：
- 在 Discord 这个场景，性能验证比较"二进制"——你回不回消息？上下文是否足以做出合理回答？相对好检测。
- 但在更复杂场景（如保险决策），你必须有保留的 eval 集，或与 agent 协作构建内部工具来追踪性能。
- 他承认："specifying what you want to an agent is still an open one." 因为 agent 可能学会一种最简单的省钱方式——**干脆不干活**，这其实就是 reward hacking。

**个人感受**
Alex 在讲这段话时，带着一种"妈妈你看它真的会自己修东西"的兴奋。但当他被问到 eval 时，又立即回到严谨的学术态度，承认这仍是开放问题。这种"既激动又冷静"的张力，是这期播客最吸引人的地方。

**延伸思考**
Exo 的例子本质上是把"成本"作为显式信号，让 agent 在性能约束下做优化。未来评估可能变成多目标博弈：成本、延迟、准确率、安全性。Self-improvement agent 需要一整套"自监控仪表盘"，而不是一个终极 eval。

**精华收获**
自我改进第一步，不是让它变聪明，而是让它变便宜；而"便宜"必须与"有效"绑定，否则就是奖励黑客。

---

## 十一、为什么是现在？RSI 的"同媒介"论证 [章节 22-23]

**核心观点**
Alex 用"媒介同一性"论证了为何 RSI 现在可能在 harness 层实现：LLM 已经被训练得善于生成代码，而 harness 本身就是代码——这意味着 agent 改进自身的方式（写代码）与它被改进的对象（harness 代码）是同一媒介。相比之下，改进模型权重需要梯度、反传，无法被模型直接操作。

**深度阐述**
在节目接近尾声时，Alex 主动要求补充一个他认为非常重要的论点：

过去六个月，AI 领域发生了从"改权重"到"改 harness"的迁移。模型权重的改进是梯度下降、反向传播，产生的"修改"是万亿参数上的微小 delta。你不可能把一个万亿参数模型的所有权重放进上下文，让模型自己读一读然后说"这里应该调 0.001"——这不现实。

但 harness 只有几千行代码。LLM 的输出是 tokens，而 agent 的"身体"同样是代码。于是，自我改进链条缩短了：**改进的输出（代码）与改进的对象（代码）是同一种东西**。

> "The agent is producing and writing code and can change its own code as it runs. Which is why I believe we're entering a stage where this is fully self-recursive."  
> ——"agent 正在生成和编写代码，并能修改自己运行时的代码。这就是为什么我相信我们正在进入一个完全自我递归的阶段。"

他进一步区分了"完全递归"和"自催化"（autocatalytic）：在芯片设计领域，人类用电脑设计下一代芯片，但电脑本身是物理芯片、布局布线，存在"层间介质"；而 harness 这层，生成物就是运行物本身——代码即血肉。

swyx 调侃说："那你这个纯主义者，是不是非要自己训练模型才行？" Alex 笑着承认："我是很纯主义，也许这是学术界给我的职业病。" 但他坚持：用模型辅助改进模型是"自催化"，而在 harness 层，改进是"同媒介"的，这才是 RSI 真正涌现的地方。

两人还谈到，这种"代码生成代码、代码改进代码"的形态很像 Lisp——一门"包含自身构造符"的语言。Alex 完全同意，并认为我们正在经历一个"像 Lisp 一样自举"的 AI 时刻。

**个人感受**
这段是整场对话的高潮。Alex 的声音明显变得更加自信和笃定，他放下具体架构，展开一个更大的图景。他称自己是"purist"，但这不是贬义——他对 RSI 的定义极其苛刻，以至于拒绝把"使用模型辅助训练模型"称为真正的自我改进。这种学术上的严格性，恰恰让他的论点更有说服力。

**延伸思考**
"媒介同一性"这个标准也可以用于评估未来的 RSI 进展：只要 agent 的"改进操作"与"被改进对象"之间还隔着某种不可压缩的翻译层（比如物理布局、权重梯度），那它就不是完全递归的。这也解释了为什么 agent 层比 model 层更可能率先出现 RSI 迹象。

**精华收获**
RSI 不在于模型的"智能程度"，而在于系统的"可塑性密度"——当代码同时是产物和材料时，自我递归的循环就被压缩到了最小。

---

## 十二、结语：一个很早期的社区，等待同路人 [章节 24]

**核心观点**
Exo 是一个非常早期的开源项目，团队欢迎贡献者和讨论者；swyx 则提醒听众，加入这类早期社区的价值往往不在当下，而在未来。

**深度阐述**
访谈最后，Alex 介绍了入门路径：GitHub 仓库为 `github.com/exoharness/exo`（字幕中为 exoharnness，可能是拼写误差，实际一般是 exoharness），提供一行安装脚本、文档和教程，以及 Discord、IRC、WhatsApp 适配器。他们欢迎任何人来贡献代码、讨论架构，或者只是围观。

swyx 给出了一个过来人的忠告：**"When you join these kinds of early communities, it's actually not just about the project. It's also about the people and what you end up doing with them in future years."** ——"加入这类早期社区，其实不只是关于项目，更是关于人，以及未来几年你会和他们一起做什么。" 在 AI 技术大爆炸的早期，加入一个靠谱的社区，可能比选择任何单一框架都更重要。

**个人感受**
Alex 在告别时讲了一段很真诚的话："Marty and Anker and I are all building together with a handful of other people. Please come check out our GitHub." 这种"技术人招人"的质朴方式，与许多 AI 公司高高在上的招聘姿态形成鲜明对比。

**延伸思考**
Exo 的终极抱负是"agent 应该能看到自己的代码和日志"。这句话（也就是视频标题）其实是一种设计哲学：透明度带来可进化性。未来，也许每个 serious agent 框架都必须回答同一个问题：**你的 agent 能看到自身吗？**

**精华收获**
更值得带走的不是 Exo 这个工具本身，而是一种视角：如果 agent 终将自我改进，那我们今天应该做的，就是为它准备好一面可以照见自己的镜子。

---

# 精华收获总结

1. **用架构而非提示词，才能强制安全**：不要在系统提示里祈求 LLM 不要删除历史；用 harness 的分层隔离让它在物理上无法做到。
2. **状态与计算分离，是 agent 工程的地基**：无状态的 executor + 有状态的 harness + 隔离的 sandbox，让自我修改、回滚、部署、迁移都成为可管理的工程问题。
3. **自我改进要先从"便宜"开始**：成本是最容易明确优化的信号，但必须有 eval 防止"省钱即偷懒"的奖励黑客。
4. **RSI 的突破口在 harness，不在 weights**：当生成物与生成者同为代码时，自我递归的循环才真正成立。
5. **早期社区的认知红利**：Exo 的未来无法预测，但在它成型之前加入，或许就是在押注下一个十年。

---

<!-- TLDR: Agent 的自我改进应从 harness 代码层开始：同媒介生成与执行，让递归自我完善成为可工程化的现实。 -->
<!-- TAGS: AI Agent, RSI, 系统架构, LLM, Exo -->
<!-- RATING: 5 -->
