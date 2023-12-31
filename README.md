# Improving prompts, changing lives

生成式 AI 的能力足以振奋人心。不管是翻译、扩写文章、还是做内容总结，都足以作为一个高级助理来提升我们的工作效率。要用好这些基于 LLM（大语言模型） 的 AI 工具，根据自己的需求，写出对应清晰有效的 prompts 很关键。

给 AI 一个 prompt，就像打开微信里的一个小程序一样，用来解决具体的场景下的具体需求，用完即走。

编写 prompt 的过程，就像用程序编写一个小程序一样，程序代码可能是用 Python 或者 Java 等不同的编程语言来编写，而编写 prompt 我们用的是自然语言。二者的编写逻辑是一样的，都是清晰明确地告诉 AI（程序运行环境）需要做什么操作，以什么样的逻辑步骤进行，有什么样的约束条件，交付什么样的结果。

如果交付的结果不符合我们的预期，那么，我们就需要对照 prompt/程序代码来调整、迭代，直到交付结果符合我们的预期。有编程经验的同学一定知道，调整 prompt 的过程其实就是 debugging 代码的过程。

如果你还没有尝试自己编写 prompts 或者不知道如何更好地编写 prompts，我强烈推荐吴恩达老师的这个免费在线课程：[ChatGPT Prompt Engineering for Developers](https://learn.deeplearning.ai/chatgpt-prompt-eng)

虽然课程名称写的是 for Developers，但是没有程序基础，一样可以听懂。在这个课程里，你会学到编写 prompts 的基础原则，并且看到使用这些基础原则编写 prompts，AI 可以呈现出什么样的能力。

吴老师在课程中提到，基本上一次就写出完美符合预期的 prompt 的可能性比较小，都需要经过几次迭代。且很难有万能的 prompts 精准符合你自己的需求。

所以，了解 prompt 的编写原则，然后在自己实际的学习、工作和生活中，编写不同的 prompt 作为不同的助理，来帮助我们更高效地处理事情。

## 结合我自己的需求编写的 prompts（持续更新中...）

### 通用助手

* [Prompt 评估助手](./prompt_eval/eval.md)
* [模型输出评估助手](./prompt_eval/result_eval.md)
* [金字塔原则分析助理](./the_pyramid_principle/pyramid_principle.md)
* [行业关键词归纳学习助理](./keywords/basic_keywords.md)
* [AI 文章翻译助手](./eng/ai_report_trans.md)

### 英语学习助手

* [雅思作文评估助理](./ielts/essay_evaluation.md)
* [雅思任务二（Task 2）作文高分范文助理](./ielts/essay_task2_example.md)
* [雅思口语考试全真模拟助理](./ielts/speaking_process.md)
* [雅思口语考试答案评估助理](./ielts/speaking_evaluation.md)
* [常规英语学习助理](./eng/translation.md)

## 笔记

* [人人都能用的生成式 AI](./notes/genaiforeveryone.md)

* [CoT 技巧总结](./notes/cot.md)

* [如何让 AI 尽量少胡说八道？](./notes/reduce_huallucination.md)

* [如何通过和 AI 对话优化提示词 (prompt)？](./notes/optimize_prompts.md)

* [写 prompt 是一件性价比很高的事情](./notes/write_more_prompts.md)

* [使用老顽童周伯通的左右互搏之术，让 AI 自己校验答案](./notes/opposite_reviews.md)

* [把人类认知过程中的类比推理用到写提示词中（Analogical Prompting）](./notes/analogical_prompting.md)

* [长上下文中如何提升 AI 回答的精确性](./notes/long_context_window.md)

## 读过的有启发的资料

### 生成式 AI 基础知识

* [Generative AI for Everyone by Andrew Ng](https://www.coursera.org/learn/generative-ai-for-everyone)

* [Generative AI for Beginners by Microsoft](https://microsoft.github.io/generative-ai-for-beginners/#/)

### 提示词技巧

* [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)

* [GPT best practices by OpenAI](https://platform.openai.com/docs/guides/gpt-best-practices)

* [Claude Prompt Design](https://docs.anthropic.com/claude/docs/introduction-to-prompt-design)

* [Prompt Engineering Guide](https://www.promptingguide.ai/)

* [Prompt engineering for Claude's long context window](https://www.anthropic.com/index/prompting-long-context)

### 提示词相关论文

* [Large Language Models Understand and Can Be Enhanced by Emotional Stimuli](https://arxiv.org/pdf/2307.11760.pdf)

* [Large Language Models as Analogical Reasoners](https://arxiv.org/pdf/2310.01714.pdf)

* [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/pdf/2205.11916.pdf)

* [Least-to-Most prompting enables complex reasoning in large language](https://arxiv.org/pdf/2205.10625.pdf)

* [Take a Step Back: Evoking Reasoning via Abstraction in Large Language Models](https://arxiv.org/pdf/2310.06117.pdf)

* [Guiding Large Language Models via Directional Stimulus Prompting](https://arxiv.org/pdf/2302.11520.pdf)

* [Generated Knowledge Prompting for Commonsense Reasoning](https://arxiv.org/pdf/2110.08387.pdf)

* [Enhancing Chain-of-Thoughts Prompting with Iterative Bootstrapping in Large Language Models](https://arxiv.org/pdf/2304.11657.pdf)

* [Enhancing Zero-Shot Chain-of-Thought Reasoning in Large Language Models through Logic](https://arxiv.org/pdf/2309.13339.pdf)

* [Chain-of-Verification Reduces Hallucination in Large Language Models](https://arxiv.org/pdf/2309.11495.pdf)

* [Promptbreeder: Self-Referential Self-Improvement Via Prompt Evolution](https://arxiv.org/pdf/2309.16797.pdf)

* [Automatic Chain of Thought prompting in Large Language Models](https://arxiv.org/pdf/2210.03493.pdf)

* [Meta-CoT: Generalizable Chain-of-Thought Prompting in Mixed-task Scenarios with Large Language Models](https://arxiv.org/pdf/2310.06692.pdf)