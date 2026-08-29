---
title: "11 Insane Things Cursor’s NEW GrokBot Can Do"
channel: "Riley Brown"
published: "2026-08-26"
source_url: "https://www.youtube.com/watch?v=XgkW4A6lrDY"
video_id: "XgkW4A6lrDY"
tags: ["AI代理", "GrokBot", "自动化", "生产力", "团队协作"]
rating: 4
language: "英文"
word_count: 29197
duration: "37:24"
---

# 11 Insane Things Cursor’s NEW GrokBot Can Do

- **Channel:** Riley Brown
- **Published:** 2026-08-26
- **Source:** https://www.youtube.com/watch?v=XgkW4A6lrDY
- **TL;DR:** 用简单代理+丰富上下文构建24/7协作的AI团队，核心不在生成而在整合与自动化。
- **Tags:** AI代理, GrokBot, 自动化, 生产力, 团队协作
- **Rating:** 4

## 版本

- [结构化文稿](2026-08-26-11-insane-things-cursor’s-new-grokbot-can-do-XgkW4A6lrDY.structured.md)
- [原始文稿](2026-08-26-11-insane-things-cursor’s-new-grokbot-can-do-XgkW4A6lrDY.transcript.md)

# 11 个疯狂的 Cursor GrokBot 新功能：AI 代理团队管理的未来

## 材料信息

- **标题**: 11 Insane Things Cursor's NEW GrokBot Can Do
- **作者/来源**: Riley Brown（YouTube 创作者频道）
- **类型**: YouTube 视频字幕
- **关键元数据**: 视频教程类内容，约30-40分钟；Riley Brown 是一位拥有超过200万社交媒体粉丝的内容创作者，同时也是 Agent Native 公司的创始人，专注于 AI 代理平台的实战应用

## 开篇引入

在这个 AI 工具以周为单位迭代的时代，Riley Brown 用一句话抓住了我的注意力："This right here is my AI agent team."——"这就是我的 AI 代理团队。"

想象一下：你有一个 24/7 从不休息的员工团队，每个员工都有自己的电脑，各自负责不同的职能，他们之间可以互相交流、互相协调，并且在你睡觉时依然为你工作。这不是科幻小说，而是 Riley Brown 在过去一周真实使用 GrokBot 的日常体验。

GrokBot，这个最初由 Cursor（后被 SpaceX 收购）开发的 AI 代理平台，被 Riley 称为"市场上增长最快的代理工具"。但最让我感兴趣的不是它的"增长"，而是 Riley 在使用过程中那种接近管理真实团队的感觉——"It is the closest I've felt to managing a real team of AI agents in an interface that makes sense."（这是我在有意义的界面中最接近管理真实 AI 代理团队的感觉。）

作为一个拥有 200 万粉丝的创作者，Riley 需要同时管理内容创作、业务合作、社交媒体、客户项目和团队协调。在这场分享中，他不仅展示了自己的实战配置——一个由多个专业代理组成的"团队"——更将其拆解为 11 个可以直接套用的技巧。这篇深度重构将带你完整理解每个技巧背后的逻辑、实际操作方法，以及如何将它们应用到自己的工作流中。

---

## 理解 GrokBot 的基础架构

### GrokBot 是什么？ `[视频开头至基础讲解]`

**核心观点**

GrokBot 本质上是一个"拥有个人电脑的 AI 代理团队"平台。每个代理都有独立的身份、记忆和工具权限，但它们共享技能与插件，从而保持统一的行动能力。

**深度阐述**

在深入 11 个技巧之前，Riley 先花了必要的时间解释基础概念。他将 GrokBot 概括为一句话："a personal team of AI agents each with their own little computer"——"一个由 AI 代理组成的个人团队，每个代理都有自己的小电脑"。

这里的核心不是"AI聊天机器人"，而是一个**自主行动体**的概念：每个代理（Agent）都运行在一个云端虚拟电脑上，能够访问文件系统、浏览器、外部工具，并在后台独立执行任务——不仅仅是回答问题。

界面布局上，GrokBot 桌面应用包含一个聊天窗口，左边是代理列表，右边用于显示代理所能访问的电脑桌面。每个代理都有自己的"身份"——包括名称、标题和描述。Riley 用了一个非常关键的细节来说明描述的重要性："The agent reads the description every time it runs, so it kind of is reminded of what it does."（代理每次运行时都会读取描述，所以它相当于不断被提醒自己的工作职责。）这意味着你只需要用自然语言写好代理的"职位描述"，它就会在每次行动时遵循这条指令。

在功能架构上，GrokBot 有三个关键概念：

1. **技能（Skills）**: 类似于可复用的"能力模块"，例如"财务洞察"（financial insights）。所有代理共享所有技能——这也是一个核心设计取舍：不需要为每个代理单独配置技能，而是一次配置、全团队可用。

2. **插件（Plugins）**: 用于连接外部服务，比如 Gmail、Intercom、日历等。和技能一样，插件对所有代理全局生效。例如，如果你给 GrokBot 添加了 Gmail 插件，那么你的"合作代理"和"监控代理"也立刻拥有了访问 Gmail 的能力。

3. **例行任务（Routines）**: 这是让代理实现"24/7 工作"的关键机制——通过设定时间或事件触发，代理可以自动醒来并执行任务。

那么，既然所有代理共享技能和插件，它们之间有什么不同？Riley 的回答非常清晰："The only thing that makes these different is each of these agents operate in their own session."（唯一区别是每个代理在自己的独立会话中运行。）这意味着每个代理拥有独立的对话历史、独立的记忆、独立的任务进展——本质上，它们就像是同一家公司里不同部门的员工：共享公司资源（技能和插件），但各有各的项目和职责。

**视觉/结构信息描述**

视频展示了一个代理列表界面，包括：
- "GrokBot"（通用代理，Riley 最常使用）
- "Partnership bot"（合作业务代理）
- "MTS bot"（监控情况代理）
- 多个其他专门代理

每个代理项看起来像一个卡片，包含头像图标（GrokBot 的图标是一个灰色小圆块）、名称和简短描述。

**个人感受**

Riley 说他在 GrokBot 上花了一周时间，这是"closest I've felt to managing a real team"——注意"real team"（真实团队）这个词。他并没有说"最好的AI工具"，而是形容这是"最接近真实团队管理"的体验。这个措辞透露出一个重要信息：GrokBot 的竞争点不在于单次对话质量，而在于它模拟了一个可以持续运作的组织系统。

**延伸思考**

GrokBot 的"全代理共享技能"设计与传统软件权限管理完全不同。这背后是一种"团队一致行动"的理念：与其给每个代理做细粒度权限控制，不如让所有代理统一能力基线，然后用会话隔离来实现专业化。这种方式降低了配置门槛，但也意味着你信任的是整个平台共享环境的安全性。

**精华收获**

GrokBot 的核心不是"更强的聊天"，而是"可编排的代理组织"。理解技能、插件、例行任务这三个全局机制，再叠加会话隔离带来的专业化分工，就能开始"管理"而非"使用"AI。

---

## 技巧一：建立"监控局势"代理（Monitor The Situation Bot）

### 永不漏掉关键变化的"哨兵" `[视频第一部分]`

