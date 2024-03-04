# Math questiong answering with TP Transoformer
This repository contains the implementation of the TP-Transformer, an enhanced version of the traditional Transformer model,
designed to explicitly encode relational structures using Tensor-Product Representations (TPR). Introduced in ["Enhancing the Transformer With Explicit Relational Encoding for Math Problem Solving"](https://arxiv.org/abs/1910.06611) by Imanol Schlag et al., this model sets a new benchmark on the Mathematics Dataset by incorporating a novel TP-Attention mechanism. This mechanism allows for a more nuanced representation of relationships between different components of the input data, significantly improving performance on complex math problem-solving tasks. Our implementation, available on GitHub, offers a comprehensive toolkit for researchers and practitioners interested in exploring the capabilities of TP-Transformers in various domains.

## Algorithm Overview
The TP-Transformer enhances the Transformer architecture by incorporating Tensor-Product Representations (TPR) to explicitly encode structural relationships within data. This approach allows the model to capture and utilize complex relational information more effectively than traditional methods.

### Core Components:
- **TP-Multi-Head Attention (TPMHA)**: A novel attention mechanism that extends the standard Multi-Head Attention by integrating tensor-product operations. This enables the model to represent relational structures more explicitly, facilitating better understanding and manipulation of data elements in tasks such as math problem solving.
- **Encoder and Decoder Structure**: The TP-Transformer follows a structure similar to the original Transformer, with layers of TP-Multi-Head Attention and feed-forward networks. The encoder processes the input sequence into a high-dimensional space, capturing the inherent relationships, while the decoder generates the output sequence based on the encoder's representations.

- **Residual Connections and Layer Normalization**: Each sub-layer in both the encoder and decoder is followed by a residual connection and layer normalization, preserving information flow and stabilizing the learning process.

<img width="849" alt="Screenshot 2024-03-04 at 09 02 42" src="https://github.com/LinYyou/Math-question-answering-with-TP-Transformer/assets/100883791/ff656c3e-6fef-440c-b9f5-41cd715f9274">


## Features
- PyTorch;
- Auto-Encoder Transformer Architecture;
- Automated Math Problem Solving.
  
## Mathematics Dataset
The TP-Transformer is trained and evaluated on the [Mathematics Dataset](https://openreview.net/forum?id=H1gR5iR5FX) by Saxton et al. (2019), designed to test neural networks' formal reasoning abilities. This dataset features a wide range of math problems, from basic arithmetic to advanced calculus, presented in a sequence-to-sequence format. It is notable for its procedural generation, offering over 120 million unique training samples across 56 modules, making it a rigorous benchmark for assessing the model's problem-solving capabilities.

For a quick start or for those with limited resources, a smaller subset of the Mathematics Dataset is available for download. 
To download, use the following command:
```
!git clone https://huggingface.co/datasets/LinYyou/TP_Transformers_data
```
## Model Evaluation
Evaluate the TP-Transformer's performance using our pre-trained model checkpoint. This checkpoint represents 20 hours of training on a Tesla V100 GPU via Google Colab, utilizing 12 million training pairs for optimal accuracy and efficiency. Follow the steps below to download the checkpoint and initiate model testing:
```
!git clone https://huggingface.co/datasets/LinYyou/TP_Transformers_data/blob/main/TP_Transfomer.ckpt
```
## References
- [Enhancing the Transformer with Explicit Relational Encoding for Math Problem Solving](https://arxiv.org/abs/1910.06611)
- [Mathematics Dataset](https://openreview.net/forum?id=H1gR5iR5FX)
- [Attention Is All You Need](https://arxiv.org/abs/1706.03762)

