# 1. Notes
- Softmax function to calcualte probability can be slow on large vocabularies.
- Representations of word or character n-grams may improve the quality of the model.
- For word similarity tasks, count-based methods perform on par with predictive methods.
# 2. For Singular Value Decomposition
- SVD is not unique (for example, the zero matrix can be decomposed in infinitely many ways).
- Any rectangular matrix with real entries has a singular value decomposition.
- Squares of singular values of a matrix X are eigenvalues of XTX or XXT.
- Truncated SD is the best rank $k$ approximation of the original matrix in terms of Forbenius norm.
# 3. Word embeddings are usually evaluated 
- By Spearman's correlation (or similar rank correlation measure) with human judgements on word similarity task.
- By the accuracy of analogy prediction (using some pre-defined dataset of 4-word analogies).
- By the interpretability of the components of the vectors.
