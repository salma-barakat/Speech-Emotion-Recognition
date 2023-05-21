# Speech-Emotion-Recognition
Speech Emotion Recognition (SER) is a field of artificial intelligence that focuses on detecting and interpreting emotions conveyed through human speech. </br></br>
**Dataset used:** CREMA-D at the following link https://www.kaggle.com/dmitrybabko/speech-emotion-recognition-en . The dataset consists of 7,442 original clips from 91 actors, Actors spoke from a selection of 12 sentences. The sentences were presented using one of six different emotions (Anger, Disgust, Fear, Happy, Neutral and Sad) and four different emotion levels (Low, Medium, High and Unspecified). The filenames of each CREMA-D audio files are following a naming convention consists of 4 blocks, separated by underscores.</br></br>
**Steps:**</br>
•	Load data using librosa library to obtain waveform and sampling rate of audios.</br>
•	Get maximum length of audio to pad all audios to reach same length.</br>
• Create the Feature Space that consists of : </br>
    1- Zero crossing rate (which is the rate of sign-changes of the signal during the duration of a particular frame) and energy (which is the sum of squares of the signal values, normalized by the respective frame length) for time domain.<br>
    2- Convert the audio waveform to mel spectrogram and use this as the feature space.</br>
 • Split the data into 70% training and validation and 30% testing. Use 5% of the training and validation data for validation.</br>
 • Then, get the feature space of each of the training data, validation data and test data.</br>
 • Convert the labels from categorical data to numerical data and fix the shapes of data to use them in the model.</br>
 • Adding the CNN models: the 1D model is for time domain feature space, while the 2D model is for the mel spectogram feature space.</br>
 Note: The models take a long time to run, so it is better to run the project using Kaggle notebook to take the advantage of its GPU.</br>
**For more details refer to the report and the notebook.**
 
 
## Contributors:
 - [Salma Barakat](https://github.com/salma-barakat)
 - [Yasmine Eshra](https://github.com/yasmin-ashraf-eshra)
 - [Habiba Hossam](https://github.com/habiba-hossam)
  
