# CDP Extension 使用说明
这是一个通过cdp自动点击所有cf turnstile验证码的chrome extension脚本
按照下面步骤把扩展安装到 Chrome（或 Chromium）浏览器：

1. 下载 ZIP
   - 将本项目打包为 ZIP 并下载到本地。

2. 打开扩展管理页
   - 在 Chrome 地址栏输入 `chrome://extensions` 并回车。

3. 启用开发者模式
   - 右上角打开「开发者模式」（Developer mode）。

4. 拖放安装 ZIP
   - 将下载好的 ZIP 文件解压后的文件夹拖拽到扩展管理页面上。
   - Chrome 会自动识别并安装该扩展。

5. 使用与验证
   - 安装后，打开目标网页（例如包含 Cloudflare/Turnstile 验证的页面），扩展会在合适的 iframe 内注入脚本并按逻辑工作。
   - 如需调试，可查看扩展页面中的背景页（background）日志或打开 DevTools 查看注入脚本的输出。
   - chrome 烦人的弹窗可以用 --silent-debugger-extension-api 来去除
