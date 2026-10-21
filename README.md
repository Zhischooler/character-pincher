# 人物捏捏乐

一个纯前端、可部署到 GitHub Pages 的人物捏脸小游戏。

## 功能

- `src/` 自动发现人物图片
- GitHub Actions 自动生成 `characters.js`
- Canvas 人物捏捏
- 橡皮泥模式：使用平滑局部网格形变，保持整体轮廓更自然
- 可直接上传图片
- 撤销 / 重做 / 重置
- 导出 PNG
- 鼠标、触摸操作
- 响应式 UI
- 无后端、无需数据库

## 变动日志

- 2026-10-20 `增加直接上传图片选项`

## 使用

把 PNG/JPG/WebP 人物图片放入 `src/`，例如：

```text
src/
├── 小明.png
├── 小红.png
└── character3.webp
```

提交到 GitHub 后，Actions 会自动扫描图片并生成 `characters.js`。

然后在仓库 Settings → Pages 中选择 GitHub Actions 作为部署方式。



或者直接上传图片，但这是一次性的。



## 本地预览


- 使用前，请确保你已安装Python

浏览器对本地文件的模块/资源加载有限制，推荐启动本地服务：

```bash
python -m http.server 8080
```

然后打开：

```text
http://localhost:8080
```
