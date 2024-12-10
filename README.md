# Scratch_detection_Text
This repo contains a modular scratch detection based on clip embeddings and different classification models

GPU REQUIREMENTS: NVIDIA P100 (15GB)

DEPENDENCIES: pip install -r requirement.txt

**WHEN CHANGING THE CLASSIFCATION MODEL MUST CHNAGE THE MODEL INPUT DIMENSIONS**

**Precision: 0.3333, F1 Score: 0.4444(ViT-B-32)**

**Precision: 0.7500, F1 Score: 0.8571(convnext_base_w)**

#How to run the code 
1. Prefer Kaggle notebook for replicating the exact result
2. install the dependencies using requirement.txt
3. change the config block also change the dimesion to change classification head
4. chnage learning rate,weight_decay,batch_size according to the model current config is for convnext_base_w
   

