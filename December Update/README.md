# December Update

### All files are commented with sample outputs for most variables.

## About the Files

### GoEmotion MultiClass Classification with Simple Transformers.ipynb 
  * RoBerta model trained on GoEmotions where the labels are multiclass only.
  * The data is augmented to ensure there is equal representation for all the labels. 
  * Accuracy - 55%

### GoEmotion MultiLabel Classification with Simple Transformers.ipynb 
  * RoBerta model trained on GoEmotions where the labels are multiclass only.
  * The data is augmented to ensure there is equal representation for all the labels. 
  * LRAP - 65%

### Raw GoEmotion with Ekman Mapping MultiLabel Classification with Simple Transformers.ipynb
  * RoBerta model trained on GoEmotions where the labels are multiclass & multilabel.
  * 27+1 emotions are mapped to 6 Ekman emotions + neutral.
  * The data is not augmented and duplicates were left untouched.
  * LRAP - 86%

### Raw GoEmotion MultiLabel Classification with Simple Transformers.ipynb
  * RoBerta model trained on GoEmotions where the labels are multiclass & multilabel.
  * The data is not augmented and duplicates were left untouched.
  * LRAP - 63%

### Raw SemEval Task 1 MultiLabel Classification with Simple Transformers.ipynb
  * RoBerta model trained on SemEval Task 1 where the labels are multiclass & multilabel.
  * LRAP - 52%

### Raw SemEval Task 1+2 MultiLabel Classification with Simple Transformers.ipynb
  * RoBerta model trained on SemEval Task 1 & 2 combined where the labels are multiclass & multilabel.
  * LRAP - 54%

### Raw SemEval Task 1+2 with Emotions MultiLabel Classification with Simple Transformers.ipynb
  * RoBerta model trained on SemEval Task 1+2 where the labels are multiclass & multilabel.
  * The text is contactenated with the emotions predicted by the GoEmotions model.
  * LRAP - 54%

### Raw SemEval Task 1+2 with Emotions MultiLabel Classification with Simple Transformers using Pretrained Model.ipynb
  * RoBerta model trained on GoEmotions where the labels are multiclass & multilabel.
  * The data is not augmented and duplicates were left untouched.
  * The model is later used to train SemEval Task 1+2 where the labels are multiclass & multilabel.
  * The text is contactenated with the emotions predicted by the GoEmotions model.
  * LRAP - 56%

## LRAP - https://scikit-learn.org/stable/modules/generated/sklearn.metrics.label_ranking_average_precision_score.html

### Acronyms in Dataset
  * GoE - GoEmotions
  * SE - SemEval
  * D - Duplicates (There were some duplicates present in GoEmotions data)
  * NoD - No Duplicates
  * MM - MultiModel
  * T1 - Task 01
  * T1T2 - Task 01 + Task 02

## Things Left to be Done

* Use Softmax output
* ~~Use GoEmotion model as pretrained model~~
* ~~Upload Data~~
* ~~Interpretation~~
* ~~Persuasion/SemEval Data~~
