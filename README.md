# 🎄 AI Gesture Controlled 3D Christmas Tree

一个基于 Web 前端技术的互动 3D 圣诞树。通过电脑摄像头识别手势，控制圣诞树的聚拢、散开、旋转以及查看悬浮照片。

[在这里插入你的演示截图或GIF]

## ✨ 特性 (Features)

- **AI 手势识别**: 使用 MediaPipe Hands 实现无接触交互。
- **3D 粒子系统**: 基于 Three.js 构建的数千个发光粒子和照片平面。
- **后期辉光特效**: 集成 UnrealBloomPass 实现电影级黑金辉光效果。
- **交互式动画**:
  - 🖐 **张开手掌**: 圣诞树炸裂散开，进入浏览模式。
  - ✊ **握拳/自然**: 粒子聚拢成树，自动旋转。
  - 👆 **手指悬停**: 在散开模式下，照片会自动吸附到屏幕中央放大。
- **自适应布局**: 适配不同尺寸的屏幕。

## 🛠️ 技术栈 (Tech Stack)

- **HTML5 / CSS3**
- **JavaScript (ES6+)**
- **[Three.js](https://threejs.org/)** - 3D 渲染引擎
- **[MediaPipe Hands](https://google.github.io/mediapipe/)** - 计算机视觉手势识别

## 🚀 如何运行 (How to Run)

由于浏览器的安全策略（CORS），本项目不能直接双击 `index.html` 打开，必须运行在本地服务器上。

### 方法 1: 使用 VS Code (推荐)
1. 安装 VS Code 插件 **Live Server**。
2. 右键点击 `index.html`，选择 **"Open with Live Server"**。

### 方法 2: 使用 Python
如果你安装了 Python，在项目根目录下运行终端命令：
```bash
# Python 3.x
python -m http.server 8000
## 自定义图片功能
下载整个文件之后点击assets文件夹，将想要展示的图片导入其中，并按规律进行命名如：1.png/1.jpg 以此类推。
找到index.html中的配置区 大概95行左右 找到const IMAGE_URLS ，将‘’中的图片名称进行更换再保存启动即可。
