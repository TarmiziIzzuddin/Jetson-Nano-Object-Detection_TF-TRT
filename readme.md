# Object detection for Jetson Nano using Tensorflow

This repo provides example on the real time implementation of object detection from a camera connected to a jetson nano, using tensorflow. Model in used is mobilenet_ssd_v2 trained using COCO dataset. Model is first optimized from a  using NVidia TensorRT (Tensorflow TF-TRT) refer to https://github.com/NVIDIA-AI-IOT/tf_trt_models for steps and examples optimized frozen tensorflow graph. An object detection performance of around 15-20 FPS should be obtained using this method.

Optimized model can also be downloaded below:

https://drive.google.com/open?id=1RnNBHPDphIOWwHCSfeMCWQ7XN3w3tKFD


# Other requirements

* Tensorflow
* Matplotlib
* OpenCV
* Jetbot https://github.com/NVIDIA-AI-IOT/jetbot (for creating camera instance - Internally, the Camera class uses GStreamer to take advantage of Jetson Nano's Image Signal Processor (ISP). This is super fast and offloads a lot of the resizing computation from the CPU. ) 
