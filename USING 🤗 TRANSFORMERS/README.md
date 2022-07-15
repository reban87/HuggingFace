## Behind Pipeline
**Pipeline** groups together 3 steps: preprocessing, passing the inputs and post processing
![image](https://user-images.githubusercontent.com/62704162/179155373-f6612bbf-7af4-4dc7-b191-845f1193899b.png)

### Preprocessing with a Tokenizer
Like other neural networks, Transformer models can’t process raw text directly, so the first step of our pipeline is to convert the text inputs into numbers that the model can make sense of. To do this we use a tokenizer, which will be responsible for:

- Splitting the input into words, subwords, or symbols (like punctuation) that are called tokens
- Mapping each token to an integer
- Adding additional inputs that may be useful to the model

### High Dimensional Vector
The vector output by the Transformer module is usually large. It generally has three dimensions:

- **Batch size:** The number of sequences processed at a time (2 in our example).
- **Sequence length:** The length of the numerical representation of the sequence (16 in our example).
- **Hidden size:** The vector dimension of each model input.


