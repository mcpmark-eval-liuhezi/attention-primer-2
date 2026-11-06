# Attention Primer

A one-place starter reference for the two papers that kicked off the attention era. Every figure below is the headline number reported in the paper's arXiv abstract, taken from live lookups — nowhere padded from memory.

## Attention Is All You Need (arXiv 1706.03762)

The Transformer: a new, simple network architecture based solely on attention mechanisms, dispensing with recurrence and convolutions entirely. On two machine translation tasks these models are superior in quality while being more parallelizable and requiring significantly less time to train.

Headline results from the abstract:

- **28.4 BLEU** on the **WMT 2014 English-to-German** translation task — improving over the existing best results, including ensembles, by over 2 BLEU.
- **41.8 BLEU** on the **WMT 2014 English-to-French** translation task — a new single-model state-of-the-art, after training for 3.5 days on eight GPUs, a small fraction of the training costs of the best models from the literature.
- The abstract also states the Transformer generalizes well, applying it successfully to **English constituency parsing** both with large and limited training data. **No figure** (BLEU or F1) for parsing appears in the abstract itself, so none is claimed here.

## BERT (arXiv 1810.04805)

BERT (Bidirectional Encoder Representations from Transformers) pre-trains deep bidirectional representations from unlabeled text by jointly conditioning on both left and right context in all layers. The pre-trained BERT model can be fine-tuned with just one additional output layer to create state-of-the-art models for a wide range of tasks, such as question answering and language inference, without substantial task-specific architecture modifications.

Headline results from the abstract — **new state-of-the-art results on eleven natural language processing tasks**, including:

- **GLUE score: 80.5%** (7.7% point absolute improvement)
- **MultiNLI accuracy: 86.7%** (4.6% absolute improvement)
- **SQuAD v1.1 question answering Test F1: 93.2** (1.5 point absolute improvement)
- **SQuAD v2.0 Test F1: 83.1** (5.1 point absolute improvement)

### Practical angle: the standard Google base-uncased checkpoint

- **Hugging Face Hub model repo id:** `google-bert/bert-base-uncased`
- **Pipeline task:** `fill-mask`
- **License:** `apache-2.0`
- The model card's citation tag (`arxiv:1810.04805`) confirms the BERT paper's arXiv id.
