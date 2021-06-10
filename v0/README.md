## Model v0

### First Test
- dataset : 7800
- training time : 15h

### train
```
  python3 train.py --img 416 --batch 72 --epochs 100 --data ./dataset/data.yaml --cfg ./models/yolov5m.yaml --weights yolov5m.pt --name koren_light

```

### test
```
  python detect.py --weights ./runs/train/koren_light5/weights/best.pt --img 416 --conf 0.5 --source {}/dataset/valid/images/traffic_lights15.jpg
```

![traffic_lights15](https://user-images.githubusercontent.com/68395698/121476631-e0c95100-ca01-11eb-923e-9f7b9bd9a874.jpg)