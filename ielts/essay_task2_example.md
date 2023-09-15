# 使用说明

这是让 AI 根据题型和指定话题，按照雅思任务二作文的要求，生成高分范文的 prompt.

雅思任务二有明确的题型，包括利弊分析、是否同意、分析原因后果（说明文）、双边讨论。每种题型可以拆分为标准的结构。如果有人能根据指定题型和话题，迅速给你各种高分范文参考，那么我相信能极大地提升任务二的写作能力(反正我正在这么做)。

点击打开或下载 [prompt 全文](./prompt_essay_task2_example.txt)，将内容复制到你在使用的 AI 工具中即可。

另外，还可以配合这个 [雅思作文评估助手](./essay_evaluation.md)，给你的作文进行打分和提出修改意见。

## 功能

根据指定的题型和话题，按照雅思 9 分的标准生成范文。并根据需要，可以列出指定题型里的高频词/词组列表。

### 全部指令

建议以这种格式发送消息：

> 题型：\[说明文\] 话题：\[\]

例子：

你甚至可以直接用雅思真题的话题，比如这个雅思 16 Test 1 的话题：

> 题型：\[说明文\] 话题：\[In some countries, more and more people are becoming interested in finding out about the history of the house or building they live in.\]

### 其他说明

使用 **Claude 2**，**GPT 3.5**  皆可。我使用了 GPT 3.5 生成的范文放到了 Claude 2 里， 使用这个 [雅思作文评估助手](./essay_evaluation.md) 打分，评估为 7 分以上的水平。达到使用预期效果。

**Q: 如果有时候 AI 不识别指令或者出现其他的问题怎么办？**

```
A: 可能是聊天内容累计过多， AI 丢失了部分上下文内容。解决方法就是新开启一个会话或者清空当前会话的上下文，然后重新发送 prompt。
```

### 示例

输入：
> 题型：\[说明文\] 话题：\[In some countries, more and more people are becoming interested in finding out about the history of the house or building they live in.\]

GPT 3.5 生成的结果：

题目：Analyzing the Reasons and Consequences of People's Increasing Interest in the History of Their Houses or Buildings

范文：

Introduction:
In recent years, there has been a growing trend in many countries where individuals are showing a keen interest in exploring the history behind the houses or buildings they reside in. This essay aims to delve into the reasons behind this phenomenon and discuss its potential consequences.

Body:

Reasons for the increasing interest in house or building history:

One of the primary reasons for the surge in curiosity regarding the history of houses or buildings is the desire to establish a sense of connection with the past. By unraveling the historical background of their living spaces, people can gain a deeper appreciation for the heritage and cultural significance associated with their homes. This connection to history fosters a sense of identity and belonging, allowing individuals to feel rooted in their community.

Furthermore, the accessibility of information plays a crucial role in driving this interest. With the advent of technology and the internet, historical records and archives have become more readily available. People can now easily access documents, photographs, and accounts that shed light on the origins and development of their houses or buildings. This easy access to information fuels curiosity and encourages individuals to engage in historical research.

Consequences of the increasing interest in house or building history:

The consequences of this growing interest in house or building history are manifold. Firstly, it contributes to the preservation and conservation of architectural heritage. When people become aware of the historical value of their houses or buildings, they are more likely to take measures to protect and maintain them. This preservation effort helps safeguard architectural treasures for future generations and prevents the loss of valuable cultural heritage.

Moreover, the exploration of house or building history fosters a sense of community and shared experiences among residents. It provides an opportunity for neighbors to come together and exchange knowledge, stories, and anecdotes about their houses or buildings. This social interaction strengthens community bonds and creates a sense of camaraderie.

Additionally, the interest in house or building history can have economic implications. It can stimulate heritage tourism, attracting visitors who are intrigued by the historical significance of certain houses or buildings. This influx of tourists can lead to the growth of local businesses, such as accommodations, restaurants, and souvenir shops, thereby boosting the local economy.

Conclusion:

In conclusion, the increasing interest in exploring the history of houses or buildings stems from the desire for connection, access to information, and the preservation of architectural heritage. This trend not only strengthens individuals' ties to their homes but also has positive consequences for the preservation of cultural heritage, community cohesion, and local economies. Encouraging this curiosity and supporting initiatives that promote the study of house or building history can lead to a more informed and culturally enriched society.

如果你需要列出与"分析原因后果（说明文）"题型相关的雅思高频词汇和词组，请告诉我。

以下是与"分析原因后果（说明文）"题型相关的一些雅思高频词汇和词组：

1. Reasons:

- Factors
- Causes
- Motives
- Influences
- Triggers
- Drivers
- Contributing factors
- Underlying reasons

2. Consequences:

- Effects
- Impacts
- Outcomes
- Results
- Ramifications
- Repercussions
- Significance
- Long-term effects

3. Expressing cause:

- Due to
- Because of
- Owing to
- As a result of
- The main reason for
- One factor that contributes to

4. Expressing consequence:

- Therefore
- Thus
- Consequently
- As a result
- This leads to
- It results in
- The outcome is

5. Connecting ideas:

- Moreover
- Furthermore
- Additionally
- In addition
- On the other hand
- Conversely
- However
- Nevertheless