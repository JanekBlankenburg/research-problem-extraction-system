# Research Problem Extraction System

The basic idea is to solve the problem as a Named Entity Recognition (NER) task, since the research problems to be extracted are components of the source texts. 
The system achieves the following results:
- precision : 1.00
- recall: 0.33
- f1: 0.50

It should be noted that for these results only the titles of the papers are considered, which leads to the fact that many of the research questions mentioned in the abstracts or in the introductions are not recognized (see the low recall). At the same time, the system has a perfect precision, which means that the research questions that are extracted match the actual research questions of the paper.

Besides the solution shown here, I have also tried to train the model on the abstracts as well as on the concatenated title and abstract. Both gave slightly lower results than the model trained only on the title.

To execute the notebook it is necessary to adjust the parameters training_data_path and test_data_path depending on local setup.