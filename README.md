# In-Silico-Models-for-Predicting-Covid-19-from-their-Speech
This repository contains the Deep Learning CNN code implementation which is used to predict covid using Cough sounds.

The cough sound Data was taken from IISC Coswara dataset.
The sound samples were first pre processed and then padded and filtered to make each sample of equal length . The mean sample length of the audio files was  found to be 8 seconds.

![Audio](https://user-images.githubusercontent.com/110150684/183032808-78285ca1-7e13-4310-afdc-fdab5c8b5820.jpg)

Then the audio files were converted into spectro grams which look like this. 

![](images/spectrogram.png)
![Spectrogram](https://user-images.githubusercontent.com/110150684/183032684-8a67c62c-9ca0-43ef-9392-14052a5580df.png)

This spectrogram is then sent to the CNN model in the input layer and then the CNN classifies it between 0 and 1.
The CNN model workflow looks like.

![CNN workflow](https://user-images.githubusercontent.com/110150684/183033039-d26c47f4-4ddc-4e1f-bb4e-3eee25493466.jpg)

After the input is given to the model. The model is built with various hidden layers and max pooling is also done.
The model trains with 98% training accuracy and 87 % validation accuracy.

![Model training and validation accuracy](https://user-images.githubusercontent.com/110150684/183033470-9f54dd9c-9965-42c4-a9e4-713ee7cda35e.jpg)

The confusion matrix and AUC - ROC curve of the model is shown below
![AUC-ROC curve](https://user-images.githubusercontent.com/110150684/183033671-fd880f2a-54f6-44e1-ae40-a9f6dc2083e0.jpg)

![confusion matrix](https://user-images.githubusercontent.com/110150684/183033718-c1b8bd94-29c5-4ba0-b834-5755587f54b2.jpg)


Thanks
