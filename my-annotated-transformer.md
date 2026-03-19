# my-annotated-transformer

这是一个基于 "The Annotated Transformer" 思路实现的简化版 Transformer 核心模块 PyTorch 复现项目。旨在帮助深入理解 Transformer 架构中的关键组件，如多头自注意力机制 (Multi-Head Self-Attention) 和前馈网络 (Feed-Forward Network)。

## 项目结构

- `transformer_modules.py`: 包含了 Transformer 核心模块的 PyTorch 实现，包括：
    - `MultiHeadAttention` (多头自注意力机制)
    - `PositionwiseFeedForward` (前馈网络)
    - `AddAndNorm` (残差连接与层归一化)
    - `PositionalEncoding` (位置编码)
    - `EncoderLayer` (编码器层)
    - `DecoderLayer` (解码器层)
    - `Embeddings` (词嵌入层)
    - `Generator` (输出生成器)
    - `Transformer` (完整的简化版 Transformer 模型)

## 如何运行代码

1.  **克隆仓库**：
    ```bash
    git clone https://github.com/dream001871-cell/my-annotated-transformer.git
    cd my-annotated-transformer
    ```


2.  **安装依赖**：
    确保你已经安装了 PyTorch。如果尚未安装，请参考 PyTorch 官方文档进行安装：[https://pytorch.org/get-started/locally/](https://pytorch.org/get-started/locally/)

3.  **运行示例**：
    `transformer_modules.py` 文件中包含了一个 `if __name__ == '__main__':` 块，用于演示如何实例化和测试 Transformer 模型。你可以直接运行该文件来查看模型的输出形状和基本功能验证。
    ```bash
    python transformer_modules.py
    ```

    运行结果应类似：
    ```
    Transformer 模型输出形状: torch.Size([2, 8, 1000])
    模型测试通过！
    ```


