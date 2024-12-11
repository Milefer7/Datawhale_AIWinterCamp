# Datawhale AI 冬令营

## task 1.1

> **动手学定制你的专属大模型**

### 定制大模型

* 主要的技术

  > 只列举两个

  * 微调（Fine-tuning）：

    - 对预训练模型进行再训练，让其适应特定任务。

  * 提示工程（Prompt Engineering）：

    > 像前段时间很火的 [提示工程：Thinking-Claude](https://github.com/richards199999/Thinking-Claude)

    * 不改变模型参数，通过设计高效的提示优化模型输出。

### 微调技术

> 这次定制 llm 实践用到的是微调技术

* 微调数据集

  > 格式要求：`Alpace` 格式

  * 什么是微调

    * 是一种技术，用特定的小规模数据集再次训练，使得模型适应特定任务。

  * 什么是 Alpaca

    * Alpaca 是 **一个微调后的模型**。模型包含数据集。
    * 格式为 `json`，每条记录对应着一条训练样本

  * 为什么要用到 Alpaca 格式微调

    * 高效，通用，灵活

      * 高效

          > “指令-输入-输出”三元组，这种格式的数据训练可以显著提高模型的指令遵循能力

          * 基本构成格式
          
            * **instruction**：
              - 用户希望模型执行的指令。
            * **input**（可为空）：
              - 提供给指令的上下文或输入。
              - 若不需要上下文，则为空字符串。
            * **output**：
              - 指令的目标响应或结果。

          * `eg.`（指令监督微调样例数据集）
          
            ```json
            {
                    "instruction": "这位是？",
                    "input": "",
                    "output": "这位是眉庄姐姐。"
            },
            ```
    
      * 通用
        * 训练产出的数据集可以跨领域使用。
      * 灵活
        * 修改输入指令就可以改变输出，而不用修改模型本身。
    
    * 如何微调
    
      * 本次使用`讯飞星辰Maas`平台。

### 效果记录

![image-20241211075936400](https://my-note-drawing-bed-1322822796.cos.ap-shanghai.myqcloud.com/picture/huanhuan_talk.png)

### 参考资料

* [Datawhale-AI活动-1.1 零基础定制你的专属大模型](https://www.datawhale.cn/activity/110/21/76?rankingPage=1)
* [数据处理 - LLaMA Factory](https://llamafactory.readthedocs.io/zh-cn/latest/getting_started/data_preparation.html#alpaca)

