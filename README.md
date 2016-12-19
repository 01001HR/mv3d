# mv3d
Source code accompanying the ECCV'16 paper "Multi-view 3D Models from Single Images with a Convolutional Network" by M. Tatarchenko, A. Dosovitskiy and T. Brox https://arxiv.org/abs/1511.06702. This is a re-implementation of the models described in the paper, so we do not guarantee both quantitative and qualitative results to be exactly the same.

## Dependencies
- Tensorflow
- Panda3D
- NumPy
- SciPy

## Data

The networks were trained on a subset of the ShapeNet dataset containing 3D models of cars http://shapenet.cs.stanford.edu/. If you want to reproduce our results, you need to get the models. Follow the download instructions from the official website. Unzipped models should be placed in the 'data/obj_cars' folder in the following structure:
*data/obj_cars/model_id/{model.obj, model.mtl}*.

For the background experiment we used a subset of the ImageNet validation set (images 00000001 - 00050000). Those should be placed in *data/bg_imagenet/val/ILSVRC2012_preprocessed_val_xxxxxxxx.JPEG*, where xxxxxxxx is an 8-digit image id.

## Code
- download_data.py - a script for downloading the pre-rendered version of the test and the pre-trained network snapshots. Run it before executing any other code.

## License and Citation

All code is provided for research purposes only and without any warranty. Any commercial use requires our consent. When using the code in your research work, please cite the following paper:

    @article{jia2014caffe,
      Author = {Jia, Yangqing and Shelhamer, Evan and Donahue, Jeff and Karayev, Sergey and Long, Jonathan and Girshick, Ross and Guadarrama, Sergio and Darrell, Trevor},
      Journal = {arXiv preprint arXiv:1408.5093},
      Title = {Caffe: Convolutional Architecture for Fast Feature Embedding},
      Year = {2014}
    }
