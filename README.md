# Ducket BOT
Ducket BOT

- Register Here : [Ducket Lobby](https://app.ducket.club/?invite=VONSSY)
- Sign In With Solana Wallet
- Connect X & DC Account

## Features

  - Auto Get Account Information
  - Auto Run With [Proxyscrape Free Proxy](https://proxyscrape.com/free-proxy-list) - `Choose 1`
  - Auto Run With Private Proxy - `Choose 2`
  - Auto Run Without Proxy - `Choose 3`
  - Auto Rotate Invalid Proxies - `y` or `n`
  - Auto Perform Arcade Game
  - Auto Claim Daily Check-In
  - Auto Claim Available Tasks
  - Multi Accounts

## Requiremnets

- Make sure you have Python3.9 or higher installed and pip.

## Instalation

1. **Clone The Repositories:**
   ```bash
   git clone https://github.com/vonssy/Ducket-BOT.git
   ```
   ```bash
   cd Ducket-BOT
   ```

2. **Install Requirements:**
   ```bash
   pip install -r requirements.txt #or pip3 install -r requirements.txt
   ```

## Configuration

- **accounts.txt:** You will find the file `accounts.txt` inside the project directory. Make sure `accounts.txt` contains data that matches the format expected by the script. Here are examples of file formats:

  ```bash
    your_solana_private_key_1 (base58)
    your_solana_private_key_2 (base58)
  ```
  
- **proxy.txt:** You will find the file `proxy.txt` inside the project directory. Make sure `proxy.txt` contains data that matches the format expected by the script. Here are examples of file formats:
  ```bash
    ip:port # Default Protcol HTTP.
    protocol://ip:port
    protocol://user:pass@ip:port
  ```

## Run

```bash
python bot.py #or python3 bot.py
```

## Buy Me a Coffee

- **EVM:** 0xe3c9ef9a39e9eb0582e5b147026cae524338521a
- **TON:** UQBEFv58DC4FUrGqinBB5PAQS7TzXSm5c1Fn6nkiet8kmehB
- **SOL:** E1xkaJYmAFEj28NPHKhjbf7GcvfdjKdvXju8d8AeSunf
- **SUI:** 0xa03726ecbbe00b31df6a61d7a59d02a7eedc39fe269532ceab97852a04cf3347

Thank you for visiting this repository, don't forget to contribute in the form of follows and stars.
If you have questions, find an issue, or have suggestions for improvement, feel free to contact me or open an *issue* in this GitHub repository.

**vonssy**

# Ducket-BOT 加密使用指南

## 安全增强说明
此版本增加了私钥加密功能，确保你的账户信息安全存储，防止被未授权访问。

## 加密功能使用方法

### 安装所需依赖
首先确保安装了额外的依赖包:
```
pip install cryptography
```

### 使用选项
启动脚本后，将显示私钥加密菜单，提供三个选项：

1. **加密accounts.txt文件**：
   - 选择此选项会创建一个加密版本的accounts.txt文件
   - 加密文件将被保存为accounts.txt.encrypted
   - 原始文件不会自动删除，建议手动删除原始文件以确保安全

2. **使用加密账户文件运行**：
   - 选择此选项将要求输入之前设置的密码
   - 然后脚本会从加密文件读取账户信息
   - 如果密码不正确，程序将退出

3. **使用标准账户文件运行**：
   - 使用未加密的accounts.txt文件运行程序
   - 不建议在共享环境中使用此选项

### 安全建议
- 使用强密码（最少8个字符，包含大小写字母、数字和特殊字符）
- 加密文件后删除原始accounts.txt文件
- 不要在共享电脑上存储密码
- 定期更改加密密码
- 加密文件不会被自动上传到任何服务器

## 使用步骤示例
1. 运行脚本: `python bot.py`
2. 在菜单中选择选项1进行加密
3. 设置并确认加密密码
4. 确认加密成功后，删除原始accounts.txt文件
5. 下次运行时，选择选项2从加密文件运行

## 注意事项
- 如果忘记密码，无法恢复加密的账户信息
- 加密仅保护静态文件，运行时内存中的私钥仍然需要解密以进行操作
- 该程序不会将您的私钥发送给任何第三方