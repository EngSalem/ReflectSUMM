# This directory contains the model outputs for the phrase summarization models.
## The directory is composed as follows
- GPT3.5 (predicted phrases are stored under gpt3_outs)
          
        - gpt3.5-noun-phrase (contains zero-shot output of GPT-noun phrase)
  
        - gpt3.5-human (contains zero-shot output of GPT with human prompt)
        
        - gpt3.5-noun_phrase_1_shot(contains one-shot output of GPT-noun phrase)
                

- PhraseSum (contains output of PhraseSum, predicted phrases are stored as keys of column Predicted Phrase Summary)



*All model outputs are in folds*
*Each file ends with _fold{i} where i is in range [1,5] each indicates a unique fold of the dataset*
*All chatGPT outputs are based on one run output, it's important to note that chatGPT is random, and different summaries can be generated at each run using our provided code*
