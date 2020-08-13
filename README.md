# Machine_Translation_with_LSH
This project conversion of English scentences to most simillar French scentences.

Click [Jupiter Notebook](https://github.com/aprasad13/Machine_Translation_with_LSH/blob/master/Machine%20Translation%20with%20LSH.ipynb) to have a look at the detailed code.

### Following steps were involved:
- Generated <strong>matrix X</strong> and <strong>matrix Y</strong>, where each row in <strong>X</strong> is the word embedding for an english word, and the same row in <strong>Y</strong> is the word embedding for the French version of that English word.
- The strategy was, given an English word embedding, <strong>e</strong>, we can multiply <strong>eR</strong> to get a new word embedding <strong>f</strong>. So we need to find an optimal value for <strong>R</strong> and for that we needed to find a matrix R that minimizes the following equation
\arg \min _{\mathbf{R}}\| \mathbf{X R} - \mathbf{Y}\|_{F}\tag{1}

