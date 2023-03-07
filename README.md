# Face_Detection_YOLOv5

<p> This project mainly aims at pruning YOLOv5 to see how its accuracy gets affected in parallel with different pruning percentages from 10% to 40%.</p>    

<p> Pruning is the process of “Modification of weights by reducing the weights parameters, that does not impact on classification of classes”  

Yolov5 is using technique of pruning in a way that “randomly in some percentage of weights parameters, nn.conv2d layers whose weights are nearly zero, pruning converts them to zeros”. </p>

## YOLOV5 Pruning Procedure
* Clone [YOLOv5](https://github.com/ultralytics/yolov5.git) model 
* Train the model on your custom dataset
* Validate the model on a test subset using val.py file
* Copy best.py file and store it in another folder, as pruning will overwrite this file
* Edit the val.py file adding the pecentage of pruning you want before configure part as [here](https://medium.com/nerd-for-tech/how-to-prune-sparse-yolov5-da19e1d84a6) 
*       from utils.torch_utils import prune
        prune(model,0.3)  ## 0.3 is pruning 30% of the weights 
* Validate the model again with val.py and compare the rersults

