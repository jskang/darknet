![Darknet Logo](http://pjreddie.com/media/files/darknet-black-small.png)

#Darknet#
Darknet is an open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.

For more information see the [Darknet project website](http://pjreddie.com/darknet).

For questions or issues please use the [Google Group](https://groups.google.com/forum/#!forum/darknet).

I added capabilities to run detection on multiple images on a single run
./darknet yolo list cfg/yolo-voc.cfg yolo-voc.weights files.list

the list function does not generate pictures, it prints out bounding boxes for
each image and detection.

example:
'''
data/dog.jpg: Predicted in 0.011297 seconds.
car, 0.827306, 242, 91, 366, 147
dog, 0.913729, 64, 149, 174, 348
bicycle, 0.845698, 66, 131, 300, 288
'''
