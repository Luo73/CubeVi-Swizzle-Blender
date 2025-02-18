<h4 align="center">
  <img src="doc/src/512x512.png" alt="openstageAI logo" style="width:70%; ">
  
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
本插件由**OpenStageAI**开发，旨在在[**C1**](https://www.openstageai.com/companion1)上实时展示Blender内部预览结果，以及预览，光场图片本地保存。



## 版本要求

本项目是用于[**C1**](https://www.openstageai.com/companion1)的Blender插件，请确保你的电脑已经正确连接的[**C1**](https://www.openstageai.com/companion1)，教程和OpenstageAI客户端下载请[点击这里](https://www.openstageai.com/download)

**目前支持的Blender版本如下**

| Blender版本 | 下载 |
| :--- | :---: | 
| Blender3.4 | [3.4](https://download.blender.org/release/Blender3.4/) | 
| Blender3.5 | [3.5](https://download.blender.org/release/Blender3.5/) | 
| Blender3.6 | [3.6](https://download.blender.org/release/Blender3.6/) | 
| Blender4.0 | [4.0](https://download.blender.org/release/Blender4.0/) | 
| Blender4.1 | [4.1](https://download.blender.org/release/Blender4.1/) | 
| Blender4.2 | [4.2](https://download.blender.org/release/Blender4.2/) | 
| Blender4.3 | [4.3](https://download.blender.org/release/Blender4.3/) | 


**此插件目前只支持Windows系统**

## 插件安装教程
**首次安装时需要以管理权限打开blender**

请参见[教程](doc/usage.md)

## 插件使用

### 设备连接

1. 请确保您的电脑已经连接了[**C1**](https://www.openstageai.com/companion1)，同时[**OpenstageAI**](https://www.openstageai.com/download)（需保持打开），可以识别到设备
    
2. 打开blender，切换到LFD插件界面，点击单击设备连接，下方会出现连接成功字样。
    
3. 若连接失败，检查显示器是否正确显示，检查OpenStageAI软件是否识别到设备。

### 相机视锥设置

4. 通过设置相机的前，后，焦平面，可以达成不同的入屏出屏效果。

5. 远近剪裁面：只有在远近剪裁面视锥内的物体才会被渲染

6. 焦平面：相机的焦平面。在焦平面上的物体将获得最清晰的视觉展示效果。焦平面靠近相机的一侧会展示出屏效果，焦平面远离相机的一侧会展示入屏效果，远离焦平面的物体会变得模糊。

详细教程请参见：[教程](doc/usage.md)

### 实时预览：

7. 在右侧栏目中，选择”输出”，将分辨率设置为540*960或1440*2560

8. 在设备成功连接后，单击实时渲染预览,在弹出的选项框里设置图片想放置的x轴分辨率

9. 由于渲染会造成一定的性能开销，此时操作blender面板会有一定卡顿。
    使用ESC键会自动退出实时渲染。

### 保存预览图片：

 10. 在屏幕右侧的栏目中选择**输出**，在该界面更改你想要将光场图保存的路径。

 11. 单击保存宫格/光场预览图片，即可保存预览的png格式图片。

### 保存渲染图片：

 12. 单击保存视点渲染图片，即可保存40张单视角的图片。

 13. 单击合成宫格图片，即可将40张单视角图片按名称顺序合成为宫格图片。


## 限制

- 由于blender的渲染引擎限制，目前渲染帧数限制在10fps

## 讨论

如果有任何问题或者发现的漏洞请在[这里](TODO)告诉我们





