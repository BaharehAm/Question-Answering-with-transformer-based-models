This repository contains a modified version of the Huggingface library example for the question answering task. 
It was a group project for the Deep Learning course offered at HEC Montreal. We we reviewed state-of-the-art transformer models for QA task applied on 
SQuAD 1.1 and 2.0 datasets. We tested five models, RoBERTa, ALBERT, BERT, XLMRoBERTa, and DistilBERT, and our experiments showed that RoBERTa-base pre-trained model 
has the best performance in terms of F1 and EM scores. 
Moreover, we examined the effect of training steps and training size on these models’ performance. 
We found that fine-tuning these models just for 2 epochs is enough to get our reported performance. 

## Experiment results on SQuAD 1.1 and SQuAD 2.0 
![image](https://user-images.githubusercontent.com/46126394/195227422-18250aa2-f65f-441d-b8a2-842fb56527ff.png)

## Effect of training size on F1 score
SQuAD 1.1
![image](https://user-images.githubusercontent.com/46126394/195229475-5071feb5-4257-41c7-9d21-deda69d97e78.png)
SQuAD 2.0
![image](https://user-images.githubusercontent.com/46126394/195229487-7cf8d09c-2747-4abf-9ace-9ac2b4db058c.png)

## The effect of number of epochs on F1 score 
SQuAD 1.1
![image](https://user-images.githubusercontent.com/46126394/195229659-3c77cb61-b046-4091-ae62-174d3192989c.png)
SQuAD 2.0
![image](https://user-images.githubusercontent.com/46126394/195229674-aad9d87f-9811-42de-adf3-2871a5f1a819.png)

## An example output of our models for QA task
![image](https://user-images.githubusercontent.com/46126394/195229966-c317892a-ea5f-40b8-96f6-d488613ea313.png)



Training loss - SQuAD 1.1
![image](https://user-images.githubusercontent.com/46126394/195227369-8913b07d-93f0-4b71-8197-eaf18b83cfa4.png)
Training loss - SQuAD 2.0
![image](https://user-images.githubusercontent.com/46126394/195227385-01bb5250-cc43-4606-baf2-873ff55c7e0e.png)
Validation loss - SQuAD 1.1
![image](https://user-images.githubusercontent.com/46126394/195227399-008ac73e-2a94-4ab7-8132-c4d8c7c8f2aa.png)
Validation loss - SQuAD 2.0
![image](https://user-images.githubusercontent.com/46126394/195227409-5fa6568f-cba9-4237-8ff6-2a3421f58773.png)





