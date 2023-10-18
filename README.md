# HIRAC-dataset

This dataset is a combination of multiple open source datasets from Roboflow: 
- https://universe.roboflow.com/vision-gxbqw/tazas-y-vasos
- https://universe.roboflow.com/shehab-emad-n2q9i/keysdetection/dataset/2
- https://universe.roboflow.com/sergey-menshikov/pen-suawu
- https://universe.roboflow.com/pen-rgrwx/pen-ufs
- https://universe.roboflow.com/dwi/pen-ctcrc
- https://universe.roboflow.com/taitora8002-yahoo-co-jp/yolo_pen/dataset/1

The data was used to train YOLOv5n to detect cups, glasses, pens and keys. Some of the bounding boxes were modified to fit tighter around each object.

Results after 40 epochs of training: 
| Image size  | Precision | Recall | mAP* all | mAP* keys | mAP* pen | mAP* cup | mAP* glass | FPS** |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| 640x640  | 0.954  | 0.954  | 0.775  | 0.782  | 0.666  | 0.825  | 0.83  | 487.8 |

*mAP50-95

** 1000 / (preprocess + inference + postprocess speed in ms)


![alt text](https://github.com/katrinmisel/HIRAC/blob/main/images/det_test.png?raw=true)

[![DOI](https://zenodo.org/badge/704862418.svg)](https://zenodo.org/doi/10.5281/zenodo.10017033)
