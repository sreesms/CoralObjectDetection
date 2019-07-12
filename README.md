# CoralObjectDetection
Coral Object detection model compiled for Edge TPU.

Pretrained model obtained from https://www.tensorflow.org/lite/models.

From Host computer execute :

$ edgetpu_compiler model_name
 
 A model file will be created by the Edge TPU compiler. Copy the model into the Coral Development board.
 
## To do the object detection execute this in the Coral Development board :

python3 object_detection.py --model ~/CoralObjectDetection/detect_edgetpu.tflite --input ~/parrot.jpg
