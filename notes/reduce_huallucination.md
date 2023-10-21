# 如何让 AI 尽量少胡说八道？

生成式 AI 胡说八道的能力，我想无人能及。能把羊头挂在狗身上，并一本正经地告诉你这样是合理的。

让它少胡说八道，性价比最高的方式是添加一句神奇咒语：如果你不知道，请说你不知道 (𝗜𝗳 𝘆𝗼𝘂 𝗱𝗼𝗻’𝘁 𝗸𝗻𝗼𝘄, 𝘀𝗮𝘆 𝘆𝗼𝘂 𝗱𝗼𝗻’𝘁 𝗸𝗻𝗼𝘄)。

我在想，有没有进一步能够提升 AI 输出精确性的办法。近期读到了两篇论文：

1. 𝗘𝗻𝗵𝗮𝗻𝗰𝗶𝗻𝗴 𝗭𝗲𝗿𝗼-𝗦𝗵𝗼𝘁 𝗖𝗵𝗮𝗶𝗻-𝗼𝗳-𝗧𝗵𝗼𝘂𝗴𝗵𝘁 𝗥𝗲𝗮𝘀𝗼𝗻𝗶𝗻𝗴 𝗶𝗻 𝗟𝗮𝗿𝗴𝗲 𝗟𝗮𝗻𝗴𝘂𝗮𝗴𝗲 𝗠𝗼𝗱𝗲𝗹𝘀 𝘁𝗵𝗿𝗼𝘂𝗴𝗵 𝗟𝗼𝗴𝗶𝗰

2. 𝗖𝗵𝗮𝗶𝗻-𝗼𝗳-𝗩𝗲𝗿𝗶𝗳𝗶𝗰𝗮𝘁𝗶𝗼𝗻 𝗥𝗲𝗱𝘂𝗰𝗲𝘀 𝗛𝗮𝗹𝗹𝘂𝗰𝗶𝗻𝗮𝘁𝗶𝗼𝗻 𝗶𝗻 𝗟𝗮𝗿𝗴𝗲 𝗟𝗮𝗻𝗴𝘂𝗮𝗴𝗲 𝗠𝗼𝗱𝗲𝗹𝘀

第 1 篇论文的核心思路是 AI 输出结果后，针对它的每一步推理过程，让 AI 从不同的角度重新进行评审，并选出它认为更合理的一方。以此来修正推理步骤中可能存在的错误。再用新的修正过的推理步骤，让 AI 重新推理。

受它的启发，我写了一个简单的左右互博的 prompt 来校验 AI 的回复。就是让 AI 针对输出结果或者输出结果中的某一项，从相反的角度进行分析和批判。详细信息：[模型输出评估助手](../prompt_eval/result_eval.md)

这个方式很难说有特别大的提升。有点像你遇到问题时，多问几个朋友的意见来作为参考。有时候参考给你提供了有价值的信息，有时候聊胜于无。

第 2 篇论文的思路和第 1 篇有点像。其核心思路是从 AI 的回复中抽取关键的事实，然后针对这些事实生成一系列问题让 AI 自己回答，最后再汇总输出最终回复。

虽然 2 篇论文的实验数据显示在特定的任务上，AI 输出的精确性都有显著的提升。但这种验证的方式，prompt 会非常长，如果用中文，可能一不小心就超过了 4K tokens 的上下文。很难在我们日常的 prompt 中使用。

但读完这 2 篇论文，也给了我一些启发。不难看出，这两篇论文的核心思路都是把回复拆分出更小的单元，然后进行校验/修正。或许，目前要尽量让 AI 少胡说八道，我们只有自己先把问题拆成小问题，利用提示词链 (Prompt Chaining) 让 AI 一个个解决，再汇总。

所以，当 AI 开始胡说八道的时候，或许也是在告诉我们：𝗟𝗲𝘁’𝘀 𝘁𝗵𝗶𝗻𝗸 𝘀𝘁𝗲𝗽 𝗯𝘆 𝘀𝘁𝗲𝗽.

## 参考资料

### 论文

* [Enhancing Zero-Shot Chain-of-Thought Reasoning in Large Language Models through Logic](https://arxiv.org/pdf/2309.13339.pdf)

* [Chain-of-Verification Reduces Hallucination in Large Language Models](https://arxiv.org/pdf/2309.11495.pdf)

### 提示词链

* [Split complex tasks into simpler subtasks](https://platform.openai.com/docs/guides/gpt-best-practices/strategy-split-complex-tasks-into-simpler-subtasks)

* [Prompt Chaining](https://docs.anthropic.com/claude/docs/prompt-chaining)