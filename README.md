![Darknet Logo](http://pjreddie.com/media/files/darknet-black-small.png)

#Darknet#
Darknet is an open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.

For more information see the [Darknet project website](http://pjreddie.com/darknet).

For questions or issues please use the [Google Group](https://groups.google.com/forum/#!forum/darknet).

# Added by jskang
* List function to do multiple images given a list of filenames
* List function does not generate images, instead it prints out bounding boxes for
each image
* Uses YOLOv2 544x544 config and weights file

Example:
```
./darknet yolo list cfg/yolo-voc.cfg yolo-voc.weights files.list
```
```
data/dog.jpg: Predicted in 0.011297 seconds.
car, 0.827306, 242, 91, 366, 147
dog, 0.913729, 64, 149, 174, 348
bicycle, 0.845698, 66, 131, 300, 288
```