**核心观点**

创建一个超级简单但极其有用的"监控局势"代理（MTS bot），让它每隔五分钟检查一次邮件、Slack、日历等信息源，只关注你关心的几个"活跃局面"，有任何更新就立刻通知你。

**深度阐述**

Riley 的第一条建议不是炫酷的自动化，而是强调："Like all of the best bots that I've seen that people have created in Grok bot, it is incredibly simple and incredibly useful. You don't want to create these really complex workflows. You want to create simple, yet really useful agents."（就像所有我在 GrokBot 中见过的最佳代理一样，它简单得不可思议，却又非常有用。你不需要创建很复杂的工作流，而是要创建既简单又特别有用的代理。）

这个"监控局势"代理的设计哲学就是一个词：**专注**。

它做的事情只有一件：维护一份"活跃局势"列表，然后周期性检查各种信息源（邮件、Slack、日历等），看是否有任何与列表中项目相关的更新。如果有更新，就生成一条简洁的更新消息。

具体工作流程如下：
1. **定义监控列表**：你告诉这个代理"当前正在进行的项目/事情"有哪些。例如，"请将 GrokBot 完整指南视频添加到活跃局势中"。代理会将此记录到它的持久列表中。
2. **定期巡检**：代理每5分钟（工作日）自动唤醒，检查所有已连接的信息源（邮件、Slack、日历），比对是否存在列表项目的相关更新。
3. **及时通知**：发现更新后，立即向你推送一条消息——包括桌面应用通知和手机应用通知。

Riley 展示了一个模拟运行：他在对话中要求一个名为"GrokBot full guide video"的局势条目模拟更新。代理立刻生成了这样的消息："GrokBot 完整指南视频这里的更新：John 刚刚把他那40分钟学会99% GrokBot 的视频放进了数据库...17种使用 GrokBot 的方法就在旁边..."并且这条消息被标记为**白色**标注，方便 Riley 快速定位是哪个局势。然后代理完整列出了当前监控的所有局势，以及每条局势的状态。

当某个局势结束时，Riley 只需说"我们完成了这段视频，我不需要再监控了"，代理就会将其从列表中移除，并更新自己的行动准则。**每次对话（turn）中，它都会显示当前的全量监控列表，让你始终知道代理在关注什么。**

**视觉/结构信息描述**

视频中显示了 MTS bot 的界面：
- 名称：MTS（Monitor The Situation）
- 描述行动准则的说明文字
- 顶部有"Active Situations"（活跃局势）列表，目前包含3个项目
- 例行任务配置显示"weekdays, every 5 minutes"（工作日，每5分钟）
- Slack通道、邮件、日历等图标并列显示其可以访问的信息源

**个人感受**

Riley 特意说明了一个真实细节：他实际使用的 MTS 代理监控的是自己业务中最敏感的数据——客户信息、合作伙伴、正在进行的商业谈判——所以他不能在视频里展示全部真实列表。这个细节让我觉得很有可信度：这不是一个纯演示产品，而是已经深入到真实工作流的工具。

**延伸思考**

"监控局势"这个模式本质上是一个**信息过滤层**。在这个信息过载的时代，AI 的另一种价值不是"生成内容"，而是"减少注意力消耗"。一个每5分钟自动检查所有信息源、只报告与重要事务相关的更新的代理，实际上是在替你完成"注意力管理"。

**精华收获**

一个有效的 AI 代理不需要复杂。给它一个明确的职责（监控）、提供必要的工具（邮件/Slack/日历）、定义好你关心的指标（局势列表），它就能创造巨大价值。简单才是可持续的设计。

---

## 技巧二：通过开发者代理连接 Cursor 实现编程自动化

### 通过 GrokBot 委托真实代码任务 `[视频第二部分]`

**核心观点**

GrokBot 不仅仅是一个通用知识工作平台，你还可以通过创建"开发者代理"并让它连接 Cursor，实现完整的编程任务委派——包括创建分支、云端运行、截图/录屏并回传结果。

**深度阐述**

Riley 说："Grok bot is meant to be a general agent platform, meaning to be used for knowledge work tasks, kind of like GPT work. However, you can actually connect to this to cursor."（GrokBot 的定位是一个通用代理平台，用于知识工作类任务，类似于 GPT 的工作。但你可以把它连接到 Cursor。）

这个连接过程非常简单，因为 Cursor 和 GrokBot 使用同一套账号体系——你就是用设置 Cursor 的那个账号登录 GrokBot 的。

连接后，你可以像这样直接对开发者代理发出指令：

> "Hey, the landing page we are working on the other day, I need you to redesign it. I want you to design it in the same style as Grok, like xAI's Grok, and try it with that simple black and white style, please. Create a new version of that of the agent native site, and then take screenshots of it and send it to me. Please use Claude Opus 5."

整个执行过程展示了 GrokBot 和 Cursor 的深度协同：

1. **任务接收**：GrokBot 收到你的自然语言指令，理解设计需求。
2. **任务委派**：它把这个任务"转交给" Cursor，并且将 Prompt 优化得更清晰——一个值得注意的细节是，GrokBot 不只是传递你的指令，它还会**优化指令**。你可以看到它写给 Cursor 的 prompt 比你的原始指令更结构化。这就像是一个聪明的项目经理帮你把需求写成了开发工单。
3. **安全执行**：Cursor 创建一个新的分支（branch），因此不会影响你现有的生产环境应用。
4. **云端运行**：代码在云端虚拟电脑中运行，而不是在你的本地电脑。
5. **结果回传**：应用运行后，代理会自动截屏（或录屏），将截图发送给你。

整个过程中，你可以随时查看任务状态。输入"status"就能获取进度更新。通过"Open in Cursor"，你还能跳转到 Cursor 云端，查看完整的执行日志和 Prompt。最后，Curoser 会创建一个 Pull Request（PR），并跳转到 GitHub 查看，这意味着整个开发流程的每一步都有记录和审计。

最关键的是，Riley 指定了模型为 Claude Opus 5——说明你可以**选择任意模型**来处理具体任务，而不是被 GrokBot 锁定。

**视觉/结构信息描述**

视频展示了：
- 开发者代理的聊天界面，包含任务描述
- Cursor 云端运行界面，显示完整的 prompt 和运行状态
- GitHub PR 页面截图
- iOS 手机应用中的任务结果展示——不仅包含桌面端，手机端可以随时查看进度
- 最后的截图结果：桌面端的首页全屏、移动端首页、其他页面等

**个人感受**

Riley 还提到一个实用场景："I use GrokBot on my phone probably more than my computer"（我在手机上使用 GrokBot 的频率可能超过电脑）。开发者代理的任务结果会直接推送到手机上，这意味着你可以在散步时发起一个编程任务，然后收到带有设计截图的完成通知——不用打开电脑就能完成整个开发委派闭环。

**延伸思考**

这种"通过通用 AI 代理委托专业工具"的模式，预示着未来 AI 工具使用方式的一个转变：你不再需要学习每个工具的界面，而是通过一个"调度中心"（GrokBot）来调用其他工具的能力。GrokBot 某种程度上正在成为"AI 的操作系统"——它不自己完成一切，而是协调其他 AI 和后端系统共同完成任务。

