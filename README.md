# Epic Free Push
automatic Email notification for epic free games.

## quick start
> https://blog.yunyuyuan.net/articles/5888

# Epic Free Push – 环境变量备忘

> 更新时间：2025-09-04  

| 变量名            | 说明                          | 示例 / 备注 |
|-------------------|-------------------------------|-------------|
| `NOTIFY_TITLE`    | 通知标题（邮件、TG、Gotify 共用） | `Epic Free Games` |
| `GOTIFY_URL`      | Gotify 服务器根地址            | `https://gotify.example.com` |
| `GOTIFY_TOKEN`    | Gotify **应用令牌**            | `xxx` |
| `ADDRESS`         | **发件人** 邮箱（163）    | `xxx@example.com` |
| `CODE`            | 发件人邮箱 **SMTP 授权码**      | `xxxxxxxxxxxx` ⚠️ 不是登录密码 |
| `TGBOT_TOKEN`     | Telegram Bot **HTTP API 令牌** | `1000000000:AHmBo7...NV-_40XwwN4` |
| `TGBOT_CHAT_ID`   | TG 接收消息的用户/群组 ID       | `1000000000` |
| `RECIVE`          | **收件人** 邮箱（可和 `ADDRESS` 相同或不同） | `xxx@example.com` |

---

### 更新指引
1. **修改邮箱或授权码** → 仅替换 `ADDRESS` 与 `CODE` 即可。  
2. **更换收件人** → 仅替换 `RECIVE`。  
3. **ENV_VAR**  → 
把以下内容整段保存到 `ENV_VARS` 即可，一行一个，无引号、无空格：
ADDRESS=xxx@example.com
CODE=xxxxxxxxxxxx
RECEIVE=xxx@example.com

> 更新后请 **重新触发一次 Action** 验证配置正确。
