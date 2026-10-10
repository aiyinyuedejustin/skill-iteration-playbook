# 参考来源

控制在约 45–50 条。分为基础、直接相关、可借用。

## 基础

- Anthropic，Demystifying evals for AI agents：https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents
- Anthropic，Effective context engineering for AI agents：https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
- Anthropic，Writing effective tools for agents：https://www.anthropic.com/engineering/writing-tools-for-agents
- Hamel Husain，A Field Guide to Rapidly Improving AI Products：https://hamel.dev/blog/posts/field-guide/
- Hamel Husain，LLM Evals: Everything You Need to Know：https://hamel.dev/blog/posts/evals-faq/
- Hamel Husain，The Revenge of the Data Scientist：https://hamel.dev/blog/posts/revenge/
- Hamel Husain，Evals Skills for Coding Agents：https://hamel.dev/blog/posts/evals-skills/
- hamelsmu/evals-skills（含 eval-audit）：https://github.com/hamelsmu/evals-skills
- Eugene Yan，Evaluating the Effectiveness of LLM-Evaluators：https://eugeneyan.com/writing/llm-evaluators/
- Who Validates the Validators?（标准漂移）：https://arxiv.org/abs/2404.12272
- Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena：https://arxiv.org/abs/2306.05685
- Lost in the Middle：https://arxiv.org/abs/2307.03172
- IFScale，How Many Instructions Can LLMs Follow at Once?：https://arxiv.org/abs/2507.11538
- Sclar 等，Sensitivity to Spurious Features in Prompt Design：https://arxiv.org/abs/2310.11324

## 直接相关：Skill / 提示词 / Agent 迭代

- Anthropic，Equipping agents for the real world with Agent Skills：https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills
- Anthropic，Skill authoring best practices：https://docs.claude.com/en/docs/agents-and-tools/agent-skills/best-practices
- Anthropic，skills 仓库（含 skill-creator）：https://github.com/anthropics/skills
- Anthropic，Improving skill-creator：https://claude.com/blog/improving-skill-creator-test-measure-and-refine-agent-skills
- Authoring Agent Skills: A Software-Engineering Approach：https://arxiv.org/abs/2607.25032
- From Anatomy to Smells（skill smells）：https://arxiv.org/abs/2607.01456
- What Keeps Agent Skills from Being Reusable?（约 138K SKILL.md）：https://arxiv.org/abs/2608.08453
- OpenAI，Self-Evolving Agents cookbook：https://developers.openai.com/cookbook/examples/partners/self_evolving_agents/autonomous_agent_retraining
- OpenAI，Agent Improvement Loop：https://developers.openai.com/cookbook/examples/agents_sdk/agent_improvement_loop
- OpenAI，Evaluation flywheel：https://github.com/openai/openai-cookbook/blob/main/examples/evaluation/Building_resilient_prompts_using_an_evaluation_flywheel.md
- OpenAI，Prompt optimizer：https://platform.openai.com/docs/guides/prompt-optimizer
- AWS Bedrock AgentCore optimization（建议 + A/B）：https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/optimization.html
- AWS，System prompt recommendation：https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/recommendations-system-prompt.html
- APE：https://arxiv.org/abs/2211.01910
- OPRO：https://arxiv.org/abs/2309.03409
- ProTeGi：https://arxiv.org/abs/2305.03495
- DSPy：https://arxiv.org/abs/2310.03714 ；https://github.com/stanfordnlp/dspy
- GEPA：https://arxiv.org/abs/2507.19457 ；https://github.com/gepa-ai/gepa
- BudgetAPO：https://arxiv.org/abs/2610.05671
- EvoSkill：https://arxiv.org/abs/2603.02766 ；https://github.com/sentient-agi/EvoSkill
- ACE：https://arxiv.org/abs/2510.04618
- Self-Refine：https://arxiv.org/abs/2303.17651
- Reflexion：https://arxiv.org/abs/2303.11366
- Voyager：https://arxiv.org/abs/2305.16291
- Agent Workflow Memory：https://arxiv.org/abs/2409.07429
- Darwin Gödel Machine：https://arxiv.org/abs/2505.22954 ；https://sakana.ai/dgm/
- A Survey of Self-Evolving Agents：https://arxiv.org/abs/2507.21046
- Harbor：https://github.com/harbor-framework/harbor ；Adapters：https://www.harborframework.com/docs/datasets/adapters-human
- Jesse Vincent，superpowers / writing-skills：https://github.com/obra/superpowers

## 可借用（间接）

下列不是 skill 迭代专文；用法见第 6 章「可借用的思路」。

- 测试驱动开发的经典表述（Beck）；实践映射见 superpowers writing-skills（上栏）
- 代码坏味道的经典表述（Fowler）；对应到 SKILL.md 见 skill smells 论文（上栏）
- 在线 A/B 与护栏指标的一般实验纪律；产品形态见 AgentCore optimization（上栏）
- 精益改善（到现场、小步、标准化）——改写为「读轨迹、一轮一类失败、移入回归集」

## 未纳入但相关

- 另一篇自我进化综述：https://arxiv.org/abs/2508.07407（与 2507.21046 重叠，正文只详引一篇）
- Anthropic Claude Code best practices：https://www.anthropic.com/engineering/claude-code-best-practices（偏日常用法，迭代专论较少）
