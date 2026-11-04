---
layout: default
title: "Horizon Summary: 2026-11-04 (ZH)"
date: 2026-11-04
lang: zh
---

> 从 949 条内容中筛选出 25 条重要资讯。

---

1. [AIRoA-0：仅凭 16,151 小时手持数据学会双臂操作，无需机器人](#item-1) ⭐️ 9.0/10
2. [多类学习理论终于破解 DS 维度密码](#item-2) ⭐️ 9.0/10
3. [TabPFN-3 在百万行数据上碾压 GBDT，LeCun 也在作者名单里](#item-3) ⭐️ 9.0/10
4. [Anthropic 的 FlashProve：用 zkSNARK 证明 LLM 推理，但代价是什么？](#item-4) ⭐️ 9.0/10
5. [AI 正迫使我们偿还 40 年的技术债务](#item-5) ⭐️ 8.0/10
6. [Go 终于有了一个不糟糕的 JSON API](#item-6) ⭐️ 8.0/10
7. [朝鲜假面试黑进 Binance，盗走 63 亿美元](#item-7) ⭐️ 8.0/10
8. [Kimi K3.1 Pro：开放权重，封闭钱包](#item-8) ⭐️ 8.0/10
9. [Google 对学校下最后通牒：接受 AI，否则失去 Search](#item-9) ⭐️ 8.0/10
10. [RSI-Dojo 教 LLM Agents 训练其他 LLMs](#item-10) ⭐️ 8.0/10
11. [Aspuru-Guzik 实验室推出用于药物发现的 LLM 科学家](#item-11) ⭐️ 8.0/10
12. [Nvidia RTX Spark 在 Linux 上性能仅 35%，令人沮丧](#item-12) ⭐️ 7.0/10
13. [AI 数据中心现在靠退役喷气发动机供电](#item-13) ⭐️ 7.0/10
14. [选民给 AI 数据中心热潮踩下刹车](#item-14) ⭐️ 7.0/10
15. [腾讯 WeVisOne-VL：一个小模型搞定检测、OCR、分割与抠图](#item-15) ⭐️ 7.0/10
16. [AI 顶会快被假论文淹没了——是时候下狠手了](#item-16) ⭐️ 7.0/10
17. [Hydrogen-1.0：开源科学模型以低 72%成本击败 GPT-6 Astra](#item-17) ⭐️ 7.0/10
18. [循环 Transformer 不节省 HBM 流量，性能分析揭示](#item-18) ⭐️ 7.0/10
19. [Amazon 重写工程手册，迎接 AI 写代码时代](#item-19) ⭐️ 7.0/10
20. [Datasette-agent 0.5a0：用聊天把数据库应用“聊”出来](#item-20) ⭐️ 6.0/10
21. [Hugging Face 谈开源 AI：到底谁在赚钱？](#item-21) ⭐️ 6.0/10
22. [Palantir 商业收入首超政府，这其实是个警告信号](#item-22) ⭐️ 6.0/10
23. [Dharma 的 2B 模型无需微调，将任意文档转为 JSON](#item-23) ⭐️ 6.0/10
24. [风投资金流向亿万富翁，而非初创企业](#item-24) ⭐️ 6.0/10
25. [CVPR 的 25 篇论文上限是 AI Slop 的许可证](#item-25) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [AIRoA-0：仅凭 16,151 小时手持数据学会双臂操作，无需机器人](https://arxiv.org/abs/2611.03815) ⭐️ 9.0/10

AIRoA-0（A-0）是一个完全基于 16,151 小时手持演示数据训练的双臂操作系统，这些数据由开源 YUBI 夹爪录制；在十项长时程任务上平均成功率达到 78%，而四个视觉-语言-动作基线模型在相同演示数据上后训练后的最佳成绩仅为 27%。 这很重要，因为它表明完全可以跳过机器人遥操作，仍然获得一个有能力操作策略——如果数据经得起检验，这将大幅降低机器人数据采集成本，并使跨具身部署真正可行。 该系统仅使用腕部摄像头（无头部或场景摄像头），学习每个腕部视图中哪些区域对任务重要，预测任务阶段，并以连续流形式解码动作；它可运行在双臂 Franka、TX-G2、OpenArm 和 UR 上，在新任务上后训练只需在单节点八块 H200 GPU 上不到四小时。

rss · arXiv AI · 11月4日 05:00

**背景**: 视觉-语言-动作（VLA）模型是当前构建机器人“大脑”的主流方案：取一个预训练的视觉-语言模型，加上动作输出，再用演示数据训练。问题一直在于，演示数据通常来自对真实机器人的遥操作，既慢又贵。像 YUBI 这样的手持夹爪改变了这一点：人只需拿着带摄像头的工具在任何地方录制任务，系统离线恢复动作。AIRoA-0 将这一思路推到极致，在任何阶段都不使用机器人数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2609.22809">Kinematic Interface for the Wild: Modular Bimanual Loco- Manipulation ...</a></li>
<li><a href="https://www.trossenrobotics.com/post/best-supported-umi-style-gripper">Best Supported UMI-Style Gripper for Robot Data Collection</a></li>
<li><a href="https://anylearn.cc/lessons/vla-vision-language-action-models">Vision - Language - Action Models — AnyLearn</a></li>

</ul>
</details>

**标签**: `#robotics`, `#manipulation`, `#imitation-learning`, `#vision-language-action`, `#cross-embodiment`

---

<a id="item-2"></a>
## [多类学习理论终于破解 DS 维度密码](https://arxiv.org/abs/2604.24749) ⭐️ 9.0/10

一篇新的 arXiv 论文证明了任何多类假设类的最大超图密度都被其 DS 维度上界所限制，从而填补了 √DS 的差距，并证实了 Daniely 和 Shalev-Shwartz 在 2014 年的猜想。这为多类学习和列表学习确立了最优样本复杂度。 这很重要，因为它最终确定了多类分类的精确样本复杂度，这个问题已经悬而未决十多年。这意味着我们现在确切知道学习一个多类模型需要多少数据，这对理论和实践都有实际意义。 关键技巧是利用 Hanneke 等人（2026）的新代数表征来证明超图密度受 DS 维度限制，从而直接得到最优界。这也解决了列表学习的样本复杂度问题，其中学习器可以输出一个小型候选标签列表。

rss · arXiv Machine Learning · 11月4日 05:00

**背景**: 在二分类中，VC 维度精确告诉你需要多少样本。对于多类问题，正确的度量是 DS 维度，但多年来上界和下界之间存在差距。这篇论文填补了这个差距，所以现在多类问题的理论就像二分类一样清晰了。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oracore.dev/en/news/tighter-sample-complexity-multiclass-learning-en">A tighter sample-complexity bound for multiclass learning | OraCore.dev</a></li>
<li><a href="https://proceedings.neurips.cc/paper_files/paper/2024/file/4b5d47949866d06ab5c03022b4a5a551-Paper-Conference.pdf">Improved Sample Complexity for Multiclass PAC</a></li>

</ul>
</details>

**标签**: `#learning theory`, `#sample complexity`, `#multiclass classification`, `#DS dimension`, `#VC dimension`

---

<a id="item-3"></a>
## [TabPFN-3 在百万行数据上碾压 GBDT，LeCun 也在作者名单里](https://arxiv.org/abs/2605.13986) ⭐️ 9.0/10

TabPFN-3 是一个新的表格基础模型，可扩展到 100 万训练行和 200 个特征，在 TabArena 基准上单次前向传播就击败了所有调优和集成基线。论文还引入了测试时计算扩展（TabPFN-3-Plus/Thinking），以 10 倍速度优势在 Elo 上超过 AutoGluon 1.5 extreme 200 分以上，而且后续的 TabPFN-3.5 已经发布。 这很重要，因为表格数据承载了大多数真实商业价值，而 GBDT 已经统治这块地盘十年了。如果一个预训练模型能开箱即用地击败调优 8 小时的 XGBoost 类基线，那么每个数据科学团队的默认技术栈都要变。 最巧妙的地方在于，TabPFN-3 完全只用自身先验生成的合成数据预训练——不用真实数据、不联网搜索、不借助 LLM——却依然获胜。缩减的 KV cache 加上行分块让它能在单张 H100 上处理 100 万行并保持快速推理，SHAP 值计算最高快 120 倍。

rss · arXiv Machine Learning · 11月4日 05:00

**背景**: 来自 Prior Labs 的 TabPFN 最初是面向小表格的基础模型——也就是那种只有几千行、深度学习通常打不过梯度提升决策树（GBDT）的数据。可以把它理解为一个在预训练时已经“见过”数百万张合成表格的模型，因此面对新数据集时只需一次前向传播就能预测，而不用从头训练。TabArena 是社区维护的表格机器学习活基准，旨在终结十年来互相矛盾的排行榜。TabPFN-3 的任务就是证明这套方法能扩展到小数据之外——而作者名单里有 Yann LeCun 和 Frank Hutter，说明这绝不是边缘项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/PriorLabs/TabPFN">GitHub - PriorLabs/TabPFN: ⚡ TabPFN: Foundation Model for ...</a></li>
<li><a href="https://arxiv.org/abs/2506.16791">[2506.16791] TabArena: A Living Benchmark for Machine ... TabArena (TabArena) - Hugging Face TabArena: A Living Benchmark for Machine Learning on Tabular Data TabArena: A Living Benchmark for Machine Learning on Tabular Data TabArena - a Hugging Face Space by TabArena Tabular Machine Learning 2026: TabArena Leaderboard — TabPFN ...</a></li>
<li><a href="https://priorlabs.ai/tabpfn-3-5">TabPFN 3.5 | Prior Labs</a></li>

</ul>
</details>

**标签**: `#tabular-data`, `#foundation-models`, `#machine-learning`, `#TabPFN`, `#benchmarking`

---

<a id="item-4"></a>
## [Anthropic 的 FlashProve：用 zkSNARK 证明 LLM 推理，但代价是什么？](https://www.marktechpost.com/2026/11/03/anthropic-flashprove-provable-inference-zksnark/) ⭐️ 9.0/10

Anthropic 发布了 FlashProve，一个 Apache 2.0 的 zkSNARK 原型，能够在不泄露权重的情况下，用密码学证明 LLM 的回复来自已承诺的权重。它在单张 H100 上以 110 tokens/秒的速度演示了 Llama 4 Maverick，证明大小为 19 MB。 这是迈向无信任 AI 的真正一步：你终于可以验证服务商确实运行了它声称的模型，而不是更便宜的替代品。但 90-100 倍的计算开销和 17 秒的验证时间意味着它还远未达到实时可用的程度。 该承诺大约可用于 1600 万次请求，之后提供方必须重新承诺；客户端下载约 6.5 MB 的承诺，外加每次请求一个证明。验证在 24 线程上需要 17 秒（单线程 21 秒），这才是真正的瓶颈。

rss · MarkTechPost · 11月3日 22:08

**背景**: zkSNARK 是一种密码学证明，让你在不泄露底层秘密的情况下证明某个陈述为真——就像证明你知道密码而不用输入它。在这里，“陈述”是某个特定模型产生了特定输出，而“秘密”是模型权重。这很重要，因为当你使用闭源 API 时，你无法知道提供方是否换成了更便宜的模型或篡改了输出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/provable-inference">Progress on provable inference for large language models \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Non-interactive_zero-knowledge_proof">Non-interactive zero-knowledge proof - Wikipedia</a></li>
<li><a href="https://huggingface.co/meta-llama/Llama-4-Maverick-17B-128E-Instruct">meta- llama / Llama - 4 - Maverick -17B-128E-Instruct · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的讨论很激烈：一位评论者声称 Anthropic 基于他们的 VerInf 工作“几乎没有署名”，而其他人指出对于开放权重模型，可证明推理很简单——只需重新计算即可。还有人质疑实际开销以及这是否能解决闭源模型的信任问题。

**标签**: `#zkSNARK`, `#provable inference`, `#AI verification`, `#cryptography`, `#Anthropic`

---

<a id="item-5"></a>
## [AI 正迫使我们偿还 40 年的技术债务](https://spectrum.ieee.org/ai-in-cybersecurity-php2shell-vulnerability) ⭐️ 8.0/10

IEEE Spectrum 的一篇新文章指出，AI 正被用于发现和修复长期存在的技术债务和安全漏洞（例如 PHP2Shell 漏洞），这在 Hacker News 上引发了 530 条评论的辩论：这究竟会带来更健壮的软件，还是无休止的修复 treadmill？ 这很重要，因为 AI 不仅仅是在写新代码——它正在审计我们几十年来一直忽视的遗留代码大山，这或许终于能让开源安全承诺成真。但它也可能制造一个永无止境的、不增加新功能的修复循环。 争论的关键在于：AI 是能处理深度重构，还是只能对 off-by-one 错误做外科手术式的窄补丁；以及它是否会顺便暴露像 Pegasus 这样的国家级 0-day。评论者还指出 HTTP2Shell/Brotli2Shell 可能比 PHP2Shell 更严重，表明人类仍会将漏洞捂上数月。

hackernews · pseudolus · 11月4日 11:52 · [社区讨论](https://news.ycombinator.com/item?id=50364336)

**背景**: 技术债务是软件中走捷径和快速修复所累积的成本——就像现在借钱、以后付利息。几十年来，开源项目一直依赖“别人会审计代码”的模糊希望，但大规模审计很少发生。现在 AI 漏洞扫描器正在自动化这种审计，发现人类遗漏的 bug，并迫使维护者面对几十年的忽视。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Technical_debt">Technical debt - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/technical-debt">What is technical debt? - IBM</a></li>
<li><a href="https://singularfeed.com/open-source-software-security-vulnerabilities/">Open Source Software Security Vulnerabilities Exposed</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的观点分化：一些人认为 AI 终于兑现了开源的安全承诺，另一些人则担心这会变成“强制性的、无休止的不增加新功能的修复 treadmill”。一位评论者庆幸 AI 降低了成本，让他能清理 5-7 年的技术债务；另一位则指出人类仍会将漏洞捂上数月。

**标签**: `#AI`, `#technical debt`, `#cybersecurity`, `#open source`, `#software engineering`

---

<a id="item-6"></a>
## [Go 终于有了一个不糟糕的 JSON API](https://go.dev/blog/jsonv2) ⭐️ 8.0/10

Go 团队推出了 encoding/json/v2，这是一个重新设计的 JSON API，旨在修复原始 encoding/json 包中长期存在的问题。新版本包含一个用于语法处理的底层 jsontext 包，并引入了 omitzero 标签等功能，同时为现有用户提供了迁移指南。 这很重要，因为 JSON 是现代 API 的通用语言，而 Go 最初的 JSON 包多年来一直是挫败感的来源——缓慢、古怪且难以扩展。一个设计更好、可能更快的 v2 版本可能使 Go 成为后端服务更具吸引力的选择，但迁移的痛苦（尤其是移除 MarshalIndent）可能会让一些团队在升级前犹豫不决。 新 API 将 JSON 处理分为两层：一个用于纯语法处理的底层 jsontext 包和一个使用反射的更高层 encoding/json/v2，这应该使构建自定义解析器更容易。早期基准测试表明，与 v1 相比，反序列化更快但序列化更慢，而 omitzero 标签最终解决了零值在你不想要时被序列化的烦人问题。

hackernews · olexsmir · 11月4日 17:52 · [社区讨论](https://news.ycombinator.com/item?id=50369106)

**背景**: Go 的 encoding/json 包从一开始就是标准库的一部分，但它设计得很快，积累了许多怪癖。例如，它默认不支持区分大小写的字段匹配，而且处理大型 JSON 负载的效率不高。社区多年来一直要求 v2，Go 团队终于在 2019 年左右开始认真开发，经过大量设计讨论后提案才落地。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pkg.go.dev/encoding/json">json package - encoding / json - Go Packages</a></li>
<li><a href="https://github.com/golang/go/issues/71497">encoding / json / v 2 : new API for encoding / json · Issue #71497...</a></li>
<li><a href="https://importstatic.com/go/go-json-v2-migration">Go JSON v 2 Migration : What Breaks in Go 1.27 | ImportStatic</a></li>

</ul>
</details>

**社区讨论**: 社区总体积极但也有一些抱怨：一位评论者称赞这次推出是“C++ 式的功能发布方式”，而另一位则对移除 MarshalIndent 表示遗憾，称替代方案“超级复杂且不直观”。还有关于 AI 编写 Go 代码的元评论，以及希望有类似 simdjson 的 SIMD 加速解析。

**标签**: `#Go`, `#JSON`, `#API design`, `#standard library`, `#parsing`

---

<a id="item-7"></a>
## [朝鲜假面试黑进 Binance，盗走 63 亿美元](https://www.theregister.com/security/2026/11/03/north-korean-fake-job-interview-led-to-63b-binance-heist/5307398) ⭐️ 8.0/10

一名朝鲜威胁行为者伪装成招聘人员，在假面试过程中诱骗 Binance 工程师在工作笔记本上安装恶意软件，并窃取部署凭证，于上周实施了创纪录的 63 亿美元盗窃案。 这很重要，因为它证明加密安全最薄弱的一环不是区块链，而是一个疲惫的工程师在工作笔记本上点了链接。如果 Binance 这样的巨头都能被假招聘人员攻破，那所有持有部署 token 的公司现在都该冒冷汗了。 被盗的不是私钥，而是容器部署 token，攻击者借此通过 CI/CD 流水线推送恶意代码——这是典型的供应链攻击手法，完全绕过了钱包层面的安全防护。

hackernews · smalltech · 11月4日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=50365755)

**背景**: 朝鲜的 Contagious Interview 行动已持续多年：假招聘人员在 LinkedIn 上联系开发者，发送编程挑战，并把恶意软件藏在项目文件里。这次目标恰好在 Binance 工作，结果造就了史上最大加密盗窃案。教训很简单——你的工作笔记本是生产凭证，不是搞副业的游乐场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theregister.com/security/2026/11/03/north-korean-fake-job-interview-led-to-63b-binance-heist/5307398">North Korean fake job interview led to $ 6 . 3 B Binance heist</a></li>
<li><a href="https://thehackernews.com/2026/07/north-korea-linked-hackers-hide.html">Fake Coding Tests Deliver OtterCookie-Aligned Malware Hidden in...</a></li>
<li><a href="https://www.ft.com/content/c7f5e395-c3a9-430e-b757-5014527b4d49?syn-25a6b1a6=1">Binance rushes to recover customer money after $ 6 . 3 bn heist</a></li>

</ul>
</details>

**社区讨论**: 评论区分成两派：一派怪工程师，一派怪 Binance 的架构——有人指出工程师机器上存在容器部署 token 是巨大红旗，本应强制只通过 CI 部署。还有人讽刺说，非人性化的自动化招聘流程把候选人推向了假招聘者，而 LinkedIn 在打击假公司方面做得远远不够。

**标签**: `#security`, `#supply-chain`, `#insider-threat`, `#cryptocurrency`, `#ci-cd`

---

<a id="item-8"></a>
## [Kimi K3.1 Pro：开放权重，封闭钱包](https://huggingface.co/moonshotai/Kimi-K3.1-Pro) ⭐️ 8.0/10

Moonshot AI 发布了 Kimi K3.1 Pro 的开放权重，这是一个 3T 级别的原生多模态 agentic 模型，基于 Kimi K3 进行后训练，并在数百个下游领域进行了大规模联合强化学习。它是 K3.1 系列的首个模型，目前已被 OpenRouter 等第三方推理提供商托管。 这很重要，因为它是一个接近前沿的开放权重模型，为企业提供了闭源 API 之外的强大选择。但说真的：除非你是 GPU 土豪，否则别想本地跑——它是给大公司准备的，不是给你的游戏主机。 架构上将 Gated MLA 换成了 Gated DSA，提升了长上下文效率——让你能塞更多 token 而不烧毁集群。另外，Together 和 Modal 等第三方提供商已经以相同价格提供 Moonshot 自家端点两倍的吞吐量，暗示优化空间巨大。

hackernews · abrarthought · 11月4日 15:30 · [社区讨论](https://news.ycombinator.com/item?id=50366999)

**背景**: 开放权重意味着训练好的参数被公开发布，任何人都可以下载使用，不像 GPT-5 那样的闭源模型只能通过 API 访问。Kimi K3.1 Pro 是一个大语言模型（LLM），能处理文本、图像和 agentic 任务，而且是“3T 级别”——可能指万亿级参数或训练 token，属于重量级选手。可以把它想象成拿到了米其林餐厅的菜谱，但你仍然需要专业厨房才能做出来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3.1-Pro">moonshotai/ Kimi -K 3 . 1 - Pro · Hugging Face</a></li>
<li><a href="https://www.kimi.ai/">Kimi AI Official Site | K 3 . 1 Pro Launches with Upgraded Coding...</a></li>

</ul>
</details>

**社区讨论**: HN 上的讨论两极分化：有人称其“刷榜”（benchmaxxed），比 DeepSeekV4.1-Flash 强不了多少，而另一些人则报告实际测试表现强劲。还有关于硬件需求的讨论——一位用户开玩笑说需要 8x B300 节点——以及对推理提供商竞争降低成本的兴奋。

**标签**: `#LLM`, `#open-weights`, `#AI`, `#model-release`, `#benchmarks`

---

<a id="item-9"></a>
## [Google 对学校下最后通牒：接受 AI，否则失去 Search](https://techcrunch.com/2026/11/04/google-faces-backlash-for-plan-that-would-turn-off-search-for-schools-that-restrict-ai/) ⭐️ 8.0/10

Google 宣布了一项 2027 年政策，拒绝启用其 AI 功能的 K-12 学校账户将被切断 Google Search，随后在 NYC 市长 Zohran Mamdani 和前 FTC 主席 Lina Khan 等政客指责其垄断行为后，于 2026 年 11 月 3 日部分软化了该规则。 这很重要，因为它表明 AI 采用正被武器化为获取基础数字基础设施的条件——Search 对学校来说不是奢侈附加品，而是作业、研究和日常课堂工具。Google 在政治压力下让步也证明，即使没有法庭审判，反垄断审查仍能影响产品决策。 原计划将 Gemini AI 功能与学生账户的 Search 访问捆绑，意味着学校无法在不完全失去 Search 的情况下退出 AI；澄清后学校可以保留 Search 同时禁用 Gemini 产品，但 2027 年的时间线仍然迫在眉睫。

rss · TechCrunch AI · 11月4日 16:17

**背景**: 可以把它想象成有线电视公司说：只有同时购买体育套餐，才能获得基础频道。Google 已经控制大部分搜索市场，并在重大联邦反垄断案中被裁定为垄断者，因此将 Search 访问与 AI 采用挂钩看起来像搭售——用一个主导产品推动另一个产品。学校是敏感战场，因为它们服务未成年人且议价能力有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnn.com/2026/11/03/tech/google-ai-search-policy">Google will let schools turn off AI, but they may also lose ...</a></li>
<li><a href="https://tech-insider.org/google-softens-school-search-rule-ai-ban-backlash-2026/">Google Search Schools AI Ban: 1 Rule Softened [2026]</a></li>
<li><a href="https://www.parentmap.com/education/google-ai-in-schools-search-policy-change-2027/">Google Gives Schools a Choice: Accept AI or Lose Search</a></li>

</ul>
</details>

**标签**: `#Google`, `#antitrust`, `#AI policy`, `#education`, `#monopoly`

---

<a id="item-10"></a>
## [RSI-Dojo 教 LLM Agents 训练其他 LLMs](https://arxiv.org/abs/2611.03698) ⭐️ 8.0/10

研究人员推出了 RSI-Dojo，一套包含 281 个可执行模型训练环境的数据集，通过 RSI-Craft pipeline 构建，并在收集的轨迹上微调 Qwen3.5-9B 和 Qwen3.6-35B-A3B，得到 RSI-Dojo-9B 和 RSI-Dojo-35B-A3B，分别在 PostTrainBench 上比基座模型提升 8.74 和 16.87 分。 这很重要，因为它超越了工作流级别的自动化，真正将 post-training 技能内化到模型本身，这是迈向递归自我改进的关键一步。如果 agents 能够可靠地训练和诊断模型，瓶颈将从人类 ML 专业知识转向算力和数据质量。 RSI-Craft 自动将顶级会议的研究论文转换为可执行环境，通过将数据集和指标实例化到统一接口中，然后按数据大小、执行可靠性和可区分性过滤任务。最终 RSI-Dojo-35B-A3B 在 PostTrainBench 上达到 29.95，在 PostTrainBench-Lite 上达到 53.29，与 GLM-5.2 和 GPT 5.5 等前沿模型相当。

rss · arXiv AI · 11月4日 05:00

**背景**: 递归自我改进（RSI）是指 AI 系统能够迭代设计出更强大的后继系统，可能引发智能爆炸。此前大多数自动化模型训练的工作集中在优化工作流或 harness，而不是教模型本身进行 post-training。RSI-Dojo 扭转了这一局面，通过创建环境让 agents 学习选择数据、训练模型、诊断失败并迭代——本质上是在学习成为 ML 工程师。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2609.26457">[2609.26457] Recursive self-improvement of AI research agents</a></li>
<li><a href="https://arxiv.org/abs/2505.21963">[2505.21963] LaMDAgent: An Autonomous Framework for Post ... A Primer on LLM Post-Training - PyTorch LaMDAgent: An Autonomous Framework for Post-Training Pipeline ... LaMDAgent: An Autonomous Framework for Post-Training Pipeline ... LLM Post-Training Experimentation Repository - GitHub Post-Training LLMs Guide: SFT, RLHF, DPO &amp; GRPO Explained ...</a></li>

</ul>
</details>

**标签**: `#LLM agents`, `#recursive self-improvement`, `#automated ML`, `#post-training`, `#arXiv`

---

<a id="item-11"></a>
## [Aspuru-Guzik 实验室推出用于药物发现的 LLM 科学家](https://arxiv.org/abs/2611.03832) ⭐️ 8.0/10

来自 Aspuru-Guzik 实验室的新 arXiv 预印本 El Agente Fármaco 是一个基于 LLM 的 AI 科学家，能将自然语言的药物发现目标转化为可扩展的计算筛选工作流，并由名为 Fármaco Atlas 的溯源追踪共享记忆支撑。在针对普通工具调用和 Codex 的 22 项任务基准测试中，它获得了最高的平均模型评判分数，同时使用的 token 更少、峰值上下文更低。 这很重要，因为它解决了计算药物发现中真正的瓶颈：不是工具本身，而是专家将它们串联起来并决定下一步做什么所付出的巨大努力。如果经得起检验，它可以让小团队运行以前需要专职计算化学家才能完成的筛选活动。 巧妙之处在于，单个请求可以为整个分子集合启动计算，而无需为每个化合物单独做 LLM 决策，这避免了随着筛选集合增长而导致的 token 使用和上下文爆炸。具备溯源感知的 Fármaco Atlas 存储分子、结构和结果，并记录它们的获取方式，因此 agent 可以精确查询每个决策所需的证据。

rss · arXiv AI · 11月4日 05:00

**背景**: 计算药物发现已经拥有大量用于提出和评估分子的工具，但将它们结合使用仍然需要人类专家来决定运行哪个工具、解释结果并规划下一步。现在人们正尝试用 LLM agent 作为自动化这一循环的粘合剂，而溯源追踪——精确记录每个结果是如何产生的——一直是科学工作流中可重复性的长期要求。El Agente Fármaco 结合了这两种思路：一个规划和执行筛选工作流的 LLM agent，加上一个让每个结果都可追溯的共享记忆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1359644626000553">AI agents in drug discovery: applications and case studies</a></li>
<li><a href="https://www.nature.com/articles/s41589-026-02295-x">Entering the agentic era of AI in drug discovery - Nature</a></li>
<li><a href="https://www.nature.com/nature-index/topics/l4/provenance-management-in-scientific-workflows">Provenance Management in Scientific Workflows - Nature</a></li>

</ul>
</details>

**标签**: `#AI scientist`, `#drug discovery`, `#LLM agents`, `#agentic workflows`, `#computational chemistry`

---

<a id="item-12"></a>
## [Nvidia RTX Spark 在 Linux 上性能仅 35%，令人沮丧](https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop) ⭐️ 7.0/10

一份实测报告显示，在 Nvidia RTX Spark 笔记本上双启动 Linux 会导致 GPU 推理性能降至 Windows 水平的 35%，原因是加密固件在 Linux 上将 GPU 时钟锁定在 780 MHz，而 Windows 上可运行在 2 GHz 以上。 这很重要，因为它表明专有固件如何将开源友好的硬件变成二等公民，并加剧了人们日益增长的担忧：AI 算力正被刻意锁定在 Windows 和云端。 关键点？降频逻辑是反的：Linux 在电池供电时全速运行，插电时反而降频，这暗示是 bug 而非故意破坏，而且加密的功率表只能由 Windows 解密。

hackernews · novaRom · 11月4日 08:46 · [社区讨论](https://news.ycombinator.com/item?id=50362905)

**背景**: Nvidia 的 RTX Spark 是一个面向轻薄笔记本和小型台式机的新平台，结合了 RTX 图形和 AI 加速，但仅随 Windows 出货。Linux 支持通常由 Nvidia 稍后提供，而在此案例中，电源管理固件是加密的，只有 Windows 能控制 GPU 时钟。没有能够解密并应用这些功率设置的 Linux 驱动，GPU 就会卡在低时钟速度，导致推理性能暴跌。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=50362905">Nvidia RTX Spark encrypted firmware slows... | Hacker News</a></li>
<li><a href="https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop">Linux on the Nvidia RTX Spark Laptop: What Actually... | MindStudio</a></li>
<li><a href="https://todayforai.com/en/story/story-37be7610-ca5">Encrypted Firmware Slows Nvidia DGX Spark Inference to 35% on ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的讨论混合了愤怒与理性：一些人认为这是刻意推动云端依赖和“精神控制”，而另一些人指出这仅仅是新 Windows 优先平台缺少 Linux 驱动支持，并非故意加密来拖慢推理。还有人质疑为何在全新的 Omarchy 发行版上测试，而不是成熟的发行版。

**标签**: `#NVIDIA`, `#Linux`, `#firmware`, `#proprietary drivers`, `#AI hardware`

---

<a id="item-13"></a>
## [AI 数据中心现在靠退役喷气发动机供电](https://techcrunch.com/2026/11/03/data-centers-are-turning-to-old-jet-engines-as-the-wait-for-power-grows/) ⭐️ 7.0/10

数据中心建设者正越来越多地转向改装退役喷气发动机——例如 FTAI Aviation 将 CFM56 发动机改装为 25 兆瓦燃气轮机——用于现场发电，因为并网和新涡轮机的等待时间已长达数年。ProEnergy 已在两个数据中心站点部署了改装燃气轮机，FTAI 计划于 2026 年开始生产。 这很重要，因为它证明 AI 热潮的真正瓶颈不再是芯片，而是电力，而电网无法足够快地输送电力。这对 ProEnergy 和 FTAI 等临时供电提供商是利好，但对那些假装 AI 基础设施正变得更环保的人来说，是一次无声的失败。 这些是航改型燃气轮机——本质上是驱动发电机的喷气发动机核心——可以在数月内发货和安装，而不是重型涡轮机或并网所需的数年时间。代价是真实的：它们比公用事业规模的涡轮机效率更低、污染更重，而且是在现场燃烧天然气，并非清洁电力。

rss · TechCrunch AI · 11月3日 22:19

**背景**: 把电网想象成一条已经堵得水泄不通的高速公路——新数据中心必须在长达数年的并网队列中等待才能接入。而喷气发动机本质上就是一台带动轴旋转的燃气轮机，所以如果你把发电机装到旧发动机上，就得到了一座可以停在服务器旁边的发电厂。这相当于停电时用发电机的基建版，只不过对于 AI 建设而言，停电成了新常态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.constructconnect.com/from-plane-power-to-power-grid-repurposing-jet-engines-for-data-centers">From Plane Power to Power Grid: Repurposing Jet Engines for ...</a></li>
<li><a href="https://www.datacenterdynamics.com/en/news/proenergy-offers-repurposed-jet-engines-to-data-cent/">ProEnergy repurposes jet engines to power data centers amid ...</a></li>
<li><a href="https://spectrum.ieee.org/ai-data-centers">Why Jet Engines Could Power the AI Data Centers Boom - IEEE ...</a></li>

</ul>
</details>

**标签**: `#data-centers`, `#energy-infrastructure`, `#power-generation`, `#grid-capacity`, `#industry-trends`

---

<a id="item-14"></a>
## [选民给 AI 数据中心热潮踩下刹车](https://www.theverge.com/policy/1026365/data-centers-midterms-results) ⭐️ 7.0/10

在 2026 年中期选举中，10 个州的选民对 41 项与数据中心相关的 ballot measures 进行了投票，几乎在所有竞争中他们都支持限制或拒绝了支持开发的措施。这对 AI 行业的基础设施增长造成了沉重打击，因为支持 moratoriums 的候选人在全国范围内获胜。 这很重要，因为数据中心是 AI 的物理支柱，而选民刚刚表明他们可以猛踩扩张的刹车。AI 行业不能再将基础设施建设视为纯粹的技术或企业问题——这现在是一场政治斗争，而他们在投票箱前正在失利。 这些措施范围广泛：41 项 ballot measures 中有 28 项会通过禁令或 moratoriums 限制开发，而选民批准了其中大多数。仅在 Ohio 就有 18 个社区将数据中心措施列入选票，包括 Hubbard 的全面禁令——这表明这是一场全国性的反抗，而非地方性的偶然。

rss · The Verge AI · 11月4日 16:05

**背景**: 多年来，AI 公司一直在疯狂建设，大举建造大型数据中心来训练和运行 ChatGPT、Claude 等模型。但这些设施消耗大量电力和水资源，已经开始惹恼当地居民。如今，随着 46 个州有 575 项 active restrictions，甚至 Bernie Sanders 和 AOC 提出了联邦 moratorium 法案，这种反弹已经主流化——选民正在发出他们的声音。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/04/data-center-ballot-measures-2026-midterm.html">Voters rebuff data centers in every ballot measure except one</a></li>
<li><a href="https://ballotpedia.org/Data_center-related_ballot_measures,_2026">Data center-related ballot measures, 2026 - Ballotpedia</a></li>
<li><a href="https://www.datacenterbans.com/">Data Center Moratoriums</a></li>

</ul>
</details>

**标签**: `#data centers`, `#AI infrastructure`, `#policy`, `#regulation`, `#midterms`

---

<a id="item-15"></a>
## [腾讯 WeVisOne-VL：一个小模型搞定检测、OCR、分割与抠图](https://www.marktechpost.com/2026/11/03/tencent-wevisone-vl-vision-language-model/) ⭐️ 7.0/10

腾讯微信视觉团队发布了 WeVisOne-VL，这是一个采用 Apache 2.0 协议的视觉语言模型，提供 2B 和 4B 两种规模，将目标检测、OCR、计数、指代分割和可提示 alpha matting 统一到一个模型中，并搭配一个仅 9.6M 参数的轻量级 pixel decoder。 这是一次真正有用的开源发布：大多数 VLM 能描述图像，却给不出像素级精确的 mask 或 alpha matte，而能做到的模型通常又大又闭源。一个 Apache 2.0 下的 2B/4B 模型，一次性完成检测、OCR、分割和抠图，正是边缘侧和产品团队一直缺的实用积木。 巧妙之处在架构：WeVisOne-VL 通过结构化的 next-token prediction 输出目标级结果，再交给一个仅 9.6M 参数的微型 pixel decoder 完成分割和 alpha matting，这样庞大的 VLM 本身不必生成稠密像素网格。这种拆分很聪明，既保持模型小巧，又能提供像素级感知。

rss · MarkTechPost · 11月4日 04:39

**背景**: 像 CLIP 或 LLaVA 这样的视觉语言模型很擅长说出图里有什么，但通常输出的是文本，而不是精确的 mask。Alpha matting 是一个经典的难题：把前景物体从背景中分离出来，并保留头发、毛发这类半透明的软边缘，传统上需要 trimap 和专门的算法。WeVisOne-VL 的主张是把这些连同检测和 OCR 一起塞进一个 VLM，让你不必再拼一条由五个独立模型组成的流水线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Tencent/WeVisOne-VL">GitHub - Tencent/WeVisOne-VL: WeVisOne-VL is a powerful VLM ...</a></li>
<li><a href="https://tencent.github.io/WeVisOne-VL/">WeVisOne-VL: Unified Visual Perception from Objects to Pixels</a></li>
<li><a href="https://arxiv.org/abs/2610.31329">[2610.31329] WeVisOne-VL: Unified Visual Perception from ...</a></li>

</ul>
</details>

**标签**: `#vision-language-model`, `#multimodal`, `#segmentation`, `#OCR`, `#open-source`

---

<a id="item-16"></a>
## [AI 顶会快被假论文淹没了——是时候下狠手了](https://www.reddit.com/r/MachineLearning/comments/1xnkbeu/a_message_to_top_tier_conferences_d/) ⭐️ 7.0/10

一位研究者在 Reddit 上发帖猛烈抨击，呼吁顶级 AI 会议强硬 desk-reject AI 生成和造假论文，并列举了最近 A 类和 A\* 会议上的多个见闻：有报告人连自己论文里的 knowledge graph 表示都解释不清，有人直接在 Q&amp;A 环节读 ChatGPT 的回答，还有人把同一篇论文同时投中两个会议，GitHub 仓库里连 LLM prompt 都没删，数据全是编的。 这不仅仅是一个暴躁研究者的吐槽——这是系统性腐烂的症状。如果会议不严厉打击，认真做研究的人会被 prompt 玩家挤走，整个 peer-review 流程也会失去公信力。事情已经发生在 A\* 会议上，说明问题早就过了临界点。 最致命的细节：一位报告人被问到如何表示 knowledge graph 时，想了整整五分钟，然后憋出一句“用 vector”——这种含糊到离谱的回答，摆明了他根本没读过自己的论文。更离谱的是，那个一稿多投的人把整个 LLM 聊天记录留在了公开的 GitHub 仓库里，造假数据暴露得彻彻底底，毫无羞耻心。

reddit · r/MachineLearning · /u/Vegetable-Formal-753 · 11月4日 09:55

**背景**: 像 NeurIPS 和 ICML 这样的顶级 AI 会议，已经成了 AI 生成内容的战场。NeurIPS 2026 用 AI 文本检测工具 Pangram 筛查后，直接 desk-reject 了 178 篇 position paper（占该 track 的 18.4%）；ICML 2026 则通过在 PDF 里嵌入隐藏 prompt 注入，抓到违反 LLM 使用政策的审稿人后，desk-reject 了 497 篇论文。军备竞赛是真的：会议在部署检测工具，作弊者也在变得更狡猾——但这里的见闻说明，光靠检测远远不够。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://strictcite.com/blog/neurips-2026-position-paper-pangram-ai-detection">NeurIPS Desk-Rejected 178 Position Papers for Being “AI ...</a></li>
<li><a href="https://byteiota.com/icml-desk-rejects-497-papers-ai-review-trap-explained/">ICML Desk Rejects 497 Papers: AI Review Trap Explained</a></li>
<li><a href="https://aiweekly.co/alerts/icml-desk-rejects-497-papers-over-llm-review-violations">ICML desk-rejects 497 papers over LLM review violations | AI ...</a></li>

</ul>
</details>

**标签**: `#peer-review`, `#machine-learning`, `#research-integrity`, `#LLM-generated-content`, `#academic-conferences`

---

<a id="item-17"></a>
## [Hydrogen-1.0：开源科学模型以低 72%成本击败 GPT-6 Astra](https://www.reddit.com/r/MachineLearning/comments/1xnjhdd/hydrogen10_openweight_scientific_model_beats_gpt6/) ⭐️ 7.0/10

Deep Principle 发布了 Hydrogen-1.0，这是一个基于 GLM-5.3 后训练的开源权重模型，专注于化学、材料科学和生命科学领域。该模型声称在 FrontierScience Research 基准上以约 72%更低的估计输出成本（每问题$0.25 vs. $0.88）领先 GPT-6 Astra 5 个百分点（通过率 38.3% vs. 33.3%）。 这很重要，因为它表明一个小型、领域专注的开源权重模型可以在专业科学基准上以极低成本超越前沿闭源模型。如果结果经得起检验，这将是支持领域数据后训练而非单纯扩展通用模型的强有力论据。 该模型使用监督微调和强化学习进行训练，数据包括领域数据、科学家反馈、实验室记录和发现轨迹。它在 NMR 结构解析上落后 GPT-6 Astra 3.33 个百分点，且工作流示例是模型加工具的演示，并非完全自主研究。

reddit · r/MachineLearning · /u/AKAMA199 · 11月4日 09:00

**背景**: Hydrogen-1.0 基于 GLM-5.3 构建，这是 Z.ai 推出的开源权重模型，擅长编码和长周期任务。FrontierScience 是 OpenAI 推出的基准，用于测试 AI 在物理、化学和生物领域的推理能力。GPQA Diamond 是这些领域的研究生水平多项选择题基准。Deep Principle 是 Mira AI Scientist 背后的团队，这是一个 AI 辅助科学研究的工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/zai-org/GLM-5.3">zai-org/GLM-5.3 · Hugging Face</a></li>
<li><a href="https://openai.com/index/frontierscience/">Evaluating AI’s ability to perform scientific research tasks</a></li>
<li><a href="https://artificialanalysis.ai/evaluations/gpqa-diamond">GPQA Diamond Benchmark Leaderboard | Artificial Analysis</a></li>

</ul>
</details>

**标签**: `#open-weight-models`, `#AI-for-science`, `#benchmarks`, `#LLM-evaluation`, `#chemistry`

---

<a id="item-18"></a>
## [循环 Transformer 不节省 HBM 流量，性能分析揭示](https://www.reddit.com/r/MachineLearning/comments/1xnskvt/do_looped_transformers_save_hbm_traffic_profiling/) ⭐️ 7.0/10

一项在 NVIDIA B200 GPU 上的新性能分析研究表明，Huginn 风格的循环 Transformer 虽然在迭代间复用相同权重以节省存储，但除非权重能放入 L2 缓存，否则每次迭代仍会从 HBM 读取权重。作者使用 Nsight Compute 测量了随机权重的完整 Huginn Core，发现八次迭代的耗时和 HBM 读取量均约为单次迭代的 8 倍。 对于那些认为权重共享能自动减少循环模型内存带宽的人来说，这是一个有用的现实检验。它表明，如果没有精心的 kernel 设计，架构层面的权重复用并不会转化为硬件层面的流量节省——这对于在内存受限的 GPU 上实现高效推理是一个关键见解。 研究发现，与八个相同副本相比，使用共享 72 MiB 权重的八个 matmul 链运行速度快 24%，且几乎不从 HBM 读取数据；但当权重达到 288 MiB（大于 L2）时，优势消失。这突显了 L2 缓存大小是权重复用收益的关键阈值。

reddit · r/MachineLearning · /u/2dayyy6 · 11月4日 16:26

**背景**: 像 Huginn 这样的循环 Transformer 通过多次复用相同的层权重来增加有效深度而不增加参数，这在内存受限的场景下听起来很棒。HBM 是 GPU 上的高带宽内存，负责向计算核心提供数据；从 HBM 读取数据的代价很高。该研究探讨了共享权重是否也能减少 HBM 流量，答案是：并非自动如此。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://interactive-active-ai.github.io/Aha-Looped-Transformer/papers/huginn/">Huginn · Aha Looped Transformer</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://docs.nvidia.com/nsight-compute/ProfilingGuide/index.html">2. Profiling Guide — NsightCompute</a></li>

</ul>
</details>

**标签**: `#transformers`, `#GPU-memory`, `#HBM`, `#profiling`, `#efficient-inference`

---

<a id="item-19"></a>
## [Amazon 重写工程手册，迎接 AI 写代码时代](https://news.google.com/rss/articles/CBMitgFBVV95cUxPRjNaNlZ1aGFDMUd4c1p4YTc0bllabG9rM09HSVZFY0RIR2xMUFRTQkhGZVA0V2psU053SWtDc0dmQ3Ita0UyWUJvdXVPUGJsc2EwaDNmOUhmVi1JcVFGUHhPa3cyUkE5S0x5RGYyNFFKVHplU3otS0lLaGNjWG5OVFBGOWdram5YNExVOG81ZldrLThQdWQ5ek9hbDd6d1dWOWZtMzBsX0JDLV9GV2xDTTk0SkF1QQ?oc=5) ⭐️ 7.0/10

据报道，Amazon 正在全面修订其软件工程手册，以适应 AI 生成大量代码的新时代。这一举措标志着公司在开发方式上的重大转变，但具体变更细节尚未公开。 这很重要，因为 Amazon 是企业工程实践的风向标。如果这样规模的公司都在围绕 AI 生成代码重写手册，很可能会加速整个行业的类似变革，并给工具供应商带来跟进压力。 虽然具体细节有限，但这一转变意味着 Amazon 正在重新思考当 AI 成为主要作者时的代码审查、测试和归属模型。真正的挑战不是生成代码，而是大规模确保质量和问责。

google\_news · GeekWire · 11月3日 20:26

**背景**: 像 GitHub Copilot 和 Amazon 自家的 CodeWhisperer 这样的 AI 编码助手，短短几年内就从新奇事物变成了主流工具。企业现在正努力解决如何在不牺牲代码质量或安全性的情况下整合这些工具。Amazon 重写手册本质上是对这一挑战的正式化——标志着临时性的 AI 使用正在让位于结构化流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tabnine.com/">Tabnine AI Code Assistant | Smarter AI Coding Agents. Total...</a></li>
<li><a href="https://slashdot.org/software/ai-coding-assistants/">Top AI Coding Assistants in 2026</a></li>

</ul>
</details>

**标签**: `#AI`, `#software engineering`, `#Amazon`, `#developer productivity`, `#industry trends`

---

<a id="item-20"></a>
## [Datasette-agent 0.5a0：用聊天把数据库应用“聊”出来](https://simonwillison.net/2026/Nov/3/datasette-agent/) ⭐️ 6.0/10

datasette-agent 0.5a0 引入了 &\#x27;panel&\#x27; 功能，可以在任意 Datasette 页面（例如表格或查询页）旁边打开一个 agent 聊天窗口。结合 datasette-apps，用户可以通过提示词直接生成一个数据库驱动的应用，并在旁边的聊天中直接修改它。 这很重要，因为它把数据探索和应用构建之间的循环压缩了：你现在可以在不离开 Datasette 界面的情况下迭代一个可用的应用。虽然还是 alpha 版，但它指向了一个未来——‘氛围编程’内部工具就像写一条 SQL 查询一样随意。 panel 是一个分屏聊天窗口，位于应用旁边；截图显示了 app\_create、app\_render 和 app\_str\_replace 等工具调用，意味着 agent 直接操作应用的 HTML/JS/CSS。示例中仅用两条提示词就构建了一个包含 185 个模型的 ‘LLM Price Explorer’，并带有黑客风格设计。

rss · Simon Willison · 11月3日 23:13

**背景**: Datasette 是 Simon Willison 的开源数据探索和发布工具，常被描述为‘Web 版的 SQLite’。datasette-agent 增加了一个 LLM 驱动的聊天界面来查询数据，而 datasette-apps 允许在 Datasette 内部托管单文件 HTML/JS/CSS 应用。新的 panel 功能将它们串联起来：你聊天，agent 构建应用，然后你继续聊天来完善它——全部在同一页面内完成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/datasette/datasette-apps">GitHub - datasette/ datasette - apps : Apps that live inside Datasette</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-apps/">Host applications inside Datasette with Datasette ... - Datasette Blog</a></li>
<li><a href="https://simonwillison.net/2026/May/21/datasette-agent/">Datasette Agent | Simon Willison’s Weblog</a></li>

</ul>
</details>

**标签**: `#datasette`, `#ai-agents`, `#llm`, `#developer-tools`, `#release`

---

<a id="item-21"></a>
## [Hugging Face 谈开源 AI：到底谁在赚钱？](https://techcrunch.com/video/open-source-ai-is-booming-hugging-face-explains-who-profits/) ⭐️ 6.0/10

TechCrunch 发布了一期视频/播客节目，邀请 Hugging Face 讨论企业如何从开源 AI 模型中获取价值，以及在中国开源模型崛起的背景下美国玩家能否跟上。这是一场对话而非发布——没有新产品、没有 benchmark，只有行业视角。 这很重要，因为变现问题是每家开源 AI 公司都绕不开的房间里的大象——权重都免费给了，收入从哪来？Hugging Face 可以说是最有资格回答这个问题的公司，而它对中国开源模型（Kimi、DeepSeek、GLM）作为竞争威胁的看法值得一听。 节目的框架很说明问题：企业、政府和初创公司都在追逐开源模型，图的是更低成本、更多控制和灵活性——而这恰恰是侵蚀闭源 API 提供商护城河的卖点。节目还重点讨论了“美国玩家能否跟上”的角度，暗示中国实验室如今已经发布了一些最强的开放权重模型。

rss · TechCrunch AI · 11月4日 19:30

**背景**: Hugging Face 是开源 AI 事实上的中心广场——这家总部位于纽约的公司，其平台托管模型和数据集，其 Transformers 库是大多数 ML 工程师的默认工具箱。它的商业模式本身就是个好案例：免费公共托管加上付费的 Compute 和 Enterprise 层级。更大的背景是，来自 DeepSeek 和 Moonshot 的 Kimi 等中国实验室的开放权重模型已经跨过前沿门槛，所以“开源更便宜但更差”的论调已经不成立了。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face - Wikipedia</a></li>
<li><a href="https://huggingface.co/">Hugging Face – The AI community building the future.</a></li>
<li><a href="https://www.secondtalent.com/resources/chinese-open-source-llms-ai-leaders/">Top 5 Chinese Open-Source LLMs Dominating 2026</a></li>

</ul>
</details>

**标签**: `#open-source AI`, `#monetization`, `#Hugging Face`, `#industry analysis`, `#AI competition`

---

<a id="item-22"></a>
## [Palantir 商业收入首超政府，这其实是个警告信号](https://techcrunch.com/2026/11/03/hiding-inside-palantirs-skyrocketing-quarter-is-a-foreboding-signal/) ⭐️ 6.0/10

Palantir 2026 年 Q3 财报显示，美国商业收入达到 9.84 亿美元，首次超过美国政府收入的 9.53 亿美元，总营收同比增长 96%至 23.1 亿美元，全年指引上调至 85.3 亿美元。 这很重要，因为它标志着企业 AI 需求已经超过政府合同——Palantir 不再只是国防承包商，而正在成为企业 AI 平台。但令人不安的是，市场以 50 倍前瞻市销率定价完美预期，商业增长一旦放缓，后果可能很惨烈。 美国商业收入同比增长 148%，而政府收入增长 96%，商业收入在短短两年内翻了五倍。这种超高速增长令人印象深刻，但也意味着未来季度的门槛已经高得离谱。

rss · TechCrunch AI · 11月3日 21:05

**背景**: Palantir 最初是一家为情报机构和军方提供数据分析的神秘公司——想想 Gotham 和 Foundry。在上市后的大部分时间里，政府合同是它的命脉。如今，借助 AIP（人工智能平台），它向企业销售 AI 驱动的数据集成服务，而这个赌注终于开始大获回报。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/02/palantir-pltr-earnings-q3-2026.html">Palantir (PLTR) earnings Q3 2026 - CNBC Palantir Revenue Breakdown: Government vs Commercial Palantir US commercial revenue passes government sales for ... Palantir’s US commercial revenue tops government for the ... Palantir&#x27;s Commercial Revenue Just Passed the U.S. Government ... Palantir raises full-year revenue outlook as US commercial ...</a></li>
<li><a href="https://www.lambdafin.com/articles/palantir-government-vs-commercial-revenue">Palantir Government vs Commercial Revenue: The 53/47 Split ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Palantir_Technologies">Palantir Technologies</a></li>

</ul>
</details>

**标签**: `#Palantir`, `#enterprise AI`, `#business analysis`, `#revenue trends`, `#industry news`

---

<a id="item-23"></a>
## [Dharma 的 2B 模型无需微调，将任意文档转为 JSON](https://huggingface.co/blog/Dharma-AI/dharma-field-extractor) ⭐️ 6.0/10

Dharma-AI 发布了 Dharma Field Extractor，这是一个 2B 参数的视觉语言模型，接收文档图像和开放式请求或严格 schema，返回带类型的 JSON，支持嵌套字段。它无需针对每类文档进行微调，并在 Hugging Face 博客文章中介绍。 对于厌倦了 OCR 流水线或为简单提取支付前沿 LLM API 费用的人来说，这是件大事。一个专门构建的小模型能处理任意文档，可能让结构化数据提取变得便宜且易用，但它是否真能泛化到发票之外还有待观察。 该模型能处理发票中的行项目等嵌套结构，返回带数量和值的排序列表，并且可以填充提供的 schema 或自行发现字段。2B 参数足够小，可在本地运行，但博客文章未详细说明在复杂布局或手写体上的准确率。

rss · Hugging Face Blog · 11月4日 17:50

**背景**: 文档提取传统上需要基于模板的 OCR（脆弱）或需要精心提示的大型 LLM（昂贵）。最近的 LayoutLM 和 NuExtract 等模型试图弥合差距，但 Dharma 的卖点是一个小型模型即可开箱即用于任何文档类型。可以把它看作从像素到数据库行的专用翻译器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/Dharma-AI/dharma-field-extractor">Dharma Field Extractor: Any Document In, Structured Fields in ...</a></li>
<li><a href="https://www.aigpu.cloud/en/blog/dharma-field-extractor-structured-json-documents">Dharma Field Extractor: 2B-Parameter Model Turns Any Document ...</a></li>
<li><a href="https://www.printingpressai.com/article/generative-ai/dharma-field-extractor-any-document-in-structured-fields-in-json-out">Dharma Field Extractor: Any Document In, Structured Fields in ...</a></li>

</ul>
</details>

**标签**: `#document extraction`, `#JSON`, `#NLP`, `#information extraction`, `#Hugging Face`

---

<a id="item-24"></a>
## [风投资金流向亿万富翁，而非初创企业](https://news.crunchbase.com/venture/startup-billionaire-founders-ai-defense-anthropic-spcx/) ⭐️ 6.0/10

2026 年前 10 个月，美国从种子轮到成长阶段的风险投资中，超过一半流向了七家由亿万富翁创立或领导的公司，股权融资总额超过 2600 亿美元。 这很重要，因为它表明风险投资正变成赢家通吃的游戏，已经富有的创始人吸走了大部分资金，而草根初创企业则难以获得关注。如果你不是亿万富翁，那就祝你能拿到投资条款清单吧。 集中度惊人：数千家公司中的七家筹集了超过 2600 亿美元，占美国风投资金的一半以上。这意味着生态系统的其余部分在争夺残羹剩饭，这可能是由 AI 和国防科技领域推动的，因为大牌人物吸引大额支票。

rss · Crunchbase News · 11月4日 12:00

**背景**: 风险投资是投资于初创企业以换取股权的资金，通常从种子轮（最早阶段）到成长阶段（后期轮次）。通常，这些资金会分散到许多初创企业，但最近，很大一部分流向了由已经是亿万富翁的人领导的公司——比如 Elon Musk、Peter Thiel 等。这很不寻常，因为风投本应资助有风险的新想法，而不是稳赢的赌注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Venture_capital">Venture capital - Wikipedia</a></li>
<li><a href="https://visible.vc/blog/startup-funding-stages/">The Ultimate Guide to Startup Funding Stages - Visible.vc</a></li>

</ul>
</details>

**标签**: `#venture capital`, `#startups`, `#billionaires`, `#funding trends`, `#AI/defense`

---

<a id="item-25"></a>
## [CVPR 的 25 篇论文上限是 AI Slop 的许可证](https://www.reddit.com/r/MachineLearning/comments/1xnscvr/why_cant_conferences_just_reasonably_reduce_the/) ⭐️ 6.0/10

r/MachineLearning 上的一篇 Reddit 帖子批评了 CVPR 2027 的指南，该指南允许每位作者提交最多 25 篇论文，超出部分才会被 desk reject。发帖人认为，在 AI 生成“slop”论文泛滥的时代，这个上限高得离谱，并希望将第一作者投稿限制削减到 2-3 篇。 这很重要，因为 25 篇的上限把会议投稿变成了拼数量的游戏，质量反而靠边站，而审稿人成了买单的人。如果 CVPR 不收紧规则，“A\* 印章”就会失去信号价值，整个同行评审流程会被低质量的 AI 产出淹没。 该政策明确表示，超过 25 篇的作者会被 desk reject 多出的部分，这意味着系统是为了处理海量投稿而设计，而不是为了阻止它们。发帖人的核心观点是，将第一作者上限设为 2-3 篇会迫使研究者真正关心每篇论文的严谨性和呈现质量。

reddit · r/MachineLearning · /u/mofoss · 11月4日 16:17

**背景**: 像 CVPR 这样的 ML 会议投稿量已经爆炸式增长，而生成式 AI 的兴起让大规模生产看起来像模像样的论文变得轻而易举。会议使用 desk rejection 来过滤违反投稿限制等规则的论文，但 25 篇的上限过于宽松，几乎起不到过滤作用。真正的瓶颈是审稿人的精力：每多一篇论文，每篇评审分到的时间就更少，从而全面拉低评审质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Computer_Vision_and_Pattern_Recognition">Conference on Computer Vision and Pattern Recognition - Wikipedia</a></li>
<li><a href="https://arxiv.org/html/2502.00690">Dissecting Submission Limit in Desk - Rejections : A Mathematical...</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_slop">AI slop - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Reddit 讨论串中充满了沮丧和冷嘲热讽，评论者一致认为 25 篇的上限对当前 AI 驱动的研究环境充耳不闻。最尖锐的观点是，某些国家和机构把 A\* 会议印章当作职业货币，所以当允许投 25 次飞镖时，伦理就被抛到脑后了。

**标签**: `#machine learning`, `#conferences`, `#peer review`, `#AI ethics`, `#academic publishing`

---