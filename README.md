# NLP_Project: Automated Fact Checking For Climate Science Claims

## Introduction
The system can analyze the claim text, then retrieve related evidence passages and classify whether the evidence passages support this claim.

Build a natural language processing model to evaluate what kind of claim is likely supported by what type of evidence passages.

Use TF-IDF (Term Frequency - Inverse Document Frequency) to determine how relevant the claim is to the evidence passages.

User BERT (Bidirectional Encoder Representations from Transformers) to understand the context of the claim and the retrieved evidence passages to classify if this claim is supported by its retrieved evidence passages.

The logic of model is shown below:

<img width="315" alt="image" src="https://github.com/ryougi-shiky/NLP_Project/assets/53469345/1ac1e7af-4481-4395-87e4-65484e2bcce3">


## User Guide
1. In the .ipynb file, Loading Datasets block, make sure to load datasets.
2. Install all dependencies.
3. In the .ipynb file, Environment variables block, adjust the variables that you expect to use.
4. Run the .ipynb file and generate the test data prediction file.
5. Use `eval.py` in `project-datasets` to test the model performance. For example: `python eval.py --predictions dev-claims-baseline.json --groundtruth dev-claims.json`

Output: 
```
Evidence Retrieval F-score (F) = 0.3377705627705628 
Claim Classification Accuracy (A) = 0.35064935064935066 
Harmonic Mean of F and A = 0.3440894901357093
```
