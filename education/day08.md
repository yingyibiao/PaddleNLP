# Day08 机器翻译作业辅导

本教程旨在辅导同学如何完成 AI Studio课程课后作业——[必修 | 文本翻译技术及应用
](https://aistudio.baidu.com/aistudio/education/objective/25710)。

## 1. 机器翻译任务与以下哪个NLP任务最相似？

    A. 文本匹配
    B. 情感分析
    C. 实体识别
    D. 生成式对话

    正确答案：D

    解析：机器翻译模型是序列到序列的生成任务，输入原文句子，输出译文句子。

        A：文本匹配是语义相似度任务。输入两个句子，输出相似度得分。
        B：情感分析一般建模成分类任务，输入一个句子序列，输出是类别标签
        C：实体识别一般建模成序列标注任务，输入是序列，输出是序列的标签，标签的个数一般与输入的序列相同。
        D：生成式对话是生成任务，输入前文句子，输出一个句子作为回应

## 2. 用BLEU评价足以反映机器翻译模型的优劣。

    A. 是
    B. 否

    正确答案：B

    解析：BLEU计算候选译文和参考答案的ngram准确度，并不能充分提现语义信息

## 3. 统计机器翻译模型一般由哪两个部分组成？

    A. 编码器+解码器
    B. 语料库+检索算法
    C. 翻译模型+语言模型
    D. 词典+规则

    正确答案：C

    解析：统计机器翻译由翻译模型和语言模型组成，翻译模型用来计算原文和译文的翻译概率；语言模型用来提现译文的流畅度

## 4. 神经网络机器翻译模型一般由哪两个部分组成？

    A. 编码器+解码器
    B. 语料库+检索算法
    C. 翻译模型+语言模型
    D. 词典+规则

    正确答案：A

    解析：神经网络机器翻译模型通常由编码器+解码器组成，也是大部分生成式任务的神经网络结构

## 5. 对于句子分类任务，我们可以把输入的句子作为源语言句子，“类别”作为目标语言句子，这样就可以当成神经网络翻译任务来解。

    A. 是
    B. 否

    正确答案：A

    解析：神经网络翻译是一个文本到文本的生成任务，其它任务只要可以建模成文本-文本这种结构，都可以在生成任务的框架下解决
