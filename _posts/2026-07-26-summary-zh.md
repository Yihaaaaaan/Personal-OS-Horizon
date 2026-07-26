---
layout: default
title: "Horizon Summary: 2026-07-26 (ZH)"
date: 2026-07-26
lang: zh
---

> 从 57 条内容中筛选出 17 条重要资讯。

---

1. [用 ARM64 汇编从头实现 YOLO26n 推理](#item-1) ⭐️ 9.0/10
2. [Ruff v0.16.0：默认规则增至 413 条——代码检查革命](#item-2) ⭐️ 8.0/10
3. [GrapheneOS 严防数据提取：自动重启与胁迫密码](#item-3) ⭐️ 8.0/10
4. [DeepSeek 因算力差距言论泄露暂停融资](#item-4) ⭐️ 8.0/10
5. [AI 对就业的影响：斯坦福剖析炒作与现实](#item-5) ⭐️ 8.0/10
6. [Cloudflare 为网站所有者提供反 AI 爬虫武器](#item-6) ⭐️ 8.0/10
7. [KAT-Coder-V2.5：瓶颈是基础设施，不是模型规模](#item-7) ⭐️ 8.0/10
8. [Photon-1 仅凭原始视频学会物理和游戏](#item-8) ⭐️ 8.0/10
9. [FAIRChem v2 UMA：一个模型统治所有原子模拟](#item-9) ⭐️ 8.0/10
10. [Open Dreamer：JAX/Flax 开源复现 Dreamer 4](#item-10) ⭐️ 8.0/10
11. [4B 模型在瑞典医学考试中媲美 o3](#item-11) ⭐️ 8.0/10
12. [LLM 在 IMO 2026 上接近满分，但 Harness Engineering 才是亮点](#item-12) ⭐️ 8.0/10
13. [NAVER、NVIDIA、Brookfield 将韩国 AI 工厂容量提升至 200 兆瓦](#item-13) ⭐️ 8.0/10
14. [Sakana AI 的 Fugu-Cyber 在安全领域超越 GPT-5.5 和 Claude](#item-14) ⭐️ 7.0/10
15. [TileLang：用于高性能 GPU 内核的 Python DSL](#item-15) ⭐️ 7.0/10
16. [中国 AI 模型进军美国：更便宜、更开放、更智能](#item-16) ⭐️ 7.0/10
17. [ML 会议对理论论文不公平吗？](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [用 ARM64 汇编从头实现 YOLO26n 推理](https://www.reddit.com/r/MachineLearning/comments/1v6w394/i_implemented_the_yolo26n_model_inference_from/) ⭐️ 9.0/10

一个本科项目在 Raspberry Pi 4 上完全用 ARM64 汇编和 C 语言实现了 YOLO26n 推理，不依赖任何框架。 这是对神经网络推理最底层的一次罕见深入探索，展示了抛弃抽象层后能达到的效果。它之所以重要，是因为边缘 AI 需要每一分性能，而手工调优的汇编能释放框架无法企及的增益。 该项目使用了 ARM NEON SIMD、Winograd 卷积、缓存感知分块和算子融合，但作者承认性能提升低于预期。模型参数被提取并重新布局为针对推理流水线优化的自定义二进制格式。

reddit · r/MachineLearning · /u/Forward\_Confusion902 · 7月26日 06:43

**背景**: YOLO26 是最新版本的 YOLO，针对边缘部署优化，具有端到端无 NMS 推理和 43%的 CPU 速度提升。Winograd 卷积减少了小卷积的算术复杂度，而 ARM NEON SIMD 实现了 ARM 处理器上的并行处理。该项目从头结合了这些技术，这是工业实验室之外很少尝试的壮举。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.roboflow.com/yolo26/">YOLO26: YOLO Model for Real-Time Vision AI [2026]</a></li>
<li><a href="https://arxiv.org/abs/2602.14582">[2602.14582] YOLO26: A Comprehensive Architecture Overview and Key Improvements</a></li>
<li><a href="https://arxiv.org/abs/2201.10369">[2201.10369] Winograd Convolution for Deep Neural Networks: Efficient Point Selection</a></li>

</ul>
</details>

**标签**: `#YOLO`, `#ARM64`, `#edge AI`, `#assembly optimization`, `#neural network inference`

---

<a id="item-2"></a>
## [Ruff v0.16.0：默认规则增至 413 条——代码检查革命](https://astral.sh/blog/ruff-v0.16.0) ⭐️ 8.0/10

Ruff v0.16.0 将默认 lint 规则从 59 条扩展到 413 条，增加了 7 倍，使其开箱即用成为全面的 Python 代码检查工具。 这对 Python 开发者来说是一次巨大的生活质量提升：无需安装几十个插件就能获得近乎完整的 lint 覆盖。这也为默认检查工具应提供的功能设定了新标准，给其他语言生态系统带来了追赶压力。 新的默认规则包括来自 Flake8 插件、pyupgrade 和 pydocstyle 的规则，但 Ruff 的运行时间仅为它们的一小部分。团队还添加了 --show-settings 标志，帮助用户在升级前预览哪些规则处于活动状态。

hackernews · vismit2000 · 7月26日 09:01 · [社区讨论](https://news.ycombinator.com/item?id=49056112)

**背景**: Ruff 是一个用 Rust 编写的极速 Python 代码检查工具，旨在替代 Flake8、isort 等众多工具。由于其速度和统一接口，它已被广泛采用。此版本大幅扩展了默认规则集，减少了配置需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://astral.sh/blog/ruff-v0.16.0">The next stable version of Ruff is out now.</a></li>
<li><a href="https://docs.astral.sh/ruff/linter/">The Ruff Linter | Ruff</a></li>
<li><a href="https://www.remio.ai/post/simon-willison-hit-ruff-v0-16-0-ci-failures-the-defaults-had-changed">Simon Willison Hit Ruff v 0 . 16 . 0 CI Failures. The Defaults Had Changed</a></li>

</ul>
</details>

**社区讨论**: 开发者们既兴奋又谨慎：有人报告了实际的代码质量提升，也有人担心 CI 会因此中断。一位评论者指出，在 AI 生成代码的时代，强大的 lint 工具更加重要，另一位则希望 Go 也能有类似的工具。

**标签**: `#ruff`, `#python`, `#linting`, `#developer-tools`, `#open-source`

---

<a id="item-3"></a>
## [GrapheneOS 严防数据提取：自动重启与胁迫密码](https://discuss.grapheneos.org/d/40700-grapheneos-protections-against-data-extraction-from-locked-devices) ⭐️ 8.0/10

GrapheneOS 详细介绍了其针对锁定设备数据提取的保护措施，包括自动重启至 BFU 模式和胁迫密码功能，使得法医取证几乎不可能。 这对记者、活动人士以及任何过境者来说意义重大——GrapheneOS 提供了针对物理设备攻击的最强实用防御，但缺乏完整的备份解决方案意味着用户仍面临安全与便利之间的艰难权衡。 自动重启功能可在可配置的时间（例如 18 小时）后将设备恢复到 BFU 状态，此时磁盘加密密钥不在内存中，而胁迫密码可以擦除设备或触发虚假配置文件。

hackernews · Cider9986 · 7月26日 05:57 · [社区讨论](https://news.ycombinator.com/item?id=49055169)

**背景**: 当手机锁定且启动后从未解锁（BFU）时，其数据完全加密，密钥存储在安全元件中。GrapheneOS 的自动重启强制手机回到 BFU 状态，使其能够抵御冷启动攻击和 Cellebrite 等取证工具。胁迫密码则增加了一层可否认性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grapheneos.org/features">Features overview | GrapheneOS</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/grapheneos-frequent-android-auto-reboots-block-firmware-exploits/">GrapheneOS : Frequent Android auto - reboots block firmware exploits</a></li>

</ul>
</details>

**社区讨论**: 用户称赞了自动重启和胁迫密码功能，但指出缺少备份/恢复解决方案是安全旅行中的关键缺口。一些人讨论了密码熵与图案锁的对比，有用户指出图案锁仅提供约 18.5 位熵。

**标签**: `#GrapheneOS`, `#mobile security`, `#data extraction`, `#privacy`, `#Android`

---

<a id="item-4"></a>
## [DeepSeek 因算力差距言论泄露暂停融资](https://github.com/demo-zexuan/liang-wenfeng-investor-meeting-2026-7-22/blob/master/%E6%A2%81%E6%96%87%E9%94%8B%E6%8A%95%E8%B5%84%E8%80%85%E4%BA%A4%E6%B5%81%E4%BC%9A-%E6%96%87%E5%AD%97%E7%A8%BF_1_18_translate_20260723201651.pdf) ⭐️ 8.0/10

DeepSeek 在创始人梁文锋关于中美算力差距的言论泄露并广泛传播后，暂停了第二轮融资。据报道，该决定已于周六告知潜在投资者。 这很重要，因为它暴露了中国高效低成本 AI 叙事与现实之间的张力——连他们自己也觉得需要大规模算力才能竞争。这也引发了一个问题：如果 AI 商品化是真的，美国数万亿美元的 AI 投资是否正面临收益递减。 泄露的文本据称包含梁文锋对中美算力差距的坦诚评估，这与通常的中国效率叙事相矛盾。该仓库被强制推送以删除文件，但通过替代链接仍可访问。

hackernews · oliculipolicula · 7月25日 23:32 · [社区讨论](https://news.ycombinator.com/item?id=49052912)

**背景**: DeepSeek 是一家中国 AI 实验室，以远低于美国前沿实验室的成本开发出具有竞争力的开源模型而闻名。“算力差距”指的是由于美国出口管制，在获取 NVIDIA GPU 等先进硬件方面的差距。这条新闻表明，即使是此前淡化大规模算力需求的 DeepSeek，现在也将其视为瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.politico.com/newsletters/digital-future-daily/2026/03/17/the-compute-gap-shaping-the-us-china-ai-rivalry-00833103">The compute gap shaping the US-China AI rivalry - POLITICO</a></li>

</ul>
</details>

**社区讨论**: 评论者正在解析这个令人困惑的标题，并指出是泄露本身而非算力差距导致了暂停。一些人认为这份文本与 OpenAI 和 Anthropic 的“狂妄自大者”相比显得坦诚得令人耳目一新，而另一些人则质疑，如果商品化使大规模算力变得不必要，DeepSeek 为何还要追求它。

**标签**: `#AI`, `#DeepSeek`, `#fundraising`, `#US-China competition`, `#compute gap`

---

<a id="item-5"></a>
## [AI 对就业的影响：斯坦福剖析炒作与现实](https://siepr.stanford.edu/publications/policy-brief/what-really-happening-jobs-separating-ai-hype-reality) ⭐️ 8.0/10

斯坦福 SIEPR 的一份政策简报审视了真实的就业市场变化与 AI 炒作之间的差距，发现生产力提升喜忧参半且采用不均，近期毕业生面临艰难市场部分归因于 AI。 这是一次关键的现实检验：虽然 AI 鼓吹者宣称革命，但数据显示迄今为止影响温和且不均衡。真正的颠覆可能还在后面，因为 coding agents 和通用 agent 直到最近才变得有效。 简报指出 AI 的生产力效应遵循帕累托分布，放大了本就高效者的优势，且企业官僚变革滞后。社区评论强调 coding agents 直到 2025 年底才开始良好运行。

hackernews · pod\_krad · 7月25日 22:51 · [社区讨论](https://news.ycombinator.com/item?id=49052570)

**背景**: 多年来，专家预测 AI 将摧毁或改变就业，但确凿证据一直稀缺。这份斯坦福简报汇总了早期数据，显示 AI 采用率在上升但集中在某些行业，生产力提升真实存在但分配不均。简报还警告，若无政策干预，不平等可能加剧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://siepr.stanford.edu/publications/policy-brief/what-really-happening-jobs-separating-ai-hype-reality">What is really happening to jobs? Separating AI hype from reality | Stanford Institute for Economic Policy Research (SIEPR)</a></li>
<li><a href="https://siepr.stanford.edu/news/ais-job-whats-worker-do">AI’s on the job: What’s a worker to do? | Stanford Institute for Economic Policy Research (SIEPR)</a></li>
<li><a href="https://news.stanford.edu/stories/2026/03/ai-workplace-job-disruption-advice-siepr-summit">How to prepare as AI reshapes the workforce | Stanford Report</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论很犀利：simonw 指出 coding agents 直到 2025 年底才有效，因此覆盖 2022-2025 年的研究错过了真正的影响。cjbgkagh 认为 AI 放大了现有的生产力不平等（80:20 变成 90:10），而 chewbacha 观察到 LLMs 帮助经验较少的工程师但阻碍专家。dzonga 指出 AI 实验室混淆了任务与工作，忽略了工作是被发现而非创造的。

**标签**: `#AI`, `#labor market`, `#productivity`, `#coding agents`, `#hype vs reality`

---

<a id="item-6"></a>
## [Cloudflare 为网站所有者提供反 AI 爬虫武器](https://blog.cloudflare.com/content-independence-day-ai-options/) ⭐️ 8.0/10

Cloudflare 宣布了新的 AI 流量控制功能，允许客户阻止 AI 爬虫和训练机器人，从 9 月 15 日起，使用“阻止训练”策略的域名将默认阻止 Googlebot。 这很重要，因为它为网站所有者提供了一个简单而强大的工具来选择退出 AI 训练数据收集，但也存在将互联网访问控制权集中到 Cloudflare 手中的风险。 新策略区分了“训练”、“代理”和“搜索”爬虫，像 Googlebot 这样的多用途爬虫如果结合搜索和训练将被阻止。

hackernews · alphabetatango · 7月25日 22:50 · [社区讨论](https://news.ycombinator.com/item?id=49052564)

**背景**: AI 公司经常未经许可抓取网站来训练他们的模型。Cloudflare 的举措让网站所有者有了拒绝的方式，但批评者担心将过多权力交给单一公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/ai-crawler-traffic-by-purpose-and-industry/">A deeper look at AI crawlers: breaking down traffic by purpose and industry | The Cloudflare Blog</a></li>
<li><a href="https://www.radware.com/blog/ai-and-user-experience/understanding-ai-crawlers/">Understanding AI Crawlers and How It Impacts Your Business</a></li>

</ul>
</details>

**社区讨论**: 社区意见分歧：一些人赞扬透明度，而像 jwr 这样的人担心将访问决策外包给 Cloudflare，tekacs 则对 Cloudflare 两面下注感到厌倦。

**标签**: `#Cloudflare`, `#AI`, `#web scraping`, `#bot management`, `#privacy`

---

<a id="item-7"></a>
## [KAT-Coder-V2.5：瓶颈是基础设施，不是模型规模](https://www.marktechpost.com/2026/07/26/kwaikat-team-releases-kat-coder-v2-5-an-agentic-coding-model-trained-on-100000-verifiable-repository-environments/) ⭐️ 8.0/10

快手 KwaiKAT 团队发布了 KAT-Coder-V2.5，这是一个基于超过 10 万个可验证仓库环境训练的智能编码模型，覆盖 12 种语言，并采用了名为 AutoBuilder 的新型基础设施。 这很重要，因为它将焦点从扩大模型规模转向扩大训练基础设施，而这往往是隐藏的瓶颈。AutoBuilder 将环境构建成功率从 16.5%提升到 57.2%，沙箱审计将 RL 反馈错误从约 16%降至 2%以下，使智能编码模型更加可靠。 AutoBuilder 自动化了可验证仓库环境的创建，此前这是一个人工瓶颈。沙箱审计系统捕获错误的 RL 奖励信号，防止模型从不良反馈中学习。

rss · MarkTechPost · 7月26日 10:46

**背景**: 智能编码模型是能够自主编写和调试真实软件仓库中代码的 AI 系统。训练它们需要大量经过验证的环境，模型可以在其中练习并获得正确的反馈。此前，构建这些环境缓慢且容易出错，限制了进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@marketing_novita.ai/kat-coder-on-novita-ai-flagship-agentic-coding-model-from-kwaipilot-98b184810424">KAT - Coder on Novita AI: Flagship Agentic Coding Model ... | Medium</a></li>
<li><a href="https://www.atlascloud.ai/models/kwaipilot/kat-coder-pro-v2">KAT Coder Pro V2 API: 73.4% SWE-Bench Agentic ... | Atlas Cloud</a></li>
<li><a href="https://openrouter.ai/kwaipilot/kat-coder-pro">KAT - Coder -Pro V1 - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#agentic coding`, `#AI training infrastructure`, `#reinforcement learning`, `#code generation`, `#Kuaishou`

---

<a id="item-8"></a>
## [Photon-1 仅凭原始视频学会物理和游戏](https://www.marktechpost.com/2026/07/26/induction-labs-photon-1-simulates-desktops-plays-checkers-and-models-billiard-physics-from-one-pretraining-run/) ⭐️ 8.0/10

Induction Labs 发布了 Photon-1，一个 106B-A5B 稀疏 MoE 想象模型，它在没有动作标签的原始视频上预训练，并能从单次预训练中模拟桌面、玩跳棋和建模台球物理。 这很重要，因为它消除了困扰视频学习的动作标签瓶颈，可能开启一种新范式：智能体通过观察而非被告知该做什么来学习。 Photon-1 采用稀疏 MoE 架构，总参数 106B 但每个 token 仅激活 5B，计算效率高，并且它纯粹从像素序列中学习模拟环境，没有任何奖励或动作监督。

rss · MarkTechPost · 7月26日 09:14

**背景**: 大多数基于视频的 AI 模型需要每帧配对的动作标签，这成本高昂且限制了可扩展性。像 Photon-1 这样的想象模型通过预测未来帧来学习潜在的世界模型，从而在没有显式监督的情况下内化物理和动态。这类似于人类通过观察学习——我们不需要为每个动作打标签就能理解因果关系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://viso.ai/deep-learning/foundation-models/">Foundation Models : Powering the AI Revolution</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>

</ul>
</details>

**社区讨论**: AI 社区对此兴奋不已，许多人称其为无监督视频理解的‘基础模型突破’。一些怀疑者质疑模拟环境是否真正稳健，还是仅仅过拟合了训练数据。

**标签**: `#AI`, `#machine learning`, `#foundation models`, `#video understanding`, `#MoE`

---

<a id="item-9"></a>
## [FAIRChem v2 UMA：一个模型统治所有原子模拟](https://www.marktechpost.com/2026/07/26/fairchem-v2-uma-for-multidomain-atomistic-simulation-across-molecules-catalysts-materials-vibrations-and-molecular-dynamics/) ⭐️ 8.0/10

Meta FAIR 发布了 FAIRChem v2 及 UMA 模型，这是一个通用的机器学习原子间势，能在单一框架中处理分子、催化剂、材料、振动和分子动力学。现在有一篇教程展示了如何通过 Hugging Face 的门控访问来设置它。 这很重要，因为 UMA 将以前分离的领域——分子化学、催化和无机材料——统一到一个模型中，使研究人员免于训练或微调多个专用势。这是朝着计算化学和材料科学真正通用力场迈出的一步。 UMA 是一个 14 亿参数模型（5000 万活跃参数），比其较小的兄弟 uma-s 更慢且更耗内存，但在所有基准测试中达到了最佳精度。模型权重在 Hugging Face 上受门控，需要认证才能访问。

rss · MarkTechPost · 7月26日 08:38

**背景**: 原子模拟依赖原子间势来计算能量和力。传统势要么太慢（DFT），要么太窄（经典力场）。像 UMA 这样的通用 MLIP 在覆盖多种化学体系的大规模数据集上预训练，旨在全面实现准确和快速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/facebookresearch/fairchem">GitHub - facebookresearch/fairchem: FAIR Chemistry&#x27;s library of machine learning methods for chemistry · GitHub</a></li>
<li><a href="https://fair-chem.github.io/index.html">fairchem</a></li>
<li><a href="https://www.nature.com/articles/s41524-025-01650-1">Universal machine learning interatomic potentials are ready for phonons | npj Computational Materials</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#atomistic simulation`, `#FAIRChem`, `#interatomic potential`, `#computational chemistry`

---

<a id="item-10"></a>
## [Open Dreamer：JAX/Flax 开源复现 Dreamer 4](https://www.marktechpost.com/2026/07/25/meet-open-dreamer-a-jax-flax-reproduction-of-the-dreamer-4-world-model-pipeline-with-the-full-training-recipe-published/) ⭐️ 8.0/10

Reactor 团队发布了 Open Dreamer，这是 DeepMind 的 Dreamer 4 世界模型管道的 JAX/Flax 开源复现，包含完整的训练配方和两个代码仓库，组件包括视频分词器、潜在动态模型、轨迹生成和 FVD 评分。 这很重要，因为 Dreamer 4 是前沿级世界模型，此前其完整训练配方是专有的。Open Dreamer 使其民主化，让任何研究人员无需 DeepMind 的基础设施即可训练或微调世界模型用于基于模型的强化学习。 该实现使用 JAX 和 Flax NNX（Google 的现代神经网络库，简化了模型创建和调试），并包含一个可玩的实时演示，展示世界模型的实时运行。

rss · MarkTechPost · 7月25日 18:59

**背景**: 世界模型是学习环境内部模拟的神经网络，使智能体无需与现实世界交互即可“在头脑中”规划和训练。DeepMind 的 Dreamer 4 是最先进的此类模型之一，但其训练细节并未完全公开。Open Dreamer 通过提供 JAX/Flax 中完整、可复现的管道填补了这一空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://next-state.github.io/open-dreamer/">How to train a frontier-level world model</a></li>
<li><a href="https://github.com/google/flax">GitHub - google/flax: Flax is a neural network library for JAX that is designed for flexibility. · GitHub</a></li>

</ul>
</details>

**标签**: `#world models`, `#JAX`, `#Flax`, `#reinforcement learning`, `#open source`

---

<a id="item-11"></a>
## [4B 模型在瑞典医学考试中媲美 o3](https://www.reddit.com/r/MachineLearning/comments/1v71wds/openweight_4b_models_approach_o3level_medical/) ⭐️ 8.0/10

像 Gemma4-E4B 和 Qwen3.5-4B 这样的开放权重 4B 模型，在瑞典医学执照考试问题上达到了 87%的准确率，接近 o3 的 88%表现，使用了推理和早期退出策略来避免无限循环。 这很重要，因为它表明小型开放权重模型可以在专业任务上与顶级闭源模型竞争，无需大量计算或专有 API 即可普及高质量医疗 AI。 尽管提示是瑞典语，模型仍用英语推理；S-GRPO 论文中的“早期退出”干预通过注入短语在设定长度关闭思考轨迹，防止推理循环。

reddit · r/MachineLearning · /u/AccomplishedCat4770 · 7月26日 11:58

**背景**: MedQA-SWE 是一个瑞典语临床问答数据集，包含 3180 道医学执照考试选择题。小型 LLM（4B 参数）通常不如大型模型，但后训练和推理技术正在缩小差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/datasets/nicher92/medqa-swe">nicher92/medqa-swe · Datasets at Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2505.07686">[2505.07686] S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models</a></li>
<li><a href="https://aclanthology.org/2024.lrec-main.975/">MedQA-SWE - a Clinical Question &amp; Answer Dataset for Swedish - ACL Anthology</a></li>

</ul>
</details>

**社区讨论**: Reddit 帖子称赞了关于推理循环和早期退出的实用见解，一些用户注意到英语推理在瑞典语任务上的惊人效果。

**标签**: `#LLM`, `#medical QA`, `#open-weight models`, `#reasoning`, `#SFT`

---

<a id="item-12"></a>
## [LLM 在 IMO 2026 上接近满分，但 Harness Engineering 才是亮点](https://www.reddit.com/r/MachineLearning/comments/1v6wskz/we_compared_different_llms_on_imo_2026_r/) ⭐️ 8.0/10

一项针对 2026 年国际数学奥林匹克竞赛题目的新基准测试显示，sol 和 fable 等前沿模型几乎获得满分，而 Sonnet 和 Opus 等较弱模型通过 harness engineering（尤其是自定义多智能体 harness AutoFyn）性能大幅提升。 这很重要，因为它证明了即使是新颖的数学难题，前沿 LLM 也几乎完美；但更重要的是，它表明围绕模型的巧妙工程可以弥合平庸与卓越之间的差距。结论：如果你不使用 harness，你就在浪费性能。 最难的题目 P3 难倒了所有非前沿模型，无论是否使用 harness——即使运行 20 小时也在同一个缺失的关键归约步骤上卡住。评分由前沿模型和曾获 IMO 奖牌的人工验证共同完成，增加了可信度。

reddit · r/MachineLearning · /u/pequalnp92 · 7月26日 07:21

**背景**: 国际数学奥林匹克竞赛（IMO）是全球最负盛名的高中数学竞赛，其题目新颖且需要深度推理。用 IMO 题目作为 LLM 的基准测试，可以检验它们处理多步骤、创造性问题的能力，而这些题目不在训练数据中。Harness Engineering 指的是编排 LLM 与工具、记忆和验证循环交互的系统——可以把它看作是将原始模型转变为有能力的智能体的脚手架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>
<li><a href="https://benchlm.ai/benchmarks/imo2026">IMO 2026 Leaderboard &amp; Scores — July 2026 | BenchLM.ai</a></li>

</ul>
</details>

**标签**: `#LLM`, `#benchmark`, `#mathematical reasoning`, `#AI evaluation`

---

<a id="item-13"></a>
## [NAVER、NVIDIA、Brookfield 将韩国 AI 工厂容量提升至 200 兆瓦](https://news.google.com/rss/articles/CBMizgFBVV95cUxNZGx4bHdVUjhSOHRfNUhadlpSOFBRVThvZ3NpSENoZm9oYjlVN3lUUm5pMDBUSkpkN29Zc1ROQVdRb3FmNlVocjRwblNJWmx3ckxFS09zQmUxdEpaSWN4R1ZDUjkwZVUtbU5oamY2cnFuX202ZUhwUWJwMHN5UE8xeHBXVWxHeHVST0ZGSkp1UF9EOVExaGxmMXk3TGJJTHpnNW1zQ3ZXazl4M3pteWs1enVkdU94Q3FLMHNSS3JmZ3ZUZEhDY1ljZFJpNzJ3dw?oc=5) ⭐️ 8.0/10

NAVER、NVIDIA 和 Brookfield 于 7 月 25 日宣布了一项 100 亿美元的交易，计划到 2028 年将韩国的国家 AI 工厂容量从 55 兆瓦提升至 200 兆瓦。 这是对国家 AI 基础设施的巨大赌注，表明各国正在竞相建设自己的计算能力，而不是依赖外国云服务商。100 亿美元的价格标签表明 AI 不再只是软件游戏——这是一场硬件和能源战争。 Brookfield 出资 90 亿美元，NVIDIA 提供 10 亿美元的硬件和技术。扩建将在 NAVER 的 GAK Sejong 数据中心进行，配备先进的 NVIDIA AI 基础设施，包括最新的 GPU 和网络设备。

google\_news · Tech Times · 7月26日 10:55

**背景**: AI 工厂本质上是为训练和运行 AI 模型而优化的大型数据中心，以兆瓦功耗衡量。韩国领先的互联网公司 NAVER 一直在建设自己的 AI 能力，这笔交易使其成为区域 AI 基础设施中心。与 NVIDIA 的合作确保了尖端芯片的获取，而 Brookfield 则提供了资金。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/321630/20260726/naver-nvidia-triple-koreas-ai-factory-200-megawatts-10-billion-deal-brookfield.htm">NAVER and NVIDIA Triple Korea&#x27;s AI Factory to 200 Megawatts in $10...</a></li>
<li><a href="https://www.globenewswire.com/news-release/2026/07/25/3333160/0/en/NAVER-NVIDIA-and-Brookfield-to-Expand-Korea-s-National-AI-Factory-Infrastructure-Buildout.html">NAVER, NVIDIA and Brookfield to Expand Korea’s National AI Factory Infrastructure Buildout</a></li>
<li><a href="https://www.koreajoongangdaily.com/business/naver-secures-combined-10-billion-investment-from-nvidia-brookfield/12791136">Naver secures $10 billion from Nvidia and Brookfield to expand global...</a></li>

</ul>
</details>

**标签**: `#AI`, `#NVIDIA`, `#infrastructure`, `#investment`, `#Korea`

---

<a id="item-14"></a>
## [Sakana AI 的 Fugu-Cyber 在安全领域超越 GPT-5.5 和 Claude](https://www.marktechpost.com/2026/07/25/sakana-ai-releases-fugu-cyber-orchestration-model-cybergym-cti-realm/) ⭐️ 7.0/10

Sakana AI 发布了 Fugu-Cyber，这是其 Fugu 编排模型的安全调优版本，在 CyberGym 上达到 86.9%，在 CTI-REALM 上达到 72.1%，超越了 GPT-5.5-Cyber 和 Claude Mythos Preview。 这很重要，因为它表明专门的、较小的编排模型可以在狭窄的安全任务上击败单一的前沿模型，挑战了“越大越好”的教条。然而，受限的访问和防御性使用政策意味着我们还不能完全验证这些说法。 Fugu-Cyber 不是单个模型，而是一个作为单个 API 调用的多智能体编排系统，它在两个严格的网络安全基准测试中超越了 GPT-5.5-Cyber 和 Claude Mythos Preview：CyberGym（真实世界漏洞分析）和 CTI-REALM（威胁情报到检测规则）。

rss · MarkTechPost · 7月26日 00:12

**背景**: Sakana AI 的 Fugu 是一个多智能体编排系统，它协调多个专门的 AI 智能体来解决复杂任务，并以单个模型 API 的形式出售。CyberGym 测试智能体在 1,507 个 CVE 中发现、利用和修补真实世界漏洞的能力，而微软的 CTI-REALM 则评估从威胁报告到检测规则的端到端生成能力。这种方法与传统的单一模型（如 GPT-5.5 和 Claude）形成对比，后者试图在一个巨大的神经网络中完成所有任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.digitalapplied.com/blog/sakana-fugu-multi-agent-orchestration-model-2026">Sakana Fugu : A Multi-Agent AI Orchestration Model 2026</a></li>
<li><a href="https://github.com/sunblaze-ucb/cybergym">GitHub - sunblaze-ucb/cybergym: CyberGym is a large-scale, high-quality cybersecurity evaluation framework designed to rigorously assess the capabilities of AI agents on real-world vulnerability analysis tasks. · GitHub</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/03/20/cti-realm-a-new-benchmark-for-end-to-end-detection-rule-generation-with-ai-agents/">CTI-REALM: A new benchmark for end-to-end detection rule generation with AI agents | Microsoft Security Blog</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#orchestration model`, `#benchmarks`

---

<a id="item-15"></a>
## [TileLang：用于高性能 GPU 内核的 Python DSL](https://www.marktechpost.com/2026/07/25/designing-high-performance-gpu-kernels-with-tilelang-tensor-core-gemm-fused-softmax-flashattention-and-autotuning/) ⭐️ 7.0/10

一篇新教程展示了如何使用 TileLang（一种 Python 领域特定语言）设计高性能 GPU 内核，涵盖张量核心 GEMM、融合 softmax 和 FlashAttention，并内置自动调优支持。 这很重要，因为编写高效的 GPU 内核非常困难，而 TileLang 抽象了底层的 CUDA 细节，让开发者专注于算法设计，编译器处理线程映射和内存布局。它可能使 AI 工作负载的高性能 GPU 编程更加普及。 TileLang 使用分块抽象来表达计算，编译器自动将块映射到 Tensor Core 并管理共享内存。教程涵盖了自动调优，以搜索最佳块大小和内存配置，这对达到峰值性能至关重要。

rss · MarkTechPost · 7月25日 18:08

**背景**: GPU 内核编程传统上需要深厚的 CUDA 和硬件架构专业知识。TileLang 是一种高级 DSL，通过让用户编写类似 Python 的代码来简化这一过程，然后将其编译为高效的 CUDA 内核。它针对关键的 AI 操作，如 GEMM（矩阵乘法）和 FlashAttention（一种高效的注意力机制）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/tile-ai/tilelang">tile -ai/ tilelang | DeepWiki</a></li>
<li><a href="https://www.emergentmind.com/topics/tilelang">TileLang : Domain-Specific Tiling Language</a></li>
<li><a href="https://en.wikipedia.org/wiki/FlashAttention">FlashAttention</a></li>

</ul>
</details>

**标签**: `#GPU`, `#DSL`, `#Kernel Design`, `#FlashAttention`, `#Autotuning`

---

<a id="item-16"></a>
## [中国 AI 模型进军美国：更便宜、更开放、更智能](https://news.google.com/rss/articles/CBMilgFBVV95cUxQdm5uUXhNOEcyUXB6LWVpNDJ3UkJZclpja1ctcFdYclhjenJISmRRZGZTT2hoTDFXa2NuQlVzdGRRYmJWTWRCelg1M3hzWnR4WjBRZThDNjRmckw5c2paZU9pZ282ZVJXeTR6SWxhSG9qdkFUdlkyWUdZRDNPVUVBZGthbExxWThEdW5DWEk1NmJCQUJzT0E?oc=5) ⭐️ 7.0/10

中国 AI 模型正以更便宜、开源的替代方案在美国市场迅速崛起，挑战 OpenAI 和 Google 等美国巨头的统治地位。 这意义重大，因为它标志着全球 AI 格局的转变：美国独霸 AI 的时代结束了。中国模型以极低的成本提供有竞争力的性能，迫使西方公司重新思考定价和开放策略。 文章强调，DeepSeek 和阿里巴巴的 Qwen 等中国模型不仅更便宜，而且通常是开源的，允许开发者自由定制和部署。这与美国供应商更封闭、昂贵的 API 形成鲜明对比。

google\_news · AP News · 7月26日 04:05

**背景**: 多年来，美国公司以强大但昂贵的模型引领 AI 发展。如今，中国企业通过聚焦效率和开源分发迎头赶上，使先进 AI 惠及更广泛的人群。这类似于早期智能手机市场的转变，中国品牌在全球份额中崛起。

**标签**: `#AI`, `#Chinese AI`, `#global competition`, `#industry trends`

---

<a id="item-17"></a>
## [ML 会议对理论论文不公平吗？](https://www.reddit.com/r/MachineLearning/comments/1v6gh43/paper_lengths_and_reasonable_assumptions_in_ml/) ⭐️ 6.0/10

一位研究者指出，NeurIPS、ICML 等 ML 会议的固定页数和无限附录对理论论文不公平，并引用个人经历，称审稿人常因难度而非影响力拒稿。 这是一个真实的问题：如果审稿人因为数学难就拒稿，这个领域可能会抑制基础理论工作，转而鼓励增量式实证结果。会议需要重新思考审稿指南，以保护理论贡献。 作者指出，审稿人常要求在主文中详细解释相关工作，即使有附录也会改变要求，从“描述 X”变成“在主文中描述 X”。他们提议一条规则：“别当混蛋——如果你缺乏先修知识，就说出来，只审你能审的部分。”

reddit · r/MachineLearning · /u/OutsideSimple4854 · 7月25日 18:48

**背景**: NeurIPS、ICML 等 ML 会议长期采用固定页数限制（如 8 页）加无限附录，最初是为了节省印刷成本。官方规则要求论文自包含，审稿人不需阅读附录。这对理论论文造成压力，因为它们通常需要更多空间来展开数学基础。

**标签**: `#machine learning`, `#conferences`, `#paper review`, `#theoretical ML`

---