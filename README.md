# scl-2021-address-extractor
## Task
Predict the POI and street of 50k raw addresses

## Approach
- Decided to try out Spacy NER to detect POI/street in address
- Had to convert data into an acceptable format for Spacy
  - Involved identifying pos of train POI/streets
  - Cleaned data to ensure there's no overlap between labels
- Trained using Google Colab to make use of GPU
- Only used 5k out of 300k rows due to slow training time caused by non-optimised GPU usage

## Results
- 0.32 accuracy

## Challenges/Improvements
- Limited GPU usage
- Abbreviations not dealt with
- Unfamiliarity with ID language
- Could have explored using transformers like IndoBert
