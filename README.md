# MOD-Licenses

MOD 插件的公开在线授权名单。插件通过固定的 `raw.githubusercontent.com` 地址匿名读取 `authorized-machines.json`，不占用 GitHub REST API 的匿名请求额度。

安全约束：

- 这里只保存 `SHA256:...` 形式的加盐机器码哈希，不保存原始机器码。
- 不要提交 GitHub Token、私钥、邮箱或客户隐私信息。
- `expiresOn` 必须存在并使用 `yyyy-MM-dd`；只有显式 `null` 表示永久授权。
- 停用授权时把 `enabled` 改为 `false`，并保留 `product` 为 `MOD`。

编辑清单后，在 Rhino 中运行 `MOD_License` 并点击“立即联网刷新”。