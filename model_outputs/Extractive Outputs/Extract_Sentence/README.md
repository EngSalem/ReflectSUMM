## This is the data we had for ReflectSUMM Extractive Reflective Summarization Task

Note that for all systems but GPT, we have five folds cross-validation setting, you can concatenate them all.
- lexrank_extractive_sent: LexRank baseline
- MatchSUM: the STOA extractive system
- text_cnndm: the model used in production
- text_finetune: BERTSUM-EXT model finetuned on our ReflectSumm Dataset, better performance than text_cnndm
  baseline.
- text_specificity_finetune: BERTSUM-EXT model finetuned on our ReflectSumm Dataset with specificity. 
- amazon: model finetuned on a opinion summarization dataset based on amazon reviews. 
For the above four system outputs, we have the "specificity_fold{i}_stat.csv" for refernce of the lecture meta data. you can simply apply table concatenation between the system results files and the meta data file.

i.e. 
in amazon, we have amazon_fold1_tune.csv with two columns "generation" and "oracle". The file in the root directory "specificity_fold1_stat.csv" has the same length and refers to the original files.

- chatGPT: the chatGPT model prompted to select five reflections per lecture, files include course_id, lecture_id. gpt3_outputs is the system generation concatenated with "|_|". "extractive summary_y" refers to the human generated summary.