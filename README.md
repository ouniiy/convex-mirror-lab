# 凸面镜实验室

浏览器中的凸面镜创作工具：上传或拍摄照片、模拟凸面反射、按压凹陷、自由绘画、独立贴纸编辑和图片导出。

## 使用

通过 GitHub Pages 打开网页。点击上传照片，在装饰面板选择贴纸，可拖动、缩放和旋转。导出时先生成图片，再选择保存／分享、下载或长按图片保存。

## 本地预览

需要通过本地静态服务器运行，不能直接双击 HTML 文件：

```bash
python3 -m http.server 8000
```

打开 http://localhost:8000。

## 文件

- `index.html`：界面
- `style.css`：样式
- `app.js`：编辑交互
- `mirror3d.js`：镜体渲染
- `exporter.js`：图片生成与保存
- `stickers.json`、`sticker-*.png`：贴纸索引与素材
- `mirror-icon.svg`、`mirror-icon.png`：应用图标

照片在访问者的浏览器内处理，不上传服务器。

贴纸来自用户提供的素材；本仓库未为这些第三方素材授予额外许可。
