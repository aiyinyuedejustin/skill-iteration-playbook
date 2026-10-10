# 1. 背景：为什么 skill 需要迭代

## skill 成了一种新的软件

过去一年，给 AI 助手写的说明文件越来越多：Anthropic 的 Agent Skills、Cursor 的 rules、各家 agent 的系统提示词、仓库里的 AGENTS.md。它们的共同点是用自然语言写，给模型读，决定 agent 怎么做事。

Anthropic 在介绍 Agent Skills 时把它描述成一个文件夹，里面有说明、脚本和参考材料。启动时 agent 只看到每个 skill 的名字和描述，需要时才读正文，正文引用的文件再按需打开。这让 skill 可以很长、包含很多细节，又不必一次全塞进上下文。

但写出来只是开始。和代码一样，skill 也有 bug，也会在环境变化（换模型、换工具）后失效，也需要测试和维护。不同的是，代码的 bug 能被编译器和测试精确定位，skill 的 bug 往往只表现为「这次 agent 没做好」。

## 为什么第二版最难

v1 通常是作者把自己的经验写下来。之后的迭代会遇到几个问题：

- **不知道改动有没有用**。没有评测，只能靠几次试用的印象。
- **修一处坏一处**。Anthropic 的评测文章把这叫作被动循环：只在生产环境里发现问题，修好一个又引出别的。
- **越改越长**。每次失败加一句，很快就没人说得清哪一句在起作用。
- **对手上的例子过拟合**。改到最后，skill 在测试用的几道题上很好，换一道就不行。
- **跑一次太贵**。端到端的 agent 任务要容器、要时间、要 API 额度，没法像改函数那样随改随测。

## 这本书的材料从哪来

大致三条线索，后面的章节会把它们交织起来：

1. **公司的官方做法**。Anthropic 的 skill-creator 和 skill 编写指南、评测文章、上下文工程文章；OpenAI 的评测飞轮、提示词优化器、自我进化 agent 示例。
2. **研究**。自动优化提示词（APE、OPRO、ProTeGi、TextGrad、DSPy、GEPA）、自我改进的 agent（Reflexion、Voyager、Agent Workflow Memory、ACE、Darwin Gödel Machine），以及关于长指令、格式敏感性、判官偏差的研究。
3. **一线经验**。Hamel Husain 的错误分析、Shreya Shankar 关于判官校准的研究、Eugene Yan 的判官综述、superpowers 项目把测试驱动开发用在 skill 上的做法。

## 小结

skill 是用自然语言写的软件，它也需要测试、版本管理和重构。下一章先给出整张地图，再逐块展开。
