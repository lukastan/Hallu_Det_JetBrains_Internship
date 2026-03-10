# Hallu_Det_JetBrains_Internship
<br>
This repository is a showcase of a solution to a task for "Hallucination Detection" internship at JetBrains.
<br>
<br>
It contains a Word2Vec model that uses negative sampling with batches on a subsampled dataset.
<br>
<h3>Dataset</h3>
<p>Dataset <a href="https://www.kaggle.com/datasets/yorkyong/text8-zip">text8</a> is in the project. It is used without changes.</p>
<h3>Negative sampling</h3>
<p>Negative sampling is applied in the model. Generally 5 random words are taken for each center word.</p>
<h3>Batches</h3>
<p>Batches of center words and their negative samples are sent instead of one by one. This improves performance.</p>
<h3>Subsampling</h3>
<p>Too frequent words are removed from consideration without lowering model predictions. For example, text8 has 170M+ words, while its subsample has 55M+ words.</p>
<h3>Sources and inspirations</h3>
Jay Alammar's <a href = "https://jalammar.github.io/illustrated-word2vec/">The Illustrated Word2vec</a> taught me about the core concepts of Word2Vec.
<br>
<br>
Additionally, geeksforgeeks.org has some <a href = "https://www.geeksforgeeks.org/nlp/negaitve-sampling-using-word2vec/">content</a>, even though PyTorch is used.
<br>
<br>
Project entirely made by <a href = "https://github.com/lukastan">@lukastan</a>
