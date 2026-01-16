# Cryptography Tools

## Common

- CyberChef
- OpenSSL/LibreSSL
- GnuPG

## Disk Encrypto

- VeraCrypt
- BitLocker
- FileVault

## Library

| **编程语言** | **模块/库名称** | **类型** | **核心用途与特点** |
| --- | --- | --- | --- |
| **Python** | **hashlib / secrets** | 标准库 | 基础哈希计算、生成安全随机数（令牌/密码） |
|     | **cryptography** | 第三方 | **现代标准**。提供 Fernet 高级加密，API 极安全 |
|     | **PyCryptodome** | 第三方 | 算法最全（含旧算法），常用于处理底层加密协议 |
| **Go** | **crypto (std)** | 标准库 | **顶尖实现**。包含 AES, RSA, TLS 等，性能极佳 |
|     | **x/crypto** | 半官方 | 补充标准库，包含 Argon2, Ed25519 等现代算法 |
| **JavaScript** | **crypto (Node.js)** | 内置模块 | 服务端 OpenSSL 封装，支持流加密、签名、证书 |
| (Node/Web) | **Web Crypto API** | 浏览器原生 | 浏览器端硬件加速加密，私钥不可导出，安全性高 |
|     | **noble-hashes / curves** | 第三方 | **现代首选**。纯 JS、无依赖、经过审计，适合区块链 |
|     | **CryptoJS / Forge** | 第三方 | 支持旧环境，功能极全（如复杂的 PKI/X.509 处理） |
| **C / C++** | **OpenSSL / BoringSSL** | 工业级 | **事实上的行业标准**。支持所有协议，极其庞大 |
|     | **libsodium (NaCl)** | 专业库 | **易用性标杆**。强制使用安全算法，防止内存错误 |
|     | **mbed TLS** | 嵌入式 | 轻量化设计，专门针对单片机（MCU）和 IoT 环境 |
|     | **Crypto++** | 类库  | 高度模板化的 C++ 类库，支持非常多的小众算法 |
| **Rust** | **ring** | 第三方 | **极速安全**。基于 BoringSSL 代码，通过 Rust 保证安全 |
|     | **RustCrypto** | 社区驱动 | 纯 Rust 实现，模块化程度极高，支持 `no_std` 环境 |
| **Java** | **JCA / JCE** | 标准架构 | Java 密码学扩展框架，通过 SPI 机制更换底层实现 |
|     | **Bouncy Castle** | 第三方 | **全球最强补充**。支持国密（SM2/3/4）、所有主流算法 |