# 吴好玮 · 作品集

平面 / 视觉设计师作品集，纯静态单页应用（HTML + 原生 JS + WebP 素材，无前端框架）。

## 在线地址

- GitHub Pages：https://byunl.github.io/
- Surge 备份：https://wuhaowei.surge.sh/

## 目录结构

- `index.html`　正式版页面（样式、脚本、作品数据全部内联在这一份里）
- `canvas.html`　调参副本，与正式版内容同步
- `assets/`　作品原图、`thumbs/` 封面缩略图、站内字体
- `dbbeb964ab643b711647b000040033.txt`　微信域名验证文件，须放在站点根目录
- `build_dist.py`　本地构建脚本：生成封面缩略图、过滤未引用素材、输出 `dist/` 发布产物

## 本地预览

```
python3 -m http.server 8765
浏览器打开 http://127.0.0.1:8765/index.html
```

## 重新构建发布产物

```
python3 build_dist.py
```

产物在 `dist/`，可直接上传到任意静态托管（GitHub Pages / Surge 等）。
