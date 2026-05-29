# wayoushe-site

瓦友社（VALORANT 高校社区）周年庆活动页面 — GitHub 公开镜像。

> 本仓库内容受密码保护。打开 `anniversary.html` 后输入访问密码即可查看。

## 在线访问

- GitHub Pages：<https://zhanggqtc.github.io/wayoushe-site/anniversary.html>
- 工蜂主仓（内网）：`markgqzhang/wayoushe-site`

## 安全说明

- HTML 内容使用 **AES-256-GCM** 加密，密钥由密码经 **PBKDF2-HMAC-SHA256（200000 轮）** 派生。
- 密码本身不存储在任何文件里，浏览器也只在 `sessionStorage` 中临时缓存（关闭标签即清除）。
- `view-source` 仅可见加密后的 base64 密文与解密代码，无法直接还原内容。
- 如需访问，请向仓库所有者索取密码。

## 同步策略

- 工蜂 `markgqzhang/wayoushe-site`：明文版，CVM 内网自动部署到 wayoushe.woa.com（仅腾讯内网账号可访问）。
- GitHub `zhanggqtc/wayoushe-site`：加密版，仅 `anniversary.html` 一个文件。
