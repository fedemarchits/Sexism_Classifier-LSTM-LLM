# LSTM, RoBERTa, LLMs for Sexism Classification of Tweets
The project consists of classifying tweets as sexist or not. To determine which architecture performs best for this task, the project has been split into two parts, described as follows.

## LSTM and RoBERTa Comparison
Data cleaning and preprocessing techniques datas have been prepared. The used dataset is a subset of [EXIST 2023](https://clef2023.clef-initiative.eu/index.php?page=Pages/labs.html#EXIST). Dataset was then fed into [GloVe](https://nlp.stanford.edu/projects/glove/) pre-trained embeddings.

Using Keras, two different LSTMs were trained and a pre-trained Transformer model [RoBERTa](https://huggingface.co/docs/transformers/model_doc/roberta) was fine-tuned for sexism speech detection. The performances of all the models have then been compared.

See the [Report](LSTM_Transformer_Comparison/Report.pdf) for more details.

## LLMs prompting
[Llama-3.1-8B-Instruct ](https://huggingface.co/meta-llama/Llama-3.1-8B-Instruct) and [Mistral-7B-Instruct-v0.3](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.3) pre-trained LLMs were loaded in their quantized (4-bit) variants and then both zero-shot and few-shot were explored using templates.

See the [Report](LLM/Report.pdf) for more details.
