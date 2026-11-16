# WebHome

本目录为 BMCU 的 Web 发布目录，可直接用于 GitHub Pages 或本地 http.server。

- index.html — 入口
- flasher.html — 在线刷写（Web Serial + WCH ISP，需 Chrome/Edge，HTTPS 或 localhost）
- guide.html — 设置指南（与 docs 同步）
- firmware/ — 固件二进制（当前 11.1.0-TYC.1）
- js/wch-isp.js — 前端 ISP 实现（与 bmcu_flasher.py 同源，持续完善中）

本地预览：
```
cd webhome
python -m http.server 8000
```
然后访问 http://localhost:8000/

在线更新：推送新固件到 firmware/ 并更新 flasher.html 的下拉列表即可。
