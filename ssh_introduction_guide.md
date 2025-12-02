# SSH入门指南：从远程连接到高效开发

## 什么是SSH？

**SSH（Secure Shell）** 是一种安全的远程操作协议，它让你能够在本地电脑上远程控制另一台电脑。

### 为什么需要SSH？

假设你遇到以下场景：

- 需要在实验室的性能更强的专业工作站上运行代码
- 需要在学校的Linux服务器上调试作业（CS专业课如PGA、OSC、CPP等作业均需运行在学校的Linux服务器上）

但是...你不能什么问题都跑到实验室解决！

**常见问题：**

- Windows和Linux编译结果不一致
- 学校网络禁用远程桌面工具（如ToDesk、向日葵、UU远程等）

## SSH的完美解决方案

SSH提供了一种安全稳定的方式，让你能够：

1. 在宿舍电脑操作实验室服务器
2. 安全稳定地进行远程开发
3. 用VS Code打开远程服务器上的文件

### SSH的核心功能

- **远程登录** - 进入另一台电脑的系统
- **远程执行命令** - 让另一台电脑干活
- **安全文件传输** - 上传代码，下载日志

## 为什么叫"Secure Shell"？

- **Shell** = 命令行
- **Secure** = 加密传输

所有SSH通信都是加密的，不会被轻易截获。

## 如何使用SSH？

### 方法一：传统命令行SSH

在系统终端中使用基本的SSH命令：

```bash
ssh user@remote-server-ip
```

**示例：**

```bash
ssh student@192.168.10.35
```

### 方法二：图形化SSH - VS Code Remote SSH

#### 工具准备

- VS Code（Visual Studio Code）
- Remote-SSH插件
- 远程Linux服务器（需要IP地址、用户名、密码或SSH私钥）

#### 连接步骤

##### 1. 安装插件

- 打开VS Code Extensions
- 搜索"Remote-SSH"
- 点击Install安装

![Remote-SSH插件安装](https://github.com/user-attachments/assets/b7d192ea-183c-42bb-bb7e-1f9c661c000e)

##### 2. 打开连接入口

- 点击左下角绿色图标(><)
- 选择"Connect to Host..."

![打开连接入口](https://github.com/user-attachments/assets/b841c57f-c179-4f89-99e3-ddf0839c47b1)

##### 3. 配置主机

输入服务器地址：user@ServerIP

**示例：**

```bash
student@192.168.10.35
```

![配置主机](https://github.com/user-attachments/assets/2a35a292-efb1-4f2e-95f1-31d1a1ad4e55)

##### 4. 输入密码

- 登录成功后，右下角显示"SSH:hostname"

## 在远程服务器上使用VS Code

连接成功后，就像在本地一样操作！

### 打开远程文件夹

- 文件资源管理器 → 打开文件夹 → `/home/student/project/`

### 远程编辑

- 编辑的代码自动保存到服务器

### 内置终端

VS Code终端就是远程服务器的Shell

可以直接运行命令：

```bash
python3 app.py
gcc main.c -o main
ls
```

## 让SSH更安全 - SSH Key

### 公钥与私钥

SSH Key是一对密钥：

- **私钥** - 保存在你的电脑，绝对不能泄露
- **公钥** - 放在服务器/GitHub，用于验证身份

**好处：** 免密码登录，更安全、更快捷

## GitHub配置SSH Key

### 步骤详解

#### 1. 生成SSH Key

```bash
ssh-keygen  # 快速生成SSH密钥对
```

#### 2. 找到密钥

打开~/.ssh/目录：

- id_ed25519（私钥）
- id_ed25519.pub（公钥）- 复制这个文件的内容

#### 3. 上传到GitHub

- GitHub → Settings
- SSH and GPG keys → New SSH key
- 粘贴公钥内容

![上传到GitHub](https://github.com/user-attachments/assets/51ff4035-a60b-481b-8ee3-14e081b7344f)

#### 4. 测试连接

```bash
ssh -T git@github.com
```

显示
**"Hi username! You've successfully authenticated..."**
表示成功

通过以上步骤，我们完成了从生成SSH密钥对到将其配置到GitHub的全过程。使用SSH密钥进行认证，不仅摆脱了重复输入密码的繁琐，更显著提升了操作的安全性。掌握这一方法，将为您的日常开发工作带来便利。希望本指南对您有所帮助！

作者：蓝毒
