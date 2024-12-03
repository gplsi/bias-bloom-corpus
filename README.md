# BiasBloom Corpus

[![DOI](https://zenodo.org/badge/894534760.svg)](https://doi.org/10.5281/zenodo.14264607)

The **BiasBloom Corpus** is a structured collection of prompts and outputs from various generative language models, curated to study bias and performance across different configurations. The corpus is divided into two main sections based on prompt formatting:

1. **Leading Prompts**: A leading prompt is one designed in a way that suggests or implies a specific answer or direction. That is, it can guide a model towards a particular conclusion, in this case towards gender biases.
2. **Non-Leading Prompts**: A non-leading prompt is more neutral and open-ended, allowing the model to generate a wider range of responses without biasing towards a particular viewpoint. It encourages exploration of various aspects of a topic without suggesting a preferred answer.

Each section includes data generated by the following models:

- Gemini 1.5
- GPT-3.5
- GPT-4o
- LLaMA 3
- Mistral 8x7b

### Corpus Structure

The data is stored in `.csv` files within the `data/` directory, structured as follows:

| **Model**     | **Leading Prompts**          | **Non-Leading Prompts**         |
|---------------|-----------------------------------|-------------------------------------|
| Gemini 1.5    | [`data/Leading/Gemini_1.5.csv`](./data/Leading/Gemini_1.5.csv)     | [`data/Non_leading/Gemini_1.5.csv`](./data/Non_leading/Gemini_1.5.csv)    |
| GPT-3.5       | [`data/Leading/GPT3.5.csv`](./data/Leading/GPT3.5.csv)         | [`data/Non_leading/GPT3.5.csv`](./data/Non_leading/GPT3.5.csv)        |
| GPT-4o        | [`data/Leading/GPT4o.csv`](./data/Leading/GPT4o.csv)          | [`data/Non_leading/GPT4o.csv`](./data/Non_leading/GPT4o.csv)         |
| LLaMA 3       | [`data/Leading/Llama_3.csv`](./data/Leading/Llama_3.csv)        | [`data/Non_leading/Llama_3.csv`](./data/Non_leading/Llama_3.csv)       |
| Mistral 8x7b  | [`data/Leading/Mistral8x7b.csv`](./data/Leading/Mistral8x7b.csv)    | [`data/Non_leading/Mistral8x7b.csv`](./data/Non_leading/Mistral8x7b.csv)   |

Each `.csv` file contains:
- **Prompt**: The input text provided to the model.
- **Output**: The corresponding text generated by the model.

### Applications

The BiasBloom Corpus can be used for:
- Analyzing performance differences between leading and non-leading prompts.
- Studying potential biases exhibited by generative models.
- Evaluating model behavior across diverse generative AI architectures.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">BiasBloom Corpus</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.<br />