**精华收获**

GrokBot + Cursor 的组合让你可以随时用手机或电脑向"开发团队"下达任务，并在安全的分支环境中执行、测试、交付，整个流程可追踪、可审计。创建专业代理时，明确指定模型、输出格式（截图/PR）、和部署路径（分支），能显著提升执行效率。

---

## 技巧三：建立"什么都不做"的通用 GrokBot

### AI 对话的"收件箱" `[视频第三部分]`

**核心观点**

一个没有特定目的、专门用于日常快速对话的通用代理，是所有高级工作流的"入口"。它就像你 AI 工作流中的"默认 Gateway"——不知道问题该放哪，就放这里。

**深度阐述**

Riley 的第三个技巧来自一个观察："I've noticed when people go to set up their AI agents, they try to like create a new bot for every type of chat. You don't need to do that."（我注意到人们在设置 AI 代理时，总想为每个聊天场景创建新代理。你不需要这样做。）

解决方案是：**建立一个"不做任何特定事"的代理**。Riley 将其命名为"GrokBot"，并将其固定在界面顶部，这样在任何情境下他都能快速进入。

这个代理的描述简单得令人惊讶，原文是：
"You do whatever. You have no specific purpose other than to respond to Riley the best you can. This chat is meant for general use, while all the others are meant for specific uses."（你随意发挥。除了尽可能好地回应 Riley 之外，你没有任何特定目的。这个聊天用于通用目的，而其他所有代理用于特定目的。）

它就是 AI 对话的"收件箱"——当你不确定应该把某个想法、问题或指令放到哪个专业代理中时，先进入这里。Riley 给出了一个真实的例子：他使用语音输入说：
"Yo, what was that conversation we were having a few days ago about ideas for using a Windows laptop for that video I want to do on a Windows AI setup?"

这个查询要求在多个历史对话中找到先前的讨论，并返回上下文。Riley 验证了其跨会话检索的能力——代理成功找到了周五的对话，包括关于 Windows AI 设置视频的详细讨论。

更重要的价值在于：当你和这个通用代理聊天时，你可能会发现某个反复出现的需求，值得将其独立成一个专门的代理。Riley 建议从这个通用代理中"孵化"专业代理——先意识到需求，再利用 GrokBot 的工具将其变成独立的自动化代理。

**视觉/结构信息描述**

视频展示了：
- 通用 GrokBot 的聊天界面
- 用语音输入命令的行为演示
- GrokBot 的详细设置页面（名称、标题、描述）；描述中只有那几句简单指令
- 代理列表顶部的"固定"（pinned）标签——Riley 说他会让这个代理始终保持固定

**个人感受**

Riley 对这种方式的态度非常务实。"I don't like to be too structured with it."（我不喜欢对它过于结构化。）他并不为这个代理设定什么宏大的目标或精心设计的提示词，而是让它保持"自然"和"足够好"。这种最小化设计的哲学，反而让这个通用代理成为他整个 AI 系统中使用频率最高的入口。

**延伸思考**

"不要为每种场景创建新工具，而是先有一个通用的入口，再基于真实使用需求逐步孵化专项工具"——这其实不仅是 AI 代理的使用哲学，也是产品开发的基本方法论。从最小可行产品出发，以用户行为为根据迭代，比一开始就构建巨型系统更容易成功。将这个逻辑迁移到其他产品的 Agent 使用上，同样成立。

**精华收获**

给每个代理一个明确的"通用型"角色不是浪费，而是**战略投资**。它提供了一种无需思考的"先放这里"的入口，降低了使用摩擦，也大大简化了信息检索路径。

---

## 技巧四：让代理们互相交谈——团队协作的聚变反应

### 让你的 AI 团队开周会 `[视频第四部分]`

**核心观点**

GrokBot 最独特的功能之一是你可以命令一个代理去联系其他所有代理，收集它们的总结、状态和任务信息，然后生成一份全局报告。你还可以创建群聊，让多个代理在同一会话中互相交流。

**深度阐述**

Riley 亲身体验了让他的"AI 团队"开周会的场景。他回到通用 GrokBot，发出指令：

> "Hey, buddy. I need you to do something for me. I would like for you to talk to all of the other agents. I want you to talk to those guys and get a good summary of the last week, and then present to me a summary of what we've done over the last week. I'm trying to look for what projects I should be focused on, and what is the next thing that I should be doing, and please do that for me."

接下来发生的事情非常震撼："Message three bots. Message four bots. Message five bots. Look at this."（给三个代理发消息。给四个代理发消息。给五个代理发消息。快看这个。）你可以在界面上看到一个代理正同时向其他代理发送消息，并且你可以**点击展开查看**它实际发送的内容。例如，它给某个代理发送说："Riley asked Grokbot for a last week recap so he can pick what to focus on next."（Riley 让 GrokBot 做上周总结，好让他决定下一步要专注什么。）

这些对话会被作为跨代理会话记录保存下来，你可以随时点击查看每条消息流——相当于整个团队的"会议纪要"。

最后，GrokBot 汇总了收到的回复，给出了一份报告。Riley 特意说明截图里模糊了很多内容，因为报告涉及他的真实客户、商业数据和正在推进的项目。报告说："Got enough recaps. Here's the week and what to do next."（收够了汇报。这是本周总结以及下一步要做什么。）然后列出了三个优先级建议（这是代理从全局信息中自动提炼出来的行动优先级），并将所有待办事项围绕此组织呈现。

**群聊功能**

除了"一代理问所有代理"，你还可以创建**群聊**——把多个代理拉进同一个会话。Riley 演示了他把 GrokBot、Partnership bot、MTS bot 加进群组，然后将群名命名为"The Boys"。在群聊中，你可以看到谁正在输入——"MTS bot is working. We have GrokBot."你还能设置群聊的指令文件（instructions file），让本群行为更规范。所有这些都可以在手机应用上看到和操作。

**视觉/结构信息描述**

视频展示了：
- 代理正在同时向多个代理发送消息的界面示意，每个接收代理都有独立的状态指示
- 点击"View conversation"后展开的所有跨代理聊天记录——包括 GrokBot 发给各代理的具体消息
- 群聊的创建界面：选择多个代理、编辑群名称（"The Boys"）、查看输入指示器（typing indicator）
- 手机端同步展示这些群聊

**个人感受**

Riley 对这个功能的反应是"really fun and just a really unique experience"。这不仅仅是"工具"的价值——看到你的 AI 代理们在实际工作中互相协调、交换信息，确实会让人产生一种"我的团队活过来了"的感觉。报告里甚至提到 "A couple bots still haven't written back. Those are probably ones that just haven't really done anything."（有两个代理还没回复，可能是它们这周真的没做什么。）这个细节非常有人情味——连 AI 代理都会有不干活的时候！

**延伸思考**

群聊机制意味着多个 AI 代理可以像人类团队一样就同一主题展开讨论、交换信息、甚至辩论观点。这为我们打开了一个新的可能性：AI 代理之间的"团队协作"——每个代理带有不同领域的"背景知识"，通过对话综合出更全面的答案。这在人类组织中叫"跨职能会议"，在 AI 代理平台中就变成了"群聊"。从"AI 代理人机交互"过渡到"AI 代理间交互"，是组织智能化的一个重要转折点。

