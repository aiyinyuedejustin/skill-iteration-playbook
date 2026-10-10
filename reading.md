# 推荐阅读

下面 8 份材料值得完整读一遍，按建议的阅读顺序排列。

1. **Anthropic《Demystifying evals for AI agents》**。agent 评测的基本概念和从零开始的路线图：任务、试验、判官、轨迹，能力评测和回归评测的区别。
   https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents
2. **Anthropic《Skill authoring best practices》**。怎么写 skill：简洁、自由度、渐进式披露、先建评测再写。
   https://docs.claude.com/en/docs/agents-and-tools/agent-skills/best-practices
3. **Anthropic skill-creator（SKILL.md、grader.md、run_loop.py）**。把上面两篇落成可以运行的流程：带不带 skill 对比、断言区分度、留出集选描述。
   https://github.com/anthropics/skills/tree/main/skills/skill-creator
4. **Hamel Husain《LLM Evals: Everything You Need to Know》**。错误分析、判官、评测集的问答合集，实操性最强。
   https://hamel.dev/blog/posts/evals-faq/
5. **OpenAI Cookbook《Self-Evolving Agents》**。一个从人工迭代到全自动迭代的完整示例，包括阈值、重试上限和版本管理。
   https://developers.openai.com/cookbook/examples/partners/self_evolving_agents/autonomous_agent_retraining
6. **GEPA 论文**。目前最有代表性的反思式提示词优化方法，讲清楚了为什么读轨迹比只看分数学得快。
   https://arxiv.org/abs/2507.19457
7. **ACE 论文《Agentic Context Engineering》**。把上下文当成不断演进的操作手册，提出简短偏差和上下文坍缩两个问题，对剪枝很有启发。
   https://arxiv.org/abs/2510.04618
8. **《A Survey of Self-Evolving Agents》**。自我进化 agent 的全景综述，适合想往研究方向深入时读。
   https://arxiv.org/abs/2507.21046

## 覆盖情况

| 材料 | 背景 | 优化目标 | 评测集 | 判分 | 错误分析 | 自动优化 | 剪枝 | 高成本运行 | 回归 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1. Anthropic 评测文章 | ✓ | ✓ | ✓ | ✓ | ✓ | | | ✓ | ✓ |
| 2. Skill 编写指南 | ✓ | ✓ | ✓ | | | | ✓ | | |
| 3. skill-creator | | ✓ | ✓ | ✓ | | ✓ | | ✓ | ✓ |
| 4. Hamel 评测问答 | | | ✓ | ✓ | ✓ | | | | |
| 5. OpenAI 自我进化示例 | | | | ✓ | | ✓ | | | ✓ |
| 6. GEPA | | | | | ✓ | ✓ | | ✓ | |
| 7. ACE | | | | | ✓ | ✓ | ✓ | | |
| 8. 自我进化综述 | ✓ | | | | | ✓ | | | |
