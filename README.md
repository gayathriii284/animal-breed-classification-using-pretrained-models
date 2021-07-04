# Animal Breed Classification using Pretrained Models
The dataset used here is from the Dockship-Animal Breed Classification challenge.It can be obtained [here.](https://dockship.io/challenges/5fdcba715f392d4d66289d43/animal-breed-classification-ai-challenge/overview)

Here,I use an ensemble of various pretrained models like Xception,EfficientNetB6 and DenseNet.

I felt EfficientNet would be a good choice because it uses a fewer number of parameters and gives comparatively better results when compared with all the other pretrained models.

The image shown below supports the above statement.

<img src="https://i.redd.it/cgd07frqdo951.png" width="500" height="400">



Now,inorder to get further improved accuracy,I concatenated features from the following pretrained models:
  - EfficientNetB6
  - Xception
  - DenseNet
    - DenseNet201
    - DenseNet169
    - DenseNet121
    
Thus by concatenating these pretrained model features and training them on my training data,the results is:
Training Accuracy | Validation Accuracy 
------------------|-------------------
98.8%             | 96.6%               
