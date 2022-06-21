# Covid-19-and-Cardiac-Disease-Classification-using-ECG-Images

Recent research on the Covid-19 and Cardiac disease classification using ECG images with a feature App development has tried to make a contribution to the society in a very simple yet efficient manner. The data is collected from Mendeley and UCI, and the custom model is built using CNN. The UCI dataset is in a numerical form which is converted into a 12-lead ECG plot. To increase the performance of the model, we have tried to use different techniques such as data augmentation, data scaling, and converting the images to grayscale. The testing of the model was performed with 1 Nvidia T4 GPU, 32GB RAM, and a 1.59GHz memory clock taking 9 hours of run time with a slow learning rate and  300 epochs which gave an accuracy of 86 and 80 on the train and test data, respectively. Taking the help of Android studio and converting the custom model to tflite, we have built our app, which gives an option for people to have a shot at knowing the ECG result during these testing times of covid-19 when the hospital is running out of staff.

## Results

When comparing the results of our custom-built model with the Vgg16 model, which was trained on image data, we found that our model accuracy and performance are higher on our dataset.
As it can be seen in the below figures that the custom model has given the accuracy of 86 and 80 on train and test,  respectively, when compared to the VGG-16 model, which gave an accuracy of 50 and 20 on train and test, respectively.
### Custom model’s accuracy and loss curve
![image](https://user-images.githubusercontent.com/50734928/166563793-84c3783d-1d48-4f2c-a8be-c1cdc9aa7ed0.png)
### VGG-16 model’s accuracy and loss curve
![image](https://user-images.githubusercontent.com/50734928/166563901-2f1521be-9d8c-4a62-888c-6d1bc846357f.png)

## Mobile Application Development

The very first point of consideration when thinking about ways to connect an ML model to a mobile app is to create an API that acts as a middle layer between the frontend (App) and the backend (ML model). However, we have adopted an innovative approach of directly integrating the ML model with the android app using the "tflite (TensorFlow lite) model import" feature available in the latest Android Studio 4.1.

![image](https://user-images.githubusercontent.com/50734928/166563710-90bcffbb-12bf-46e9-9ca4-4a64d4f64c6b.png)

Note: Dataset can be found at https://drive.google.com/drive/folders/14ngeAPpoukv4acQg2RMzB3tutN1kZRPD?usp=sharing.
