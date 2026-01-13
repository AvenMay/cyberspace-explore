# Cryptography

## Resources

### Books

- [图解密码技术 第三版.pdf]({{ files_server }}/cybersecurity/cryptography/%E5%9B%BE%E8%A7%A3%E5%AF%86%E7%A0%81%E6%8A%80%E6%9C%AF%20%E7%AC%AC%E4%B8%89%E7%89%88.pdf)
- [应用密码学协议、算法与C源程序.pdf]({{ files_server }}/cybersecurity/cryptography/%E5%BA%94%E7%94%A8%E5%AF%86%E7%A0%81%E5%AD%A6%E5%8D%8F%E8%AE%AE%E3%80%81%E7%AE%97%E6%B3%95%E4%B8%8EC%E6%BA%90%E7%A8%8B%E5%BA%8F.pdf)

### Tools

- OpenPGP
- GnuPG
- OpenSSL
- LibreSSL
- Cyber Chef

## Getting Started

- [Encoding](/software-engineering/programming/preparation/encoding/)
- Classical-Cryptography


## Cryptography

- Symmetric-key Cryptography
- Asymmetric-key Cryptography (Public-key)
- Hash-Function
- Digital-Signatures
- Key Exchange Protocols
- Message-Authentication-Code
- Pseudo-Random Number Generator

## PKI

## Use-Cases

| Use-Case | 核心目标 | 主要方法 | 典型应用 |
| --- | --- | --- | --- |
| 数据保密 | 防止信息泄露 | 对称/非对称加密 | TLS、VPN、云存储加密 |
| 数据完整性 | 防篡改 | 哈希函数、MAC | 软件校验、消息认证 |
| 身份认证 | 验证身份 | 数字签名、MAC、PKI | HTTPS证书、区块链 |
| 不可否认性 | 防抵赖 | 数字签名 | 电子合同、数字发票 |
| 密钥管理 | 安全分发和存储密钥 | 密钥交换、KDF、HSM | TLS握手、KMS |
| 随机性 | 防预测 | CSPRNG | 密钥生成、会话令牌 |
| 高级安全 | 隐私保护和未来安全 | 同态加密、零知识证明、量子抗性密码 | 云计算隐私、区块链、量子安全通信 |
