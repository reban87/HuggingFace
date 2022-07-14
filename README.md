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

## 🔖 Terminologies

- **Architecture:** This is the skeleton of the model — the definition of each layer and each operation that happens within the model.
- **Checkpoints:** These are the weights that will be loaded in a given architecture.
- **Model:** This is an umbrella term that isn’t as precise as “architecture” or “checkpoint”: it can mean both. This course will specify architecture or checkpoint when it matters to reduce ambiguity.

💡 **The attention mask** can also be used in the encoder/decoder to prevent the model from paying attention to some special words — for instance, the special **padding word** used to make all the inputs the same length when batching together sentences.

More Details [click here](https://huggingface.co/course/chapter1/4?fw=pt)
