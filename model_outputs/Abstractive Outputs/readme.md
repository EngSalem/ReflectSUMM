# This directory contains the model outputs for the abstractive summarization models.
## The directory is composit as follows
-Finetune BART-Large
                  |
                  |FinetuneBART (contains vanilla finetuning output of BART-Large model)
                  |
                  |FinetuneBART+specificity (contains finetuning output of BART-Large + specificity tokens) 

-Zeroshot-GPT
            |
            |gpt3.5-turbo-zeroshot (zeroshot output of chatGPT)
            |
            |gpt3.5-turbo-zeroshot+specificity (zeroshot output of chatGPT with specificity information included in the prompt)


-Oneshot-GPT (contains oneshot output of chatGPT)


*All model outputs are in folds*
*Each file ends with _fold{i} where i is in range [1,5] each indicates a unique fold of the dataset*
*All chatGPT outputs are based on one run output, it's important to note that chatGPT is random, and different summaries can be generated at each run using our provided code*




                              
