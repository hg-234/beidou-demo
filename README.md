# 溯源·北斗 演示系统 · GitHub Pages 部署包

本文件夹用于部署到 GitHub Pages，生成**永久、无广告**的公网访问地址，供答辩二维码使用。

## 文件
- `index.html` ...... 主演示系统（已将其 iframe 引用的伪3D 文件改为 `beidou-3d.html`）
- `beidou-3d.html` ... 伪3D 实景推演页
- `.nojekyll` ........ 关闭 GitHub Pages 的 Jekyll 处理（避免潜在解析问题）

## 部署步骤
1. 在 GitHub 新建一个**空**仓库（如 `beidou-demo`），不要勾选 README/.gitignore。
2. 将本文件夹全部内容推送为该仓库的 `main` 分支（见 `deploy 说明`）。
3. 仓库 `Settings → Pages → Build and deployment → Source` 选 `Deploy from a branch`，分支选 `main`、目录选 `/ (root)`，保存。
4. 等待约 1 分钟，访问 `https://<你的用户名>.github.io/beidou-demo/` 即为永久地址。
5. 用仓库里准备的二维码脚本（或把地址发给助手）重生成指向该地址的 `demo_qr.png`，拖进 PPT。

> 注：部署出去的是参赛演示件（纯模拟数据、非隐私），属对外展示。