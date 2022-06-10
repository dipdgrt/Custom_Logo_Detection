# Custom_logo_detection
Detection of only Allianz logo from Images
# Dataset
Collected Allianz images from open source and with help of labelimg package manually annotate the bounding boxes
# Model Traing

Used the TFOD2 pipeline from github
used the object detection API's and used ssd Resnet101 from tfod2zoo "https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md" for custom training my model
Converted the annotated image .xlm files to .record by generate_tfrecords.py for trainig 
In a my_model/my_ssd_resnet101_v1_fpn folder saved the custom pipeline.config file for taining 
custom model started training with model_main_tf2.py 
After traing the model weights and check point are saved for further tuning and model is saved to save_model.pb with xporter_main_v2.py
# Inferencing
Used the Inferencing function to visualize the bounding boxes and detection score and also crop the detected bounding box and display and it can be further saved.


