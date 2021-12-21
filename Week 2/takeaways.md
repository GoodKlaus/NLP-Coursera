## 1. Perplexity Computation
- N is the length of the test corpus
- V is the number of unique unigrams in the train corpus plus 1

## 2. Language Modeling
- If the test corpus does not have out-of-vocabulary words, smoothing is still needed. Because there may be n-grams that does not exist
- The smaller holdout perplexity is. the better the model
- End-of-sentence tokens are necessary for modelling probabilities of sentences of different lengths
- N-gram language models cannot capture distant contexts

## 3. Sequence Tagging with Probabilistic Models
- At each time step of the Viterbi algorithm, for each state the probability of the best tag sequence ending in this state is computed. This probability is estimated using the similar probabilities from the previous step and the current word.
- Viterbi algorithm can find dynamically the most probable sequence of hidden tags in O(N^2*T)operations. The brute force search of this solution would take an exponential time on T.
