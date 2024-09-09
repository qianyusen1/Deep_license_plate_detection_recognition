# Deep_license_plate_detection_recognition
The previous one missed, so i have to reupload it


**环境要求: python >=3.6  pytorch >=1.7**
直接运行detect_plate.py 或者运行如下命令行：

```
python detect_plate.py --detect_model weights/plate_detect.pt  --rec_model weights/plate_rec_color.pth --image_path imgs --output result
```

测试文件夹imgs，结果保存再 result 文件夹中
python detect_plate.py --detect_model weights/plate_detect.pt  --rec_model weights/plate_rec_color.pth --video 2.mp4
python onnx_infer.py --detect_model weights/plate_detect.onnx  --rec_model weights/plate_rec_color.onnx  --image_path imgs --output result_onnx
```

3.**tensorrt** 部署见[tensorrt_plate](https://github.com/we0091234/chinese_plate_tensorrt)

4.**openvino demo** 版本2022.2

```
 python openvino_infer.py --detect_model weights/plate_detect.onnx --rec_model weights/plate_rec.onnx --image_path imgs --output result_openvino
```

