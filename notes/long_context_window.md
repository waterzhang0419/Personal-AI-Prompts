# 很长的上下文中如何提升 AI 回答的精确性

Claude 官方发了一篇博客，关于在很长的上下文中（Claude 2 支持 100k 上下文）如何提升 AI 回答的精确性。比如上传一个文档，在基于文档信息的对话中，如何让 AI 的回答更精确，减少错误和歧义。

里面提到了一个很有意思的概念：scratchpad（便签簿/中间结果暂存器）。

按照我的理解，这是长上下文对话中的核心原则。比如在 Claude 官方提供的例子中，应用 scratchpad 技巧可能就是一句话：'Pull 2-3 relevant quotes from the record that pertain to the question and write them inside <scratchpad\></scratchpad\> tags.'

就是让 AI 在回答问题前，先从指定的章节或者文档片段中抽取 2-3 条和问题相关的信息，然后存到 scratchpad 标签里，方便后面引用。

一开始我没有理解。我想，这和我们平常写在 guidelines（操作步骤）中有什么区别呢？

我又仔细读了一下官方提供的例子的 prompt 全文，同时把文章发给了 Claude，看它自己咋说。

哦，原来这么做的目标只有一个：提供针对问题的上下文锚点，缩小问题搜索范围。也就是在 AI 回答问题前，告诉它这个问题相关章节/片段在哪一块，然后归纳出更多的针对问题的相关信息，最后以这些信息为基础来回答问题。

意思就是告诉 AI：你别在整个文档中瞎搜了，文档太长，我怕你把握不住，我告诉你相关信息可能在哪里好了。

这么做，收敛了 AI 的推理过程，从而提升精确性。

scratchpad 和 guidelines （操作步骤）的区别在于，scratchpad 是为了提供更多的问题相关信息，帮助 AI 更好地理解问题；Guidelines 则是侧重于告诉 AI 如何做，比如要避免什么，要包含什么，详细到什么程度，以什么样的格式输出等等。

scratchpad 的技巧让我想到了提示词链（Prompt Chain）。当我们把一个复杂的 prompt 拆分为一个个的子 prompt 的时候，每一个子 prompt 的结果就可以看作是一个 scratchpad。在不超出会话支持的上下文长度的情况下，后面执行的 prompt 都是可以引用已经执行过的 prompt 的结果作为辅助输入信息的。

最简单的例子就是在一个 prompt 中写「把结果命名为 XXX」或者说「把结果写入 <scratchpad\></scratchpad\>标签中」，然后接下来的 prompt 中都可以用 {XXX}/{scratchpad} 这种方式来引用到之前的结果。

总结一下 Claude 这篇博客，就是提供上下文锚点(scratchpad)、样例、操作步骤，来收敛 AI 的推理过程，从而提升回答具体问题的精确性。

[Claude 博客原文](https://www.anthropic.com/index/prompting-long-context)