# Peax - Pattern Similarity Expriments

We compared the perceived similarity of patterns in sequential data at 3
different sizes. The sequential data is a [DNase-seq](https://en.wikipedia.org/wiki/DNase-Seq) experiment from the
[ENCODE project](https://www.encodeproject.org). We extracted 9 different patterns at increasing sizes of 3 kilobase pairs (kb), 12 kb, and 120 kb.

![Results of both user studies](/user-study-1-2-results.png?raw=true "Results of both user studies")

## Experiment 1: groupwise comparison of 7 similarity search techniques

![Results of the groupwise similarity comparison](/user-study-1-results.png?raw=true "Results of the groupwise similarity comparison")

## Experiment 2: pairwise comparison of CAE and ED

![Results of the pairwise similarity comparison](/user-study-2-results.png?raw=true "Results of the pairwise similarity comparison")

![Results of the pairwise similarity comparison per search result](/user-study-2-results-by-knn.png?raw=true "Results of the pairwise similarity comparison per search result")

## Reproduce results

```
conda env create --file environment.yml
jupyter lab
```

The staistical analysis and the code for generating the figures is available in
the following three notebooks:

- [user-study-1-results.ipynb](user-study-1-results.ipynb)
- [user-study-2-results.ipynb](user-study-2-results.ipynb)
- [user-study-1-2-combined-results.ipynb](user-study-1-2-combined-results.ipynb)