**精华收获**

跨代理对话是 GrokBot 最大的差异化能力。各种周报、跨项目总结、优先级建议，都可以通过简单命令触发的全局集结来完成。同时，群聊提供了一个轻量级的"多领域顾问团"——让不同专业代理在同一问题上给出多角度答案。

---

## 技巧五：创建通用项目代理，快速"孵化"新特种代理

### 从通用对话中糊化出的项目专属代理 `[视频第五部分]`

**核心观点**

当一个项目在你的多个对话中被反复提及、需要专门跟进时，你可以快速将它"孵化"成一个独立的项目代理。GrokBot 可以自动把你之前对话中收集到的相关信息转交给新代理，并为其配置例行任务。

**深度阐述**

在例子中，GrokBot 的周报总结提到 Riley 需要一个短格式视频编辑。Riley 将这件事升级为一个独立代理——"video editor bot"。关键在于他让自己的通用 GrokBot 去自动配置这个新代理：

> "Hey, I think it's really important that we get this video editor on-ramped and make sure that we give them all the information that they need to do a really high-quality job for my short-form content. Can you please go to the new video editor bot and give them everything that they need to get set up properly to be a good video editor bot? Just make sure that this agent has context over this new video editor."

然后，新代理自动从通用 GrokBot 那里获取关于视频编辑器需求的所有上下文——包括此前讨论的招聘需求、编辑要求、内容方向等。你甚至可以指定它"listen to @GrokBot"（听从 GrokBot 的指挥），自行确定新名字。

接下来，作为一个新代理，你可以立即给它配置**例行任务（routine）**："Every morning at 8:00 a.m., I want you to remind me to write a short-form script or ask for like, literally ask me what things have been interesting, and also check my bookmarks on Twitter and give me some suggestions for things that I should talk about in short form."（每天早上8点，提醒我写短格式脚本，问我最近对什么感兴趣，同时检查推特书签给我内容建议。）

GrokBot 会解释这个需求，生成一个名为"First Frame"的新代理，并创建了"Set weekday 8:00 a.m. ping"（设置工作日早8点提醒）的例行任务，附带完成该例行任务所需的详细指令。一个新项目组就这样诞生了——**有上下文、有例行任务、有明确角色**。

**隐藏而非删除**

Riley 还提出了一个重要的管理习惯：如果代理暂时不需要使用，不要删除，而是"hide from sidebar"（从侧边栏隐藏）。他自己的工作区中就有15个隐藏代理——这些是过去实验过或暂时不再需要的代理，但保留着它们的历史和配置。这就像是一个"未使用的员工档案"，随时可以调回来。

而且，即使隐藏了，**通过命令面板也可以快速重新访问**——只需按 Cmd+K 输入代理名。这实际上形成了"聚焦当前活跃项目、保留历史资源"的管理模式。

**视觉/结构信息描述**

视频展示了：
- 新代理创建的完整流程：点击新建、输入名称和描述
- GrokBot 自动把信息分享给新代理、新代理自动获得上下文
- 新代理的详细配置页面：名称（"First Frame"）、例行任务指令、说明
- 隐藏代理列表的展示——隐藏后侧边栏更干净
- 通过 Cmd+K 命令搜索并找回隐藏代理的演示

**个人感受**

Riley 对创建新代理的态度是"方便但不轻率"——他不会为所有任务都新建代理，只有当真实的复用需求出现时才将其正式化。这反应了一种成熟的"AI 团队组织"管理思维：人员编制不要随意增加，但合适时可快速组建新部门。

**延伸思考**

"从通用对话中孵化专业代理"这个流程，本质上反映了人类知识型团队中常见的"员工成长"模式：你先是让通用型员工做各种杂事，随着逐渐发现他处理某类任务的专长，你再正式将其转为一个专门的岗位。GrokBot 把这个组织管理过程自动化了——普通会话中的经验和上下文可以直接迁移到新代理中，这将成为 AI 组织高度可扩展的管理方式。

**精华收获**

推动你的 AI 代理团队发展壮大的正确路线是从通用到专业——先积累需求，然后利用历史上下文一键孵化新代理。这比事先搭建一个大而全的复杂系统务实且高效得多。

---

## 技巧六：连接 Twitter/X——你的社交媒体分析助理

### 让 AI 成为你的社交观察者 `[视频第六部分]`

**核心观点**

GrokBot 可以通过插件连接多个 X（Twitter）账户，让你用自然语言命令分析你的推文表现、书签、甚至找出哪些 VC 喜欢了你的内容——将社交媒体情报化、自动化。

**深度阐述**

Riley 展示了连接 X/Twitter 的多种真实用法。

**用法一：分析你的推文表现**

Riley 在 GrokBot 中说：
"Please analyze my last 50 videos on X and put them with a link below and how they did. Only videos that are over 3 minutes."（请分析我在 X 上最近50个视频，把它们和链接、表现一起列出来，只看超过3分钟的视频。）

GrokBot 能够自动定位并分析这些视频帖。当你点击某条推文时，它会直接跳转到 X 上的原始帖子。这种能力让 AI 不只是一个分析工具，还是一个"导航入口"。

**用法二：检查书签并生成摘要**

在手机端，Riley 可以随时随地发出指令：
"Hey, I want you to please list out all of my bookmarks for the week that have to do with AI agents and then what it means in a few sentences for each one and I want a hyperlink to all of those bookmarks so I can kind of review all the things that I bookmarked."

结果是：GrokBot 拉取了一周内的所有书签，筛选出与 AI 代理相关的条目，附上每条的简要解释和超链接。Riley 透露，这实际上是他每周更新视频创意的核心流程——他只用书签功能收藏那些关于 AI 进展、AI 代理的重要信息，然后让 GrokBot 汇总这些书签，作为本周视频更新的素材库。他向观众展示了周日上午和周三的书签摘要报告是自动执行的例行任务。

**用法三：找出谁在关注你**

Riley 还演示了一种更高级的社交情报能力：
"Of the most popular videos in the last month, what VCs liked my posts?"（在过去最受欢迎的视频中，有哪些 VC 喜欢了我的帖子？）

GrokBot 可以检索所有点赞者中具有知名 VC（风险投资人）身份的用户，并列出他们为哪条帖文点赞了。这种"谁在关注我"的方法论脉脉含情地揭示了 X 平台的开放性——公开的点赞数据，经过 AI 的整理，变成了可用的社交情报。

**设置方式**

要启用这些功能，你只需前往插件列表，找到 X，添加你的账号并授权即可。Riley 在自己账户下添加了两个 X 账号：个人账号（Riley Brown）和商业账号（Agent Native），还演示了添加其他账号的流程。同一个平台可以控制多个不同身份账户，适合管理多个品牌或个人号。

**视觉/结构信息描述**

视频展示了：
- GrokBot 列出的推文分析表格——包含推文链接、浏览量数据、每条视频的具体统计
- 点击推文后跳转到 X 原始页面的流程
- 手机端运行书签摘要任务的界面
- 桌面端每周三/周日自动运行的"书签摘要"例行任务清单
- 插件设置页面——默认账号、附加账号列表

