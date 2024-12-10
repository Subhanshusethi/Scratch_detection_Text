# Scratch Detection Text Repository

This repository contains a modular scratch detection system based on CLIP embeddings and various classification models.

---

## **GPU Requirements**
- NVIDIA P100 (15GB)

---

## **Dependencies**
Install the required packages using:
```bash
pip install -r requirements.txt
```

---

## **Important Note**
- **When changing the classification model, you must update the model input dimensions accordingly.**

---

## **Performance Metrics for bad images**
| Model               | Precision | F1 Score |
|---------------------|-----------|----------|
| **ViT-B-32**        | 0.8333    | 0.7844   |
| **convnext_base_w** | 0.7500    | 0.8571   |

---

## **Preprocessing**
1. Rename bad images to `scratches` and good images to `no_scratches`.
2. Place the images in a designated directory.

---

## **How to Run the Code**
1. Prefer using a Kaggle notebook to replicate the exact results.
2. Adjust the dataset path as required.
3. Install dependencies using:
   ```bash
   pip install -r requirements.txt
   ```
4. Update the configuration block and ensure the input dimensions are adjusted if changing the classification head.
5. Modify the learning rate, weight decay, and batch size according to the model. The current configuration is optimized for `convnext_base_w`.

## **How to Run the Inference**
1. Download model weights for VIT-32(512) and convnext_base_w(640)
2. Change the weights path in notebook and chnage image path to test 

## **Why `convnext_base_w`?**
- It achieves a classification accuracy of 70.1% on zero-shot tasks.
```
## **Model Weights link: https://drive.google.com/drive/folders/1w3VvCH5cfHsqJNSnKoro9bD47vzF2W-t?usp=sharing **
