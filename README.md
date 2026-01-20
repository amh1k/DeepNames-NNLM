# makemore

**makemore** is an autoregressive character-level language model. It outputs more of things that are like the things you give it.

## Dataset

The dataset used in this project is `names.txt`, which contains approximately 32k names. The models are trained to generate new name-like sequences based on this dataset.

## Models

The repository contains a sequence of notebooks implementing increasingly complex language models:

- **`1-bigramModel.ipynb`**: Implements a Bigram Language Model. It explores both a count-based approach and a simple neural network approach to predict the next character based on the previous one.
- **`2-mlp.ipynb`**: Implements a Multi-layer Perceptron (MLP) character-level language model, following the approach described in [Bengio et al. 2003](https://www.jmlr.org/papers/volume3/bengio03a/bengio03a.pdf).
- **`3-mp2.ipynb`**: Builds upon the MLP model, focusing on initialization techniques, batch normalization, and using diagnostics to improve model training and performance.
- **`4-backprop_scratch.ipynb`**: deeply dives into the backpropagation algorithm. It involves manually implementing backpropagation for the neural network, providing a low-level understanding of gradient calculation.
- **`5-wavenet.ipynb`**: Implements a Wavenet-like architecture. It moves away from simple MLPs to use hierarchical or dilated convolutions (or tree-like structures) to capture longer-range dependencies more efficiently.

## Usage

To explore the models, open the notebooks in a Jupyter environment:

```bash
jupyter notebook
```

You can then run the cells in each notebook to train the models and generate new names.