**个人感受**

Riley 对书签功能显然有很深的依赖："Especially for me, I do my weekly agent updates. The way that I get started with that is I just summarize all my bookmarks because I only bookmark things that have to do with AI advancements, AI agents."（对我而言，我做每周代理更新时，首先就是总结我的所有书签，因为我只收藏那些跟 AI 进展和 AI 代理有关的内容。）把"做内容"的流程压缩为"收藏素材+让 AI 整理"两个步骤，这就是创作者使用 AI 的正确姿势。

**延伸思考**

建立在公共数据上的 AI 社交分析将成为标配。X 的公开点赞和关注数据、推文表现统计，这些数据一直存在，但以前需要人工浏览或专门的 SMM 工具才能分析。GrokBot 将这类分析变成了自然语言查询——这正是 AI 赋能创作者的正确方向：不需要学习新工具，用一句话就把复杂的数据变成了情报。

**精华收获**

连接你的社交账号是 GrokBot 输出的放大器。定期让 AI 汇总书签并生成摘要，能直接作为内容创作的一手素材；深度分析推文数据（如找出哪些大 V 看过你的内容）则能帮你发现之前忽略的潜在合作机会。

---

## 技巧七：基于触发器的自动化——代理等事件睡觉

### 从"到点上班"到"看见情况就行动" `[视频第七部分]`

**核心观点**

GrokBot 支持基于事件或触发器的例行任务（Routines）——当 Slack 收到消息、GitHub 发生活动、Sentry 发出警报时，代理会立即被唤醒并执行预设操作。这是其他通用代理平台目前尚不具备的差异化能力。

**深度阐述**

Riley 将 GrokBot 的例行任务分为两类：

**第一类：时间驱动型例行任务**——这是最基础的，例如"每天早上8点检查邮件"或"每5分钟检查日历"。MTS 代理的每5分钟巡检就是这种模式。

**第二类：事件驱动型（触发器）例行任务**——Riley 说这是其他通用代理平台目前所不具备的独创功能。如果你操作 GrokBot 添加新例行任务，你会看到可用触发器列表：Slack、GitHub、Microsoft Teams、Linear、Sentry、PagerDuty。Riley 还提到未来会加入更多触发器，如 email triggers（邮件触发）、webhooks（网络钩子）等。

以 Slack 为例——这是 Riley 使用最多的触发器——你可以创建如下规则：当某个频道出现任何消息时，代理自动唤醒，执行预设的操作序列。这些操作可以包括：解析消息内容、更新数据库、创建文档、通知相关人员、甚至触发外部系统。Riley 说这些自动化中有很多是"hidden"的，比如用于处理发票、客户服务等敏感业务的自动化。

创建触发器例行任务也极其自然——不需要花太多精力在调整流程上。Riley 演示了当新代理时，他让代理"记住"自己是一个 Slack 提醒者："Anytime something happens in any Slack channel, I want you to tell me in all caps what that thing is."（无论任何 Slack 频道发生什么，用全大写字母告诉我发生了什么。）然后代理会自动创建一条例行任务，触发条件是"on all messages anywhere on Slack"（Slack 上任何地方的所有消息）。你必须显式指定触发时机之后，它才会开始"watching Slack"（观察 Slack）。

**在这个场景中，触发器用法的价值是变形金刚级别的**：对一个共享 Slack 频道（shared Slack channel）触发，意味着当外部合作伙伴/客户发送消息时，代理能够即时捕获并自动处理——不需要你盯着 Slack 频道。

**视觉/结构信息描述**

视频展示了：
- 例行任务列表——名称、触发类型（时间/事件）、状态
- 新例行任务的触发选择界面——展示了 Slack、GitHub、Microsoft Teams、Linear、Sentry、PagerDuty 等触发器选项
- 一个已配置的"deal Slack alerts"（交易Slack预警）——在任何 Slack 频道或特定频道出现消息时触发

**个人感受**

Riley 明确表示计划做一个"专门视频"深入讲解触发器自动化——这个线索说明他自己判断这是非常值得深入的主题。"The most useful one for me is Slack. There are certain channels where if something happens, I need to know about it really quick, or something needs to happen externally like someone else needs to know, or we need to update a database, or it needs to create some sort of document."（对我最有用的是 Slack。某些频道一旦有事情发生，我必须立刻知道……要么需要通知其他人、要么需要更新数据库、要么需要创建某种文档。）

**延伸思考**

事件驱动型代理是 AI 从"被动工具"走向"主动参与"的重要一步。时间驱动让你可以按计划获取信息，而事件驱动让代理可以实时响应外部信号。这真正把 AI 带入了"内部业务流程"中——它不是你要去查的工具，而是当重要事件发生时它主动来找你。

**精华收获**

有了触发器，你的 AI 代理就获得了"感官"——它们可以实时感知外部世界的信号并立刻行动。将工具从"时间轮询"升级为"事件驱动"，是 AI 代理专业化的关键一步。

---

## 技巧八：插件的杠杆效应——上下文是 AI 的灵魂

### 每加一个连接器，代理就变得更懂你 `[视频第八部分]`

**核心观点**

插件是 GrokBot 能力的"倍增器"。你添加的每一个外部服务插件（Google Drive、Notion、日历、Twitter、Linear 等），都扩大了代理的上下文视野和行动范围。Riley 详细解释了为什么要谨慎而积极地配置插件，以及每个插件的具体价值。

**深度阐述**

在 GrokBot 的插件菜单中，Riley 列出了他自己配置的全部插件，并逐一解释其用途：

1. **Google Drive**: 访问 Google Docs 中的文档。Riley 说自己的很多灵感都记录在 Google Docs 中，这给了代理读取这些初始构想的能力。

2. **Google Calendar**: 让代理能获取日程信息。Riley 特别强调了这个插件的实际应用——他有一个 **calendar bot**（日历代理）。这个代理每 5 分钟（工作日 6:00-22:00）检查日历，并在会议开始前 5 分钟和 15 分钟各提醒一次，同时告诉 Riley 关于该会议需要知道的所有上下文信息。这是一个真正"用 AI 替代闹钟和会议录取"的落地场景。

3. **Notion**: 代理可以创建和编辑 Notion 文档。Riley 用 Notion 管理内容脚本和知识库。

4. **Linear**: 用于产品更新。Riley 的公司在 Linear 中追踪产品开发进度，代理可以读取并汇报。

5. **Twitter（X）**: 代理可以分析推文、书签等；Riley 强调它还可以"grab my voice on Twitter"（获取他在 Twitter 上的语气/风格），这样如果要他让代理想出建议的推文，它会模仿 Riley 的写作风格。

6. **ClickUp**: 与咨询公司协作时的项目管理工具，代理可以自动检查任务信息。

7. **Granola**: 自动读取会议笔记的应用。Riley 说这个他还没有正式设置，但可以利用它让代理理解所有会议内容。

