# Text-Generation-with-RNNs

## Introduction
Welcome to my RNN practice repository. This repository was created as a part of my learning journey to explore and practice Recurrent Neural Networks (RNNs). The primary focus is on experimenting with various RNN architectures, including LSTMs, and understanding their applications in text generation.

## Purpose
The main goals of this repository are to:
- Practice and implement RNN models.
- Understand the intricacies of sequence models.
- Experiment with different model architectures and hyperparameters.
- Explore the limitations and constraints of training RNNs on limited computational resources.

## Technical Summary

### Models Implemented
- **Basic RNNs**: Implemented simple RNN layers to understand the basic concepts of sequence modeling.
- **Long Short-Term Memory (LSTM) Networks**: Used LSTM layers for better handling of long-range dependencies.
- **Bidirectional LSTMs**: Implemented bidirectional LSTMs to capture context from both past and future sequences.

### Data Preparation
1. **Tokenization**: Used Keras' `Tokenizer` to convert text into sequences of integers.
2. **Padding Sequences**: Applied padding to ensure uniform input length using `pad_sequences`.
3. **Categorical Labels**: Converted labels to categorical format using `to_categorical`.

### Training Strategy
Due to limited computational resources, several strategies were employed to optimize training:
- **Model Simplification**: Reduced the complexity of models by decreasing the number of layers and units.
- **Max Sequence Length Reduction**: Shortened the sequence length to fit memory constraints.
- **Batch Size Adjustment**: Used smaller batch sizes to manage memory usage.
- **Resource Management**: Leveraged TPU and GPU accelerators for efficient training.
- **Gradient Accumulation**: Experimented with gradient accumulation to simulate larger batch sizes.

### Performance and Evaluation
- **Accuracy and Loss Metrics**: Tracked during training to monitor performance.
- **Text Generation Examples**: Provided to demonstrate the models' ability to generate coherent text sequences.

### Results
- The repository includes trained models, training scripts, and example outputs.
- Despite the simplifications, the models effectively learned to generate text based on the training data.

## Usage

### Prerequisites
- Ensure you have the necessary dependencies installed. The primary dependencies are TensorFlow and Keras.
- Use the following command to install dependencies:
  ```sh
  pip install tensorflow keras

### Challenges and Solutions
- **Limited** Computational Resources
- **Problem**: High memory consumption during training.
- **Solution**: Simplified models, reduced sequence length, and used smaller batch sizes.
### Resource Management
- **Problem**: Efficient use of available **TPU/GPU** resources.
- **Solution**: Employed TPU strategy for distributed training and adjusted training parameters dynamically.
### Conclusion
This repository serves as a practical guide and a hands-on experience in building and training **RNN** models. It highlights the challenges of working with limited resources and provides solutions to manage these constraints effectively.