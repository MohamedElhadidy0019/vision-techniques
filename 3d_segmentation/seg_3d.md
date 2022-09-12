# 3D Segmentation Techinques
# Just thoughts and notes and not in detail

## UNET 3D(on uniform voxels)
- Amazingly just take 2d UNET and change the convolution pooling layers from 2D to 3D and let the input be voxels instead of images and you will get a 3D UNET that does semetic segmentation on 3D voxelised point clouds.
<!--  paper -->
- [3D UNET Paper](https://arxiv.org/pdf/1606.06650.pdf)
## SqueezeSeg
SqueezeSeg is just a encoder-decoder architecture which uses FireModule and Deconvolution. It takes the point cloud and generates by it 2d channels by cylderical projection (one for intensity,range,x,y,z) and then the nn takes these 2c channels as input
<!-- link -->
[SqueezeSeg Explanation](https://www.youtube.com/watch?v=Xyn5Zd3lm6s&t=15s&ab_channel=%E5%90%B4%E7%92%A7%E8%BE%B0)

## For non-uniform voxels OCNet can be used
<!-- paper -->
[OCNet Paper](https://arxiv.org/pdf/1809.00916.pdf)



## Random notes
3D segmentaition is a really complex problem, there are methods based on 2d images and prior knowledge to ratio of objects, and then stronger methods that use pointcloud whehter by normal CNN, multi model nn or even gnns and transformer based approaches.
Most of the methods are hybrid methods and huerisitcs that just happened to work and some of themy try to proof why their approaches are better but really it's a hassle.



cylenderical 3d paper
pvkd -> used cyldrical 3d




