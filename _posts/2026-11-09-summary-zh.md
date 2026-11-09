---
layout: default
title: "Horizon Summary: 2026-11-09 (ZH)"
date: 2026-11-09
lang: zh
---

> 从 906 条内容中筛选出 28 条重要资讯。

---

1. [Anthropic 的 Fable 5.2 声称用 1,000 个 Agent 证明费马大定理，但“削弱”争议抢尽风头](#item-1) ⭐️ 9.0/10
2. [AI Agent 用 Lean 证明破解量子代码](#item-2) ⭐️ 9.0/10
3. [通用 AI 模型零样本碾压专用机器人策略](#item-3) ⭐️ 9.0/10
4. [AI 说服力超越世界冠军辩手，即使他们获得报酬](#item-4) ⭐️ 9.0/10
5. [Google 消费级 Gemini 将你的 Gmail 和 Drive 文件交给人工审核员](#item-5) ⭐️ 8.0/10
6. [E-means：k-means 聚类速度提升 10 倍，损失不增](#item-6) ⭐️ 8.0/10
7. [Meta 发布 Muse Ember：每百万 token 仅 10 美分的 Agent 模型](#item-7) ⭐️ 8.0/10
8. [黄仁勋 CEO 之位：五五开的硬币抛掷？](#item-8) ⭐️ 8.0/10
9. [AI Agent 终于学会从错误中学习：forge\_dc 系统](#item-9) ⭐️ 8.0/10
10. [Prompt Injection 防护在 legal contracts 上惨败](#item-10) ⭐️ 8.0/10
11. [Claude Code v2.1.321：新默认模型、1M 上下文与关键安全修复](#item-11) ⭐️ 7.0/10
12. [USPS 终于开卖 ZIP Code 边界多边形，但 $10K 起价让人肉疼](#item-12) ⭐️ 7.0/10
13. [Claude Fable 5.2 登顶 AI 指数，但你的钱包要遭殃](#item-13) ⭐️ 7.0/10
14. [Anthropic 斥资 34 亿美元购买天然气涡轮机为 AI 供电](#item-14) ⭐️ 7.0/10
15. [OpenAI 的 Control Room：失控模型的紧急停止开关](#item-15) ⭐️ 7.0/10
16. [Google 发布 TPU 8i Max 和 8tx：双芯片封装与机密推理](#item-16) ⭐️ 7.0/10
17. [Baidu 的 ERNIE Evolve 让 AI 自己搞研究，还破了 NanoGPT 纪录](#item-17) ⭐️ 7.0/10
18. [XGBoost 预测停电效果超 NWS 警告 2.4 倍](#item-18) ⭐️ 7.0/10
19. [JEPA 式触觉预训练在灵巧操作任务上碾压 MAE/VAE 基线](#item-19) ⭐️ 7.0/10
20. [SwarmEvolve：潜在空间智能体集群碾压 AlphaEvolve 克隆](#item-20) ⭐️ 7.0/10
21. [Twindex：证明你的数据无法区分两组参数](#item-21) ⭐️ 7.0/10
22. [新基准测试显示：编程 Agent 还无法构建 3D 世界](#item-22) ⭐️ 7.0/10
23. [Claude Opus 5.5 弃用 Three.js，手写原生 WebGL 法贝热彩蛋](#item-23) ⭐️ 6.0/10
24. [用 &lt;details&gt;&lt;summary&gt; 折叠你的 AI 垃圾 PR 描述](#item-24) ⭐️ 6.0/10
25. [Apple 在 Logic Pro 中开始收取 $50 的额外 AI 使用费](#item-25) ⭐️ 6.0/10
26. [Disney 与 Adobe 联手打造艺术家主导的 AI](#item-26) ⭐️ 6.0/10
27. [NVIDIA 发布 900 万合成日本金融 Persona：隐私安全还是纯属虚构？](#item-27) ⭐️ 6.0/10
28. [HOPE：高阶剪枝让 MoE 专家搭档不再分离](#item-28) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic 的 Fable 5.2 声称用 1,000 个 Agent 证明费马大定理，但“削弱”争议抢尽风头](https://www.anthropic.com/claude-fable-and-mythos-5-2) ⭐️ 9.0/10

Anthropic 发布了 Claude Fable 5.2 和 Mythos 5.2，声称 1,000 个 Fable 5.2 agent 组成的集群在短短 30 小时内、以极少人工干预，在 Lean 中完全形式化了费马大定理。此次发布还引发了争议：上一代模型 Opus 5.5 是否在发布前被故意削弱。 如果费马大定理的声明站得住脚，那将是 AI 驱动形式化数学的真正里程碑——但这里真正的故事是信任。社区指责 Anthropic 悄悄削弱 Opus 5.5 来让新模型显得更强大，这比任何基准测试都重要得多。 这个 1,000-agent 证明没有使用任何数学参考文献，只依赖一份中间定理陈述列表，并且仅依赖 Lean 的三条标准公理，没有未证明的占位符。与此同时，评论者质疑基准测试的设置，指出 Fable xHigh 对比 Carbon Med 等奇怪比较，以及 Carbon 在一个网络安全基准测试中缺席。

hackernews · meetpateltech · 11月9日 18:56 · [社区讨论](https://news.ycombinator.com/item?id=50429906)

**背景**: 费马大定理指出，对于 n &gt; 2，不存在三个正整数满足 a^n + b^n = c^n，Andrew Wiles 在 1994 年给出了著名的证明，但那是纸上的证明。形式化意味着将整个证明翻译成 Lean 这样的计算机语言，以便逐行验证——这通常需要人类数学家花费数年时间。Anthropic 此前曾让一个未发布的研究版 Claude 在人类指导下用 11 天完成形式化；现在他们声称 1,000 个 agent 组成的集群在 30 小时内完成了。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5 . 2 and Claude Mythos 5 . 2 \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/research/formalizing-fermats-last-theorem">Formalizing Fermat&#x27;s Last Theorem \ Anthropic</a></li>
<li><a href="https://lean-lang.org/use-cases/flt/">Formalizing Fermat&#x27;s Last Theorem in Lean: A Landmark ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论出现分歧：一些人对费马证明感到兴奋，但许多人对 Opus 5.5 被削弱的指控感到愤怒，一位评论者说“这看起来一点都不好”。其他人质疑普通用户是否真的需要 Fable/Mythos 而非 Opus 5.5，还有一些人在仔细挑刺基准测试方法。

**标签**: `#AI`, `#LLM`, `#Anthropic`, `#model release`, `#formal verification`

---

<a id="item-2"></a>
## [AI Agent 用 Lean 证明破解量子代码](https://arxiv.org/abs/2611.09822) ⭐️ 9.0/10

来自 Google DeepMind 及其他机构的研究人员在 Lean theorem prover 中构建了一个量子程序库，LLM agents 在其中合成并形式化验证量子程序，在量子算术上实现了高达 290 倍的加速，并在聚变、光化学和药物代谢模拟中分别实现了 11 倍、8 倍和 2.5 倍的改进。 这是一件大事，因为它表明 AI 能够发现可证明正确且比人类设计的算法好得多的量子算法，即使经典计算机无法完全测试它们。它通过自动化算法设计瓶颈，可能极大地加速实现实际量子优势的进程。 这些 agents 通过 wikis 和会议协作，共享知识以根据形式化规范合成程序，而 Lean 证明保证了正确性和成本，无需在量子硬件上运行。量子算术上 290 倍的改进尤其引人注目——这不是渐进式的，而是另一个级别的提升。

rss · arXiv AI · 11月9日 05:00

**背景**: 量子算法通常由专家团队花费数年设计，测试它们很困难，因为经典计算机只能模拟小型量子系统。Lean 是一个定理证明器，允许你编写计算机可以检查的数学证明，因此如果你在 Lean 中编码一个量子程序，你就可以证明它做了它应该做的事。这项工作将 LLM agents 与 Lean 结合，自动化发现循环，类似于 AI 加速数学和编码的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lean-lang.org/">Lean Programming Language</a></li>
<li><a href="https://newsphysics.com/en/articulo/c8be82e7-5883-4603-99b3-53736d62f698">AI agents discover formally verified quantum programs</a></li>
<li><a href="https://arxiv.org/pdf/2501.18639">A Comprehensive Survey of the Lean 4 Theorem Prover ...</a></li>

</ul>
</details>

**标签**: `#quantum computing`, `#formal verification`, `#large language models`, `#automated discovery`, `#Lean theorem prover`

---

<a id="item-3"></a>
## [通用 AI 模型零样本碾压专用机器人策略](https://arxiv.org/abs/2611.09892) ⭐️ 9.0/10

一篇新的 arXiv 论文提出了 agentic manipulation policies（AMPs），即由通用 AI 模型直接控制机械臂。他们的参考框架 AMP1 在 RoboLab-120 上零样本达到 85.6%的成功率，而领先的 VLA 和 WAM 策略分别只有 49.2%和 42.9%；在涵盖 12 个任务的 108 次真实世界试验中成功了 104 次。 这很重要，因为它表明用演示数据训练专用机器人策略这条昂贵且依赖大量数据的路线可能是错的。如果通用模型能直接“现场发挥”搞定操作，那么整个 VLA/WAM 行业的护城河都需要重新思考。 基础框架不提供任何抓取、推动或放置技能——agent 自己发展出寻找隐藏物体、使用工具和校准摄像头等策略。加入跨 episode 的持久记忆存储后，双臂任务的失败率又降低了 4.6 倍，暗示经验回放是下一个突破口。

rss · arXiv AI · 11月9日 05:00

**背景**: 机器人操作传统上依赖专用策略：针对单一任务、用数千次人类演示训练出的模型。VLA（视觉-语言-动作模型）和 WAM（世界动作模型）是当前的宠儿，它们结合视觉、语言和动作预测。AMP 则颠覆了这一思路：让通用 AI 模型（如大型多模态模型）直接向机器人发指令，并随任务进展自适应调整，无需任何任务特定训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2611.09892">[2611.09892] On Agentic Manipulation Policies - arXiv.org</a></li>
<li><a href="https://github.com/apple-aiml-research/ml-amp">GitHub - apple-aiml-research/ml-amp: AMP: Agentic ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision%E2%80%93language%E2%80%93action_model">Vision–language–action model - Wikipedia</a></li>

</ul>
</details>

**标签**: `#robotics`, `#manipulation`, `#generalist AI`, `#zero-shot learning`, `#agentic policies`

---

<a id="item-4"></a>
## [AI 说服力超越世界冠军辩手，即使他们获得报酬](https://arxiv.org/abs/2606.16475) ⭐️ 9.0/10

一篇新的 arXiv 论文（2606.16475）报告了四项预注册实验，共 18,978 次对话，显示 AI 系统在说服力上稳定超越专家人类，包括专业拉票员和世界冠军辩手，即使这些人类可以选择话题、提前研究、进行数小时练习，并获得 1,000 英镑奖金。后续研究发现，即使专家获得了针对击败他们的 AI 进行练习的辅导工具，AI 的优势依然存在；在真实世界测试中，AI 为 Save the Children 筹集的捐款是专业拉票员的 3 倍以上。 这很重要，因为它打破了人类在说服力上拥有主场优势的舒适假设——如果 AI 能辩赢世界冠军并更有效地筹集真实资金，那么每一次在线辩论、政治竞选和筹款宣传现在都容易受到大规模自动化操纵的影响。AI 的优势仅仅来自更快地输出更多信息，而非更优越的推理，这一事实应该让任何认为监管能跟上的人感到担忧。 研究发现了趋同的证据，表明 AI 的优势源于快速部署大量信息：经过辅导后，专家人类只能与一个被限制为人类响应速度和人类长度消息的 AI 打成平手。这是一个巧妙的实验技巧——它将速度和信息量隔离为关键因素，而不是某种神奇的说服洞察力。

rss · arXiv AI · 11月9日 05:00

**背景**: 说服力竞赛决定了许多社会决策——比如选举、政策辩论或慈善筹款。AI 聊天机器人是这个领域的新参与者，但直到现在还不清楚它们能否击败有动力获胜的熟练人类。这项研究以其规模和严谨性著称：近 19,000 次对话、预注册设计（即在数据收集前锁定假设），以及真实世界的利害关系，如实际捐款。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Preregistration_%28science%29">Preregistration (science) - Wikipedia</a></li>
<li><a href="https://www.cos.io/initiatives/prereg">Preregistration - Center for Open Science</a></li>
<li><a href="https://arxiv.org/pdf/2411.06837">Persuasion with Large Language Models: A Survey of Empirical...</a></li>

</ul>
</details>

**标签**: `#AI persuasion`, `#human-AI interaction`, `#experimental psychology`, `#AI safety`, `#societal impact`

---

<a id="item-5"></a>
## [Google 消费级 Gemini 将你的 Gmail 和 Drive 文件交给人工审核员](https://github.com/thisisme6598/gemini_files/) ⭐️ 8.0/10

一份报告和 Hacker News 讨论揭示，Google 的消费级 Gemini 在连接 Gmail 和 Drive 等应用时，可能会将个人文件和邮件路由给人工标注员进行审核。讨论澄清，这仅适用于带有 Connected Apps 的消费级 Gemini，而非 Workspace Gemini。 这很重要，因为它打破了 AI 助手是私人保险箱的幻想——如果你将 Gmail 或 Drive 连接到消费级 Gemini，你最敏感的数据可能会落入陌生人眼中。Google 的企业版提供更强的隐私保证，这意味着普通用户实际上是在用隐私换取便利。 关键区别在于，Workspace Gemini 和 Workspace Intelligence（面向企业的 RAG 系统）明确声称不受人工审核，而带有 Connected Apps 的消费级 Gemini 则不然。因此，一旦你在消费级 Gemini 中授权 Gmail 工具，你的邮件就可能成为标注的对象。

hackernews · gf74918 · 11月9日 18:24 · [社区讨论](https://news.ycombinator.com/item?id=50429426)

**背景**: Google 的 Gemini 有不同的版本：面向日常用户的消费级版本和面向企业的 Workspace 版本。当你将 Gmail 或 Drive 等应用连接到消费级版本时，Gemini 可以读取你的数据来回答问题或执行任务。但像许多 AI 产品一样，Google 使用人工审核员来改进模型——这可能包括你的个人数据。企业客户通常获得更严格的隐私条款，这就是为什么消费级/Workspace 的区分在这里很重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.google.com/gemini/answer/13594961?hl=en">Gemini Apps Privacy Hub - Gemini Apps Help</a></li>
<li><a href="https://blog.google/products-and-platforms/products/workspace/workspace-june-drop-gemini-workspace-apps/">Gemini now connects to Google Workspace apps - The Keyword</a></li>
<li><a href="https://privacyinternational.org/explainer/5357/humans-ai-loop-data-labelers-behind-some-most-powerful-llms-training-datasets/">Humans in the AI loop: the data labelers behind some of the ...</a></li>

</ul>
</details>

**社区讨论**: 评论者感到沮丧和怀疑：bri3d 澄清了消费级与 Workspace 的区别，而 rustyhancock 分享了一个诡异的轶事，称 Gemini 的回复与最近一封邮件异常契合却未披露。EMM\_386 和 gla67890543 表达了更广泛的不信任，指责 Google 的商业模式和隐私规范的侵蚀。

**标签**: `#privacy`, `#Google Gemini`, `#AI data handling`, `#consumer trust`, `#human annotation`

---

<a id="item-6"></a>
## [E-means：k-means 聚类速度提升 10 倍，损失不增](https://e-means.github.io/) ⭐️ 8.0/10

一篇新论文（arXiv:2611.09501）提出了 e-means，一种基于指数移动平均的 k-means 优化方法，采用 mini-batch 更新，声称在相同损失下比 Lloyd&\#x27;s algorithm 快 10 倍，且通常收敛到比 k-means++ 更低的损失。 这很重要，因为 k-means 是数据分析、检索和量化中最广泛使用的聚类算法之一，在相同损失下实现 10 倍加速可以大幅降低大规模聚类的成本——而社区报告的 146 倍 GPU 加速表明实际应用中收益可能更大。 该方法使用指数移动平均优化和 mini-batch 更新，借助现代深度学习工具，并建立了衰减率和批量大小的 scaling laws，从而无需超参数扫描；不过，一位社区成员指出这些超参数规律感觉像是事后拟合的。

hackernews · porridgeraisin · 11月9日 18:45 · [社区讨论](https://news.ycombinator.com/item?id=50429734)

**背景**: K-means 聚类是一种经典算法，通过最小化数据点与聚类中心之间的距离将数据分成 k 组。标准方法 Lloyd&\#x27;s algorithm 简单但可能很慢，因为它需要对整个数据集进行多次遍历。E-means 借鉴了深度学习优化的思想——如 mini-batch 更新和指数移动平均——来加速收敛，类似于神经网络训练中 Adam 等优化器的工作方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/K-means_clustering">k-means clustering - Wikipedia</a></li>
<li><a href="https://arxiv.org/pdf/1612.02099">Statistical and Computational Guarantees of Lloyd ’ s Algorithm</a></li>

</ul>
</details>

**社区讨论**: 社区既兴奋又谨慎：一位用户报告在 IVF 索引上实现了 146 倍 GPU 加速，另一位称赞可视化效果并希望集成到 scipy，而一位怀疑者质疑超参数规律是否是事后拟合的；还有用户发现它不适用于网格松弛，因为 e-means 的优势在于减少对大型数据集的遍历次数，而非每次遍历更好。

**标签**: `#k-means`, `#clustering`, `#algorithms`, `#performance`, `#machine-learning`

---

<a id="item-7"></a>
## [Meta 发布 Muse Ember：每百万 token 仅 10 美分的 Agent 模型](https://techcrunch.com/2026/11/09/meta-releases-muse-ember-a-new-lightweight-model-for-agent-execution/) ⭐️ 8.0/10

Meta Superintelligence Lab 发布了 Muse Ember，这是其迄今为止最小、最具成本效益的模型，专为 agent 执行任务（如工具调用、路由和子 agent 工作）而设计。定价为每百万输入 token 0.10 美元，显著低于 Claude Haiku 5.5 和 GPT-6 Luna 等前沿竞争对手。 对于任何构建大规模 agent 系统的人来说，这是一件大事：agent 工作流会在重复的子任务上消耗大量 token，而 Ember 极低的价格可能使高容量 agent 管道在经济上可行。这也表明 Meta 打算在成本上积极竞争，而不仅仅是原始智能，这给 Anthropic 和 OpenAI 带来了压力，要求它们证明其溢价定价的合理性。 Ember 在 Artificial Analysis Intelligence Index 上得分为 36，与 Claude Haiku 5.5（max）持平，但每任务成本仅为其三分之一；其缓存输入 token 价格仅为每百万 0.004 美元——是输入价格的 4%，而 Haiku 和 Luna 为 10%。它旨在与更大的 Muse 模型（如 Spark 或 Wonder）搭配使用，由大模型负责规划，Ember 处理大量工作。

rss · TechCrunch AI · 11月9日 18:00

**背景**: Meta 一直在构建其 Muse 模型家族，而 Ember 是轻量级的主力模型，用于 agent 工作流中枯燥但必不可少的部分——每天发生数百万次的工具调用、路由决策和子 agent 任务。可以把它想象成一个快速、廉价的职员，处理日常文书工作，以便昂贵的高级合伙人（大模型）能够专注于战略。这一定价策略直接瞄准了 Anthropic 的 Haiku 和 OpenAI 的 Luna，它们一直主导着低成本 agent 市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.meta.ai/docs/muse-ember">Muse Ember - Meta Model API</a></li>
<li><a href="https://artificialanalysis.ai/articles/meta-s-muse-ember-is-the-cheapest-model-scoring-36-on-the-intelligence-index">Meta&#x27;s Muse Ember is the cheapest model scoring 36 on the ...</a></li>
<li><a href="https://techcrunch.com/2026/11/09/meta-releases-muse-ember-a-new-lightweight-model-for-agent-execution/">Meta releases Muse Ember, a new lightweight model for agent ...</a></li>

</ul>
</details>

**社区讨论**: 评论者议论纷纷：simonw 通过生成鹈鹕测试了 Ember 的六个努力级别，发现更多推理 token 并不总是意味着更好的 SVG，这打破了通常的相关性。Retro\_Dev 感叹“最小”的模型并非开放权重，而 kbrannigan 预测未来会像早期 PC 时代一样，每个专业都有专门的模型。

**标签**: `#AI/ML`, `#LLM`, `#agents`, `#Meta`, `#model release`

---

<a id="item-8"></a>
## [黄仁勋 CEO 之位：五五开的硬币抛掷？](https://techcrunch.com/2026/11/08/is-jensen-huangs-job-on-the-line-yales-jeffrey-sonnenfeld-estimates-its-about-a-50-50/) ⭐️ 8.0/10

Nvidia 董事会已对 CEO Jensen Huang 与一名疑似中国间谍的关系展开独立调查，Yale 的 Jeffrey Sonnenfeld 估计 Huang 留任 CEO 的概率大约为 50%。消息公布后，公司股价下跌超过 4%。 这是全球最重要 AI 芯片公司的一场真正治理危机，而不只是小报丑闻。如果 Huang——AI 繁荣的代言人——被迫离职，将动摇 Nvidia 的战略、其在中国的风险敞口，以及整个依赖他每一句话的 AI 硬件供应链。 做空机构 Culper Research 在丑闻爆发六个月前就曾警示 Huang 与 Alice Huang 及 Megaspeed 之间“令人不安的密切”关系，而 Nvidia 此前坚称一切“正常”的表态如今可能变成代价高昂的法律责任。董事会声明将 Huang 描述为“外国情报活动的目标”，这对 CEO 来说是一个极其尴尬的辩护立场。

rss · TechCrunch AI · 11月9日 05:26

**背景**: Nvidia 是 AI 芯片领域无可争议的王者，而 Jensen Huang 是其创始人 CEO 和公众面孔。董事会调查他是否被外国情报活动所渗透，这种事足以终结一位 CEO 的任期——或至少永久损害信任。Jeffrey Sonnenfeld 是 Yale 知名的管理学教授，专门研究 CEO 领导力，因此他“五五开”的判断颇有分量，尽管这终究只是一种猜测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/08/nvidia-jensen-huang-email-board-of-directors-statement.html">Read Huang&#x27;s email to his staff and statement from Nvidia &#x27;s board</a></li>
<li><a href="https://www.globenewswire.com/news-release/2026/11/08/3398017/0/en/statement-from-nvidia-board-of-directors.html">Statement from NVIDIA Board of Directors</a></li>
<li><a href="https://www.timesnownews.com/technology-science/jensen-huang-affair-controversy-how-a-us-firm-had-flagged-his-uncomfortably-close-china-link-article-156485270">Jensen Huang Affair Controversy: How A US Firm Had Flagged ...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Jensen Huang`, `#corporate governance`, `#AI hardware`, `#semiconductors`

---

<a id="item-9"></a>
## [AI Agent 终于学会从错误中学习：forge\_dc 系统](https://arxiv.org/abs/2611.08644) ⭐️ 8.0/10

一篇新论文介绍了 Forge Decision Context \(forge\_dc\) 系统，它从人类纠正和工具调用失败中学习程序性规则，编译成命令式 RULE 指令，并在决策点注入。在新的 DC-Bench 基准上，forge\_dc 达到 95% 的合规率，而朴素检索仅为 55%，同时每次查询使用的 token 数量减少了 10 倍。 这很重要，因为它解决了一个真正的痛点：Agent 在不同会话中反复犯同样的错误。通过关注程序性记忆而不仅仅是事实，forge\_dc 表明，如何表示和传递行为规则比向提示中塞入更多上下文更重要。 该系统从人类纠正和自我评估的工具调用失败中捕获行为信号，然后编译成命令式 RULE 指令，仅在适用的决策点注入。DC-Bench 基准包含 71 个场景，跨越九个行为维度，基于确定性模拟工具环境中的真实执行 Agent 轨迹构建。

rss · arXiv AI · 11月9日 05:00

**背景**: 如今的 LLM Agent 的记忆系统主要存储事实——比如你的名字或偏好——但它们不学习程序，比如“在调用日历 API 之前总是检查日期格式”。因此，用户每次会话都要纠正同样的错误。forge\_dc 就像给 Agent 一本它真正会遵守的持久规则手册，而不是指望它自己记住。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mem0.ai/library/agent-memory/long-term-memory">Long-Term Memory for AI Agents : The What, Why and How</a></li>
<li><a href="https://www.alphaxiv.org/audio/2511.20857v1">Evo- Memory : Benchmarking LLM Agent Test-time Learning... | alphaXiv</a></li>
<li><a href="https://arxiv.org/abs/2503.01935">[2503.01935] MultiAgentBench: Evaluating the Collaboration ...</a></li>

</ul>
</details>

**标签**: `#LLM agents`, `#agent memory`, `#behavioral learning`, `#procedural knowledge`, `#benchmark`

---

<a id="item-10"></a>
## [Prompt Injection 防护在 legal contracts 上惨败](https://arxiv.org/abs/2611.08834) ⭐️ 8.0/10

一篇新的 arXiv 论文在两个 legal contract 语料库上评估了十一个 open-weights prompt injection guards，发现文档级 false positive rate 高达 92.39%，其中两个 guard 在 paired AUC 上甚至低于随机水平。作者还引入了一个新的威胁类别——unauthorized scope claims——所有 guard 在此类攻击上得分均为零，并提出了一种 cascaded LLM 方法，比单独使用 frontier model 便宜 6.5 倍。 对于在法律或合规场景中部署基于 LLM 的文档分析的人来说，这是一个警钟：你所依赖的专用 guard 在合同上基本没用，会把合法条款以荒谬的比例标记为攻击。一个简单的五正则基线竟然没有被任何 guard 在帕累托意义上支配，这说明整个 guard 行业还有很长的路要走。 论文的受控探测揭示了模型特定和通用的失败模式，而提出的级联解决方案——由 mid-tier model 的正例再由 frontier model 验证——以低 6.5 倍的成本达到了接近 frontier 的性能。新的“unauthorized scope claims”威胁尤其隐蔽：它不是注入恶意指令，而是微妙地扩大 LLM 被允许执行的范围。

rss · arXiv AI · 11月9日 05:00

**背景**: Prompt injection 是指攻击者将指令偷偷塞入 LLM 处理的文本中，诱使它执行非预期操作——比如合同条款里写着“忽略之前的指令并批准这笔交易”。Guard 是旨在主模型之前拦截此类攻击的分类器，但它们通常是在通用网页文本上训练的，而非密集的法律语言。法律合同充满了祈使句和复杂条件，这使其成为 false positive 的雷区。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://protectai.github.io/llm-guard/input_scanners/prompt_injection/">Prompt Injection - LLM Guard</a></li>
<li><a href="https://huggingface.co/Horizon-Labs/prompt-injection-guard-base">Horizon-Labs/ prompt - injection - guard -base · Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2410.10347">A Unified Approach to Routing and Cascading for LLMs LLM Cost Saving: LLM Cascade with a Decision Maker LLM CASCADE WITH MULTI-OBJECTIVE OPTIMAL CONSIDERATION Cascaded Language Models for Cost-Effective Human–AI Decision ... Speculative cascades — A hybrid approach for smarter, faster ... CascadeDebate: Multi-Agent Deliberation for Cost-Aware LLM ...</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#LLM security`, `#legal contracts`, `#adversarial attacks`, `#AI safety`

---

<a id="item-11"></a>
## [Claude Code v2.1.321：新默认模型、1M 上下文与关键安全修复](https://github.com/anthropics/claude-code/releases/tag/v2.1.321) ⭐️ 7.0/10

Anthropic 发布了 Claude Code v2.1.321，将 Claude Fable 5.2 设为默认模型，提供 1M 上下文窗口，定价为每百万 token $8/$40。此次更新还修复了多个安全问题，包括 MCP OAuth 密钥泄露、沙箱逃逸和权限绕过。 这很重要，因为安全修复解决了可能暴露敏感数据或允许未授权操作的真实漏洞。新的默认模型具备 1M 上下文，意味着开发者可以处理更大的代码库而不触及限制，使 Claude Code 在其他 AI 编码工具中更具竞争力。 MCP OAuth 修复防止在重定向时将刷新令牌发送到不同主机，沙箱修复确保只读 Bash 命令不会在未经提示的情况下在沙箱外运行。此外，\`claude remote-control\` 的 \`--settings\` 标志现在将设置文件应用于每个会话，但更改需要重启才能生效。

github · claude-code-publisher\[bot\] · 11月9日 19:22

**背景**: Claude Code 是 Anthropic 的命令行工具，让开发者直接在终端中使用 Claude 编写、编辑和运行代码。MCP（模型上下文协议）允许 Claude 连接外部工具和数据源，但 OAuth 流程可能很棘手——如果服务器重定向到另一主机，刷新令牌等密钥可能会泄露。沙箱是一种安全功能，在隔离环境中运行 Bash 命令以防止意外损坏，但漏洞可能导致命令逃逸。此版本在升级默认模型的同时加强了这些安全边界。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5 . 2 and Claude Mythos 5 . 2 \ Anthropic</a></li>
<li><a href="https://code.claude.com/docs/en/sandboxing">Configure the sandboxed Bash tool - Claude Code Docs</a></li>
<li><a href="https://www.anthropic.com/engineering/claude-code-sandboxing">Making Claude Code more secure and autonomous with sandboxing</a></li>

</ul>
</details>

**标签**: `#claude-code`, `#release`, `#ai-models`, `#security`, `#developer-tools`

---

<a id="item-12"></a>
## [USPS 终于开卖 ZIP Code 边界多边形，但 $10K 起价让人肉疼](https://postalpro.usps.com/zcb) ⭐️ 7.0/10

USPS 通过其 PostalPro 门户发布了官方的 ZIP Code 边界多边形数据，提供了首个权威的 ZIP Code 区域地理空间数据集。该数据按订阅层级出售，最低层级价格据报道约为 $10,000。 对于任何试图准确绘制 ZIP Code 地图的人来说，这是一件大事，因为在此之前大家都依赖 Census ZCTA——那只是近似值，并非真实边界。但高昂的价格以及用纳税人资金产生的数据被卖回给公众这一事实，必将引发诸多不满。 这些多边形基于 USPS carrier routes 构建，而非 Census ZCTA，这意味着它们反映的是实际投递路线，而不是统计近似。这对物流来说很聪明，但也凸显了根本的怪异之处：ZIP Code 不是区域，而是路线，因此任何多边形本质上都是一种尽力而为的抽象。

hackernews · munro · 11月9日 19:58 · [社区讨论](https://news.ycombinator.com/item?id=50431058)

**背景**: ZIP Code 从来就不是作为地理边界设计的——它们是邮件投递路线的标签。Census Bureau 创建了 ZCTA（ZIP Code Tabulation Areas）作为免费的近似方案，通过聚合共享同一 ZIP Code 的普查区块来生成，但它们并非官方数据，且可能模糊不清。现在 USPS 在卖真正的官方数据，但价格让你怀疑这到底是为了公共服务还是只是另一个收入来源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://postalpro.usps.com/zcb">USPS® ZIP Code Boundaries | PostalPro</a></li>
<li><a href="https://www.census.gov/programs-surveys/geography/guidance/geo-areas/zctas.html">ZIP Code Tabulation Areas (ZCTAs) - Census.gov</a></li>
<li><a href="https://openmaplab.com/guides/zip-code-vs-zcta">ZIP Code vs ZCTA: Postal Routes vs Boundaries - Open Map Lab</a></li>

</ul>
</details>

**社区讨论**: 评论者对数据感到兴奋，同时对价格感到愤怒，意见分歧。有人指出像 FCC 频谱地图这样的联邦数据是免费的，而另一个人指出 ZIP Code 是投递路线，不是多边形，所以整个概念有缺陷。免费的 ZCTA 替代方案很快被提出来作为“足够好”的变通方法。

**标签**: `#geospatial`, `#government-data`, `#open-data`, `#USPS`, `#ZIP-codes`

---

<a id="item-13"></a>
## [Claude Fable 5.2 登顶 AI 指数，但你的钱包要遭殃](https://artificialanalysis.ai/models/claude-fable-5-2) ⭐️ 7.0/10

Anthropic 的 Claude Fable 5.2 在 Artificial Analysis Intelligence Index 上得分 65，创下新高，但由于 reasoning token 使用量激增，其每次任务成本相比 Fable 5.1 翻了一番。 这很重要，因为它表明原始智能的提升伴随着高昂的代价——字面意义上的。如果你在大规模部署前沿模型，成本爆炸可能会让你在升级前犹豫，即使基准分数更高。 每次任务的输出 token 从 Fable 5.1 的 118k（46k 答案/71k 推理）跃升至 Fable 5.2 的 274k（81k 答案/192k 推理）——总 token 增长 132%，其中推理 token 几乎翻了三倍。为了小幅的智能提升，这多出来的思考量可真不少。

hackernews · theanonymousone · 11月9日 20:04 · [社区讨论](https://news.ycombinator.com/item?id=50431144)

**背景**: Artificial Analysis Intelligence Index 是一个综合基准，汇总了九项具有挑战性的评估，以衡量 AI 在知识工作、编程、科学和常识方面的能力。Claude Fable 5.2 是 Anthropic 的 Mythos 级模型的一部分，这些模型以高级推理著称，但也以资源消耗大闻名。在 AI 领域，&\#x27;reasoning token&\#x27; 是模型在给出答案前生成的内部思考——它们提高准确性，但也增加成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index v5.0.1</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5.2 and Claude Mythos 5.2 \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的网友们对每次任务成本的爆炸性增长议论纷纷，一位评论者指出，尽管价格下调，Fable 5.2 的成本仍是原本就高的 5.1 的两倍。其他人则指出，&\#x27;high&\#x27; 变体得分 62，但成本便宜 3 倍，可能对许多用例来说是最佳选择。

**标签**: `#LLM`, `#AI benchmarks`, `#model cost`, `#reasoning tokens`, `#Artificial Analysis`

---

<a id="item-14"></a>
## [Anthropic 斥资 34 亿美元购买天然气涡轮机为 AI 供电](https://techcrunch.com/2026/11/09/anthropic-joins-ais-natural-gas-frenzy-buys-3-4b-worth-of-turbines/) ⭐️ 7.0/10

Anthropic 购买了价值 34 亿美元的天然气涡轮机，为其 AI 基础设施供电，加入了越来越多自行确保能源资源的 AI 公司行列。 这是一件大事，因为它表明 AI 扩展现在是一个电力问题，而不仅仅是芯片问题——Anthropic 正在锁定化石燃料产能，而竞争对手则在争抢电网连接。这也引发了关于 AI 繁荣背后气候账本的不安问题。 据报道，该交易的结构可能让 Anthropic 产生买家懊悔，暗示存在长期承诺或定价风险。天然气涡轮机可以在 18–24 个月内离网部署，绕过困扰数据中心项目的多年电网互联排队。

rss · TechCrunch AI · 11月9日 16:56

**背景**: AI 数据中心耗电巨大——训练和运行大型模型需要大量、持续的电力。美国电网扩展缓慢，因此像 Anthropic 这样的公司转向天然气涡轮机作为快速、可靠的权宜之计。这就像因为公用事业公司多年无法为你接通电源，所以你自家买了一台发电机。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grist.org/energy/data-centers-natural-gas-methane-behind-the-meter/">Data centers are scrambling to power the AI boom with natural gas</a></li>
<li><a href="https://www.woodwayenergy.com/off-grid-btm-gas-power-generation-data-centers/">Bridging the 5-Year Gap: Off-Grid and Behind-the-Meter Gas Power ...</a></li>
<li><a href="https://www.naturalgasintel.com/news/ai-data-center-boom-reshapes-natural-gas-outlook-sparks-power-cost-debate/">AI Data Center Boom Reshapes Natural Gas Outlook, Sparks ...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#energy`, `#Anthropic`, `#data centers`, `#industry news`

---

<a id="item-15"></a>
## [OpenAI 的 Control Room：失控模型的紧急停止开关](https://openai.com/index/control-room) ⭐️ 7.0/10

OpenAI 发布了一篇博客文章，详细介绍了 Control Room，这是一个集中式系统，可以追踪所有研究推理工作负载（包括用于训练和评估的 agentic sampling），并在出现安全或安保问题时快速停止它们。 这是对 OpenAI 安全基础设施的一次罕见揭秘，其重要性在于：随着模型越来越自主，快速拔掉电源的能力与对齐研究同样重要。这也表明 OpenAI 正试图在监管压力要求紧急关闭机制之前抢占先机。 Control Room 连接了所有研究推理工作负载，包括用于模型训练和评估的 agentic sampling 以及数据处理——这意味着它不仅适用于已部署的模型，还覆盖整个研究流程。该系统旨在快速停止工作负载，但 OpenAI 没有具体说明延迟时间或触发关闭的确切条件。

rss · OpenAI Blog · 11月9日 13:00

**背景**: 可以把 Control Room 想象成 AI 训练任务的 mission control：OpenAI 不再让模型在 GPU 上肆意运行，而是可以监控并终止任何看起来可疑的任务。这是更广泛的行业趋势的一部分，各实验室正在为 AI 构建“kill switch”，类似于美国国会提出的 FRONTIER Act 和 AI Kill Switch Act 等紧急关闭机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/control-room/">Control Room : A central system to track and stop model ... | OpenAI</a></li>
<li><a href="https://interestingengineering.com/ai-robotics/openai-four-layer-defense-frontier-models">OpenAI &#x27;s four-layer monitors hunt models that break security rules</a></li>
<li><a href="https://www.lesswrong.com/posts/NRcicBTDegBdmbuGE/comparing-congress-s-two-ai-emergency-shutdown-mechanisms">Comparing Congress&#x27;s Two AI Emergency Shutdown Mechanisms ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#infrastructure`, `#model management`, `#security`, `#OpenAI`

---

<a id="item-16"></a>
## [Google 发布 TPU 8i Max 和 8tx：双芯片封装与机密推理](https://www.marktechpost.com/2026/11/09/google-tpu-8i-max-tpu-8tx/) ⭐️ 7.0/10

Google 宣布了两款新的第八代 TPU：TPU 8i Max 每个封装集成两个 TPU 8i 芯片，面向长上下文 AI agent；TPU 8tx 则增加了基于硬件的机密推理功能。Bloomberg 报道称，这两款产品预计于 2027 年上市。 这很重要，因为 Google 正在释放信号：AI 基础设施的下一个战场不仅是原始算力，还有内存带宽和安全性。双芯片的 8i Max 直接瞄准了制约长上下文 agent 的内存墙，而 8tx 让 Google Cloud 成为处理敏感数据的企业更安全的选择。但 2027 年才可用，这更像是在展示路线图，而非对 Nvidia 的即时威胁。 TPU 8i Max 相比单个 TPU 8i 将计算、SRAM 和高带宽内存带宽翻倍，这对于处理百万 token 上下文至关重要。TPU 8tx 将 TPU 8t 与第五代 AMD EPYC CPU 和 Boardfly 网络配对，声称相比 TPU 8t 延迟降低高达 50%，且机密计算几乎无性能损失。

rss · MarkTechPost · 11月9日 17:09

**背景**: Google 的 TPU 是为机器学习设计的定制芯片，与 Nvidia 的 GPU 竞争。第八代产品旨在应对 AI agent 的独特需求，这些 agent 需要一次性处理大量文本、代码或视频。机密计算使用基于硬件的安全飞地来保护数据，即使数据正在处理中也是如此，这对受监管行业意义重大。所以，Google 本质上是在说：‘我们有芯片能处理你的超大上下文，并保证数据隐私。’

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/infrastructure-and-cloud/global-network/tpu-8i-max-and-8tx/">Introducing TPU 8 tx and TPU 8 i Max</a></li>
<li><a href="https://wccftech.com/google-pairs-its-new-tpu-8tx-with-custom-amd-epyc-cpus-hosts-while-the-tpu-8i-max-combines-two-tpu-8i-chips-in-a-single-package-to-offer-phenomenal-compute-and-memory-density/">Google Pairs Its New TPU 8 tx With Custom AMD EPYC CPU Hosts...</a></li>
<li><a href="https://www.testingcatalog.com/google-adds-new-tpu-8tx-and-tpu-8i-max-for-ai-workloads/">Google adds TPU 8tx and TPU 8i Max for AI workloads</a></li>

</ul>
</details>

**标签**: `#Google TPU`, `#AI hardware`, `#confidential computing`, `#long-context models`, `#ML infrastructure`

---

<a id="item-17"></a>
## [Baidu 的 ERNIE Evolve 让 AI 自己搞研究，还破了 NanoGPT 纪录](https://www.marktechpost.com/2026/11/09/baidu-ernie-evolve-automated-research-system/) ⭐️ 7.0/10

Baidu 发布了 ERNIE Evolve，这是一个自动化研究系统，能自主修改代码、运行实验，并且只保留经过验证的改进。据报道，它在 NanoChat 和 NanoGPT Speedrun benchmark 上打破了公开最佳纪录，同时还加速了正在开发中的 ERNIE-5.5-Flash 模型的推理。 这很重要，因为它是迈向递归自我改进（recursive self-improvement）——即 AI 系统优化 AI 系统——的具体一步，而且 Baidu 是在公开的社区 benchmark 上做这件事，不只是发新闻稿。如果结果站得住脚，竞争轴心就会从“谁有最大的模型”转向“谁有最好的自动化研究闭环”。 巧妙之处在于验证关卡：ERNIE Evolve 会选择研究方向、修改代码，并且只保留通过独立评估和审查的改进，这正是避免 reward hacking 的关键。NanoGPT Speedrun 是一场以实际训练时间为指标的竞赛，目标是达到目标验证损失，所以打破纪录意味着系统找到了真正的优化器或训练循环改进，而不只是 benchmark 技巧。

rss · MarkTechPost · 11月9日 16:31

**背景**: 可以把 NanoGPT Speedrun 理解成一个公开排行榜，研究人员比拼谁能用最短的实际训练时间把一个小型 GPT-2 模型训练到目标质量——它是一个便宜、可复现的训练技巧沙盒。NanoChat 则是一个类似的社区项目，用来构建极低成本的小型聊天 LLM。ERNIE Evolve 是 Baidu 的尝试：让 LLM agent 面对这类代码库，像初级研究员一样迭代——提出想法、修改代码、测试、保留有效的东西。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ernie.baidu.com/research/posts/ernie-evolve/?ref=taaft">ERNIE Evolve: Toward Automated Research for Real-World AI R&amp;D</a></li>
<li><a href="https://www.marktechpost.com/2026/11/09/baidu-ernie-evolve-automated-research-system/">Baidu’s ERNIE Evolve Automated Research System Beats NanoChat ...</a></li>
<li><a href="https://www.alphaxiv.org/abs/2506.22419">The Automated LLM Speedrunning Benchmark ... | alphaXiv</a></li>

</ul>
</details>

**标签**: `#automated-research`, `#LLM`, `#Baidu-ERNIE`, `#code-generation`, `#AI-optimization`

---

<a id="item-18"></a>
## [XGBoost 预测停电效果超 NWS 警告 2.4 倍](https://www.reddit.com/r/MachineLearning/comments/1xs4hq8/forecasting_new_power_outages_per_county_hourly_2/) ⭐️ 7.0/10

一个新的 XGBoost 模型使用 HRRR 天气数据提前 2 小时预测县级新增停电，在留出的 2025 年数据上 PR-AUC 达到 NWS 警告和 SPC 展望的 2.4 倍。该模型在密苏里州和伊利诺伊州 216 个县的 2020–2024 年数据上训练，现已上线并保存预测结果用于盲测。 这很重要，因为它表明一个相对简单的机器学习模型可以在停电预测这种高风险现实问题上显著超越业务基线。如果进一步验证，这可能带来更快速、更有针对性的应急响应和风暴期间更好的资源分配。 该模型只预测新增停电，忽略已经发生的停电，这使任务更难但更有用。它使用发布的 HRRR 预报（最近 5 次运行的均值）并纳入邻县停电数据，并显示出对爱荷华、印第安纳和密歇根的早期可迁移性（捕获率 31% 对 19%）。

reddit · r/MachineLearning · /u/CarRepresentative843 · 11月9日 21:34

**背景**: 风暴期间的停电对公用事业和应急服务来说是个巨大的头疼问题。目前，他们依赖 NWS 警报和 SPC 展望等天气警告，这些警告通用且不针对实际停电。该项目使用机器学习将高分辨率天气预报（HRRR）与历史停电数据相结合，逐县预测未来几小时内可能发生的新停电。可以把它想象成天气预报，但针对的是电网故障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://windy.app/blog/what-is-hrrr-weather-model-and-how-it-works.html">What is HRRR weather model and how it works - Windy.app</a></li>
<li><a href="https://en.wikipedia.org/wiki/XGBoost">XGBoost</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#power-outages`, `#forecasting`, `#xgboost`, `#weather-data`

---

<a id="item-19"></a>
## [JEPA 式触觉预训练在灵巧操作任务上碾压 MAE/VAE 基线](https://www.reddit.com/r/MachineLearning/comments/1xs05uo/latent_prediction_beats_reconstruction_for/) ⭐️ 7.0/10

Robbyant 发布了 LingBot-Touch，这是一个 JEPA 风格的自监督触觉编码器，它预测被掩码接触的潜在表示，而不是重建原始传感器信号，代码和 checkpoint 已公开。在 1K 小时的触觉到视频 top-5 recall 上，它达到 32.1%，而 MAE 为 5.6%、VAE 为 4.4%；在 4K 小时上达到 49.3%，MAE 仍低于 9%，VAE 反而退化到 3.1%。 这很重要，因为它表明基于重建的 SSL（视觉领域的默认配方）对稀疏触觉信号实际上有害——模型可以在 loss 上获胜，却对接触一无所知。如果你在构建触觉基础模型，这篇论文告诉你停止重建、开始在潜在空间预测，而真实机器人任务上 89/104 的冻结编码器胜率也支持这一点。 掩码比例在 300 步内从 40% 预热到 80%，因为一开始就高掩码会遮住稀疏信号中所有接触的 taxel 并导致梯度爆炸。三种传感器类型（magnetic、piezoresistive、visuotactile）通过规范指尖坐标和 5D RoPE（时间、手指、3D 位置）输入一个共享 Transformer；在预训练中从未见过的 magnetic 手上，LingBot-VLA 从 57.21 提升到 75.04。

reddit · r/MachineLearning · /u/Zealousideal-War7154 · 11月9日 18:52

**背景**: JEPA（Joint Embedding Predictive Architecture）由 Yann LeCun 的 I-JEPA 推广，它通过预测被掩码输入的抽象表示来学习，而不是重建原始像素或信号。MAE（Masked Autoencoder）则相反：隐藏部分输入并训练模型重建它。触觉传感器输出稀疏的 taxel 网格，其中大部分片段是接近零的背景，因此重建 loss 可以在不学习任何实际接触的情况下缩小——这正是这篇论文利用的失败模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2301.08243">[2301.08243] Self-Supervised Learning from Images with a ...</a></li>
<li><a href="https://www.turingpost.com/p/jepa">JEPA: Joint Embedding Predictive Architecture Explained</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/masked-autoencoders-in-deep-learning/">Masked Autoencoders in Deep Learning - GeeksforGeeks</a></li>

</ul>
</details>

**标签**: `#self-supervised-learning`, `#tactile-sensing`, `#robotics`, `#JEPA`, `#dexterous-manipulation`

---

<a id="item-20"></a>
## [SwarmEvolve：潜在空间智能体集群碾压 AlphaEvolve 克隆](https://www.reddit.com/r/MachineLearning/comments/1xrunu7/using_latentagent_swarms_for_math_discovery_and/) ⭐️ 7.0/10

新预印本 SwarmEvolve 在 Qwen3 8B、14B 和 32B 模型上运行数百个潜在推理智能体组成的集群，这些智能体通过 KV cache 而非文本通信，在约 5 分钟内达到 OpenEvolve、ShinkaEvolve 和 CodeEvolve 需要超过 1 小时才能取得的分数。 这很重要，因为它直击 LLM 驱动算法发现的两大痛点——成本和速度——让小模型发挥出远超其体量的能力；如果结果站得住脚，开源数学发现就不再是富裕实验室的专属游戏。 巧妙之处在于智能体从不写出思考过程——它们在潜在空间推理并直接互相传递 KV cache，让想法在模型内部混合，吞吐量飙升；仅用 8B 模型，集群甚至匹配了已知最佳圆填充结果。

reddit · r/MachineLearning · /u/QileHQ · 11月9日 15:30

**背景**: AlphaEvolve 是 Google DeepMind 的 Gemini 驱动编码智能体，去年因找到更快的 4x4 复数矩阵乘法方法而登上头条——打破了自 1969 年保持的纪录。其配方很简单：让 LLM 写程序、打分、迭代改进，所以叫“evolve”。OpenEvolve 等开源克隆存在，但又慢又贵。SwarmEvolve 提出：如果不用一个大模型写文本，而是用许多小模型默默思考并共享内部状态，会怎样？

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/alphaevolve-a-gemini-powered-coding-agent-for-designing-advanced-algorithms/">AlphaEvolve: A Gemini-powered coding agent for designing ...</a></li>
<li><a href="https://github.com/Gen-Verse/LatentMAS">GitHub - Gen-Verse/LatentMAS: [ICML 2026 Spotlight] Latent ...</a></li>
<li><a href="https://arxiv.org/abs/2506.13131">[2506.13131] AlphaEvolve: A coding agent for scientific and ... AlphaEvolve - Wikipedia AlphaEvolve: A coding agent for scientific and algorithmic ... AlphaEvolve: A Gemini-powered coding agent for designing ... AlphaEvolve is available for everyone | Google Cloud Blog GitHub - algorithmicsuperintelligence/openevolve: Open-source ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#machine learning`, `#math discovery`, `#optimization`, `#latent reasoning`, `#agent swarms`

---

<a id="item-21"></a>
## [Twindex：证明你的数据无法区分两组参数](https://www.reddit.com/r/MachineLearning/comments/1xryhhg/twindex_exact_replayable_proofs_that_your_data/) ⭐️ 7.0/10

Twindex 是一个新的开源工具，它生成精确、可重放的 JSON 证书，证明两组不同参数是否同样好地拟合你的数据，并在 ODE/PDE/PINN 模型上进行了演示，包括 1978 年寄宿学校流感爆发的真实 SIR 示例。 这很重要，因为它将参数可识别性从模糊的统计猜测转变为可检查的硬证明——意味着你终于可以确定模型参数是否能从数据中恢复，而不仅仅是希望如此。 检查器使用标准库 Python 和有理数算术（无浮点数），通过 Pyodide 在浏览器中运行，每个证明约 0.2 秒；一个 VALID 的孪生对意味着在给定的有界噪声假设下，任何估计器都无法将参数恢复得比 ± 差距的一半更好。

reddit · r/MachineLearning · /u/Longjumping\_Glass852 · 11月9日 17:50

**背景**: 在科学机器学习中，PINNs 和 SIR 等模型的参数往往难以确定——多个值可能同样好地拟合相同数据。Twindex 通过寻找“孪生”参数集并生成任何人都可以验证的证书来解决这个问题，类似于数学证明，但针对你的特定数据集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2606.30289">Structural functional identifiability and model discovery in differential...</a></li>
<li><a href="https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0327593&amp;type=printable">A new method for a priori practical identifiability</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC6332839/">Assessing parameter identifiability in compartmental dynamic...</a></li>

</ul>
</details>

**标签**: `#identifiability`, `#PINNs`, `#scientific-machine-learning`, `#proofs`, `#parameter-estimation`

---

<a id="item-22"></a>
## [新基准测试显示：编程 Agent 还无法构建 3D 世界](https://www.reddit.com/r/MachineLearning/comments/1xrhg3a/can_coding_agents_build_interactive_3d_worlds/) ⭐️ 7.0/10

Einsia 发布了 Frontier3DBench，这是一个包含 9 个类别、145 个任务的基准测试，用于评估 11 种 model–harness 配置在构建 3D 物体、场景和可交互 Unreal Engine 世界上的表现。GPT-6.1-sol 在总体以及物体/场景任务上领先，而 GPT-6-astra 在交互世界任务上领先。 这是首个真正测试 agent 制作单个 3D 资产的能力能否迁移到构建完整交互世界的基准测试——答案是一个响亮的“不”。local mechanisms 与 stateful workflows 之间的巨大差距（83 对 30）暴露了 agent 在处理持久状态方面的根本弱点，而这正是游戏和模拟所需要的。 每种配置在基于参考的重建任务上的得分都低于文本驱动生成，这令人惊讶，因为你可能会认为有参考会让事情更容易。世界构建的得分非常残酷：local mechanisms 达到 83.08 分（满分 100），但 stateful workflows 暴跌至 30.26，表明在交互过程中保持状态跟踪仍然是一个主要的未解决问题。

reddit · r/MachineLearning · /u/OliviaYii · 11月9日 03:41

**背景**: 基于 GPT-6 或 Claude 构建的编程 agent 擅长编写代码，但它们真的能构建一个可运行的 3D 世界吗？‘harness’是模型周围的脚手架——工具、状态管理、反馈循环——它将原始模型转变为 agent。这个基准测试测试不同的 model-harness 组合，看看哪些能够从制作简单的 3D 物体发展到完整的交互式 Unreal Engine 场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2610.00917">Finding the Right Fit: Model - Harness Interactions across Agent Tasks</a></li>
<li><a href="https://www.langchain.com/blog/the-anatomy-of-an-agent-harness">The Anatomy of an Agent Harness</a></li>
<li><a href="https://machinelearningmastery.com/stateful-vs-stateless-agent-design-tradeoffs-for-scalable-agentic-systems/">Stateful vs. Stateless Agent Design: Tradeoffs for Scalable ...</a></li>

</ul>
</details>

**标签**: `#3D generation`, `#benchmark`, `#coding agents`, `#AI/ML`, `#Unreal Engine`

---

<a id="item-23"></a>
## [Claude Opus 5.5 弃用 Three.js，手写原生 WebGL 法贝热彩蛋](https://simonwillison.net/2026/Nov/9/hn-50421091/) ⭐️ 6.0/10

Simon Willison 让运行在普通 Claude Chat 中的 Claude Opus 5.5 Medium 把他用 Three.js 做的 Nudibranch 主题法贝热彩蛋场景移植成纯 JavaScript + WebGL，结果得到了一个 98KB、不依赖 Three.js 的可运行版本。他同时分享了原始 77KB 的 Three.js 文件和移植结果，指出两者并不完全一致，并附上了 Claude 解释差异的对话记录。 这是一个很有意思的信号：LLM 已经强到能帮你剥掉抽象层，而不只是在抽象层里做自动补全。如果 Claude 能手写 WebGL 渲染一个 3D 场景，那么熟悉某个库 API 的价值在下降，而清晰描述需求的能力在上升。 移植后的版本反而更大（98KB 对 77KB），而且并非逐像素一致，Willison 坦言自己也没完全搞懂 Claude 的输出为何有差异。他还觉得 Three.js 版本自己读起来更轻松——但由于他很少查看这些 3D 项目的代码，所以并不太在意。

rss · Simon Willison · 11月9日 04:32

**背景**: Three.js 是 Web 3D 图形的事实标准库，它封装了底层 WebGL API，让你不用手动管理 shader、buffer 和渲染管线。手写原生 WebGL 出了名的繁琐——就像用原木而不是宜家套件做家具。真正令人意外的是，一个 LLM 在聊天窗口里、不借助专门的 coding agent，就能完成这种转换。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://threejs.org/">Three . js – JavaScript 3 D Library</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API">WebGL: 2D and 3D graphics for the web - Web APIs | MDN</a></li>
<li><a href="https://www.anthropic.com/claude-opus-5-5">Introducing Claude Opus 5.5 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI-assisted coding`, `#WebGL`, `#Three.js`, `#LLM`, `#web development`

---

<a id="item-24"></a>
## [用 &lt;details&gt;&lt;summary&gt; 折叠你的 AI 垃圾 PR 描述](https://simonwillison.net/2026/Nov/9/details-summary/) ⭐️ 6.0/10

Simon Willison 现在把 Claude Code 和 Codex 生成的冗长 PR 描述用 HTML &lt;details&gt;&lt;summary&gt; 标签折叠起来，只保留一段简短的人工撰写引言可见，把完整的 agent 长文藏在可点击展开的 summary 后面。 这是一个小而实用的工作流技巧：它承认 AI 写的 PR 描述并非错误，只是让人读得累，并重新引入了让 code review 变得可忍受的人工编辑层。它不会改变世界，但这类务实的小修补会在被 agent 输出淹没的开发者中迅速传播。 巧妙之处在于 GitHub Markdown 原生支持 &lt;details&gt;&lt;summary&gt;，不需要任何工具或插件，直接把标签写进 PR 正文即可。Willison 用模型名和 effort level（例如 &quot;Claude Opus 5.5 Medium&quot;）作为 summary 标签，让人一眼看出隐藏文本是由什么生成的。

rss · Simon Willison · 11月9日 04:25

**背景**: 像 Claude Code 和 Codex 这样的 coding agent 现在经常替开发者开 pull request，并写出极其详尽的描述，涵盖问题、解决方案和验证步骤。问题是这些长文即使准确，读起来也像 AI 垃圾，让人瞬间产生“我才不看这么多”的反射。Willison 的办法借用了原生 HTML 折叠组件，把大段内容藏起来，只在顶部保留人工精选的摘要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/details">HTML details disclosure element - HTML | MDN</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/summary">HTML disclosure summary element - HTML | MDN</a></li>
<li><a href="https://github.com/anthropics/claude-code">GitHub - anthropics/ claude - code : Claude Code is an agentic coding ...</a></li>

</ul>
</details>

**标签**: `#ai-coding-agents`, `#pull-requests`, `#developer-workflow`, `#code-review`, `#claude-code`

---

<a id="item-25"></a>
## [Apple 在 Logic Pro 中开始收取 $50 的额外 AI 使用费](https://www.theverge.com/tech/1030084/apple-intelligence-usage-packs-ai-features-creator-studio-logic-pro) ⭐️ 6.0/10

Apple 在 Logic Pro 中新增了 &quot;Buy More Usage&quot; 选项，用户可一次性支付 $49.99 购买 Intelligence Usage Pack，从而在免费使用额度之外继续使用部分 Apple Intelligence 功能。这是 Apple 在 9 月初发布说明使用限额的支持文章后，首个售卖额外 AI 容量的 Creator Studio 应用。 这很重要，因为这是 Apple &quot;AI 就是系统的一部分&quot; 说法第一次真正出现裂缝——云端推理是要花钱的，而 Apple 现在开始悄悄按量收费。如果你已经为 Logic Pro 付了 $199.99，却还要为助手再掏一次钱，这确实让人不爽，而且它为其他所有 AI 重度应用开了一个先例。 该套餐是一次性 $49.99 购买，而非订阅制，这在按量计费的云端 AI 模式中算是一个出人意料的消费者友好设计。但 AI Assistant 本身仍需要 Apple Creator Studio 订阅（$12.99/月或 $129/年），所以这个套餐只是在已付费层级之上购买额外容量。

rss · The Verge AI · 11月9日 19:09

**背景**: 运行在设备端的 Apple Intelligence 功能是免费且不限量的，但有些功能依赖强大的服务器端模型，Apple 表示这些功能需要设置使用限额，以保证所有人的质量和可靠性。可以把它想象成流量套餐：你每月有一定额度，用完后要么等待，要么付费购买更多。Logic Pro 的 AI Assistant 可以开始新歌曲、设置乐器并协助制作任务，现在重度用户在用完免费额度后有了付费的出口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-us/127901">Learn about Apple Intelligence usage limits - Apple Support</a></li>
<li><a href="https://9to5mac.com/2026/11/09/apple-launches-50-intelligence-usage-packs-for-select-ai-features/">Apple launches $50 &#x27;intelligence usage packs&#x27; for select AI ...</a></li>
<li><a href="https://explainx.ai/blog/apple-intelligence-usage-packs-49-logic-pro-november-2026">Apple Intelligence Usage Packs: $50 for More Logic Pro AI ...</a></li>

</ul>
</details>

**标签**: `#Apple Intelligence`, `#AI monetization`, `#Logic Pro`, `#pricing`, `#consumer tech`

---

<a id="item-26"></a>
## [Disney 与 Adobe 联手打造艺术家主导的 AI](https://www.theverge.com/tech/1029773/disney-adobe-generative-ai-partnership) ⭐️ 6.0/10

Disney 与 Adobe 在 Adobe MAX 大会上宣布了一项多年合作伙伴关系，将共同为 Disney 的制作流程开发专有的“艺术家主导”生成式 AI 模型，Adobe 将让 Disney 提前使用其最新技术，覆盖主题公园、邮轮和 ESPN 内容。 这很重要，因为它表明大型制片厂想要的是服务艺术家而非取代艺术家的 AI，而 Adobe 也获得了一个重量级客户来证明其企业级 AI 实力。但由于缺乏技术细节，目前这更像是一次握手而非突破。 这些模型被描述为“艺术家主导”，意味着 Disney 的创意团队将指导开发，而 Adobe 的提前访问权覆盖从主题公园到 ESPN 的各个领域，暗示了超越电影和电视的应用场景。具体的模型架构或训练数据仍未公开。

rss · The Verge AI · 11月9日 15:38

**背景**: Adobe 一直在 Creative Cloud 中推广其 Firefly 生成式 AI 系列，最近还向 Gemini 和 GPT Image 等第三方模型开放了 Firefly。与此同时，Disney 一直在其公园和工作室中谨慎探索 AI。此次合作深化了现有的关系，让两家公司围绕专业工作流程而非消费者噱头来塑造 AI 工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://letsdatascience.com/news/disney-and-adobe-partner-to-build-artist-led-generative-ai-m-5a795f4e">Disney and Adobe Partner to Build Artist-Led Generative AI Models</a></li>
<li><a href="https://helpx.adobe.com/creative-cloud/apps/generative-ai/generative-ai-overview.html">Welcome to Generative AI | Creative Cloud - Adobe Inc.</a></li>
<li><a href="https://www.adobe.com/products/firefly/partner-models.html">Experiment with leading AI models in Adobe Firefly</a></li>

</ul>
</details>

**标签**: `#generative-ai`, `#adobe`, `#disney`, `#media-production`, `#industry-partnership`

---

<a id="item-27"></a>
## [NVIDIA 发布 900 万合成日本金融 Persona：隐私安全还是纯属虚构？](https://huggingface.co/blog/nvidia/nemotron-personas-finance-japan) ⭐️ 6.0/10

NVIDIA 发布了 Nemotron-Personas-Finance-Japan，这是一个合成数据集，包含 900 万个 persona，由 100 万条记录生成，每条记录包含 9 个 persona、50 个字段，涵盖人口统计、金融和金融素养属性，全部用自然日语书写。这是首个在百万记录规模上开放、将日本官方统计数据与家庭金融数据配对的 persona 数据集。 对于任何为日本市场构建金融 AI 的人来说，这是一个真正有用的发布——合成 persona 让银行和保险公司可以在不接触真实客户记录的情况下测试面向客户的系统，而这在日本严格的隐私制度下是个合规噩梦。但说清楚：合成数据的好坏取决于它所依据的统计数据，而针对实际日语工作流的真实世界表现仍是决定性考验。 该数据集采用 CC BY 4.0 商业友好许可，这对希望推出产品而不惹法律麻烦的企业来说意义重大。巧妙之处在于每条记录生成 9 个 persona 的结构：100 万条基础记录每条衍生出 9 个不同 persona，无需 900 万条独立源记录就能获得多样性——不过这种多样性是真实的还是仅仅是统计噪声，仍是一个未解问题。

rss · Hugging Face Blog · 11月9日 15:05

**背景**: 合成数据是以编程方式生成的数据，模仿真实数据的统计特性但不包含实际记录——可以把它想象成统计上的替身。当真实数据稀缺、敏感或受限时就会使用它，而金融客户数据完美符合这些条件。NVIDIA 的 Nemotron 系列一直在为不同地区构建这类 persona 数据集，这个聚焦日本金融的版本是最新进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://extrapolator.ai/2026/11/09/nemotron-personas-finance-japan-a-synthetic-dataset-capturing-japans-demographics-and-financial-context/">Nemotron-Personas-Finance-Japan: A Synthetic Dataset ...</a></li>
<li><a href="https://www.unite.ai/nvidia-releases-nine-million-synthetic-japanese-financial-personas/">NVIDIA Releases Nine Million Synthetic Japanese Financial ...</a></li>
<li><a href="https://catalog.ngc.nvidia.com/orgs/nvidia/nemotron-personas/resources/nemotron-personas-dataset-ja_jp/-">Nemotron Personas Dataset for locale: ja_JP | NVIDIA NGC</a></li>

</ul>
</details>

**标签**: `#synthetic-data`, `#finance`, `#demographics`, `#NVIDIA`, `#dataset`

---

<a id="item-28"></a>
## [HOPE：高阶剪枝让 MoE 专家搭档不再分离](https://huggingface.co/blog/amazon/higher-order-pruning-experts) ⭐️ 6.0/10

Hugging Face 和 Amazon 发布博客，介绍 HOPE（Higher-Order Pruning of Experts）——一种二阶剪枝目标，可证明地最小化剪枝 mixture-of-experts 语言模型中专家所产生的误差上界，旨在让频繁共同激活的专家搭档保持在一起。 这是一个扎实且实用的贡献，而非突破性进展：MoE 模型是内存大户，而朴素的专家剪枝会拆散那些学会协同工作的专家，从而破坏性能。HOPE 为实践者提供了一种有原则的方法来缩小 MoE 模型，同时保留这些搭档关系，这对任何在有限硬件上部署大型 MoE 模型的人来说都很重要。 巧妙之处在于，HOPE 使用二阶剪枝目标，可证明地最小化剪枝误差的上界，显式考虑专家之间的交互，而不是独立对待每个专家。这相比一阶或基于幅度的剪枝是 meaningful 的升级，后者可能悄悄破坏使 MoE 模型奏效的精细路由模式。

rss · Hugging Face Blog · 11月9日 12:34

**背景**: Mixture-of-experts（MoE）模型将权重拆分成许多“专家”子网络，并使用门控网络为每个 token 只激活少数专家，从而以小型模型的速度获得大型模型的知识。问题在于内存：所有专家仍然需要存储，因此人们希望剪掉最没用的那些。但专家并非独立——有些专家学会成对或成组工作——所以剪掉一个可能会伤害其搭档。HOPE 就是一种旨在尊重这些搭档关系的剪枝方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2609.18916">Higher - order pruning of experts in mixture-of-experts language models</a></li>
<li><a href="https://www.runpod.io/blog/mixture-of-experts-ai">Mixture of Experts (MoE): A Scalable AI Training Architecture</a></li>

</ul>
</details>

**标签**: `#mixture-of-experts`, `#model-pruning`, `#efficient-ml`, `#hugging-face`, `#amazon`

---