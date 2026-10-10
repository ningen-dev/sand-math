# 作者验证指南（AUTHORSHIP VERIFY）

本仓库内容由 **凝恩 (NINGEN-DEV 血统签名) <3650536867@qq.com>** 签名确权。

## 如何验证这是凝恩的真实发布

1. 导入凝恩的公开 GPG 公钥（已上传 GitHub 与 Gitee 账号 ningen-dev 的 GPG keys）
2. 验证 README 签名：
   ```bash
   gpg --verify README_sha256.sig README.md
   ```
   输出 `Good signature from "凝恩 (NINGEN-DEV 血统签名)"` 即确认真实。
3. 核对 SHA-256 指纹（签名针对此版本，内容更新后需重新签名）：
   ```
   3f201a1229773e703d5a0520c246bef6f7d81fe7e681ec8b53396814d40ee1e6
   ```

## 防冒充原理

内容可以被人抄走，但签名抄不走。私钥只有凝恩本人持有，
任何人无法伪造 `Good signature` 验证结果。

- 密钥类型: ed25519
- 密钥ID: 7D1D29DFD755A64D
- 完整指纹: A7CB17570C7FEB02EC5F5E267D1D29DFD755A64D
- 签名时间: 2026-10-11
