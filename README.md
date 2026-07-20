# LM Design · SV16.4 Desktop Optimized

GitHub Pages 静态发布包，桌面端画质优先，已针对浏览器上传和首屏稳定性优化。

## 发布入口

- `index.html`：仓库根入口
- `portfolio-sv16.4.html`：独立版本入口
- `.nojekyll`：必须上传到仓库根目录

## 关键修复

- Hero 失败回退已替换为深水视频真实帧，不再包含旧俄文美容页面 `hero.jpg`。
- 主脚本与媒体 URL 使用版本 `20260720-web3`，降低旧缓存误加载风险。
- 视频统一检查 H.264 / faststart，大文件按 1080p / 30fps / CRF 25 优化。
- 大图转换为高质量 WebP，视觉规范图保留更高质量。

## 浏览器分批上传

使用旁边的 `LM-Design-SV16.4-GitHub-Desktop-Optimized-WEB-UPLOAD` 目录：

1. 先上传 `01-CORE` 中的全部内容到仓库根目录并提交。
2. 再严格按编号逐批上传 `02-MEDIA-*`、`03-MEDIA-*`……到同一仓库根目录，每批单独提交。
3. 上传文件夹本身，不要上传 ZIP；必须保留 `media/...` 相对目录。
4. 全部完成后在 Settings → Pages 选择 `Deploy from a branch / main / root`。

完整包大小：45.46 MiB。
