# simple-object-detection

Simple Object Detection Setup Guide

1. Git clone this repository 
2. $ cd simple-object-detection 
3. $ virtualenv -p python3 venv 
4. $ source venv/bin/activate 
5. $ pip install -r requirements.txt 
6. $ git clone git@github.com:tensorflow/models.git <- copy the models/research/object_detection folder to repository; 
delete models folder
7. $ protoc object_detection/protos/*.proto --python_out=. 
8. Go to https://github.com/bourdakos1/Custom-Object-Detection/blob/master/object_detection/g3doc/detection_model_zoo.md; download pre-trained model; extract folder to your repository; remove everything other than the .pb file
        
9. go to http://www.cvlibs.net/datasets/kitti/raw_data.php?type=campus; download your dataset; extract to the images folder
10. Edit tf_simple_object_detection.py
..*modify PATH_TO_TEST_IMAGES_DIR to your dataset
..*replace /home/hc/github/simple-object-detection/ with path of your repository
11. Open the venv/bin/activate file, add the line
..*export PYTHONPATH=path_to_your_repository

12. $ python3 tf_simple_object_detection.py 
