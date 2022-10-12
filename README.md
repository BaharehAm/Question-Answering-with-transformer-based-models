This repository contains a modified version of the Huggingface library example for the question answering (QA) task. 
It was a group project for the Deep Learning course offered at HEC Montreal. We reviewed state-of-the-art transformer models for QA task applied on 
SQuAD 1.1 and 2.0 datasets. We studied fine-tuning performance of five models, namely RoBERTa, ALBERT, BERT, XLMRoBERTa, and DistilBERT under various settings.
Due to our limitations in computational power, we fixed the values for learning rate, weight decay, and other hyperparameters as presented in the original papers
and used batch size of 16 to be able to run our models.
Our experiments showed that RoBERTa-base pre-trained model has the best performance in terms of F1 and Exact Match (EM) scores on both
SQuAD 1.1 and 2.0 while DistillBERT model performs the poorest. 
Moreover, we examined the effect of training steps and training size on these models’ performance.  
To study the effect of training size in fine-tuning step on the performance of our models, we used
33%, 66%, and 100% of each dataset. This experiment showed that DistilBERT and BERT models are more sensitive to the fine-tuning data size, especially
for SQuAD 2.0 dataset. For SQuAD 1.1, reducing the size of the training dataset has a small impact
in case of RoBERTa model.
In terms of training steps, we found that fine-tuning these models just for 2 epochs is enough to get our reported performance. 


## Experiment results on SQuAD 1.1 and SQuAD 2.0 
![image](https://user-images.githubusercontent.com/46126394/195227422-18250aa2-f65f-441d-b8a2-842fb56527ff.png)

## The effect of training size on F1 score
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



## Training and Validation loss behaviors
![image](https://user-images.githubusercontent.com/46126394/195227369-8913b07d-93f0-4b71-8197-eaf18b83cfa4.png)
![image](https://user-images.githubusercontent.com/46126394/195227385-01bb5250-cc43-4606-baf2-873ff55c7e0e.png)
![image](https://user-images.githubusercontent.com/46126394/195227399-008ac73e-2a94-4ab7-8132-c4d8c7c8f2aa.png)
![image](https://user-images.githubusercontent.com/46126394/195227409-5fa6568f-cba9-4237-8ff6-2a3421f58773.png)





