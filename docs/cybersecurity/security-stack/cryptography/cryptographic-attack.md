# Cryptographic Attack

## Tools

- Hashcat
- John the Ripper
- RsaCtfTool

密码学研究中，将“攻击”视为评估安全性的工具。目的不是破坏系统，而是理解模型与算法的安全边界。

---

## **一、按攻击者获得的信息分类（最经典）**

### 1. **唯密文攻击（Ciphertext-only Attack, COA）**

攻击者只看到若干密文，希望推断明文或密钥。  
例如：早期替换密码可从字频反推明文。

### 2. **已知明文攻击（Known-plaintext Attack, KPA）**

攻击者同时知道某些明文及其对应密文，试图利用这些信息恢复密钥。  
例如：二战时期对 Enigma 的部分攻击依赖已知格式的电文。

### 3. **选择明文攻击（Chosen-plaintext Attack, CPA）**

攻击者可以选择明文并获得对应密文，从而分析系统。  
现代对称密码必须抵抗 CPA（如 AES 在很多模式下满足）。

### 4. **选择密文攻击（Chosen-ciphertext Attack, CCA）**

攻击者可以选择密文并获得其解密结果。  
例如：RSA 原始版不可抵抗 CCA，后来的 **RSA-OAEP** 才实现 CCA 安全。

---

## **二、按攻击方式的技术/策略分类**

### 1. **暴力破解（Brute-force Attack）**

尝试所有可能的密钥空间。  
防御方式：增大密钥长度（如 AES-256）。

### 2. **字典攻击（Dictionary Attack）**

对低熵输入（密码）尝试典型猜测集。  
常见于口令系统，而非数学意义的密码算法。

### 3. **中间相遇攻击（Meet-in-the-middle Attack）**

用于双重加密，减少时间复杂度。  
例如：对 Double-DES 的经典攻击（导致使用 3DES）。

### 4. **差分密码分析（Differential Cryptanalysis）**

研究明文差异如何影响密文差异，是分析块密码的核心工具。

### 5. **线性密码分析（Linear Cryptanalysis）**

试图用线性关系逼近非线性 S 盒，收集统计偏差求密钥。

### 6. **旁路攻击（Side-channel Attack）**

不攻击算法数学结构，而是攻击实现过程的物理泄漏：

- 时间攻击（timing attack）
  
- 电磁辐射攻击
  
- 功耗分析（Power Analysis）
  
- 缓存攻击（cache attack）
  

研究重心是**如何让算法的实现对物理信息泄漏免疫**。

### 7. **故障攻击（Fault Injection Attack）**

通过向设备注入错误（激光、电压），观察输出偏差以恢复密钥，例如对 RSA CRT 的攻击（Bellcore 攻击模型）。

---

## **三、通信协议层面的攻击**

### 1. **重放攻击（Replay Attack）**

攻击者记录有效的通信消息并重新发送。  
防御：随机数、时间戳、不可重用 nonce。

### 2. **中间人攻击（Man-in-the-Middle, MITM）**

攻击者插入通信双方之间，窃听或篡改。  
典型防御：认证、证书、公钥基础设施（PKI）。

### 3. **降级攻击（Downgrade Attack）**

让通信双方使用更弱的协议/密钥算法，例如对 TLS 的降级攻击。

---

## **四、针对公钥密码特有的攻击**

### 1. **数论方面的攻击**

用于破解基于数学难题的算法：

- 因数分解攻击（RSA）
  
- 离散对数攻击（Diffie–Hellman, DSA）
  
- 椭圆曲线离散对数攻击（ECDSA, ECDH）
  

### 2. **量子攻击（理论层面）**

量子计算机上可用：

- Shor 算法：破解 RSA 和 ECC
  
- Grover 算法：对对称加密造成平方级加速（但仍可通过更长密钥抵抗）
  

所以出现了 **后量子密码学（Post-quantum Cryptography, PQC）**。

---

## **五、软件实现层面的攻击**

### 1. **实现漏洞（Implementation Attacks）**

如随机数生成器（RNG）不安全导致密钥可预测。

### 2. **协议逻辑攻击**

不攻击数学算法，而是攻击协议中的逻辑错误。  
例如：认证顺序错误、缺少绑定（binding）