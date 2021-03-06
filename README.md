## Task 1 - Object Detection
:dart: Implementing an object detector which identifies the classes of the objects.

<img src="https://raw.githubusercontent.com/rahulrai-sudo/object-detection/main/assets/Task1.png"/>

In this repo, you'll find codes for 
- Object detection on Image (Using FasterRCNN, backbone as  InceptionResNetv2)
- Object detection on Video (Using FasterRCNN, backbone as ResNet50v1 640x640)

<img src = "https://raw.githubusercontent.com/rahulrai-sudo/object-detection/main/assets/faster-rcnn.png"/>


- :rocket: Model Architecture : Using pre-trained Faster-RCNN and InceptionResNetV2 feature extractor(acting as backbone) to identify objects in images and webcam. InceptionResNetV2 was trained on [ImageNet](http://image-net.org/) (images scaled to 640x640 resolution) and fine-tuned with FasterRCNN on [OpenImages V4 dataset](https://storage.googleapis.com/openimages/web/index.html), containing 600 classes.
This pre-trained model is taken from [TensorFlow Hub](https://www.tensorflow.org/hub).
- Without using [TensorFlow 2 Object Detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2.md).
- :bulb: Features : Apply object detection on downloaded image or captured image from webcam
- ✅ Accuracy : Mean Average Precision of **0.58** on OpenImagesV4 test set (OpenImages Challenge metric)



- :rocket: Model Architecture : Using pre-trained Faster-RCNN to identify objects on images and webcam. The ResNet50v1 feature extractor(acting as backbone) was trained on [ImageNet](http://image-net.org/) and fine-tuned with FasterRCNN on [COCO2017](https://cocodataset.org/#home), containing 172 classes. This pre-trained model is taken from [TensorFlow Hub](https://www.tensorflow.org/hub).
- Using [TensorFlow 2 Object Detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2.md)
- :bulb: Features : Apply object detection on saved videos or live webcam(both in google colab and anaconda environment)
- ✅ Accuracy : Mean Average Precision of **29.3** on COCO 2017 test set




##  Framework and Libraries used 
- TensorFlow 2.0
- TensorFlow Hub
- Matplotlib
- Numpy
- PIL
- OpenCV

## :bookmark: References
- [TensorFlow Hub](https://www.tensorflow.org/hub)
- [Faster-RCNN](https://arxiv.org/abs/1506.01497)
