# wayoushe-site

瓦友社（VALORANT 高校社区）活动页面 — GitHub 公开镜像。

> 本仓库内容受密码保护。打开对应页面后输入访问密码即可查看。

## 在线访问

- 站点主页（活动导航）：<https://zhanggqtc.github.io/wayoushe-site/>
- 返校集结活动页（公开）：<https://zhanggqtc.github.io/wayoushe-site/campus-assembly.html>
- 周年庆活动页（密码）：<https://zhanggqtc.github.io/wayoushe-site/anniversary.html>
- 开学季活动规则（密码）：<https://zhanggqtc.github.io/wayoushe-site/activity-rules.html>
- 2026全国大赛H2 报名工具（密码）：<https://zhanggqtc.github.io/wayoushe-site/h2-signup.html>
- 冠军玩家报名（密码）：<https://zhanggqtc.github.io/wayoushe-site/champions-player-entry.html>
- 工蜂主仓（内网）：`markgqzhang/wayoushe-site`

## 页面说明

- `campus-assembly.html` — 返校集结活动页（**公开**，无需密码），含新生 / 老生 / 先锋三条线与校友链接、摆摊申请。
- `anniversary.html` — 周年庆活动页（加密）。
- `activity-rules.html` — 开学季「活跃特权」活动资源使用规则图（加密），含临时活动版（1 个月）与长期赛季版（3 个月，类三角洲 3×3 安全箱）两套方案。
- `h2-signup.html` — 2026全国大赛H2 报名工具（加密）。
- `champions-player-entry.html` — 冠军玩家报名（加密）。

## 安全说明

- HTML 内容使用 **AES-256-GCM** 加密，密钥由密码经 **PBKDF2-HMAC-SHA256（200000 轮）** 派生。
- 密码本身不存储在任何文件里，浏览器也只在 `sessionStorage` 中临时缓存（关闭标签即清除）。
- `view-source` 仅可见加密后的 base64 密文与解密代码，无法直接还原内容。
- 如需访问，请向仓库所有者索取密码。

## 同步策略

- 工蜂 `markgqzhang/wayoushe-site`：明文版，CVM 内网自动部署到 wayoushe.woa.com（仅腾讯内网账号可访问）。
- GitHub `zhanggqtc/wayoushe-site`：加密版，含 `anniversary.html`、`activity-rules.html`、`h2-signup.html`、`champions-player-entry.html`；`campus-assembly.html` 为明文公开页（已获授权对外发布，供外部设计师查看），并由 `index.html` 站点主页聚合导航。
