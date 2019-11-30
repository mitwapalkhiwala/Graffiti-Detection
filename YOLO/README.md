# YOLO

https://modelzoo.co/model/yolo-tensorflow

* Created tiny-yolo-voc-text.cfg

modified line 114 filters = 105
modfified line 120 classes = 16

* Modified labels.txt with labels

* Train model using 

flow --model cfg/tiny-yolo-voc-text.cfg --load tiny-yolo-voc.weights --train --annotation train/annotations --dataset train/Images


* Prediction

 flow --model cfg/yolo_text.cfg --imgdir Test_Text/ --load 11500 --labels labels.txt 
