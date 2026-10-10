# 推荐阅读

下面材料值得完整读一遍，按建议顺序排列。

1. **Anthropic《Demystifying evals for AI agents》**  
   https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents  
   agent 评测的基本概念：任务、试验、判官、轨迹；能力评测 vs 回归评测。

2. **Anthropic《Skill authoring best practices》**  
   https://docs.claude.com/en/docs/agents-and-tools/agent-skills/best-practices  
   简洁、自由度、渐进式披露、先评测再写。

3. **Anthropic skill-creator**（SKILL.md、grader.md、run_loop.py）  
   https://github.com/anthropics/skills/tree/main/skills/skill-creator  
   带/不带 skill 对比、断言区分度、留出集选描述。

4. **Hamel Husain《LLM Evals FAQ》+《Evals Skills》+《Revenge of the Data Scientist》**  
   https://hamel.dev/blog/posts/evals-faq/  
   https://hamel.dev/blog/posts/evals-skills/  
   https://hamel.dev/blog/posts/revenge/  
   错误分析、「先看数据」、eval-audit 技能包。

5. **OpenAI Cookbook《Self-Evolving Agents》**  
   https://developers.openai.com/cookbook/examples/partners/self_evolving_agents/autonomous_agent_retraining  
   从人工到自动的闭环、阈值、回退。

6. **GEPA 论文**  
   https://arxiv.org/abs/2507.19457  
   反思式提示词优化，为何读轨迹比只看分数学得快。

7. **EvoSkill 论文 + 仓库**  
   https://arxiv.org/abs/2603.02766  
   https://github.com/sentient-agi/EvoSkill  
   从失败发现/修改整个 skill 文件夹，留出集与迁移。

8. **BudgetAPO 论文**  
   https://arxiv.org/abs/2610.05671  
   紧预算下如何分配评估调用；噪声自适应切片。

9. **ACE 论文《Agentic Context Engineering》**  
   https://arxiv.org/abs/2510.04618  
   操作手册式上下文；简短偏差与上下文坍缩。

10. **Skill smells 论文《From Anatomy to Smells》**  
    https://arxiv.org/abs/2607.01456  
    推荐写法 vs 真实 SKILL.md；26 种坏味道。

## 覆盖情况

| 材料 | 背景 | 目标 | 评测集 | 判分 | 错误分析 | 自动优化 | 剪枝 | 高成本 | 回归 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1. Anthropic 评测 | ✓ | ✓ | ✓ | ✓ | ✓ | | | ✓ | ✓ |
| 2. Skill 编写指南 | ✓ | ✓ | ✓ | | | | ✓ | | |
| 3. skill-creator | | ✓ | ✓ | ✓ | | ✓ | | ✓ | ✓ |
| 4. Hamel 系列 | | | ✓ | ✓ | ✓ | | | | |
| 5. OpenAI 自我进化 | | | | ✓ | | ✓ | | | ✓ |
| 6. GEPA | | | | | ✓ | ✓ | | ✓ | |
| 7. EvoSkill | ✓ | | ✓ | | ✓ | ✓ | | | ✓ |
| 8. BudgetAPO | | | ✓ | | | ✓ | | ✓ | |
| 9. ACE | | | | | ✓ | ✓ | ✓ | | |
| 10. Skill smells | ✓ | | | | | | ✓ | | ✓ |
