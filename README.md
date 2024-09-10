# DepthAnything on Browser

<img src="img/screenshot.jpg" title="screenshot" alt="screenshot" style="text-align: center">


### **Description / Rationale**
This repository demonstrates web-based implementation of <a href="https://github.com/LiheYoung/Depth-Anything">Depth Anything: Unleashing the Power of Large-Scale Unlabeled Data. Foundation Model for Monocular Depth Estimation</a>. This project demonstrates 2 implementations:
1. Basic DepthAnything, which shows only generated depth ("basic" folder)
2. Interactive DepthAnything, which shows 3D model based on generated depth and Three.js ("interactive" folder).

### **Instructions**
To use a DepthAnything example, copy the corresponding html file contents. 

To dowload and locally serve models download them from the link provided:
1. Small model: https://cdn.glitch.me/0f5359e2-6022-421b-88f7-13e276d0fb33/depthanything_vits14.onnx
2. Quantized model: https://cdn.glitch.me/0f5359e2-6022-421b-88f7-13e276d0fb33/depthanything-quant.onnx

<b>Please note:</b>
1. To increase quality, increase the input image size, for example make it 1024px.
```js
  const size = 1024; // change input size as needed
```
2. To omit points in pointcloud generated, indicate how many:
```js
 const skip = 2; // skip points here
```
3. To increase point cloud point size:
```js
gl_PointSize = 5.0; // change size here
```   
### ""Tech Stack""
The project was made possible thanks to DepthAnything repository, ONNX runtime web and Three.js.

### **Demo**
To see interactive DepthAnything at work, visit the following page: <a href="https://depthanything.glitch.me/">Demo</a>
