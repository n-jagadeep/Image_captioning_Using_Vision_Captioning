# Image_captioning_Using_Vision_Transformer
By,
   Jagadeep Nannuri(700755937)

# Model Archetecture:

![Archetecture](https://github.com/n-jagadeep/Image_captioning_Using_Vision_Captioning/assets/142545023/3f2df858-8e09-43ea-8f32-b29b96423e22)

# how to Run:
The `Image_Captioning.ipynb` file can run locally through Jupyter Notebook or Google Colab.

Before running, go to the mentioned link below and download the glove.6B.100d.txt.zip which contains the word embeddings. Link: https://drive.google.com/file/d/1IRq8lybZAwyyvj-ywUECa29PEpYIscPH/view?usp=share_link

If using google colab, just upload the .zip file to the instance.

## Performance and Results:

Vision Transformer as the Encoder:
 |Epochs| 1-gram BLEU |2-gram BLEU|3-gram BLEU|4-gram BLEU|
 |-------|------|-------|-----|----|
| 10   | 42.177    |25.6924|   14.33078|7.1955|
 |20|   58.279  | 39.3787   |24.7216|14.5401|
 |30 |67.186 | 47.0968|  31.0677|19.6122|
 |40|69.532 | 49.6889|  33.4294|21.5386|

 |Encoder| 1-gram BLEU |2-gram BLEU|3-gram BLEU|4-gram BLEU|
|---|---|---|---|---|
 |ViT   |67.186 | 47.0968|  31.0677|19.6122|
 |ResNet50|   65.765  | 45.423  |29.892|18.236|
 |Inception |63.825 | 44.055|  28.74|17.813|
 |DenseNet|61.758 | 42.0103|  26.814|16.268|

|Parameters|Values|
|----|-----|
 |Loss Function | Cross Entropy|
 |Learning Rate | 0.00001|
 |Batch Size | 32|
 |Optimizer | Adam|
 |Regularization | L2 Penalty|
 |Gradient Regularization | Gradient Clipping|

 # correct caption:
 <img width="509" alt="238800462-3ab7d987-59bd-4787-94ce-1ffa788b25f8" src="https://github.com/n-jagadeep/Image_captioning_Using_Vision_Captioning/assets/142545023/682d38d1-ef65-4cd4-bf71-48a2aed37573">

 # incorrect caption:
 <img width="512" alt="238800446-b990627d-533e-4449-8f09-4498b50f134d-2" src="https://github.com/n-jagadeep/Image_captioning_Using_Vision_Captioning/assets/142545023/9c065265-328c-4a6a-bc3b-18fac3948558">


 
