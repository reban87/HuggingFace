# HuggingFace


It contains a list of projects while following **HuggingFace** documentation and book.

# General Architecture of Transformer Model

## 🤔 Introduction
The model is primarily composed of two blocks:

- **Encoder (left):** The encoder receives an input and builds a representation of it (its features). This means that the model is optimized to acquire understanding from the input.

- **Decoder (right):** The decoder uses the encoder’s representation (features) along with other inputs to generate a target sequence. This means that the model is optimized for generating outputs.

![image](https://user-images.githubusercontent.com/62704162/178923569-71c1f4b2-b659-4bf5-bb7a-7350e2bf016f.png)


Each of these parts can be used independently, depending on the task:

- **Encoder-only models:** Good for tasks that require understanding of the input, such as sentence classification and named entity recognition.

- **Decoder-only models:** Good for generative tasks such as text generation.

- **Encoder-decoder models or sequence-to-sequence models:** Good for generative tasks that require an input, such as translation or summarization.

More Details [click here](https://huggingface.co/course/chapter1/4?fw=pt)
