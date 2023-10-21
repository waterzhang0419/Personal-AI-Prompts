# 如何通过和 AI 对话优化提示词 (prompt)？

生成式 AI 神奇的地方在于用不同的语言结构描述相同的任务/目标，会得到不同的甚至可能差异巨大的结果。更进一步，相同的提示词组合，不同的顺序都可能影响 AI 的输出结果。

只要经常写提示词 (prompt)，并且笃定生成式 AI 能极大地提升工作和学习效率，自然就会想着怎么不断地优化提示词。我之前的初步想法是让 AI 自己评估提示词的逻辑和结果的有效性：[Prompt 评估助手](../prompt_eval/eval.md)

又读到了一篇 Google DeepMind 出品的论文：𝗣𝗿𝗼𝗺𝗽𝘁𝗯𝗿𝗲𝗲𝗱𝗲𝗿: 𝗦𝗲𝗹𝗳-𝗥𝗲𝗳𝗲𝗿𝗲𝗻𝘁𝗶𝗮𝗹 𝗦𝗲𝗹𝗳-𝗜𝗺𝗽𝗿𝗼𝘃𝗲𝗺𝗲𝗻𝘁 𝗩𝗶𝗮 𝗣𝗿𝗼𝗺𝗽𝘁 𝗘𝘃𝗼𝗹𝘂𝘁𝗶𝗼𝗻

这篇论文的核心思想是用不同的思维角度 (𝗧𝗵𝗶𝗻𝗸𝗶𝗻𝗴 𝘀𝘁𝘆𝗹𝗲𝘀) 让 AI 重新复述和拆解问题，然后尝试用各种不同的表达方式 (𝗠𝘂𝘁𝗮𝘁𝗼𝗿 𝗣𝗿𝗼𝗺𝗽𝘁𝘀) 让 AI 自己对原提示词进行修改。

PromptBreeder 这个名字也很有意思，我理解为提示词助产士。先哲苏格拉底有一个著名的方法，叫“精神助产术”或者“知识启发术”。通过提问和对话来引导他人思考和发现自己内在的真理和智慧。

举个简单的例子。假设有个人认为自己是一个非常聪明的人，并且总是对别人的观点抱有怀疑和否定的态度。苏格拉底可能会问这个人一些问题，比如：“你是如何定义聪明的？”、“你认为怀疑别人的观点是否总是正确的？”、“你是否有时候也会犯错误？”等等。

论文中的核心思路和苏格拉底的“精神助产术”很相似。首先是通过提问来拆解和优化问题本身，比如：

How can I simplify the problem so that it is easier to solve?（我该如何简化这个问题，使其更容易解决?）

What are the key assumptions underlying this problem?（这个问题背后的关键假设是什么?）

What are the potential risks and drawbacks of each solution?（每个解决方案的潜在风险和缺点是什么?）

类似的思维角度 (𝗧𝗵𝗶𝗻𝗸𝗶𝗻𝗴 𝘀𝘁𝘆𝗹𝗲𝘀) 论文中还有 30 多条例子，我把中英对照版放到了末尾。

通过这样的提问，一是可以帮助我们自己理解问题，二是我们让 AI 更好地理解问题。根据这样的多轮问答，我们就可以对问题本身做一个优化，让 AI 能更好理解问题。

接下来，就是利用不同的表达方式 (𝗠𝘂𝘁𝗮𝘁𝗼𝗿 𝗣𝗿𝗼𝗺𝗽𝘁𝘀) 让 AI 对我们的原始提示词进行修改，是那种像基因突变一样的修改。比如：

Modify the following instruction creatively, giving some advice on how to solve it: （修改以下指令，创造性地提供一些如何解决它的建议:）

Just change this instruction to make it more fun, think WELL outside the box: （改变这个指令，使它更有趣，思维更加开放:）

Modify this instruction in a way that no self-respecting LLM would! （以一种常规的谨慎的LLM绝不会使用的方式修改这个指令！）

类似的表达方式 (𝗠𝘂𝘁𝗮𝘁𝗼𝗿 𝗣𝗿𝗼𝗺𝗽𝘁𝘀) 论文中还有 50 多条例子，同样，我把中英对照版放到了末尾。

在指导 AI 推理的时候，我常用的是“Let's think step by step.” 论文中汇总了其他几种不同的要求 AI 推理的方式，比如同样知名的“Take a deep breath and work on this problem step-by-step.” 还有其他几条，一并放到末尾的参考资料里了。

写提示词 (prompt) 除了各种拿来即用的技巧/招式之外，其内功心法还是“对话的艺术”。

大家可以用这些不同的表达方式和思维角度在和 AI 的对话中多玩一下，相信会很好玩。

参考资料：

* [Promptbreeder: Self-Referential Self-Improvement Via Prompt Evolution](https://arxiv.org/pdf/2309.16797.pdf)

* [Zero-shot-CoT 触发词](./zero_shot_cot_triggers.md)

* [思维角度 Thinking styles](./thinking_styles.md)

* [不同的表达方式 Mutator Prompts](./mutator_prompts.md)