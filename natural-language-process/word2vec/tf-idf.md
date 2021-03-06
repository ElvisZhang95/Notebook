# TF-IDF

tf-idf就是tf和idf的乘积。

$$tf(w)=\frac{w \text{出现在该文档的次数}}{\text{该文档中总的词汇量}}$$ 

$$idf(w)=\log\frac{\text{文档的总个数}}{\text{包含}w\text{的文档的个数}}$$ 

$$tf\text{-}idf(w)=tf(w)\times idf(w)$$ 

**为什么IDF前面要加log?**

1. 其实，信息论的学者们已经发现并指出，其实 IDF 的概念就是一个特定条件下、关键词的概率分布的交叉熵（Kullback-Leibler Divergence\)（详见上一系列）。这样，信息检索相关性的度量，又回到了信息论。
2. 缩小数据的差距 比如说次数 2 Millions跟 1 Millions的次数差距 压缩完比较小

**为什么要取对数？**

让方差恒定，即让波动相对稳定，映射到正态分布。

所以对数变换能够很好地将**随着自变量的增加，因变量的方差也增大的模型**转化为我们熟知的问题。

