# un-sustainable-dev--goals
This project was inspired from the United Nations platform to verify that each document uploaded belongs to a certain topic.

This notebook file starts by scanning all the word documents uploaded by the united nations on their sustainable development goals website and merges them into one document.
Note that we have 17 different topics.
After that we applied text preprocessing for each document belonging to these topics. Now that our documents are ready, we used GloVe vectorization technique to transform each topic document as a reference vector.
Then, for every received document, we transform it to a vector and compare it with the reference vectors using cosine similarity to check with which topic it is the closest.
Note that we used pickle files to save our reference vectors so we do not have to generate them every time.
