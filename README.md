# mv3d
Source code accompanying the ECCV'16 paper "Multi-view 3D Models from Single Images with a Convolutional Network" by M. Tatarchenko, A. Dosovitskiy and T. Brox https://arxiv.org/abs/1511.06702. This is a re-implementation of the models described in the paper, so we do not guarantee both quantitative and qualitative results to be exactly the same.

**Data**
The networks were trained on a subset of the ShapeNet dataset containing 3D models of cars http://shapenet.cs.stanford.edu/. If you want to reproduce our results, you need to get the models. Follow the download instructions from the official website. Unzipped models should be placed in the 'data/obj_cars' folder using the following structure:
*/data/obj_cars/<model_id>/{model.obj, model.mtl}*
