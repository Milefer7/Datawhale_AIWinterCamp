##  前世今生

> 搞明白为什么诞生这个技术，不深究原理

* 早期 `NLP` 方法

  * 人工设计特征与规则
  * 单词固定，处理上下文能力差

* `Transformer` 模型诞生

  > 2017年

  * 现代 `NLP` 的核心架构

* `BERT` 

  * 它是 Transformer 的一种扩展，并引入了 **预训练和微调** 的理念
  * 预训练模型越来越大，全量调参对硬件的要求越来越高
    * 新技术 —— 高效参数微调

* 高效参数微调

  * `LoRa` 等技术

* `LLM` 压缩

  > 模型越来越大，为了降低成本，需要有压缩技术

  * 模型剪枝

---

* `LLM` 数据工程

  ![llm-pretrain-pipeline](https://my-note-drawing-bed-1322822796.cos.ap-shanghai.myqcloud.com/picture/llm-pretrain-pipeline-v2.png)

  * 如何做