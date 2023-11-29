# Image_captioning_Using_Vision_Captioning

Team Members:

Jagadeep Nannuri(700755937)

Varshitha Reddy(700757574)

Vennela Pulavarti(700756480)

Sudeep Reddy Kanthala(700755923)

# Model Archetecture:

![Archetecture](https://github.com/n-jagadeep/Image_captioning_Using_Vision_Captioning/assets/142545023/3f2df858-8e09-43ea-8f32-b29b96423e22)

# how to Run:
The `VisionCaption.ipynb` file can run locally through Jupyter Notebook or Google Colab.

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
 
