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

#### 输入

> 题型：\[双边讨论\] 话题：\[Some people believe that it is best to accept a bad situation, such as an unsatisfactory, job or shortage of money. Others argue that it is better to try and improve such situations. Discuss both these views and give your own opinion.\]

#### GPT 3.5 生成的结果

题型：双边讨论
话题：有人认为接受不好的情况，如不满意的工作或缺乏金钱，是最好的选择。而另一些人认为努力改善这些情况更好。讨论这两种观点并给出你自己的意见。
Word count: 281

Introduction:

In life, people often encounter challenging situations such as unsatisfactory jobs or financial shortages. While some individuals argue that it is best to accept these circumstances, others believe that making efforts to improve them is more favorable. This essay will discuss both perspectives and present my own opinion on this matter.

Body Paragraph 1 - Accepting a bad situation:

Those who advocate accepting a bad situation argue that doing so can lead to contentment and peace of mind. Acceptance allows individuals to adapt and find satisfaction within their current circumstances. By cultivating a positive mindset and focusing on the aspects they appreciate, individuals can minimize stress and maintain emotional well-being. Moreover, accepting unfavorable situations can also serve as a motivation for personal growth and resilience.

Body Paragraph 2 - Improving a bad situation:

On the other hand, proponents of improving a bad situation assert that taking action is crucial for personal development and a better future. By recognizing deficiencies and actively seeking solutions, individuals can overcome challenges and create positive change. For example, if someone is dissatisfied with their job, they can acquire new skills, explore alternative career paths, or enhance their qualifications to pursue a more fulfilling profession. Similarly, addressing financial shortages through budgeting, saving, or seeking additional income sources can lead to improved financial stability.

Conclusion:

In conclusion, the debate between accepting a bad situation and striving to improve it revolves around differing perceptions of happiness and personal growth. While accepting unfavorable circumstances can bring contentment and resilience, making efforts to improve these situations offers the possibility of a more fulfilling life and future prospects. Personally, I believe that a balanced approach is essential. Acceptance should be coupled with proactive measures to enhance one's circumstances, allowing individuals to find peace while continually striving for improvement.

Vocabulary:
1. Challenging situations - 具有挑战性的情况
2. Unsatisfactory - 不令人满意的
3. Financial shortages - 资金短缺
4. Contentment - 满足
5. Peace of mind - 心安
6. Adapt - 适应
7. Emotional well-being - 情感健康
8. Resilience - 韧性
9. Proponents - 支持者
10. Personal development - 个人发展

Advanced Phrases:
1. Cultivating a positive mindset - 培养积极的心态
2. Minimize stress - 减少压力
3. Pursue a more fulfilling profession - 追求更有意义的职业
4. Enhance qualifications - 提升资格
5. Balanced approach - 平衡的方法