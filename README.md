# Fault-detection

Using synthetic datasets to train an end-to-end convolutional neural network for 3D seismic fault segmentation.

Dataset
To train our CNN network, we automatically created 200 pairs of synthetic seismic and corresponding fault volumes, which were shown to be sufficient to train a good fault segmentation network.

Training
Run train.py to start training a new faultSeg model by using the 200 synthetic datasets

Validation
Fault detections are computed on a syntehtic seismic image by using 8 methods of C3 (Gersztenkorn and Marfurt, 1999), C2 (Marfurt et al., 1999), planarity (Hale, 2009), structure-oriented linearity (Wu, 2017), structure-oriented semblance (Hale, 2009), fault likelihood (Hale, 2013; Wu and Hale, 2016, code), optimal surface voting (Wu and Fomel, 2018, code) and our CNN-based segmentation.
