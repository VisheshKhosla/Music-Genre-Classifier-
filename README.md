# Music-Genre-Classifier 

Implementation of music genre classifier using Deep Learning Model called Convolutional Neural Networks(CNNs) on Marsyas Dataset,CNNs are widely used for image classification problems because with the help of filters we can try to identify lines which further identifies shapes which leads to the detection of objects.The filters can be used as detectors and we can change their weights with the help of back-propagation.

There are a total of 10 genres in the dataset:
1.Blues
2.Reggae
3.Rock
4.Disco
5.Pop
6.Metal
7.Classical
8.Jazz
9.Hiphop
10.Country

# Preparation of Data

Since CNNs work really well on images we can represent audio as  images of depth 1 using spectrogram by applying short time fourier transformation or by using MFCCS(mel frequency cepstrul coeffecients)
