# Face_Detection_YOLOv5

<p> This project mainly aims at pruning YOLOv5 to see how its accuracy gets affected in parallel with different pruning percentages from 10% to 40%.</p>    

<p> Pruning is the process of “Modification of weights by reducing the weights parameters, that does not impact on classification of classes”  

Yolov5 is using technique of pruning in a way that “randomly in some percentage of weights parameters, nn.conv2d layers whose weights are nearly zero, pruning converts them to zeros”. </p>

## YOLOV5 Pruning Procedure


