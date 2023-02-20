# Supplementary Materials for the paper "Testing the Effectiveness of the Diagnostic Probing Paradigm on Italian Treebanks"

# Gold and Control datasets + Probing Results 

The two folders contain the gold/control datasets and the results obtained by the probing model trained with BERT's internal representations.

## Datasets

The folder is divided in two subfolders:
-- ``Standard_Subset``: containing the datasets with the values of linguistic features characterising the set of sentences belonging to the standard subset;
-- ``Shortest_Longest_Subsets``: containing the datasets with the values of linguistic features characterising the set of sentences belonging to the two groups of shortest (< 10) and longest sentences (> 30).

The first row of each .tsv file contains the label of the linguistic features automatically extracted by Profiling-UD, while the second row shows the label of the group to which each feature belongs. 

## Results

As for the ``Dataset`` folder, ``Results`` is divided in the two ``Standard_Subset`` and ``Shortest_Longest_Subsets`` subfolders.

Each file contains the probing scores reported in terms of Spearman correlations achieved for every linguistic feature. For each row we have the following information:
>> first column: label of the group to which the linguistic feature belongs;
>> second column: label of the linguistic feature;
>> third-fourteenth columns: number of BERT's layers considered to extract the sentence-level representations used by the probing model.
