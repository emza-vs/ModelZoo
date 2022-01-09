# ModelZoo
Set of object detection ML models optimized for ultra low power edge devices.

# Face detection: 

yolo-fastest_192_face_v4.tflite

This project is a full implementation of face detection model running on Arm micro NPU Ethos U55.

The CNN model is based on:

https://github.com/dog-qiuqiu/Yolo-Fastest

dog-qiuqiu. (2021, July 24). dog-qiuqiu/Yolo-Fastest: yolo-fastest-v1.1.0 (Version v.1.1.0). Zenodo. http://doi.org/10.5281/zenodo.5131532


We trained the model for face detection with private and public datasets including: Wider (http://shuoyang1213.me/WIDERFACE/) and our private datasets.

Input image 192x192x1 (grayscale).

Quantization method is standard TFLM, INT8.

The model is running on Arm virtual platform, execution time for single frame inference is (in U55 128 MACs configuration): 5.4 ms (vela compiler).
