# 滑动变阻器 · AI 连续版（Android 应用）

手机端独立应用版：**241 帧逐帧进化，从「小难梁」到「梁祖」，离线可用，随时下载**。

## ✨ 特点

- 🎚️ **241 档调节**：滑杆逐帧 scrub，0.125 级步进，30 级 6 阶段（小难梁→牢梁→梁子→梁圣→梁神→梁祖）
- 📱 **手机随时下载使用**：GitHub Releases 直接下载 APK 安装，无需服务器、无需网络
- 🎬 **AI 连续插帧**：OpenAI Image2 首尾帧 + MiniMax H3 FL2VA 连续插帧，原生连续进化
- 📴 **完全离线**：页面 + 视频全部内嵌 assets，无任何权限申请

## 📲 下载安装

打开 [Releases](https://github.com/Cuiyi-Srama/liang-intensity-calibrator-app/releases) 下载最新 APK，手机直接安装即可。

## 🛠️ 技术架构

- WebView 壳 + [WebViewAssetLoader](https://developer.android.com/reference/androidx/webkit/WebViewAssetLoader)（https 虚拟域映射 assets，保证视频 Range seek 正常）
- AndroidX WebKit 1.14 / AppCompat 1.6 / minSdk 24 / targetSdk 34
- 静态资源完全来自 [HunLuanZhiZhu/liang-intensity-calibrator](https://github.com/HunLuanZhiZhu/liang-intensity-calibrator)（致敬 [Lichtspektrum 原项目](https://github.com/Lichtspektrum/liang-intensity-calibrator)）

## 🔨 本地构建

```bash
gradle :app:assembleDebug --no-daemon
```

## ⚖️ 许可

壳代码 MIT；页面/视频素材版权归原作者所有（AI 生成内容，使用请遵守平台条款）。
