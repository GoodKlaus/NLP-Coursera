# 1. Introduction to Machine Translation
- Evaluation in Machine Translation is hard, mostly because of many variations in transitions.
- Neural Machine Translation is able to produce translations for language pairs that have never been observed in train.
# 2. Encoder-Decoder Architectures
- The three vectors should be passed to a decoder state in a seq2seq with attention model are
  - v(j): the context vector for position j, calculated using attention
  - y(j-1): the previous word in the target sequence
  - s(j-1): the previous decoder state
- If the data has rich morphology, informal spelling and other sources of OOV tokens, the techniques would help are 
  - Sub-word modeling 
  - Byte-pair encoding
  - Copy mechanism
# 3. Summarization and Simplification
- The type of information used for evaluation in machine translation (e.g. in BLEU score)
  - Human reference
  - System output
- The type of information used for evaluation in simplification task (e.g. in SARI score)
  - Human reference
  - System input
  - System output
- The coverage trick helps to avoid repetitions of the input fragments, because we accumulate some scores about what have already been seen and try not to repeat ourselves.
- The point-generator network performs abstractive summarization, it has an ability to generate words that did not occur in the input due to the "generation" part of the network.
