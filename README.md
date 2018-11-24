# simple-object-detection

Simple Object Detection Setup Guide

Git clone
$ cd simple-object-detection 
$ virtualenv -p python3 venv 
$ source venv/bin/activate 
$ pip install -r requirements.txt 
$ git clone git@github.com:tensorflow/models.git <- get tensorflow models folder, cut and paste the models/research/object_detection folder into the simple-object-detection folder
$ protoc object_detection/protos/*.proto --python_out=. 
Edit tf_simple_object_detection.py
Replace <PATH_TO_TENSORFLOW> with <path to the simple-object-detection folder> 
Add the project to the venv/bin/activate of the virtualenv so the modules can be found
export PYTHONPATH=<path to the simple-object-detection folder>
$ sudo apt-get install python3-tk 
$ python3 tf_simple_object_detection.py 
