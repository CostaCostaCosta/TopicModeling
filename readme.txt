The repository Assign topics automatically to documents in the dataset.

Dataset location: https://s3-us-west-2.amazonaws.com/rm-exercise/rm_topic_modeling_data.zip

Example:
Sample line in input file: {"_id": "abcdef", "text": "This is an example document."}
Sample line in output file: {"_id": "abcdef", "topics": ["topic1", "topic2", "topic3", "topic4", "topic5”]}

Dependencies:
Python 3.6
scikit-learn
numpy
matplotlib
gensim (for Word2Vec model)
Jupyter notebook

To run on a novel dataset, first run the TopicModeling-RM until k must be determined. 
Then, run Parameter_Selection-RM to determine an optimal k. 
Input this k into TopicModeling-RM, and continue running the notebook, to create the final output.

Links and References:
Lee, D. D., & Seung, H. S. (1999). Learning the parts of objects by non-negative matrix factorization. Nature. http://www.columbia.edu/~jwp2128/Teaching/E4903/papers/nmf_nature.pdf
Blei, D. M. (2012). Probabilistic topic models. Communications of the ACM, 55(4). https://cacm.acm.org/magazines/2012/4/147361-probabilistic-topic-models/fulltext
O’Callaghan, D., Greene, D., Carthy, J., & Cunningham, P. (2015). An analysis of the coherence of descriptors in topic modeling. Expert Systems with Applications. http://derekgreene.com/papers/ocallaghan15eswa.pdf
https://github.com/derekgreene/topic-model-tutorial
