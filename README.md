# Pixel Objectness

The following repository contains pretrained model for pixel objectness.

If you use this in your research, please cite the following paper:

@article{pixelobjectness,
Author = {Jain, Suyog and Xiong, Bo and Grauman, Kristen},
Journal = {arXiv preprint arXiv:1701.05349},
Title = {Pixel Objectness},
Year = {2017}
}

## Using the pretrained models:

This model is trained using Deeplab-v1 caffe library. Please cite [1] and [2] if you use the code.

- Setup: Download and install Deeplab-v1 from [here](https://bitbucket.org/deeplab/deeplab-public/)

- Refer to demo.py for step-by-step instruction on how to run the code.

- Store the images that you want to process in the images folder.

- Update the caffe binary path and image extension variable in demo.py

- Running demo.py will produce three files 1) input_list.txt : contains list of of input images, 2) output_list.txt: contains names to be used to store the output of pixel objectness 3) test.protoxt: prototxt file required for loading the pretrained model.

## Visualizing the results:

After execution demo.py will store pixel objectness results as matlab files.

Please refer to show_results.m to see how to visualize and extract foreground masks.

[1] Caffe:
@article{jia2014caffe,
Author = {Jia, Yangqing and Shelhamer, Evan and Donahue, Jeff and Karayev, Sergey and Long, Jonathan and Girshick, Ross and Guadarrama, Sergio and Darrell, Trevor},
Journal = {arXiv preprint arXiv:1408.5093},
Title = {Caffe: Convolutional Architecture for Fast Feature Embedding},
Year = {2014}
}

[2] Deeplab-v1:

@inproceedings{chen14semantic,
title={Semantic Image Segmentation with Deep Convolutional Nets and Fully Connected CRFs},
author={Liang-Chieh Chen and George Papandreou and Iasonas Kokkinos and Kevin Murphy and Alan L Yuille},
booktitle={ICLR},
url={http://arxiv.org/abs/1412.7062},
year={2015}
}