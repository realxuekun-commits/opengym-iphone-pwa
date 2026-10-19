openGym 个人本机 PWA
====================

这是 VITE_DEMO=1 的静态访客模式构建：
- 不需要账号
- 不请求 openGym API
- 训练数据写在当前浏览器的 localStorage
- 需要通过 HTTPS 访问，Service Worker 才能提供离线启动

iPhone 使用：
1. 将本目录部署到 HTTPS 静态站点。
2. 用 iPhone Safari 打开并等待首次加载完成。
3. 分享 -> 添加到主屏幕 -> 作为 Web App 打开。
4. 首次点击“开始演示”。
5. Settings -> Data & backup -> Reset everything 清除预置示例数据。
6. 训练后定期 Export backup。

注意：这是 Safari PWA，不是 Capacitor 原生 App；没有 opengym-state.json 文件镜像，也没有原生本地通知。清除 Safari 网站数据或设备重置可能删除未导出的数据。
详见同目录外的 opengym-local-pwa-deployment.html。
