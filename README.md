# Inception_V3_transfer_learning

1.Download Google trained inceptionv3 network https://storage.googleapis.com/download.tensorflow.org/models/inception_dec_2015.zip
2.Download dataset http://download.tensorflow.org/example_images/flower_photos.tgz
3.Replacing the last softmax layer, the network layer before the last fully connected layer is called the bottleneck layer bottleneck. The process of passing the new image through the trained convolutional neural network to the bottleneck layer can be regarded as the process of feature extraction on the image. In the trained inceptionV3 model, because the output of the bottleneck layer can be well distinguished by 1000 types of images through a single-layer fully connected layer neural network, it is reasonable to think that the node vector output by the bottleneck layer can be used as A more compact and expressive feature vector of the image.
