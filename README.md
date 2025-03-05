<h4 align="center">
  <img src="doc/src/512x512.png" alt="openstageAI logo" style="width:15%; ">
  
<h1 align="center">CubeVi-Swizzle-Blender</h1>

</h3>




[![OpenStageAI](https://img.shields.io/badge/OpenStageAI-web-blue)](https://www.openstageai.com/)
[![Blender](https://img.shields.io/badge/Blender-download-red)](https://www.blender.org/download/)
[![Chat](https://img.shields.io/badge/chat-discord-blue)](https://discord.gg/kAucVzbvQM)
[![Chat](https://img.shields.io/badge/chat-Wechat-yellow)](TODO)
 <!-- this badge is too long, please place it in the last one to make it pretty --> 

<p align="center">
    👋 加入我们的 <a href="TODO" target="_blank">WeChat</a> 和 <a href="https://discord.gg/kAucVzbvQM" target="_blank">Discord</a> 
</p>

## 项目介绍
本插件由**CubeVi**开发，旨在在[**光场显示屏产品**](https://www.openstageai.com/companion1)上实时展示Blender预览结果，进行预览和渲染图像/动画的保存和上传。



## 版本要求

本项目是用于[**光场显示屏产品C1**](https://www.openstageai.com/companion1)的Blender插件，请确保你的电脑已经正确连接[**光场显示屏C1**](https://www.openstageai.com/companion1)，教程和OpenstageAI客户端下载请[点击这里](https://www.openstageai.com/download)

**目前支持的Blender版本如下**

| Blender版本 | 下载 |
| :--- | :---: | 
| Blender3.4 | [3.4](https://download.blender.org/release/Blender3.4/) | 
| Blender3.5 | [3.5](https://download.blender.org/release/Blender3.5/) | 
| Blender3.6 | [3.6](https://download.blender.org/release/Blender3.6/) | 
| Blender4.0 | [4.0](https://download.blender.org/release/Blender4.0/) | 
| Blender4.1 | [4.1](https://download.blender.org/release/Blender4.1/) | 
| Blender4.2 | [4.2](https://download.blender.org/release/Blender4.2/) | 
注：Blender4.3自身API调用存在bug，导致预览结果中纹理部分会出现偏移，仅可正常输出渲染图像。
| Blender4.3 | [4.3](https://download.blender.org/release/Blender4.3/) | 


**此插件目前只支持Windows系统**

## 插件安装教程

安装及详细教程请参见[教程](doc/usage.md)

## 插件使用

### 设备连接

1. 请确保您的电脑已经连接了[**光场显示屏设备**](https://www.openstageai.com/companion1)，同时打开[**OpenstageAI**](https://www.openstageai.com/download)平台（平台需更新到最新版本），可以识别到设备。
    
2. 打开blender，在编辑->偏好->插件部分，导入插件zip文件安装包，安装成功后，在右侧可以看到LFD面板。
    
3. 单击面板中的连接，提示连接成功，并自动设置相机分辨率。

### 相机设置

4. 通过设置相机的前，后，焦平面，可以达成不同的入屏出屏效果。

5. 远近剪裁面：只有在远近剪裁面视锥内的物体才会被渲染

6. 焦平面：相机的焦平面。在焦平面上的物体将获得最清晰的视觉展示效果。焦平面靠近相机的一侧会展示出屏效果，焦平面远离相机的一侧会展示入屏效果，远离焦平面的物体会变得模糊。


### 预览界面：

7. 在设备成功连接后，单击实时光场预览，会自动在C1上显示当前相机的光场预览图片。

8. 单击保存宫格预览图片，会在当前设置的文件路径下保存宫格预览图片。

9. 单击保存光场预览图片，会在当前设置的文件路径下保存光场预览图片。

### 渲染：

 10. 在设备成功连接后，点击保存视点预览图片，相机会自动在当前位置拍摄40张单视点图片（ESC取消)，在当前设置的文件路径下命名为_000.png - _039.png.

 11. 在40张单视点图片渲染完成后，单击合成宫格图片，会自动将_000.png - _039.png合成为一张多视点宫格图

 12. 在设备成功连接，平台打开的情况下，单击上传宫格图到3D图库，会将多视点宫格图上传到3D图库中，打开3D图库->头像->我的创作 即可观看该宫格图生成的光场图。 （宫格图最大大小为70MB)

### 渲染动画：

 13. 设置动画渲染的开始帧-结束帧， 单击渲染动画(ESC取消)，会自动将开始帧-结束帧的每帧宫格图渲染完成, 命名并保存到当前文件路径下的 quilt_frame_帧数.png

 14. 设置动画渲染的开始帧-结束帧，设置输出视频的fps，单击将宫格图序列合成为视频，插件将把开始帧-结束帧的宫格图合成为output.mp4.

 15. 单击将视频上传到3D图库，会将宫格图视频上传到3D图库中，打开3D图库->头像->我的创作 即可观看该光场视频。 （视频最大大小为70MB)



## 限制

- 由于blender的渲染引擎限制，对于带纹理细节的场景，进行实时光场预览时会较为卡顿。
- 目前上传平台的，可供公开的宫格图和宫格图视频大小限制为70MB。

## 讨论

如果有任何问题或者发现的漏洞请在[这里](TODO)告诉我们





