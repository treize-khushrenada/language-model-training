***language model training***

the obejective of this repo is to use transformer and tokenizer for language model training.

1. setting up

the language data we use is esperanto, which is invented as an artificial language in the last centry, that claimed to be merging characteristics of different languages from the world, and 'getting the best of (so many) worlds'.

to get the training data, use the following command in your terminal:

```
wget -c https://cdn-datasets.huggingface.co/EsperBERTo/data/oscar.eo.txt

```
after that we can prepare packages we need:
```
pip install git+https://github.com/huggingface/transformers
```
to show the current versions of transformers and tokenizers:
```
pip list | grep -E 'transformers|tokenizers'
```
2. after training the tokenizer, save the model to directory
```
mkdir esperanto-bert
```
3. training a new language model. First make sure pytorch is install:
```
pip install torch torchvision
```