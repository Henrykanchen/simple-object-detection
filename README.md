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
8. Edit tf_simple_object_detection.py
9. Replace sys.path.append(<PATH_TO_TENSORFLOW>) with 'pwd/object_detection'
10. Open the venv/bin/activate file, add the line
        export PYTHONPATH='pwd'

12. $ sudo apt-get install python3-tk 
13. $ python3 tf_simple_object_detection.py 
