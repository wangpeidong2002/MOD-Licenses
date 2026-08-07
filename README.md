# MOD-Licenses

MOD 插件的公开在线授权名单。插件通过 GitHub Contents API 匿名读取 `authorized-machines.json`。

安全约束：

- 这里只保存 `SHA256:...` 形式的域分离机器哈希，不保存原始机器码。
- 不要提交 GitHub Token、私钥、邮箱或客户隐私信息。
- `expiresOn` 必须存在；使用 `yyyy-MM-dd`，只有显式 `null` 表示永久。
- 停用授权时把 `enabled` 改为 `false`，需要 MOD 功能时保留 `"MOD"`。

编辑清单后，在 Rhino 中运行 `MOD_License` 并点击“立即联网刷新”。