Riley 在此分享了插件策略的核心哲学："Every plugin that you add to GrokBot, obviously, it does increase the risk of like security issues, but it also increases the amount of context your agents can get. The more context you give your agent, the more it will understand you and the more it'll be able to make good decisions in what to show you or what to create for you based on the tasks you give it."（你添加的每个插件显然都会增加安全风险，但它也增加了代理能获得的上下文量。你给代理的上下文越多，它就越能理解你，越能为你要执行的任务做出好的决策。）这是所有 AI 工具使用的基本原则：上下文决定输出质量。

最后，Riley 还透露 Cursor 和 GrokBot 的插件体系在未来会趋同："Basically over time all of the plugins that Cursor has GrokBot will have and vice versa"（随着时间推移，Cursor 有的插件 GrokBot 也会有，反之亦然）——这背后是同一家公司统一战略的结果，对用户来说是好消息。

**视觉/结构信息描述**

视频展示了一个插件列表界面，包括所有已配置插件的图标和名称。下方还有"features、agent orchestration"等选项。

**个人感受**

Riley 提醒了"安全风险"的权衡，但他没有夸大风险。对于优化上下文的需求，他显然认为收益大于风险。"The more context you give your agent, the more it will understand you"（你给 AI 的上下文越多，它就更能理解你）——这是全视频中最重要的一句实践箴言。

**延伸思考**

在一个组织环境中，多个插件给了代理大量访问权限，这会带来安全和隐私隐患。但换个角度想，代理的价值不正是建立在"更懂你"的基础上吗？在竞争激烈的 AI 代理平台市场，谁能提供更安全的权限控制、同时集成更多的数据源，谁就能赢得关键的市场份额。这是一个需要用户与平台共同权衡的领域，而非一味追求"连接一切"。

**精华收获**

插件是 AI 代理的"感知器官"。每连接一个外部数据源，你的代理对世界的理解就增加一个维度。在实际配置时，可以用一句话概括优先级："上下文多，而不是功能多"。每个插件都应该能帮助代理更好地理解你或世界，而不仅仅是增加"自动化能力"。

---

## 技巧九：连接多个 Gmail 账户，让 AI 替你"省钱"

### 让 AI 翻遍你的邮箱，找到被遗忘的订阅费 `[视频第九部分]`

**核心观点**

GrokBot 的 Gmail 插件支持连接多个邮箱账户。这意味着你可以让 AI 把你所有邮件中关于订阅、扣费、自动续费的信息全部汇总起来，帮你发现被遗忘的付费项目并在几秒内计算出"砍掉这些开销能省多少"。

**深度阐述**

Riley 对这一功能的评价是 "this might be one of the most useful"（这可能是最有用的一个）。

他的第一个故事极具说服力：当第一次发现可以连接多个 Gmail 账户时，他做的第一件事就是让 AI 检查自己所有的邮件（他一共连接了 5 个邮箱），找出让他继续付费的订阅服务：
"When I first got GrokBot and found out that you could connect multiple Gmail accounts, the first thing I did is I had AI go through all five of them looking for subscriptions that I should cancel because I've collected a lot of emails over the years. I needed to find where like what accounts I've signed in with and how I can cancel them, and it went through all of them and saved me a ton of money."（当我第一次拿到 GrokBot 并发现可以连接多个 Gmail 账户时，我做的第一件事就是让 AI 翻遍所有五个邮箱，寻找我应该取消的订阅。因为这么多年我积累了太多邮箱账户，需要找出我到底注册了哪些服务、怎么取消它们。AI 翻遍了所有邮箱，帮我省了一大笔钱。）

这个场景非常真实，也极具说服力——任何人都能理解"注册了一堆服务，但忘了自己订阅了什么"的痛苦。AI 的价值在这里不是创造，而是**还原**：帮你盯着你忽略的细节。

第二个例子是将多邮箱和"智能助手"结合起来。Riley 对 GrokBot 下达指令：
"Yo, buddy, I need you to go through both of my emails, find all the things that I've paid for over the last 3 months and list them out right here, please. Everything that we've paid for. Ignore big massive business expenses. We're not looking for my personal stuff."（兄弟，我需要你翻两遍我的邮箱，找出过去三个月我付过款的所有项目，列在这里。所有我们付过的项目。忽略大额商业支出，我们是找你个人的。）

Riley 进一步展示了用 AI 做"活跃追踪任务"的场景：他让 GrokBot 给同事 Emily 发一封邮件说 "You should really try GrokBot"，然后 "Please check for her response every hour until she responds. Once she responds, delete that automation."（请每小时查一次她的回复，直到她回复为止。一旦她回复了，就删除这个自动任务。）GrokBot 会自动创建一个每小时检查邮件的工作流，直到 Emily 回复后自动终止。"If it checks, if nothing happens, it'll just do nothing, which is exactly what you want."（如果检查时没有新动态，它就什么都不做——这正是你想要的行为。）

**视觉/结构信息描述**

视频展示了：
- GrokBot 的 Gmail 插件配置界面——显示多个已连接账户（Riley 的个人邮箱和商业邮箱）
- 自动创建"等待响应"例行任务（每小时检查 Emily 是否回复）的界面

**个人感受**

Riley 到今天仍然"基本上通过 AI 代理平台发邮件"，他说："I basically just send all my emails through an AI agent platform. Grok isn't my primary agent platform, but when I use GrokBot, I do send emails directly from it."（我基本上都通过 AI 代理平台发邮件。GrokBot 不是我主要的代理平台，但当我用 GrokBot 时，我真的会直接从它那里发邮件。）这句话透露了一个微妙的信息——多种 AI 代理平台并存是当前的真实状态，没有一个平台能完全取代一切。

**延伸思考**

"让 AI 监控邮件直到某人回复"这种模式，把 AI 从"处理数据"升级为"承担等待"——调用者和被调用者的角色发生了变化。这在异步协作中非常有价值，因为它把人工监测的负担转移给了 AI。也许在未来，我们会看到更多类似应用：AI 盯邮箱、AI 盯短信、AI 盯社媒私信，只把值得注意的事件报告给您。

**精华收获**

多邮箱连接带来的实际好处远超你的想象。除了订阅审计和邮件发送外，"每月检查一次订阅、每三小时追踪一次重要邮件、每五分钟看一次某人的回复"这些**持续轮询任务**正是让 AI 代你"盯着某件事"的典型场景。

---

## 技巧十：连接 Notion + 自定义技能——让 AI 在不打扰你的前提下添加上下文

### 让 AI 做一个安静的"文档协作者" `[视频第十部分]`

**核心观点**

通过 Notion 插件与自定义"添加上下文"技能的结合，GrokBot 可以在不修改主文档结构的情况下，以可折叠/收起的格式向你的工作文档中添加补充信息。这对于内容创作流程中的"补充思路"极为实用。

**深度阐述**

Riley 展示了自己在制作当前视频时使用的具体工作区配置。在 Notion 中，他有一个非常特定的视频大纲格式——段落、分节、时间点等。他对 Notion 文档质量非常在意，不希望 AI 擅自修改主要结构或内容（这可能是很多创作者都会担心的问题——AI 改乱你的文档格式）。

解决方案是：他创建了一个自定义技能，名为 **add context**（添加上下文）。这个技能做了什么？

将补充上下文放入文档中一个指定的 **callout（标注框）** 内，并以 **drop-down（下拉菜单）** 格式展示——不占用太文档太多空间，但仍能随时展开查看。如果你需要取得上下文，打开下拉菜单就能看到；如果不需要，它也不会扰乱你的大纲结构。

