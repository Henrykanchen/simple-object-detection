# simple-object-detection

Simple Object Detection Setup Guide

1. Git clone
2. $ cd simple-object-detection 
3 .$ virtualenv -p python3 venv 
4. $ source venv/bin/activate 
5. $ pip install -r requirements.txt 
6. $ git clone git@github.com:tensorflow/models.git <- get tensorflow models folder, cut and paste the models/research/object_detection folder into the simple-object-detection folder
7. $ protoc object_detection/protos/*.proto --python_out=. 
8. Edit tf_simple_object_detection.py
9. Replace <PATH_TO_TENSORFLOW> with <path to the simple-object-detection folder> 
10. Add the project to the venv/bin/activate of the virtualenv so the modules can be found
11. export PYTHONPATH=<path to the simple-object-detection folder>
12. $ sudo apt-get install python3-tk 
13. $ python3 tf_simple_object_detection.py 
