---
layout: default
title: "Horizon Summary: 2026-10-16 (ZH)"
date: 2026-10-16
lang: zh
---

> 从 992 条内容中筛选出 20 条重要资讯。

---

1. [四个 Gemini 4 Argon agents 通关 Minecraft，途中死了 605 次](#item-1) ⭐️ 9.0/10
2. [Meta 发布 816B Muse Spark Open，两台 Mac Studio 就能跑](#item-2) ⭐️ 9.0/10
3. [OpenBSD 藏了 37 年的 kernel bug 终于被攻破了](#item-3) ⭐️ 8.0/10
4. [Anthropic 把钥匙交给 METR，还放弃了审稿权](#item-4) ⭐️ 8.0/10
5. [Nvidia RTX Spark N1X 登陆笔记本：一周亲测这颗 Superchip](#item-5) ⭐️ 8.0/10
6. [NVIDIA 与 Hugging Face 为 Indic 语言投下 2.8 万亿 token 的重磅炸弹](#item-6) ⭐️ 8.0/10
7. [Reflection 发布 Beam：一个你真正能拥有的 501B 开源模型](#item-7) ⭐️ 8.0/10
8. [世界不会等你：为什么慢吞吞的天才 Agent 会输给反应快的笨蛋](#item-8) ⭐️ 8.0/10
9. [IneqAgent 在 Lean4 中攻克 94% 的不等式证明](#item-9) ⭐️ 8.0/10
10. [Bengio 想用数学定义什么叫「组合结构」](#item-10) ⭐️ 8.0/10
11. [MAI-Gym：一个平台搞定所有 GUI Agent 训练](#item-11) ⭐️ 8.0/10
12. [NVIDIA 发布 120B 开源多模态 Agent 模型，单台 DGX Spark 即可运行](#item-12) ⭐️ 8.0/10
13. [Meta 悄悄声称有权免费抓取新闻网站内容用于 AI 训练](#item-13) ⭐️ 7.0/10
14. [OpenAI 向学术实验室免费开放 GPT-Rosalind](#item-14) ⭐️ 7.0/10
15. [IBM Granite Switch 4.1：一个 endpoint 搞定 chat、决策与语音](#item-15) ⭐️ 7.0/10
16. [Liquid AI 的 d1-ultra 押注 decision model 是下一个风口](#item-16) ⭐️ 7.0/10
17. [两款新图像生成器登场：FLUX 3 Klein 开源，Krea 3 押注速度](#item-17) ⭐️ 7.0/10
18. [怀旧博客被网友上课：那根本不是 software rendering](#item-18) ⭐️ 6.0/10
19. [Folders：用空文件夹写代码的 esolang](#item-19) ⭐️ 6.0/10
20. [Chirp Pong：两台手机、一个游戏、零网络](#item-20) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [四个 Gemini 4 Argon agents 通关 Minecraft，途中死了 605 次](https://arxiv.org/abs/2610.22319) ⭐️ 9.0/10

四个 Gemini 4 Argon agents 在 27 小时 14 分钟内自主击败了 Minecraft 的 Ender Dragon，从零编写了 2,783 个程序，仅通过游戏内聊天和共享内存进行协调。它们基于开源库 Mineflayer 运行，从随机种子出发、Easy 难度开局，没有任何人类分配的角色或游戏逻辑。 这确实是件大事，因为这是首次在没有任何人类编写游戏逻辑的情况下端到端自主通关 Minecraft——跨越数千个依赖步骤的长时程规划，正是真实软件工程和企业级 agent 任务所需要的核心能力。如果 agents 能在死 605 次的情况下依然保持 27 小时的连贯计划并恢复，那么“agents 做不了长任务”这个借口正一天天站不住脚。 这些 agents 自己编写并调试每一个程序，分工协作、共享学到的知识，甚至会在队友死亡后帮对方捡回掉落的物品——对多 agent 系统来说这是一种相当有“社交性”的行为。研究人员保留了带暂停和停止按钮的实时 dashboard，但全程无需干预，这才是真正厉害的地方。

rss · arXiv AI · 10月16日 04:00

**背景**: Minecraft 看起来像个儿童游戏，但通关它是对规划能力的残酷考验：你得采集资源、制作工具、搭建 Nether portal、找到 fortress，最后还要在另一个维度里打一只会飞的 boss。Gemini 4 Argon 是 Google 为复杂软件工程和自主多步 agents 打造的旗舰推理模型，而 Mineflayer 是一个 JavaScript 库，能让 bot 像真人一样操控 Minecraft 玩家。把两者结合，就得到了一个能把“AI 能不能连续规划一整天？”变成可测量问题的沙盒。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/google/gemini-4-argon">Gemini 4 Argon - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://github.com/PrismarineJS/mineflayer">GitHub - PrismarineJS/ mineflayer : Create Minecraft bots with...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#Minecraft`, `#multi-agent systems`, `#autonomous planning`, `#reinforcement learning`

---

<a id="item-2"></a>
## [Meta 发布 816B Muse Spark Open，两台 Mac Studio 就能跑](https://www.marktechpost.com/2026/10/15/meta-muse-spark-open-816b-open-weight-model/) ⭐️ 9.0/10

Meta 发布了 Muse Spark Open，这是一个 816B 参数的开源权重 Mixture-of-Experts 模型，激活参数 42B，支持 1M token 上下文窗口。Meta 声称这是迄今为止最强的美国开源权重模型，也是同类中首个能通过 Apple 的 MLX 框架在两台 Apple M5 Ultra Mac Studio 上本地运行的模型。 这确实是个大事件，因为它把开源权重模型推到了过去只有数据中心才能触及的领域，同时也给 Apple 的统一内存硬件送上了绝佳演示。但真正的赢家可能是 Apple 而不是 Meta——每个想本地跑这个模型的开发者，都突然变成了两万美元 Mac Studio 的潜在买家。 MoE 架构意味着每个 token 只激活 816B 参数中的 42B，这才让桌面级推理勉强可行。但有个坑：据称 Meta 自己的 benchmark 是用 4-bit 量化的 Muse Spark 去对比原生 BF16 的 Qwen，这种比法对 Meta 有利，任何懂量化的工程师看了都会挑眉。

rss · MarkTechPost · 10月16日 02:26

**背景**: Mixture-of-Experts 本质上是一群专家子网络的委员会：不是一个巨型大脑干所有活，而是由 router 把每个 token 分发给少数相关专家。这就是为什么能做到万亿参数规模，却不用为每个 token 付全额算力账单。Apple 的 MLX 是专为 Apple silicon 统一内存打造的开源框架，CPU 和 GPU 共享同一份数据、无需来回拷贝——这正是 816B 模型能塞进两台高端 Mac 的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MLX_%28machine_learning_framework%29">MLX (machine learning framework) - Wikipedia</a></li>
<li><a href="https://github.com/ml-explore/mlx">GitHub - ml-explore/mlx: MLX: An array framework for Apple ... MLX Getting Started with MLX: Apple&#x27;s AI Framework for Mac Local and Distributed Large LLM Inference with MLX and RDMA ... Exploring LLMs with MLX and the Neural Accelerators in the M5 ... MLX (machine learning framework) - Wikipedia</a></li>
<li><a href="https://www.aiiq.org/benchmarks/mcp-atlas/">MCP Atlas Benchmark — AI IQ</a></li>

</ul>
</details>

**社区讨论**: 评论区在真兴奋和尖锐质疑之间分裂。有用户指出 benchmark 的猫腻——Meta 用 4-bit 对比 Qwen 的 BF16——并说如果自己手上有 512GB 的 M5，Muse Spark 连前十都排不进。有人指出功耗“只是普通烤面包机的一小部分”，还有人冷幽默地说 Meta 烧几十亿，就为了让大家给 Apple 送两万美元。

**标签**: `#AI/ML`, `#open-weight models`, `#Mixture-of-Experts`, `#Meta`, `#large language models`

---

<a id="item-3"></a>
## [OpenBSD 藏了 37 年的 kernel bug 终于被攻破了](https://calif.io/research/big-fish) ⭐️ 8.0/10

安全公司 Calif 于 2026 年 10 月 16 日发布了一个 proof-of-concept exploit，将 OpenBSD 原始 BSD kernel 代码中一个 37 年历史的 integer overflow 与一个 kernel use-after-free 串联起来，在 OpenBSD 7.9 上实现本地 root 提权。这两个漏洞目前均已被修补。 这是件大事，因为 OpenBSD 一直以近乎偏执的代码审计作为安全卖点，而一个熬过 37 年审查的 bug 是对这种信念的一记重击。这并不意味着 OpenBSD 不安全，但它确实证明了单靠人工审查存在盲区，再多的眼睛也无法完全覆盖。 这个 exploit 串联了两个独立的漏洞——那个 37 年历史的 integer overflow，加上一个 kernel use-after-free——这再次提醒我们，单个 bug 往往不够用，真正把好奇心变成 root 的是漏洞链。更讽刺的是：NetBSD 早在 1999 年 8 月的一次常规代码重写中就意外修掉了同一个 bug，也就是说 OpenBSD 在兄弟项目已经翻篇之后，还多背了 27 年。

hackernews · rs\_rs\_rs\_rs\_rs · 10月16日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=50118977)

**背景**: OpenBSD 是一个以安全为最高优先级的类 Unix 操作系统，其开发者以逐行审计代码而闻名，从 OpenSSH 到别人的软件都挖出过 bug。Kernel bug 尤其危险，因为 kernel 是操作系统的核心，掌控一切，一旦被利用，攻击者就能完全接管机器。这个 bug 可以追溯到 1980 年代的原始 BSD 源代码，堪称早期 Unix 时代的活化石。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/10/researchers-demonstrate-openbsd-root.html">Researchers Demonstrate OpenBSD Root Exploit Chaining 37-Year ...</a></li>
<li><a href="https://cybersecuritynews.com/37-year-old-kernel-openbsd-flaw/">37-Year-Old Kernel Flaw Exploited to Gain Root Access on ...</a></li>
<li><a href="https://thedailytechfeed.com/37-year-old-kernel-bug-in-openbsd-finally-patched-after-root-exploit-poc/">37-Year-Old Kernel Bug in OpenBSD Finally Patched After Root ...</a></li>

</ul>
</details>

**社区讨论**: HN 上的讨论既佩服又带点哲学意味。有评论指出，一个 bug 能在审计最密集的代码库中存活 37 年实在惊人，并追问 fuzzing 或 static analysis 是否真能发现这类 bug，还是必须靠人类去思考 exploit primitive。另一位则点出了那个绝妙的讽刺：NetBSD 早在 1999 年就意外把它修好了。

**标签**: `#OpenBSD`, `#kernel`, `#security`, `#vulnerability`, `#exploit`

---

<a id="item-4"></a>
## [Anthropic 把钥匙交给 METR，还放弃了审稿权](https://techcrunch.com/2026/10/15/anthropic-is-letting-metr-researchers-look-under-the-hood-with-employee-level-access/) ⭐️ 8.0/10

Anthropic 已授予 METR 研究人员 employee-level access，让他们独立评估公司的风险、incidents 和内部实践，并永久放弃了阻止其发布研究结果的权利。这一安排作为三步计划的第一步公布，让独立评估人员以与 Anthropic 自家 risk-assessment 团队同等的权限常驻公司内部。 这确实是一件大事：一家 frontier lab 主动把和自家员工同等的权限交给外部审计方，还放弃对结果的 editorial control，这是我们见过的、最接近真正外部问责的举动。如果它能持续下去，就会成为衡量其他所有 lab 的模板，而“我们自己审计自己”将不再是可接受的答案。 最引人注目的细节是那份弃权声明：METR 可以在没有 Anthropic 批准的情况下发布对其风险和 incidents 的评估，而这恰恰是大多数公司绝不会让步的部分。METR 还是一家明确拒绝接受 frontier AI 公司员工捐款的非营利组织，这个细节虽小，却清楚表明它对自身独立性的谨慎守护。

rss · TechCrunch AI · 10月15日 19:14

**背景**: METR（Model Evaluation and Threat Research）是一家评估 frontier AI 模型风险与能力的非营利组织，前身是从 Alignment Research Center 分拆出来的评估部门 ARC Evals。可以把它想象成 AI 领域的独立碰撞测试实验室：不是让汽车厂商自己给安全性打分，而是让外部团队去戳一戳这辆车，并公布发现。通常情况下，lab 会严格控制外部人员能看到什么、能说什么；Anthropic 这次是在赌，放弃这种控制换来的可信度比付出的代价更值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://metr.org/">METR</a></li>
<li><a href="https://metr.org/about">About METR</a></li>
<li><a href="https://www.anthropic.com/news/an-update-on-independent-evaluators">Anthropic update on independent evaluators \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#AI governance`, `#Anthropic`, `#METR`, `#AI policy`

---

<a id="item-5"></a>
## [Nvidia RTX Spark N1X 登陆笔记本：一周亲测这颗 Superchip](https://www.theverge.com/tech/1012748/nvidia-rtx-spark-windows-arm-laptops-asus-hp-lenovo-impressions) ⭐️ 8.0/10

The Verge 花了一周时间测试来自 Asus、HP 和 Lenovo 的笔记本，它们都搭载了 Nvidia 全新的 RTX Spark N1X——一颗将 20 核 Grace CPU 与 Blackwell RTX GPU 及统一内存结合的 Arm-based SoC。评测覆盖了实际性能表现，以及它与 Apple、Intel、AMD、Qualcomm 的对比。 这确实是件大事：Nvidia 把它在数据中心的打法直接搬进了笔记本市场，如果 N1X 表现到位，它将威胁 Qualcomm 在 Windows-on-Arm 上的势头，同时给 Apple Silicon 带来第一个真正的对手。问题在于价格——这些机器很贵，而且焊死的统一内存意味着你得一次性付清并永远接受这个选择。 N1X 拥有 20 个核心（Turbo 最高 4.1GHz），搭配拥有 5,120 个 CUDA cores 的 Blackwell RTX GPU，统一内存配置从 24GB 一直到 128GB。这些内存是焊死的，完全没有升级空间——对于一个靠可升级 GPU 起家的公司来说，这是个非常 Apple 风格的设计决定。

rss · The Verge AI · 10月16日 15:00

**背景**: 多年来笔记本一直依赖 Intel 和 AMD 的 x86 芯片，但 Apple Silicon 和 Qualcomm X 系列这样的 Arm 设计证明了你能获得更好的每瓦性能。Nvidia 与 Microsoft 于 2026 年 5 月 31 日发布了 RTX Spark，本质上是把它数据中心 superchip 背后的 Grace CPU 和 Blackwell GPU 组合缩小，塞进 Windows 笔记本和紧凑台式机。目标是在不依赖云端的情况下实现本地 AI、创作和游戏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nvidia_RTX_Spark">Nvidia RTX Spark - Wikipedia</a></li>
<li><a href="https://www.pcgamer.com/hardware/gaming-laptops/now-we-know-the-prices-of-the-new-rtx-spark-laptops-and-theyre-as-expensive-as-im-sure-you-feared/">Now we know the prices of the new RTX Spark laptops ... | PC Gamer</a></li>
<li><a href="https://www.servethehome.com/microsoft-launches-surface-laptop-ultra-surface-rtx-spark-dev-box/">Microsoft Launches Surface Laptop Ultra, Surface... - ServeTheHome</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Arm`, `#Laptop Processors`, `#Hardware Review`, `#SoC`

---

<a id="item-6"></a>
## [NVIDIA 与 Hugging Face 为 Indic 语言投下 2.8 万亿 token 的重磅炸弹](https://huggingface.co/blog/nvidia/scaling-indic-pretraining) ⭐️ 8.0/10

NVIDIA 联合 IIT Madras 和 AI4Bharat 实验室发布了 Nemotron-pretraining-Indic-v1，这是一个约 2.8 万亿 token 的合成预训练语料库，覆盖 22 种印度语言，同时开源了一套 GPU 加速的数据生成 pipeline，于 2026 年 10 月 16 日在 Hugging Face 上公布。 这确实是一件大事，因为 Indic 语言在 LLM 预训练中长期以来一直被忽视，而 2.8 万亿 token 的语料库加上开源 pipeline，为研究者提供了构建模型的原材料，不再把十亿级的使用者当作可以忽略的零头。真正的胜利不只是数据集本身，而是 pipeline 是开源的，这意味着社区可以持续扩展它，而不必等待大实验室的下一次施舍。 这个语料库是合成的，而非爬取的，这绕开了困扰网络爬取多语言数据的大量版权和质量问题，而且它覆盖了印度全部 22 种表列语言，而不只是 Hindi 和少数几种凑数的语言。GPU 加速的 pipeline 才是真正巧妙的地方——它把数据生成变成了可以真正复现和迭代的东西，而不是一次性的魔术。

rss · Hugging Face Blog · 10月16日 01:44

**背景**: 训练大型语言模型需要海量文本，而英语基本上是一片汪洋。对大多数印度语言来说，这片汪洋更像是一个小水坑——所以模型要么忽略它们，要么表现很差。合成数据生成是一种变通方案：与其爬取网络，不如用模型和 pipeline 大规模制造高质量的训练文本。AI4Bharat 早先的 IndicLLMSuite 和 Sangraha 数据集（2510 亿 token）是朝这个方向迈出的步伐，但 2.8 万亿 token 在量级上大了一个数量级。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/nvidia/scaling-indic-pretraining">Scaling Indic Pretraining: 2.8 Trillion Tokens and an Open ...</a></li>
<li><a href="https://www.explainx.ai/blog/nvidia-indic-pretraining-2-8-trillion-tokens-open-pipeline-2026">Nemotron Indic Pretraining: 2.8T Tokens, 22 Languages ...</a></li>
<li><a href="https://www.unite.ai/nvidia-unveils-2-8t-token-indic-pretraining-corpus-and-open-pipeline/">NVIDIA Unveils 2.8T-Token Indic Pretraining Corpus and Open ...</a></li>

</ul>
</details>

**标签**: `#multilingual`, `#pretraining`, `#dataset`, `#Indic languages`, `#open source`

---

<a id="item-7"></a>
## [Reflection 发布 Beam：一个你真正能拥有的 501B 开源模型](https://huggingface.co/blog/reflection-beam) ⭐️ 8.0/10

Reflection AI 发布了 Beam，这是其首个 open-weight 模型，采用 sparse Mixture-of-Experts \(MoE\) 架构，总参数 501B，但仅激活 23B，专为 coding、reasoning 和 agentic workloads 打造。Hugging Face 正在托管这次发布，并将其定位为一个用户可以拥有、定制和扩展的模型。 这很重要，因为一家估值 250 亿美元的初创公司推出 501B open-weight 模型，说明开源前沿不再只是中国的故事——Reflection 明确对标 DeepSeek、Qwen 和 GLM。如果 Beam 真能以 4 倍更少的算力提供有竞争力的性能，它将给闭源实验室带来巨大压力，并让高端模型所有权成为资金充足团队的现实选项。 巧妙之处在于稀疏性：总参数 501B 但仅激活 23B，意味着你能获得大模型容量却不必支付完整的推理成本，这正是 Reflection 能宣称算力减少 4 倍的原因。但要注意，&\#x27;open-weight&\#x27; 仍不等于 &\#x27;open-source&\#x27;——你拿到的是权重，未必包括训练数据或完整配方。

rss · Hugging Face Blog · 10月16日 00:00

**背景**: 可以把 Mixture-of-Experts 模型想象成一家大公司：每个任务只让少数专家处理，而不是所有人都来开每一次会。这就是为什么 Beam 纸面上有 501B 参数，实际运行却很便宜。Reflection AI 是一家相对较新的初创公司，以 250 亿美元估值完成融资，Beam 是它的首个 open-weight 发布——直接瞄准 DeepSeek、Qwen 等中国开源模型领头羊。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://reflection.ai/blog/introducing-beam">Introducing Beam: Reflection’s 501B open-weight model</a></li>
<li><a href="https://huggingface.co/blog/reflection-beam">Welcome Beam: a 501B open model you can own, customize, and scale</a></li>
<li><a href="https://siliconangle.com/2026/10/05/reflection-ai-debuts-open-source-beam-model-with-501b-parameters/">Reflection AI debuts open-source Beam model with 501B parameters</a></li>

</ul>
</details>

**标签**: `#open-source`, `#large language models`, `#AI`, `#model customization`, `#Hugging Face`

---

<a id="item-8"></a>
## [世界不会等你：为什么慢吞吞的天才 Agent 会输给反应快的笨蛋](https://arxiv.org/abs/2610.20665) ⭐️ 8.0/10

一篇新的 arXiv 论文提出了 RealtimeBench，一个包含六种游戏类型、共 180 个任务的 benchmark，在 LLM 推理期间让游戏持续运行；同时提出 TORSI，一种 two-timescale 的 offline recursive self-improvement 方法。在配对测试中，GPT-6.1-sol 在游戏暂停时击败更快的 Jev，但当时钟不停走动时反而落后；TORSI 经过两轮训练把 Jev 的平均分从 13.51 提升到 24.19（0-100 进度分）。 这很重要，因为整个 agent 行业一直在优化能力，却悄悄忽略了延迟；这篇论文表明，在任何实时环境中，速度不是锦上添花，而是胜负本身。如果你的 agent 思考 30 秒而世界已经向前走了，它再聪明也没用——它已经输了。 最巧妙的地方是 two-timescale 的拆分：慢速 teacher 在两次尝试之间、在暂停的游戏里研究失败并测试修正，然后为快速 student 写下可复用的指令，student 在游戏进行中行动、完全不调用 teacher。更妙的是，这些指令还能在无需重新调参的情况下提升另外三个模型的表现，说明学到的经验是可迁移的，而不是针对某个模型定制的。

rss · arXiv AI · 10月16日 04:00

**背景**: 想象一下：一位国际象棋特级大师和一位水平不错的俱乐部棋手下超快棋。时间无限时，特级大师每局都赢。但把时钟调到每步一秒，特级大师的深度计算反而成了负担——那个只管快速落子的俱乐部棋手会赢。这正是 LLM agent 在现实世界中面临的问题：推理和 tool call 都要花时间，而在持续变化的环境里，一个来得太晚的正确动作就等于错误动作。RealtimeBench 是第一个认真衡量这一点的尝试，而 TORSI 则通过把慢速深思和快速执行分开来围绕这个问题做训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2610.20665">The World Won&#x27;t Wait: Evaluating and Teaching Agents Under a ...</a></li>
<li><a href="https://www.printingpressai.com/article/research/the-world-won-t-wait-evaluating-and-teaching-agents-under-a-live-clock">The World Won&#x27;t Wait: Evaluating and Teaching Agents Under a ...</a></li>
<li><a href="https://arxiv.org/abs/2308.03688">[2308.03688] AgentBench: Evaluating LLMs as Agents - arXiv.org [2502.18836] REALM-Bench: A Benchmark for Evaluating Multi ... Best LLMs for Agentic — October 2026 Leaderboard | BenchLM.ai GitHub - genglongling/REALM-Bench: REALM-Bench: A Real-World ... Daily Agent Benchmarks — New LLM agent benchmarks on arXiv ... GitHub - THUDM/AgentBench: A Comprehensive Benchmark to ...</a></li>

</ul>
</details>

**标签**: `#LLM agents`, `#real-time evaluation`, `#benchmark`, `#self-improvement`, `#reinforcement learning`

---

<a id="item-9"></a>
## [IneqAgent 在 Lean4 中攻克 94% 的不等式证明](https://arxiv.org/abs/2610.20681) ⭐️ 8.0/10

IneqAgent 是一个新的 agentic 框架，将 LLM 推理与符号计算结合，在 Lean4 中证明不等式，使用 DeepSeek-V4-Flash 解决了 186 个基准问题中的 175 个（94.09%）。它还在四维和五维中得到了 Dittert 猜想的 Lean 验证强化，并证明了 Holens-Djokovic \(4,4\) 不等式。 这是一件大事，因为它表明 LLM agent 可以完成真正可验证的数学工作，而不仅仅是模式匹配证明。如果这能规模化，可能会改变数学家使用形式验证的方式，并给那些认为「LLM 不会推理」的人施加压力。 巧妙之处在于 lemma-level Monte Carlo Tree Search，它协调引理构造、目标重写，以及在 sum-of-squares、Bernstein 和 successive difference-substitution 后端之间进行选择。这些后端生成精确证书，因此最终证明会在 Lean 中对照原始定理陈述进行检查，而不是仅仅被信任。

rss · arXiv AI · 10月16日 04:00

**背景**: Lean4 是一种证明助手和函数式编程语言，可以让你编写计算机能够检查的数学证明。不等式证明对 AI 来说出了名的困难，因为它既需要创造性推理，又需要精确的代数计算，而这两者并不总能很好地配合。IneqAgent 基本上是一个机器人数学家，用 LLM 来头脑风暴步骤，用符号求解器来做繁重的代数运算，并让 Lean 担任最终裁判。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://en.wikipedia.org/wiki/Monte_Carlo_tree_search">Monte Carlo tree search</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sum-of-squares_optimization">Sum-of-squares optimization</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#Lean4`, `#inequality proving`, `#symbolic computation`, `#LLM agents`

---

<a id="item-10"></a>
## [Bengio 想用数学定义什么叫「组合结构」](https://arxiv.org/abs/2610.20922) ⭐️ 8.0/10

一篇新的 arXiv 论文（2610.20922）作者名单里有 Yoshua Bengio，用 algorithmic information theory 形式化了组合结构，把它定义为「当各部分被放在一起考虑时浮现、而单独建模各部分时捕捉不到的共享结构」。作者随后反转这个框架，通过直接优化目标结构（而不规定具体内容）来生成具有组合性的字符串和图像。 这很重要，因为 compositionality 是所有人解释「为什么 LLM 泛化不行」时都会挂在嘴边的词，但从来没人给出严格的数学定义。如果这个框架站得住，它就给研究者一个可度量的目标，而不是模糊的感觉——还可能重新定义关于神经网络 depth 和训练课程设计的争论。 最巧妙的一步是用了 algorithmic information theory（压缩的数学），因为它能在不预先规定结构长什么样的前提下，从任意数据中识别出结构。作者还证明他们的定义捕捉的是真正的层级式部分-整体组织，而不只是泛泛的复杂性或规律性——正是这个区分让这篇论文不只是换个说法。

rss · arXiv Machine Learning · 10月16日 04:00

**背景**: Compositionality 指的是你可以通过复用和重组更简单的部件来构建复杂事物——原子组成分子，分子组成细胞，词组成句子。这就是为什么你能理解一句从没听过的话。但尽管它感觉如此直观，数学家一直没有一个干净的方法来区分「这份数据有组合结构」和「这份数据只是很复杂」。这篇论文试图用 Kolmogorov complexity 的工具来填补这个空白——该理论认为某事物的「信息量」就是生成它的最短程序的长度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Algorithmic_information_theory">Algorithmic information theory</a></li>
<li><a href="https://arxiv.org/html/2406.08787v1">A Survey on Compositional Learning of AI Models: Theoretical ...</a></li>
<li><a href="https://arxiv.org/pdf/2504.18568">Lecture Notes on Algorithmic Information Theory</a></li>

</ul>
</details>

**标签**: `#compositionality`, `#algorithmic information theory`, `#AI theory`, `#machine learning`, `#complexity`

---

<a id="item-11"></a>
## [MAI-Gym：一个平台搞定所有 GUI Agent 训练](https://arxiv.org/abs/2610.20939) ⭐️ 8.0/10

研究者发布了 MAI-Gym，一个开源的 all-in-one 平台，统一了 mobile、computer 和 web 环境下的 GUI agent 评估、数据收集与 online RL 训练，可扩展到 20,000 个并行环境实例。他们用它训练出统一的 9B agent MAI-Gym-9B，在 MobileWorld 上达到 78.4%、在 OSWorld-Verified 上达到 76.2%，并开源了框架、mocked apps、2,000 个已验证任务和模型 checkpoint。 这很重要，因为 GUI agent 的真正瓶颈从来不是模型，而是环境。交互式 GUI 训练成本高昂、任务稀缺，所以大多数实验室只能在静态轨迹上做 fine-tune 然后祈祷。MAI-Gym 把它变成了可扩展、可复现的 pipeline，而且一个 9B 模型能击败大多数 10B 以下的开源对手，说明护城河正从纯规模转向基础设施。 最巧妙的地方在于共享的 rollout pipeline，让 agent 在评估和训练时的行为保持一致，再加上自动合成可重置的 mocked apps 和连贯的跨应用世界，并配有执行验证的 verifier。最惊艳的是：在 mocked 火车票应用上做 RL 能迁移到现实世界，把真机上的任务成功率从 28.8% 提升到 48.1%——sim-to-real 的鸿沟真的在缩小。

rss · arXiv AI · 10月16日 04:00

**背景**: GUI agent 是能像人一样看屏幕、点击、滑动和输入的 AI 系统。用 reinforcement learning 训练它们很难，因为每次尝试都意味着真的去运行一个应用，既慢又乱——就像每次教人开车都得递上一辆真车。RLVR（RL with verifiable rewards）在数学和代码上已经很好用，因为 checker 能立刻判定对错；MAI-Gym 的赌注是，可重置的 mocked apps 能给 GUI agent 同样的即时反馈循环。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2504.20464">[2504.20464] A Survey on GUI Agents with Foundation Models ... GitHub - ZJU-REAL/ClawGUI: Build, Evaluate, and Deploy GUI ... Experience-driven Multi-turn Reinforcement Learning for GUI ... Enhancing the Power of GUI Agents by Reinforcement Learning UI-R1: Enhancing Efficient Action Prediction of GUI Agents by ...</a></li>
<li><a href="https://www.reinforcement-learning.com/kb/rlvr">RLVR: RL with Verifiable Rewards, Explained</a></li>
<li><a href="https://github.com/Steve2457/Awesome-RL-GUI-Agents">Awesome Reinforcement Learning for GUI Agents - GitHub</a></li>

</ul>
</details>

**标签**: `#GUI agents`, `#reinforcement learning`, `#evaluation platform`, `#mobile automation`, `#computer use`

---

<a id="item-12"></a>
## [NVIDIA 发布 120B 开源多模态 Agent 模型，单台 DGX Spark 即可运行](https://www.marktechpost.com/2026/10/15/nvidia-nemotron-3-5-super-vl-release/) ⭐️ 8.0/10

NVIDIA 发布了 Nemotron 3.5 Super VL，这是一个开源的 120B 参数多模态 MoE 模型，激活参数为 12B，支持 1M-token 上下文，并采用 NVFP4 权重，可在单台 DGX Spark 上运行，同时还推出了两个更小的 Bolt 边缘模型。 这对本地 AI 来说确实是个大事件：一个 120B 级别的多模态 Agent 能塞进桌面设备，意味着严肃的 Agent 工作负载不再需要云账单或数据中心。这也给闭源前沿实验室带来真实压力，因为开源权重的差距一下子缩小了很多。 巧妙之处在于 MoE 的拆分：每个 token 只激活 12B 参数，所以运行速度像小模型，但所有 expert 都必须常驻内存，因此你仍然要为完整的 120B 占用买单。NVFP4 权重正是让这个占用能塞进单台 DGX Spark 的关键，而 1M-token 上下文才是把它从聊天机器人变成真正 Agent 的原因。

rss · MarkTechPost · 10月15日 19:53

**背景**: MoE（Mixture-of-Experts）是一种技巧：模型把权重拆成许多专门的 expert，每个 token 只唤醒其中少数几个。这样你就能用小模型的速度获得大模型的知识，但有个代价：所有 expert 都必须加载进内存，所以显存占用取决于总参数量，而不是激活参数量。NVFP4 是 NVIDIA 的 4-bit 浮点格式，能在几乎不损失质量的前提下大幅压缩权重。DGX Spark 则是 NVIDIA 基于 Blackwell 打造的紧凑型桌面 AI 超级计算机，专为常驻本地 Agent 设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/products/workstations/dgx-spark/">Personal AI Supercomputer Powered by Blackwell | NVIDIA DGX Spark</a></li>
<li><a href="https://localmodel.run/guides/mixture-of-experts">Mixture of experts ( MoE ) explained for local LLMs · localmodel.run</a></li>
<li><a href="https://quantumzeitgeist.com/performance-microscaling-fp4-quantization-gptq-achieves-speedup-bridging-promise/">Microscaling FP 4 Quantization</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#multimodal`, `#open-source`, `#MoE`, `#large language models`

---

<a id="item-13"></a>
## [Meta 悄悄声称有权免费抓取新闻网站内容用于 AI 训练](https://www.theverge.com/tech/1012846/meta-business-terms-scrape-news-publishers) ⭐️ 7.0/10

根据 Nieman Lab 的报道，Meta 更新的商业条款将于 10 月 30 日生效，似乎授予该公司抓取和爬取与其平台相关企业网站（包括在线新闻出版商）内容的权限，用于「开发、改进、研究」和「训练」AI 模型。这一变化被埋在一次例行的服务条款更新中，而非作为独立的政策转变来宣布。 这是一件大事，因为这是经典操作：修改条款、不公开宣布，让出版商发现自己被默认加入了。如果这在法律上站得住脚，Meta 就免费获得了一个不断更新的新闻语料库，而出版商什么也得不到——没有授权费、没有流量、没有署名。等着看诉讼吧，也等着看其他 AI 巨头照搬这套剧本。 狡猾之处在于「associated」这个词——它足够模糊，几乎可以涵盖企业链接或运营的任何网站，而且条款把抓取权与「开发、改进、研究」和「训练」一口气打包在一起。文中没有提到出版商的退出机制，而这正是监管机构和法院往往会注意到的典型不对称。

rss · The Verge AI · 10月16日 14:02

**背景**: 可以这样理解：像 Meta 的 Llama 这样的 AI 模型需要海量文本进行学习，而其中很多文本是受版权保护的新闻作品。多年来，AI 公司一直主张，在公开可获取的网络内容上进行训练属于「合理使用」——这一法律抗辩至今仍在 Kadrey v. Meta 和 Bartz v. Anthropic 等案件中争论不休。Meta 的新条款本质上是在试图从企业自身那里以书面形式获得这种许可，而无需谈判或付费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ailawsuittracker.com/issues/training-data-copyright/">AI Training Data &amp; Copyright (2026): The Rulings</a></li>
<li><a href="https://astraea.law/insights/ai-training-data-copyright">AI Training Data Copyright: Fair Use and Licensing</a></li>

</ul>
</details>

**标签**: `#AI training data`, `#Meta`, `#news publishers`, `#web scraping`, `#terms of service`

---

<a id="item-14"></a>
## [OpenAI 向学术实验室免费开放 GPT-Rosalind](https://openai.com/index/introducing-the-rosalind-academic-plan) ⭐️ 7.0/10

OpenAI 推出了 Rosalind Academic Plan，为符合条件的学术实验室提供 GPT-Rosalind 的赞助访问权限，这是其面向生命科学领域的模型系列，并附带研究工具。实验室可以代表团队提交申请以获得访问权限。 这是 OpenAI 的一步妙棋，意在竞争对手如 Google DeepMind 的 AlphaFold 生态锁定用户心智之前，先让下一代生命科学家用上自己的平台。对学术界免费听起来很慷慨，但这也是经典的圈地策略——先让研究人员上瘾，之后他们自然会推动所在机构付费。 GPT-Rosalind 是一个限量访问的模型系列，专为生命科学工作打造，覆盖已发表证据、数据、工具和实验，而非通用聊天机器人。据报道，该计划包含旨在防止滥用的程序性检查，这表明 OpenAI 对谁能使用它持谨慎态度。

rss · OpenAI Blog · 10月15日 19:00

**背景**: 可以把 GPT-Rosalind 想象成 ChatGPT 的专用版本，它被训练来理解生物学论文、实验室数据和实验流程，而不只是写邮件和诗歌。这个名字致敬了 Rosalind Franklin，她的 X 射线晶体学工作对发现 DNA 结构至关重要。学术实验室往往负担不起企业级 AI 定价，因此赞助访问消除了一个实实在在的门槛——但这也引发了公共科学是否应依赖单一商业供应商的疑问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-rosalind/">Introducing GPT - Rosalind for life sciences research | OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-the-rosalind-academic-plan/">Bringing GPT- Rosalind to academic research labs | OpenAI</a></li>
<li><a href="https://qelvato.com/openai-launches-rosalind-academic-plan-to-expand-gpt-rosalind-access/">OpenAI launches Rosalind Academic Plan to expand GPT‑ Rosalind ...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT`, `#academic research`, `#life sciences`, `#AI for science`

---

<a id="item-15"></a>
## [IBM Granite Switch 4.1：一个 endpoint 搞定 chat、决策与语音](https://huggingface.co/blog/ibm-granite/granite-switch-4-1) ⭐️ 7.0/10

IBM 在 Hugging Face 上发布了 Granite Switch 4.1，这是一个统一的模型 endpoint，把 chat、决策和语音能力打包进一个 checkpoint。&\#x27;batteries included&\#x27; 版本 Granite-Switch-4.1-8B 和 -30B 预装了一组 adapter，另外还有一个 3B preview 版本。 对于厌倦了为了做一个 multi-modal 应用而同时管理五个模型和 API key 的开发者来说，这是一个真正有用的举措。IBM 押注的是整合能力——而不是单纯的 benchmark 排名——才是企业真正想要的，说实话，他们可能是对的。 最巧妙的地方在于 adapter 架构：Granite Switch 通过热插拔 Granite Core 和 Guardian Libraries 中的 LoRA adapter，让你可以组合出单个 checkpoint，之后再单独替换或升级某项能力。你也不必被 IBM 预定义的 adapter 组合绑死——完全可以自己构建。

rss · Hugging Face Blog · 10月15日 20:34

**背景**: 把大多数 AI 技术栈想象成一个塞满单一功能小家电的厨房：一台 blender 负责 chat，一台负责语音，一台负责决策逻辑。Granite Switch 就是 IBM 试图打造的一把瑞士军刀——通过换入不同的 LoRA adapter（一种无需重新训练整个模型就能微调基础模型行为的小型附加模块），让单个模型 checkpoint 承担多种任务。IBM 一直在 Hugging Face 上稳步扩展 Granite 家族，而 Switch 是它面向那些希望减少组件数量的企业开发者所下的一步棋。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/ibm-granite/granite-switch-4-1">Granite Switch 4 . 1 : Chat, Decisions, and Speech from One Endpoint</a></li>
<li><a href="https://github.com/generative-computing/granite-switch">GitHub - generative-computing/ granite - switch : Granite Switch : the...</a></li>
<li><a href="https://mellea.ai/blogs/every-layer-one-conversation/">Every layer of Granite 4 . 1 in one conversation | Mellea</a></li>

</ul>
</details>

**标签**: `#AI`, `#IBM Granite`, `#multi-modal`, `#model release`, `#Hugging Face`

---

<a id="item-16"></a>
## [Liquid AI 的 d1-ultra 押注 decision model 是下一个风口](https://www.marktechpost.com/2026/10/15/liquid-ai-d1-ultra-decision-model/) ⭐️ 7.0/10

Liquid AI 发布了 d1-ultra，这是一个 text 和 image 的 decision model，能在一次 forward pass 中返回 calibrated probabilities，在 Artificial Analysis Decision Index 上得分 65，价格为每百万 input tokens 0.042 美元。 这是一个真正有意思的转变：不是让 LLM 靠聊天绕到答案，而是让 d1-ultra 一次性给出每个选项的概率——这正是做 triage、routing 或 risk scoring 的生产系统真正需要的东西。如果 calibration 在真实场景中站得住脚，它可能会悄悄吃掉大量目前人们用 GPT 级别 token 去烧的“无聊但值钱”的活。 最巧妙的地方是 single-forward-pass 设计——没有 chain-of-thought，没有 sampling，只是对选项输出一个 calibrated distribution，这让 latency 和成本变得可预测。每百万 input tokens 0.042 美元的价格足够便宜，可以对每个进来的请求都跑一遍，不过 65 分算是体面，还谈不上碾压。

rss · MarkTechPost · 10月16日 06:26

**背景**: 现在大多数 AI 模型都很“话痨”：你问一个问题，它生成一段文字，然后你祈祷答案是对的。Decision model 不一样——它天生就是在选项之间做选择，并告诉你它有多确信，就像天气预报说“70% 概率下雨”，而不是只说“可能会下雨”。Calibration 是这里的关键词：一个 well-calibrated 的模型说 70%，那它在现实中就应该大约 70% 的时候是对的，这才让它可以被信任地放进自动化 pipeline。Liquid AI 是一家做高效模型的创业公司，d1-ultra 是它进军这个由 Artificial Analysis 刚刚开始 benchmark 的 decision model 新品类的一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/articles/artificial-analysis-decision-index">Artificial Analysis Decision Index v1.0</a></li>
<li><a href="https://arxiv.org/html/2501.19047v2">Understanding Model Calibration - A gentle introduction and ...</a></li>
<li><a href="https://ollama.com/library/d1">d 1 is a 3B decision model from Liquid AI , built on LFM2.5-VL-3B</a></li>

</ul>
</details>

**标签**: `#multimodal`, `#decision-model`, `#calibrated-probabilities`, `#AI`, `#Liquid-AI`

---

<a id="item-17"></a>
## [两款新图像生成器登场：FLUX 3 Klein 开源，Krea 3 押注速度](https://bfl.ai/blog/flux-3-image-klein) ⭐️ 7.0/10

BFL 发布了 FLUX 3 Image Klein，一个 5.6B 的开源权重模型，支持原生 4MP 生成、最多 10 个参考图，以及通过 bounding box 控制物体位置；同时 Krea 推出了 Krea 3 beta，主打快速编辑，支持最多 6 个参考图。INT8 版本仅需 8GB VRAM，在 RTX 4070 上生成 1MP 不到 9 秒，价格从每 1K $0.009 起，而 Krea 3 每 1K 收费 $0.03、每 2K 收费 $0.06。 这对开源图像生成社区来说是一记漂亮的双拳：FLUX 3 Klein 把原生 4MP 和多参考编辑带到了消费级硬件上，在 5.6B 参数下确实令人印象深刻。而 Krea 3 则是速度优先，牺牲了 text2image 质量来换取编辑一致性——这是个聪明的细分定位，但还不足以威胁 FLUX 的通用性。 FLUX 3 Klein 有两个版本：一个用于微调的 base 版本，和一个蒸馏的 16-step 版本，后者无需 CFG 且速度约快 6 倍，权重采用限制商业用途的 FLUX Kommunity License。Krea 3 承诺在原生 2K 下编辑时间低于 8 秒，并保持人脸和商品一致性，但据说其 text2image 输出伪影严重——这是个很能说明问题的取舍。

telegram · ai\_newz · 10月16日 10:40

**背景**: FLUX 是 Black Forest Labs 推出的一系列图像生成模型，以高质量的开源权重发布著称，能与 Midjourney、DALL·E 等闭源模型竞争。Krea 是个更小的玩家，专注于实时创意工具，Krea 3 是它试图在快速、基于参考的编辑领域（而非原始生成）开辟细分市场的尝试。FLUX Kommunity License 是一种非商业许可证，允许你运行和修改模型，但限制出售生成内容——这是开源权重世界里常见的折中方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bfl.ai/models/flux-3-image-klein">FLUX 3 Image Klein : Open weights image generation and editing</a></li>
<li><a href="https://www.krea.ai/blog/introducing-krea-3">Introducing Krea 3 - Krea</a></li>
<li><a href="https://github.com/black-forest-labs/flux-3-image-klein">GitHub - black-forest-labs/ flux - 3 - image - klein : FLUX 3 Image Klein ...</a></li>

</ul>
</details>

**标签**: `#image-generation`, `#open-source`, `#FLUX`, `#Krea`, `#AI-models`

---

<a id="item-18"></a>
## [怀旧博客被网友上课：那根本不是 software rendering](https://www.jamesfmackenzie.com/2026/10/13/i-love-software-rendering/) ⭐️ 6.0/10

一篇题为 &quot;I Love Software Rendering&quot; 的博客文章在 Hacker News 上获得 200 个赞和 144 条评论，但评论区很快指出作者实际上描述的是 pixelated textures 和关闭 anti-aliasing，而非真正的 software rendering。delta\_p\_delta\_x 和 BugsJustFindMe 等评论者认为文章应该改名为 &quot;I love pixelated textures&quot;。 这有趣地提醒我们，即使是备受喜爱的怀旧情怀也可能在技术上站不住脚，而评论区最终比原文更有教育意义。它的意义在于展示了我们对图形术语的使用有多随意，以及社区如何实时集体纠正一个误解。 关键区别在于，software rendering 意味着 CPU 完成所有像素工作，而作者喜欢的其实只是在纹理上关闭 spatial anti-aliasing 和 bilinear filtering。正如评论者 bob1029 指出的，software rendering 常常比早期 GPU 产生更好的效果，因为在 2001 年 GeForce 3 带来可编程 shader pipeline 之前，通用 CPU 可以充当完全可编程的 pixel shader。

hackernews · speckx · 10月16日 12:52 · [社区讨论](https://news.ycombinator.com/item?id=50117746)

**背景**: Software rendering 是指计算机完全依靠 CPU 而非显卡来生成 3D 图像，在专用 GPU 普及之前这是唯一的选择。Anti-aliasing 是一种平滑数字图像中锯齿边缘的技术，关闭它会带来许多复古爱好者喜爱的锐利像素化外观。所以作者怀念的是一种视觉风格，而不是真正的基于 CPU 的渲染过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Software_rendering">Software rendering</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anti-aliasing">Anti - aliasing - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论区既有温和的纠正，也有怀旧轶事。delta\_p\_delta\_x 给出了技术上的致命一击，而 Waterluvian 补充了一段搞笑的回忆：&quot;啊，software rendering 时代。我加了一块声卡就多了 10fps。&quot; proc0 还指出，现代系统总会有某种 GPU，所以 &quot;software rendering&quot; 这个词基本已经过时了。

**标签**: `#software-rendering`, `#graphics`, `#retro-gaming`, `#pixel-art`, `#anti-aliasing`

---

<a id="item-19"></a>
## [Folders：用空文件夹写代码的 esolang](https://danieltemkin.com/esolangs/folders) ⭐️ 6.0/10

Daniel Temkin 于 2015 年创建的 esoteric programming language「Folders」，能把整个程序编码进磁盘上由空文件夹组成的目录结构里。它本周在 Hacker News 上重新翻红，拿下 182 分和 31 条评论，大家纷纷研究它的各种怪癖。 老实说，这东西完全不会改变任何人交付软件的方式——而这恰恰就是它的意义。像 Folders 这样的 esolang 存在的目的，就是去挑战我们对「代码到底是什么」的假设；一棵文件夹树居然能承载程序逻辑，这是个真正有趣的思维实验，而不是什么生产力工具。 解释器号称按字母顺序求值文件夹，但评论区发现它实际上用的是 natural sort order——也就是 Windows Explorer 显示文件夹时用的那套排序，所以「folder10」排在「folder9」后面。另外，Windows 上空文件夹确实报告 0 字节，这既是真的也是假的，因为目录项其实存在 MFT 里。

hackernews · gurst · 10月16日 05:11 · [社区讨论](https://news.ycombinator.com/item?id=50114342)

**背景**: Esoteric programming language（esolang，即「深奥编程语言」）是故意设计得很怪的语言——要么是玩笑，要么是软件艺术，要么是为了探索语言设计的边界，而不是用来真正做项目的。著名例子包括 Malbolge，它被刻意设计得几乎无法编程。Folders 把这种思路推到极致：程序不是文本文件，而是你目录树的形状，所以「运行」它本质上就是遍历一遍文件系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Esoteric_programming_language">Esoteric programming language</a></li>
<li><a href="https://medium.com/@elniak/folders-an-esolang-like-no-other-f8e8261f4c95">“ Folders ”: An Programming Language Like No Other | Medium</a></li>
<li><a href="https://github.com/SinaKhalili/Folders.py">GitHub - SinaKhalili/ Folders .py: Implementation of the Folders ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的讨论里既有狂喜也有恐惧。有人开玩笑说，想象一下运维发现 Windows 服务器上塞了 2300 万个空文件夹，结果它们是在定义生产环境的软件；另一位则精准总结了气氛：「这玩意儿又疯又没意义……我爱死它了！这种点子 AI 永远想不出来。」

**标签**: `#esoteric programming`, `#programming languages`, `#Hacker News`, `#creative coding`, `#Windows`

---

<a id="item-20"></a>
## [Chirp Pong：两台手机、一个游戏、零网络](https://simonwillison.net/2026/Oct/15/chirp-pong/) ⭐️ 6.0/10

Simon Willison 做了个叫 Chirp Pong 的双人 Pong 类游戏：两台手机靠在一起，通过 Web Audio 的 microphone API 用音频 chirp 互相传递游戏状态。整个项目是他用一句 prompt 在 Claude Code 里让 Claude Opus 5.5 Extra 生成的，跑的是纯静态 HTML，不需要服务器也不需要网络。 这不是什么重大突破，但确实是个很聪明的 hack——它提醒我们「联网」不一定非得靠 Wi-Fi、Bluetooth 或服务器。对于做本地多人游戏或离线小玩具的人来说，音频 chirp 是一种被严重低估的传输方式；而 LLM 能一句话把整套东西写出来，也说明了现在 AI 辅助原型开发到了什么水平。 最妙的地方在于：两台手机不需要配对、不需要握手、不需要共享网络——只要靠得够近、有麦克风就行，游戏状态被编码成可听见的音调，由 Web Audio API 实时解码。但明显的坑是它很脆弱：背景噪音、距离、或者房间太吵都会断链，而且也没什么值得一提的纠错机制。

rss · Simon Willison · 10月15日 19:47

**背景**: 可以把它想象成两个人玩「Marco Polo」互相喊话，而不是发短信——数据是以声音的形式在空气中传播，而不是无线电。用音频传数据并不新鲜（Chirp 之类的工具已经做了好多年），但在两个浏览器页面之间做点对点、完全不要后端，这个玩法挺有意思。Claude Code 是 Anthropic 的 agentic 编程工具，住在你的终端里，能替你写代码、改文件、跑命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/solst-ice/chirp">GitHub - solst-ice/chirp: Send data with sound · GitHub</a></li>
<li><a href="https://www.bleepingcomputer.com/news/software/new-chirp-tool-uses-audio-tones-to-transfer-data-between-devices/">New Chirp tool uses audio tones to transfer data between devices</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**标签**: `#game-design`, `#web-audio`, `#generative-ai`, `#peer-to-peer`, `#experiment`

---