具体工作流程：
1. Riley 完成视频脚本/大纲的初稿。
2. 他向 GrokBot 询问："What else did I forget? Please, can you add context?"（我还忘了什么？请添加上下文。）
3. GrokBot 根据 Notion 中已有的文档内容、他的想法库和其他插件提供的上下文，生成补充建议（如补充案例、背景信息、注意事项）。
4. 这些建议被自动写入 Notion 文档的 callout 下拉框中，不改变文档原有布局。

这套方案完美处理了 AI 辅助创作时最常见的矛盾——"AI 能提供有价值的输入"与"AI 添加的内容干扰了创作者的原结构"之间的冲突。

**视觉/结构信息描述**

视频展示了 Notion 文档的界面：
- 视频大纲的结构化文本
- 一个 callout 区块（下拉菜单）中包含 AI 生成的补充信息
- 打开下拉菜单可以看到 AI 添加的上下文列表

**个人感受**

Riley 对内容质量的执着体现在这一技巧中——AI 添加信息不是"往文档里堆料"，而是"在读者需要时才展开的补充层"。他说这个技能"incredibly useful"（无比有用），因为它的收益不是一次性的——每当有新文档需要补充时，只需调用这个技能，它就会遵循同样的"安静"方式。

**延伸思考**

这个技巧的本质是"AI 与人类创作之间的边界管理"。AI 的辅助输出应该是有序、结构化的，而非无序、混乱的。如何让 AI 添加的信息既保留在创作者的视野内，又不对其工作流造成干扰，是 AI 协作工具设计的常态课题。GrokBot 的自定义技能模式让我们看到了一个答案：不要控制 AI 说什么，而要为它的输出规定一个"呈现容器"。

**精华收获**

自定义技能（Skills）的价值不在于"AI 能做什么"，而在于"AI 应该以什么方式做"。通过这个案例可见：让 AI 帮你补充内容时，利用Notion 的下拉菜单功能，让 AI 的输入"可见但不打扰"。

---

## 技巧十一（最终）：让 AI 有自己的电脑——"教它做事"的新范式

### 云端电脑：目前被低估的未来接口 `[视频第十一部分]`

**核心观点**

GrokBot 中每个代理都拥有一台云端虚拟电脑，用户和代理都可以操作它。Riley 认为很快"这台电脑"会变成极具价值的接口——因为你可以通过录制演示来**教**代理完成操作，但目前它的实用场景还不多。

**深度阐述**

Riley 的第十一个技巧来自他自己的"Journal bot"（日志代理）的实践。这个代理大部分在手机上使用，配合名为 **grill me**（拷问我）的自定义技能使用。

"Journal bot"的工作方式独特且有趣：当你有一个模糊的想法或混乱的情绪，可以在手机上像对朋友倾诉一样随意说话（"yap out my ideas"——Riley 的说法），然后 AI 会用一系列追问来"逼问"你。例如：

"Which of those are you actually making this week? Which one are just sitting in the pile?"（其中哪些这周你真会做？哪些还只是躺在待办堆里？）

这种"拷问式提问"的价值在于："It wants to stump me, which is those are the most useful questions because it finds gaps in your logic."（它想要难住我，而正是这些问题最有用，因为它们能发现你逻辑中的漏洞。）Riley 透露这种对话往往持续七八轮，通常足以帮他想清楚行动方向。

经过拷问之后，本次对话中的想法被整理成一个较长的日志条目，存储在代理的计算机上。Riley 选择不把日志同步到 Notion，而是存储**在代理自己的云端电脑的文件系统里**——一个不易丢失、只属于这个代理的空间。

**"教代理做事"的演示功能**

Riley 展示了代理远程桌面上运行的浏览器——例如访问 twitter.com。但他坦诚目前没有找到足够多的实用场景："I haven't found a ton of use for this specific feature yet. I've found that this IP address just gets blocked because a lot of these sites want to block bots, which this is literally GrokBot."（我还没找到大量应用场景。我发现这个 IP 地址会被屏蔽，因为很多网站想屏蔽机器人——而这事确实是 GrokBot。）

不过，他指出了一个重要的未来潜力：**你可以在电脑上演示一系列步骤，让代理观察学习**。比如，你在浏览器中完成注册流程、配置流程、数据录入等操作，代理会逐步记录你的演示过程。当你回放记录时，代理能够学着执行相同的过程。这相当于一种"行为教学"——你不必写代码，只需演示几遍，代理就能复刻你的操作。

Riley 最后向观众提出请求："If you guys have any really good use cases for using the computer that the agent has access to, please let me know in the comments. I'll review all of them and that'll probably be in my updated video that I make in a month or so."（如果你们对代理的电脑有什么好的使用场景，请在评论区告诉我。我会一一查看，并很可能把它们放进我一个月后的更新视频里。）

**视觉/结构信息描述**

视频展示了：
- Journal bot 的 Grill Me 技能界面——AI 提出的追问式问题
- 代理的云端电脑桌面——可以看到浏览器打开，访问了 twitter.com
- 操作录制模式——用户可以录制演示、代理随后播放学习
- 存储在代理电脑上的文件列表

**个人感受**

Riley 对这个功能的态度有些矛盾：一边承认目前"实用性有限"，一边又表示"未来会变得非常有用"。这种诚恳的表达与大量博主夸张宣传形成对比。"I don't think this computer is that useful yet, but I do think in the future it'll get really useful because you can literally teach it a task."（我认为这台电脑目前还不是很有用，但我认为将来它会变得非常有用，因为你可以直接教它做一项任务。）

**延伸思考**

这台云端电脑的意义在于，它让"从人教、到模型学"成为可能。传统的 AI 技能创建需要写 paper 或用自然语言描述；而"演示教学"可以覆盖那些难以用文字精确描述的复杂操作。例如"公司的报销审批流程"、"如何导出发布所需的特定报表"——这些边缘案例正是语言模型不适合解决的任务。未来，当"代理使用电脑"的内容质量成熟后，每个代理都将拥有属于自己的技能泛化能力。

**精华收获**

让代理拥有"个人电脑"意味着它不仅能"懂你"，还能"动手做事"。虽然目前应用场景还很有限，但"演示教学"这个方向值得关注：未来你可能不需要写代码，不需要写提示词，只需要向它演示如何完成一项任务，它就能学会并重复执行。

---

## 综合总结：11个技巧的完整视图

### 通览全部关键配置 `[视频末尾总结段]`

Riley 在视频最后快速回顾了所有11个要点。让我们将这些要点整合为一个完整的实战体系。

