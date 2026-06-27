# thesis-analysis
This repository contains the analysis code for a study on Linguistic alignment in human-chatbot interaction

## Installation
Run the following commands to install the necessary dependencies:
```
pip install pandas scipy spacy sentence-transformers scikit-learn matplotlib
```
```
python -m spacy download en_core_web_sm
```
### `demographics.ipynb`
This notebook investigates participant demographics based on responses to the pre-experiment survey

### `manipulation_check.ipynb`
This notebook checks whether language manipulations in the experiment were significantly different. The following metrics are calculated on pairs of text (user text, ai response)
- Linguistic Style Matching (LSM)
- Local Lexical Alignment (LLA)
- Style Cosine Similarity
Wilcoxon Signed-Rank tests are performed on the differences

### `rating_analysis.ipynb`
This notebook contains the main analysis of alignment effects. The following items are caculated and visualized
- Mean persuasion across conditions
- Mean trust across conditions
- Mean rating of additional questions across conditions
- Mean persuasion by participant
- Correlation between trust and persuasion scores
  
Wilcoxon Signed-Rank tests are performed on the following items:

- Persuasion scores across conditions
- Trust scores across conditions
- Additional question scores across conditions
  
Spearman Correlations are computed on the following items:

- Trust and persuasion
- Significant additional questions and outcome (trust and persuasion)
- background demographics and persuasion in the misaligned condition

Additional calculations include:

- Engagement indicators across conditions 
