# Dockerfile_collection
collection of Dockerfile.



- [x]  cuda10.1-cudnn7-tenorrt6.0.1.5
- [x] Yolov4-trt-deployment
- [ ] YOLOv4-darknet: `train/detect`
  - For YOLOv4-darknet model training
  - For YOLOv4-darknet model deploy
- [ ] tfod-train-1.15.2
  - TensorFlow1.15.2 object detection training image.
- [ ] ...





### YOLOv4-trt-deployment usage
> Thanks for the nice repo. from [jkjung-avt](https://github.com/jkjung-avt/tensorrt_demos), where almost all `*.py` codes borrown from.


default starting the container effctively behave as
```shell
docker run -itd -p 11221:5000 --name yolotrt512 --gpus '"device=5"' yolov4/deploy:trt -m yolov4-512
```

You can simply change the `CMD` in the `CLI` as:

```shell
docker run -itd -p 11221:5000 --name yolotrt512 --gpus '"device=5"' yolov4/deploy:trt -m yolov4-416
```

or using `yolov4-608`.

### TFOD1.15.2
refer to [tensorflow/models](https://github.com/tensorflow/models/tree/master/research/object_detection)