| 编号 | 核心技巧 | 类型 | 核心价值 |
|------|----------|------|----------|
| 1 | Monitor The Situation Bot | 信息监控 | 持续监控关键局势，搜索高价值信息变化的推送 |
| 2 | Developer Bot + Cursor | 编程开发 | 通过自然语言委派编程任务，自动在安全分支中完成开发并交付截图/PR |
| 3 | 通用 GrokBot（什么都不做） | 通用入口 | 所有非特定任务的默认对话入口，降低管理复杂度 |
| 4 | Agents Talking to Each Other | 团队协作 | 让代理们互相沟通、汇报，甚至开"群聊会议" |
| 5 | General Project Bot | 项目交付 | 从通用对话中快速"孵化"一个专门管理项目的代理 |
| 6 | Connecting to X/Twitter | 社交媒体 | 分析推文表现、生成书签摘要、发现高价值互动者 |
| 7 | Trigger-based Automations | 事件驱动 | 让代理对 Slack/GitHub/Sentry 等实时事件做出响应 |
| 8 | Plugins | 外部连接 | 扩大代理的上下文和行动范围（Drive、Notion、日历、Linear...） |
| 9 | Multiple Gmail Accounts | 沟通自动化 | 跨邮箱分析（省钱）、发送邮件、监控回复、自动终止任务 |
| 10 | Notion + Skills | 创作工作流 | 用可折叠的 callout 格式让 AI 给文档添加上下文，不破坏文章结构 |
| 11 | Agent Has a Computer | 动手执行 | 代理拥有云端电脑，可做远程操作、录制学习、未来执行复杂任务 |

### 整个系统的宏观理解与深化

看完这 11 个技巧，我们可以提炼出一些超越单个技巧的系统性洞察：

**洞察一：GrokBot 的管理哲学是"多代理"而非"单代理"**

它并不追求一个超级智能的"全能 AI"，而是把能力分发到多个专门的代理中。这些代理各司其职，通过会话隔离保持专注，但通过技能/插件的共享保持一致，通过跨代理对话实现协同。这是一种**组织管理思维**，而不是单纯的"工具"思维。

**洞察二：简单代理 + 丰富上下文 > 复杂工作流**

Riley 反复强调"Simple but useful"（简单但有用）的设计原则。最好用的代理往往只有一两个触发条件、一两个任务目标，但如果给它们接入了丰富的上下文来源（邮件、日历、Slack、Notion、Drive），它们就能展现出远超复杂工作流的价值。这条原则也和软件开发的"简单性"原则不谋而合。

**洞察三：AI 价值不在"生成"，而在"整合"**

视频中大量案例（监控更新、订阅审查、书签汇总、多代理周报）证明了 GrokBot 的核心能力不是内容生成，而是把散落于多处的、碎片化的信息**整合成一个人可以消化的格式**。这比"生成一篇文章"更有价值。

**洞察四：流程式自动化正取代提示式交互**

一方面是"每5分钟巡查"的时间驱动自动化，另一方面是"收到消息就触发"的事件驱动自动化，Riley 展示的高级用法大多不是"问一句答一句"，而是"设好后让 AI 替我盯着"。这也呼应了未来 AI 产品的演进方向——从聊天转向自动化。

**洞察五：平台合并是一种趋势**

由于 GrokBot 是 X 和 SpaceX 的产品，它将与其他主流工具（Claude、GitHub、Cursor）深度融合。Riley 举例说明从 GrokBot 可以直接调用 Claude Opus 5 完成编程任务——未来的 AI 产品不仅要构建自己的生态，还要突破壁垒，将自己嵌入到更宽的 AI 网络中去。

### 如何立即开始：从零搭建你的 GrokBot 工作区

Riley 虽然没有给出"从零开始教程"的分步清单，但我们可以从是他整个演示过程中提炼出一套渐进式的启动路径：

**第一步：下载桌面端和移动端应用**
- 使用与 Cursor 相同的账号登录
- 探索个人电脑界面，了解每个代理的虚拟电脑的样子

**第二步：配置基础插件**
- 按你的需求为全团队添加插件：
  - 如果你有 Gmail → 连接 Gmail（尤其是你的个人邮箱）
  - 如果你使用日历 → 连接日历（GrokBot 构建"5分钟/15分钟会议提醒代理"非常快）
  - 如果你在 Notion 中管理项目 → 连接 Notion
  - 如果你是内容创作者 → 连接 X/Twitter
  - 如果你是开发者 → 连接 GitHub/Linear

**第三步：创建两个初始代理**

- **通用代理（GrokBot）**：设置描述“You do whatever. Respond to me the best you can. This chat is meant for general use.”
- **监控代理（MTS）**：
  - 规则：工作日每5分钟运行
  - 指令：“Check Slack, email, calendar, and other connected sources for any updates related to the following situations: [列出你关心的项目]”
  - 当有更新时，创建包含全列表更新的消息

**第四步：录制演示（可选）**
- 在你的代理电脑上打开浏览器，完成一个有价值的操作（比如“创建Google日历事件”的序列）
- 按“录制演示”，让代理学习；之后它就能复刻这个操作。

**第五步：随时从手机上使用**
- 安装iOS/Android应用，开启推送通知
- 散步时，用语音向通用代理“吐”想法
- 你的代理团队在云端继续工作，不必开着电脑

### 额外资料与资源

Riley 承诺会在视频描述中免费提供他创建的所有技能和代理配置，包括：
- **第一个技能**：financial insights（财务洞察）
- **第二个技能**：add context（添加上下文）
- **第三个技能**：grill me（拷问我）
- 并列出所有他创建的代理（GrokBot、MTS、Partnership bot、Journal bot、Calendar bot、Twitter bot、Slack bot、First Frame 等）

他还提到未来计划制作更多深入视频，包括：
- 触发器自动化（Trigger-based automations）的专项详细教程
- 使用 GrokBot 云电脑的使用场景合集
- 更多关于如何在业务中部署代理团队的经验

---

## 最终评价与前瞻

当我们在阅读 Riley Brown 在视频中的展示时，这不是一个关于"最新 AI 工具"的炒热帖子，而是一个**真实企业家如何将 AI 代理组织融入自己日常工作流的真实报告**。他强调实用性、强调简单但真正的价值、不回避限制和不足。这种诚实和务实的态度本身就传达了问题的真实意义。

"GrokBot"仍然在高速迭代，功能列表仍在快速增长（例如插件和触发器数量将扩展，与其姊妹产品 Cursor 的集成将更平滑）。Riley 的经验表明，AI 代理平台的爆发将不再体现在"聊天正确率"上，而是体现在"成为工作时真正的帮手"这种组织级的"代理团队"体验上。

当你真正尝试构建自己的 GrokBot 代理团队时，可以回顾 Riley 这条最核心的策略：**保持简单、充分利用上下文、让代理之间协作、用自动化释放注意力。** 这样无论未来工具怎么变，这条核心原则都能为你提供方向。

最后，借用 Riley 的一句话作为本文的收尾：**"The more context you give your agent, the more it will understand you and the more it'll be able to make good decisions in what to show you or what to create for you based on the tasks you give it."**
（"你给代理的上下文越多，它就越能理解你，就越能根据你交给它的任务，为你做出更优的决策——无论是展示给什么，还是为你创造什么。"）

这也许是整个 AI 代理时代最核心的元技能：**不是提示词，而是上下文。不是单兵作战，而是团队协同。**

---

<!-- TLDR: 用简单代理+丰富上下文构建24/7协作的AI团队，核心不在生成而在整合与自动化。 -->
<!-- TAGS: AI代理, GrokBot, 自动化, 生产力, 团队协作 -->
<!-- RATING: 4 -->
