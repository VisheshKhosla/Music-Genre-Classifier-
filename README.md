# Music-Genre-Classifier </br>
Implementation of music genre classifier using Deep Learning Model called Convolutional Neural Networks(CNNs) on Marsyas Dataset,CNNs are widely used for image classification problems because with the help of filters we can try to identify lines which further identifies shapes which leads to the detection of objects.The filters can be used as detectors and we can change their weights with the help of back-propagation.</br>
There are a total of 10 genres in the dataset:</br>
1.Blues</br>
2.Reggae</br>
3.Rock</br>
4.Disco</br>
5.Pop</br>
6.Metal</br>
7.Classical</br>
8.Jazz</br>
9.Hiphop</br>
10.Country</br>

# Preparation of Data
</br>
Since CNNs work really well on images we can represent audio as  images of depth 1 using spectrogram by applying short time fourier transformation or by using MFCCS(mel frequency cepstral coeffecients) which helps us in perceiving the sound as human auditory system,in the given project MFCCS have been used as inputs.In order to create more samples,the songs which are of 30 seconds have been chopped off into 10 segments leading to a total of 10,000 samples.The data has been then saved into a json file.Each of the segment has a  (130x13)  input data  where we have 130 MFCC vectors,each of them having 13 coeffecients.Librosa is a great library for doing anny work related to audio processing and we can easily convert an audio to a spectrogram or MFCC using librosa.</br>

# Architecture of the Model
</br>
First of all the input is fed in the form of MFCC to a convolution layer with the activation function relu
