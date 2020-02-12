# Object-Detection
This is a PyTorch Project to Object Detection.

To build a model that can detect and localize specific objects in images.
We will be implementing the Single Shot Multibox Detector (SSD), a popular, powerful, and especially nimble network for this task.

    Implementation

The sections below briefly describe the implementation.

They are meant to provide some context, but details are best understood directly from the code, which is quite heavily commented.

    Dataset
We will use Pascal Visual Object Classes (VOC) data from the years 2007 and 2012.

    Description

This data contains images with twenty different types of objects.

         {'aeroplane', 'bicycle', 'bird', 'boat', 'bottle', 'bus', 'car', 'cat', 'chair', 'cow', 'diningtable', 'dog', 'horse', 'motorbike', 'person', 'pottedplant', 'sheep', 'sofa', 'train', 'tvmonitor'}

Each image can contain one or more ground truth objects.

Each object is represented by

- a bounding box in absolute boundary coordinates

- a label (one of the object types mentioned above)

- a perceived detection difficulty (either 0, meaning not difficult, or 1, meaning difficult)

        Download
        
Specfically, you will need to download the following VOC datasets

- 2007 trainval (460MB)

- 2012 trainval (2GB)

- 2007 test (451MB)

Consistent with the paper, the two trainval datasets are to be used for training, while the VOC 2007 test will serve as our validation and testing data.

Make sure you extract both the VOC 2007 trainval and 2007 test data to the same location, i.e. merge them.
