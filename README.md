# Protecting Gender and Identity with disentangled speech representations

Besides its linguistic component, our speech is rich in biometric information that can be inferred by classifiers. Learning privacy-preserving representations for speech signals enables downstream tasks, such as speech recognition, without sharing unnecessary private information about an individual. In this short presentation we will show how gender recognition and speaker verification tasks can be reduced to a random guess, protecting against classification-based attacks.

## Requirements
Install pip dependencies:
    ```pip install requirements.txt```
    
 ## Data Processing
 1. Create train/test splits and extrat root directory 
 2. Preprocess audio and extract train/test mel spectrograms
 
 ## Training
 1. download pretrained weights for VQ-CPC model [here](https://github.com/bshall/VectorQuantizedCPC/releases/tag/v0.1)):
 2. Train the vocoder  
 Example usage:
    ```
    python train_vocoder.py cpc_checkpoint=checkpoints/cpc/english2019/model.ckpt-24000.pt checkpoint_dir=checkpoints/vocoder/english2019
    ```
 ## Evaluation
    
