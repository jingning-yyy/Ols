# OLS 回归工作台

纯前端最小二乘拟合工具（y = k·x + b，支持多自变量），GitHub Pages 在线可用：
https://jingning-yyy.github.io/Ols/

## 结构

- `index.html` — 唯一源文件，改它就行
- `xlsx.full.min.js` — Excel 解析库，必须和 index.html 同目录（挂了会自动走 CDN）
- `data/` — 示例数据，页面上的下载链接指向这里
- `local/` — 本地工具，不入库（离线单文件版、局域网服务）

## 更新

```bash
git add . && git commit -m "..." && git push   # Pages 一分钟内自动更新
```

- 算法在 index.html 的 `ALGO-START/END` 标记块内
- 离线单文件版更新：`python local/重建单文件版.py`
- 升级解析库：替换根目录的 xlsx.full.min.js
