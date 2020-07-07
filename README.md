# Mask-RCNN
Mask R-CNN is basically an extension of Faster R-CNN. Faster R-CNN is widely used for object detection tasks. For a given image, it returns the class label and bounding box coordinates for each object in the image.

The Mask R-CNN framework is built on top of Faster R-CNN. So, for a given image, Mask R-CNN, in addition to the class label and bounding box coordinates for each object, will also return the object mask.

Let’s first quickly understand how Faster R-CNN works. This will help us grasp the intuition behind Mask R-CNN as well.

Faster R-CNN first uses a ConvNet to extract feature maps from the images
These feature maps are then passed through a Region Proposal Network (RPN) which returns the candidate bounding boxes
We then apply an RoI pooling layer on these candidate bounding boxes to bring all the candidates to the same size
And finally, the proposals are passed to a fully connected layer to classify and output the bounding boxes for objects

![Test Image 1](https://github.com/DB11051998/Mask-RCNN/blob/master/images/1045023827_4ec3e8ba5c_z.jpg)
