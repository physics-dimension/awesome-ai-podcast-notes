---
title: "OpenAI just released Codex Voice (It's basically Jarvis)"
channel: "Riley Brown"
published: "2026-07-24"
source_url: "https://www.youtube.com/watch?v=hLFs9JtMaRg"
video_id: "hLFs9JtMaRg"
tags: ["AI Agent", "OpenAI Codex", "语音交互", "自动化工作流", "iOS 开发"]
rating: 5
language: "英文"
word_count: 9361
duration: "16:28"
---

# OpenAI just released Codex Voice (It's basically Jarvis)

- **Channel:** Riley Brown
- **Published:** 2026-07-24
- **Source:** https://www.youtube.com/watch?v=hLFs9JtMaRg
- **TL;DR:** 实时语音驱动的 AI Agent 首次实现了现实版 "贾维斯"，重塑人机协作。
- **Tags:** AI Agent, OpenAI Codex, 语音交互, 自动化工作流, iOS 开发
- **Rating:** 5

## 版本

- [结构化文稿](2026-07-24-openai-just-released-codex-voice-(it's-basically-jarvis)-hLFs9JtMaRg.structured.md)
- [原始文稿](2026-07-24-openai-just-released-codex-voice-(it's-basically-jarvis)-hLFs9JtMaRg.transcript.md)

# 深度重构：OpenAI Codex Voice —— 现实版 Jarvis 完全体解读

## 材料信息

- **标题**：OpenAI just released Codex Voice (It’s basically Jarvis)
- **作者/来源**：Riley Brown / YouTube
- **类型**：YouTube 视频字幕 / 沉浸式产品深度体验演示
- **关键元数据**：视频覆盖场景包括实时语音 Agent 操控、邮件自动化处理、多线程并行研发、iOS 应用语音构建、远程手机跨设备控制等。

---

## 开篇引入

在《钢铁侠》中，托尼·斯塔克与贾维斯（Jarvis）的对话场景定义了我们对 AI 终极形态的想象：一个听得懂复杂意图、能自主执行多线程任务、能控制所有电子设备、并且能跟你自由聊天的全能管家。Riley Brown 的这段视频，展示的正是这个梦想最接近现实的时刻。

他直言不讳地宣告：“**This is the closest thing I’ve seen to Jarvis.**”

这个名为“Codex Voice”的新功能，并不是简单的语音转文字输入（Dictation），而是一个嵌入在编程环境 Codex 内部的**实时语音 Agent**。在 Riley 的半小时体验中，它不仅完成了客服邮件的批量回复与总结、并行创建了多个大型软件项目的代码框架、实时调整了 iOS 应用的 UI 界面，甚至允许他躺在沙发上用手机远程指挥家里的电脑干活。

本文将带你深入 Riley 的沉浸式测试过程，解构这一次“Jarvis 时刻”背后的人机协作范式革命，并提供超越视频本身的深度洞察。

---

## 详细内容

### 【1】超越语音助手：真正的 Jarvis 诞生 `[章节：引言与概念界定]`

**核心观点**

Codex Voice 并非传统意义上的语音助手或语音输入法，而是一个具备了“自我意识”与“行动力”的操作系统级 Agent。它将语音交互与计算机深度自动化进行了融合。

**深度阐述**

Riley 在视频开头就奠定了全文的基调：兴奋与震撼。他指着 Codex 界面右下角的“Start New Voice Chat”按钮，定义了这个划时代的功能。

> “This is what I call the new Jarvis feature, which is different than dictating, right? Jarvis is real-time voice.” `[章节：引言 / 功能定义]`

这句话极其关键。Dictation（听写）仅仅是取代了你的键盘，让你用嘴巴打字——本质上依然是“单向输入”。而“Jarvis 模式”意味着你是在对一个**真正理解你的、能够自主思考并执行复杂任务**的智能体说话。你可以下达一个包含多步骤、多目标的高层次指令，剩下的全部交给这个 Agent 去规划和执行。

Riley 特别强调了他过去六个月积累的“Skills”（技能）现在可以被即时调用。这些 Skills 涵盖了调用 Gmail、操作 Notion、控制本地文件系统、编译代码库、管理浏览器标签页等众多能力。在过去，这些能力被封装在各自孤立的 API 脚本或自动化工具中；但在 Codex Voice 中，它们被语音这个**人类最自然的接口**串联成一个整体，以“神经网络”的形式统一调度。

这标志着 AI 从一个需要人类不断喂指令的“工具”，进化成了可以接受模糊目标、自主分解任务、动态调用工具的“数字代理”。Riley 将这一时刻称为 **Jarvis 时刻**，正是抓住了这个本质。

**个人感受**

Riley 的激动难以言表。他不禁感叹道：

> “I will never get tired of this.” `[章节引言 / 情感基调]`

他并不是在展示一个冷冰冰的功能列表，而是在分享一种全新的、与计算机协作的范式。那种“我只是说说，它就全给干了”的掌控感，对于任何一个长期被繁琐数字操作所困的人来说，都极具冲击力。

**延伸思考**

语音不仅仅是输出指令的通道，更是反馈回路的一部分。以往我们需要用眼睛盯着屏幕来确认 AI 是否执行正确，现在 Agent 能用自然语言实时汇报：“处理完毕”、“正在编译”、“已打开全部标签页”。这种**多模态的融合**极大加速了人机交互的节奏。当人类从“扫描屏幕等待结果”的桎梏中解放出来，他的大脑可以腾出更多的认知带宽专注于更高层次的战略思考。

---

### 【2】实战一：邮件风暴与客服排雷 `[章节：真实商业场景压力测试]`

**核心观点**

在真实的商务工作流中，Codex Voice 展示了惊人的并行处理与多步骤规划能力，将原本可能需要半小时的客服邮件处理流程，压缩进几句自然对话之中。

**深度阐述**

Riley 并没有拿这个功能去做什么炫技的事情，而是直接对准了最枯燥、最耗时的日常工作——邮件处理。他发出了第一条作战指令：

> “Hey buddy, can you hear me? ... I need you to go to my email right now. I want you to find any complaints for customer support. I want you to draft a response to all of them and I want you to open them inside the Codex browser.” `[章节：邮件处理 / 初始指令]`

这是一句包含四个子目标的指令：
1. 连接并扫描邮箱；
2. 进行语义搜索，识别“投诉”；
3. 为每一封邮件撰写回信草稿；
4. 将所有邮件在浏览器的独立标签页中打开。

Agent 的回应干脆利落：“**Sure, I'll take care of that.**”

几秒钟后，12 个包含投诉邮件的标签页在 Codex 内置浏览器中瞬间铺开。不仅打开了邮件，Agent 同时报告已经写好了 11 封回信草稿。整个过程是实时的，Riley 甚至可以在中途静音麦克风跟观众解释情况。

紧接着，Riley 继续用语音驱动物流：
“Turn all of these into... a new Google Doc... open it up in a new tab in the browser... a good summary of the issues going on with our product.”

几分钟前还是分散在收件箱里的垃圾邮件，现在变成了一份结构化的内部报告。但这还没完——Riley 继续发号施令：
“Make this document public... and then I want you to text it to Emily Lambert for me.”

Agent 完成了文档权限设置，准备好发送。但 Riley 突然想起了更重要的事：
“Add a little extra note... Hey, can we get these fixed by the end of the day?”

Agent 再次确认并执行：“**Got it. Sending that. I'm sending it now.**”

**个人感受**

当 Agent 完成短信发送后，Riley 沉默了片刻，然后给出了这个环节的最高评价：
“**This is Jarvis. You’re literally Jarvis.**” `[章节邮件流程结束 / Riley 评价]`

他的兴奋不仅仅来自于“事情办成了”，而是来自于角色体验的彻底颠覆。在这个过程中，他不再是那个需要埋头在收件箱里一封封点开、阅读、回复、复制粘贴、打开短信工具、调整文档权限的“数字打工人”。他变成了一个发号施令的指挥官，而 Agent 就是那个不知疲倦的、拥有一秒钟处理完所有数字操作能力的精英小队。

**延伸思考**

这个案例揭示了一个深层次的工作流变革：**自然语言正在成为新的编程语言。** Riley 的指令本质上是一种高度结构化的 Prompt。在过去，实现这个自动化流程意味着要写一个复杂的 Google Apps Script，或者对接 Zapier 和 Make 等无代码工具的 API。现在，这一切被简化成了自然对话。更重要的是，**交互具备极高的容错性和动态调整性**——你可以随时中断任务、追加修正、模糊表达，Agent 都能理解。

---

### 【3】多线程并行主义：脑暴中的意识分裂 `[章节：异步与多任务处理]`

**核心观点**

Codex Voice 通过后台派生独立会话的方式，实现了真正意义上的多线程并行工作。用户可以在与主 Agent 保持实时对话的同时，协管后台的复杂任务。

**深度阐述**

接下来的场景切换到了 Excalidraw（一个实时协作白板工具）进行产品功能的头脑风暴。Riley 想让 Agent 去搜索关于“Codex Voice”这个功能的资料，并将结果整理成一个结构化的 Notion 文档，使用他自己的特定排版风格（Tab 分页、超链接）。

然而，这里发生了一个极具代表性的场景——Agent 展现出了它的**元认知能力**。

> Riley: “I want you to go off, do some research, and I want you to create a new Notion doc... do in-depth research on this.”
> Riley: “Actually, wait. I kind of want to continue talking to you. So, can you actually do this in a different chat?”
> Agent: “**Yes. I spun that into a separate task so we can keep talking here.**” `[Quote / Agent 主动并行化]`

这太关键了。Agent 意识到这个研究任务会长时间占用后台资源，从而阻塞主会话的实时交互。于是它主动创建了一个全新的、**上下文完全隔离**的聊天会话来处理搜索和文档生成。Riley 几乎不敢相信自己的耳朵：
“So, did you just create a new chat so that we could just continue talking, right?”
“Yes.”

在这个子任务在后台默默运行的同时，Riley 继续在主会话中与 Agent 对话，调整 Excalidraw 画板上的产品定义，要求 Agent 添加“Spin up new sessions”等用例，它都实时响应了。几分钟后，当研究任务完成，Agent 自动将已经排版好的 Notion 文档在浏览器中打开。
“And by open it, I just mean I want it in the Codex browser. Got it. I’ll open the notion note here as soon as the task finishes.”

**个人感受**

当那个严格按照 Riley 风格（Tab 分页、带有超链接、标题层级清晰）的 Notion 文档出现在屏幕上时，Riley 发出了彻底被征服后的惊叹：
“**Oh my god, it opened it. Look at this. This is truly insane.**” `[章节：Notion 文档生成 / Riley 反应]`

他不敢相信自己随口说说的格式要求被完美复现，更不敢相信在这个文档创建的全过程中，他一直在忙着做另一件事，没有丝毫等待。

**延伸思考**

这种“任务拆分与隔离”的能力，彻底解决了当前 AI 对话窗口的最大痛点：**上下文污染**。过去，如果你在一个窗口中让 AI 写完了长篇小说，再让它帮你规划周末行程，前者的叙事画风和角色名字很可能会莫名其妙地出现在你的购物清单里。Codex Voice 通过动态派生新会话，保证了不同任务之间的“记忆隔离”，同时又通过主 Agent 保留了“全局协调”的能力。**这是迈向通用 Agent 架构的关键一步。**

当被问及安全限制时，Agent 提供了非常透明的答复：“A skill won't override those safeguards... I can draft a text... but I won't actually send anything unless you explicitly tell me to.” 这体现了“人在回路中”的核心设计原则，平衡了效率与安全。

---

### 【4】闭环创作：用嘴写一个 iOS 应用 `[章节：代码工程与可视化输出]`

**核心观点**

语音不再仅仅是处理文字或调度软件的接口——它能够直接介入图形用户界面（GUI）的编程与编译循环。Riley 仅用几分钟的对话时间，就完成了一个包含全部逻辑和精美 UI 的 iOS 备忘录应用。

**深度阐述**

这可能是在全片中最令人瞠目结舌的环节。Riley 对着麦克风，像点菜一样轻松地说出了当天的核心开发任务：

> “I want to create an iOS app... a Swift app that is like an exact replica of the Apple Notes app and I want you to run it in the inapp simulator in Codex.” `[章节：iOS 开发 / 初始需求]`

翻译过来就是：帮我写个软件，跑起来给我看看。

在代码生成的同时，Riley 一句话说不满足于只做一个 App：
“And you know what? While you're at it, can you please spin up two more chats? And I want one to be a Notion clone and then the other one to be a Trello clone. Spin off two more chats and do that for me, please.”

三个大型软件项目——Apple Notes 克隆体、Notion 克隆体、Trello 克隆体——同时被语音驱动，在后台并行开发和编译。而在主会话中，Riley 依然在和 Agent 讨论设计细节，Agent 则一边听着调改指令，一边修改代码，一边在 Codex 内置的模拟器中运行演示。

最令人印象深刻的设计迭代环节：
“I actually want the default to be light mode. Change it to light mode. And please make the bottom tab, like the liquid glass tab at the bottom, higher quality.”

Agent 当场回应：“**Got it. Making those updates now.**” 几秒钟后，模拟器中的 App 界面更新了：亮色模式、精致的毛玻璃浮动标签栏，全部实现。

**个人感受**

当 Agent 完成调整，把精美的“Memo Canvas”模拟器界面展示给 Riley 时，Riley 深吸一口气，给出了最高评价：
“**Wow. This is just truly insane. Thank you, Codex.**” `[章节 / iOS App 完成 / Riley 评价]`

这一刻，编程的门槛被彻底击穿。对于 Riley 这样的开发者来说，他不再需要在一堆代码中艰难定位 `color` 和 `cornerRadius` 的变量；对于非开发者来说，一个全新的创造世界打开了——任何人都可以用自己的母语，自然地构建属于自己的数字工具。

**延伸思考**

这引发了一个关于“创造力释放”的深度思考。工具的终极形态是“消失”（Invisible）。Codex Voice 正在让电脑操作系统变得“不可见”。交互回归到了最本质的语言：**我想要什么，你就帮我做什么。** 软件开发正在从“工匠时代”进入“指令时代”。未来的软件工程师，将更像一个乐团的指挥家，懂得如何将庞大的系统拆解成可对话的模块，然后用自然语言去协调它们在后台的协奏。

---

### 【5】最后一公里：来自手机端的远程灵魂 `[章节：生态联动与移动端控制]`

**核心观点**

利用 ChatGPT 官方 iOS 应用对“配对远程访问”新功能的支持，Codex Voice 实现了跨设备的实时无缝连接。用户可以通过手机，远程驱动工作电脑上的 AI Agent。

**深度阐述**

视频末尾，Riley 展示了可能是最科幻的场景：他直接拿起 iPhone，打开 ChatGPT，用实时语音模式连接到了远端的 MacBook 上的 Codex 环境。

> “I'm using you for the first time. I'm using this on remote... so apparently you're working on my Mac.” `[章节：手机远程 / 初始连接]`

仅仅通过手机语音，他直接操控了远端 Mac 上的 Codex 环境。他要求 Agent 查看之前正在运行的“Memo Canvas”应用的当前状态，以及检查客服邮件的摘要。

Agent 不仅完成了任务，还展示了一个极其强大的能力：**全局会话意识**（Cross-session awareness）。
Agent 回答道：“That's the Memo Canvas app task you made earlier, and it's active. The latest light mode build with the liquid glass tab bar is still running in the simulator.”

这意味着 Agent 能够感知到“其他地方发生了什么”——它知道手机端这个新会话和桌面端正在执行的任务是同一个人的、是同一套生态。你的 AI 不再是某个具体界面的附属品，而是一种**持续存在的、跨设备的云端数字力量**。

**个人感受**

Riley 在自己总结时反复强调自己被“blown away”。这种跨设备无缝漂移的体验，彻底颠覆了他对 AI 功能边界的认知。Riley 感叹道：“You just fully control your computer in real-time voice directly from the ChatGPT iOS app.” `[章节：总结 / 体验评价]` 你的大脑不再被禁锢在某个特定的工作台前。

**延伸思考**

这是“无所不在的计算”（Ubiquitous Computing）的真正落地。你的个人计算 Agent 不再是“屏幕里的一个窗口”，而是随时可以通过语音唤起的服务。哪怕你出门在外，家里或办公室的电脑依然在你的语音指令下运转。如果你有任何想法，不需要等到坐在电脑前，掏出手机说出来，一切就已经开始落实。

---

### 【6】结语：这只是个开始 `[章节：总结与未来展望]`

**核心观点**

Riley 非常坦诚地表示，这只是他上手 30 到 45 分钟后的初步体验。真正的生产力探索刚刚开始，这是一个新时代的序幕。

**深度阐述**

在密集放完一系列“大招”后，Riley 并没有强行给出一个天花乱坠的结论。相反，他表现出了非常克制的、负责任的分享态度：

> “Obviously I've only spent like 30 minutes to 45 minutes using this. So, I'll probably do a much more in-depth video once I kind of learn the best practices.” `[章节：结尾 / Riley 承诺]`

他承认自己在测试过程中遇到了浏览器标签页被误关闭、新模式下的界面适应等问题，但他展示的“可能性”已经远远超过了当前任何一种 AI 产品。他表示未来几天将深度使用，并制作一套“最佳实践指南”，这无疑是给所有被电影震撼到的观众留下了一个巨大的期待空间。

**精华收获**

1. **实时全栈操控**：从邮件到代码，从 GUI 操作到文档生成，一个语音通道完成。
2. **后台多线程并行**：能够自主创建子任务，进行“同一大脑、不同脑叶”的并行工作。
3. **跨设备远程介入**：手机端远程唤醒电脑端的 Agent 生态，实现永不间断的接入。
4. **安全边界坚固**：Agent 可以起草高危操作（发短信、付款），但杜绝自主执行，必须由人显式确认。这兼顾了效率与安全。
5. **编程范式的彻底转移**：软件开发正在从“基于关键字和逻辑”转向“基于意图和自然语言”。未来的软件交互，始于你说出“我想要……”

---

## 总结

Riley Brown 用半小时的沉浸式体验，向全世界展示了 OpenAI Codex Voice 带来的冲击。这不是一次简单的功能更新，而是宣告了 **AI Agent 正式进入实时语音驱动机器控制** 的时代。当你能够用最自然的对话，去命令电脑并行运行三个软件的编译、处理客服投诉、管理短信与文档权限、调整设计稿的细节，**你就不再是在“使用”电脑，而是在与一个能够理解你的数字伙伴“协作”**。

你准备好了吗？

---

<!-- TLDR: 实时语音驱动的 AI Agent 首次实现了现实版 "贾维斯"，重塑人机协作。 -->
<!-- TAGS: AI Agent, OpenAI Codex, 语音交互, 自动化工作流, iOS 开发 -->
<!-- RATING: 5 -->
