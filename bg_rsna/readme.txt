##############################################################Resultados de entrenamiento de Yolov5s###########################################################################
Aquí se encuentran los resultados del entrenamiento de la arquitectura yolov5s proporcionada en https://github.com/ultralytics/yolov5 


Se entreno usando los datos de rsna desechando la clase de los pacientes sin opacidad y usando esas imagenes como imagenes de fondo (sin daño alguno) por lo que no cuentan con bboxes asociados, la clase restantes que si cuentan con anotacion de bboxes [c13] se ditribuyo de forma uniforme dentro de cada conjunto utilizado es decir train=0.8c1
validation=0.1c1 y test validation=0.1c1.

train: weights=yolov5s.pt, cfg=, data=dataset.yml, hyp=data/hyps/hyp.scratch-low.yaml, epochs=500, batch_size=16, imgsz=640, rect=False, resume=False, nosave=False, noval=False, noautoanchor=False, noplots=False, evolve=None, bucket=, cache=None, image_weights=False, device=, multi_scale=False, single_cls=False, optimizer=SGD, sync_bn=False, workers=8, project=runs/train, name=exp, exist_ok=False, quad=False, cos_lr=False, label_smoothing=0.0, patience=100, freeze=[0], save_period=-1, seed=0, local_rank=-1, entity=None, upload_dataset=False, bbox_interval=-1, artifact_alias=latest
github: up to date with https://github.com/ultralytics/yolov5 ✅
YOLOv5 🚀 v7.0-249-gf400bba Python-3.11.5 torch-2.1.1+cu118 CUDA:0 (NVIDIA GeForce RTX 3090 Ti, 24214MiB)

hyperparameters: lr0=0.01, lrf=0.01, momentum=0.937, weight_decay=0.0005, warmup_epochs=3.0, warmup_momentum=0.8, warmup_bias_lr=0.1, box=0.05, cls=0.5, cls_pw=1.0, obj=1.0, obj_pw=1.0, iou_t=0.2, anchor_t=4.0, fl_gamma=0.0, hsv_h=0.015, hsv_s=0.7, hsv_v=0.4, degrees=0.0, translate=0.1, scale=0.5, shear=0.0, perspective=0.0, flipud=0.0, fliplr=0.5, mosaic=1.0, mixup=0.0, copy_paste=0.0



Transferred 343/349 items from yolov5s.pt
AMP: checks passed ✅
optimizer: SGD(lr=0.01) with parameter groups 57 weight(decay=0.0), 60 weight(decay=0.0005), 60 bias
train: Scanning /home/jair/COVID/YOLO/datasets/coco/labels/train.cache... 4791 i
val: Scanning /home/jair/COVID/YOLO/datasets/coco/labels/validation.cache... 580

AutoAnchor: 4.71 anchors/target, 1.000 Best Possible Recall (BPR). Current anchors are a good fit to dataset ✅
Plotting labels to runs/train/exp/labels.jpg... 
Image sizes 640 train, 640 val
Using 8 dataloader workers
Logging results to runs/train/exp
Starting training for 500 epochs...


Stopping training early as no improvement observed in last 100 epochs. Best results observed at epoch 102, best model saved as best.pt.

203 epochs completed in 10.447 hours.
Optimizer stripped from runs/train/exp/weights/last.pt, 14.4MB
Optimizer stripped from runs/train/exp/weights/best.pt, 14.4MB

Validating runs/train/exp/weights/best.pt...
Fusing layers... 
Model summary: 157 layers, 7012822 parameters, 0 gradients, 15.8 GFLOPs
                 Class     Images  Instances          P          R      mAP50   
                   all       2647        956      0.466      0.529      0.468      0.149
Results saved to runs/train/exp



