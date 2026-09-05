<div align="right">
  <strong>🇸🇦 العربية</strong> | 
  <strong><a href="#english">🇬🇧English</a></strong> | 
  <strong><a href="#chinese">🇨🇳中文</a></strong>
</div>

---

# 📱 vphone-cli

> Boot a virtual iPhone via Apple's Virtualization.framework using PCC research VM infrastructure.

![poc](https://github.com/Lakr233/vphone-cli/blob/main/docs/demo.jpeg?raw=true)

---

## 👨‍💻 المطور / Developer

<div align="center">
  <table>
    <tr>
      <td align="center">
        <img src="https://img.shields.io/badge/Developer-Yaz%20Salaq-6C63FF?style=for-the-badge&logo=github&logoColor=white" />
        <br/>
        <a href="https://www.instagram.com/yaz.salaqq" target="_blank">
          <img src="https://img.shields.io/badge/Instagram-yaz.salaqq-E4405F?style=for-the-badge&logo=instagram&logoColor=white" />
        </a>
        <a href="https://www.facebook.com/YazSalaq" target="_blank">
          <img src="https://img.shields.io/badge/Facebook-Yaz%20Salaq-1877F2?style=for-the-badge&logo=facebook&logoColor=white" />
        </a>
        <a href="https://t.me/YAZsalaq" target="_blank">
          <img src="https://img.shields.io/badge/Telegram-YAZsalaq-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" />
        </a>
        <br/>
        <img src="https://img.shields.io/badge/AI%20Software%20Engineer-6C63FF?style=for-the-badge" />
        <img src="https://img.shields.io/badge/Ollama%20Developer-000000?style=for-the-badge&logo=ollama&logoColor=white" />
        <img src="https://img.shields.io/badge/iOS%20%26%20Android-Developer-blue?style=for-the-badge" />
      </td>
    </tr>
  </table>
</div>

---

<a id="arabic"></a>
## 🇸🇦 العربية

### 📝 عن المشروع
هذا المشروع من تطوير **Yaz Salaq** - مهندس برمجيات متخصص في الذكاء الاصطناعي وتطوير نماذج Ollama.

### 🏷️ المؤلف
**Yaz Salaq**  
- 🐙 GitHub: [@yazsalaq](https://github.com/yazsalaq)  
- 📸 Instagram: [@yaz.salaqq](https://www.instagram.com/yaz.salaqq)  
- 📘 Facebook: [Yaz Salaq](https://www.facebook.com/YazSalaq)  
- ✈️ Telegram: [@YAZsalaq](https://t.me/YAZsalaq)  

### 📋 المحتويات
- [المتطلبات الأساسية](#prerequisites-ar)
- [التثبيت](#install-ar)
- [البناء](#build-ar)
- [البدء السريع](#quickstart-ar)
- [الأوامر](#commands-ar)
- [الاتصال](#connecting-ar)

<a id="prerequisites-ar"></a>
### المتطلبات الأساسية

**المضيف:**
- Apple Silicon
- macOS 15+ (Sequoia)
- Xcode + iOS SDK

**الاعتماديات:**
```bash
brew install python@3.13 aria2 wget gnu-tar openssl@3 ldid-procursus sshpass keystone cmake libusb ipsw zstd
```

<a id="install-ar"></a>
### التثبيت
```bash
brew install zqxwce/tap/vphone-cli
```

<a id="build-ar"></a>
### البناء
```bash
git clone --recurse-submodules https://github.com/Lakr233/vphone-cli.git
./scripts/setup_tools.sh
./scripts/build.sh
cd .build/vphone-cli.app/Contents/MacOS/
vphone-cli --help
```

<a id="quickstart-ar"></a>
### البدء السريع
```bash
vphone-cli vm create myphone -V jb
vphone-cli vm launch myphone
```

<a id="commands-ar"></a>
### الأوامر
```bash
vphone-cli vm list                         # عرض الآلات الافتراضية
vphone-cli vm info myphone                  # عرض معلومات آلة
vphone-cli vm new myphone                   # إنشاء آلة جديدة
vphone-cli vm config myphone --cpu 8 --memory 8192
vphone-cli vm clone myphone myphone-2       # نسخ آلة
vphone-cli vm export myphone --out myphone.tzst
vphone-cli vm import myphone.tzst --name restored
vphone-cli vm rename myphone iphone16
vphone-cli vm delete iphone16
```

<a id="connecting-ar"></a>
### الاتصال
- **SSH (jailbreak):** `ssh -p 22222 mobile@<vm-ip>` (كلمة المرور: `alpine`)
- **SSH (regular/dev):** `ssh -p 22222 root@<vm-ip>`
- **VNC:** `vnc://<vm-ip>:5901`

---

<a id="english"></a>
## 🇬🇧 English

### 📝 About
This project is developed by **Yaz Salaq** - AI Software Engineer & Ollama Model Developer.

### 🏷️ Author
**Yaz Salaq**  
- 🐙 GitHub: [@yazsalaq](https://github.com/yazsalaq)  
- 📸 Instagram: [@yaz.salaqq](https://www.instagram.com/yaz.salaqq)  
- 📘 Facebook: [Yaz Salaq](https://www.facebook.com/YazSalaq)  
- ✈️ Telegram: [@YAZsalaq](https://t.me/YAZsalaq)  

### 📋 Table of Contents
- [Prerequisites](#prerequisites-en)
- [Install](#install-en)
- [Build](#build-en)
- [Quick Start](#quickstart-en)
- [Commands](#commands-en)
- [Connecting](#connecting-en)

<a id="prerequisites-en"></a>
### Prerequisites

**Host:**
- Apple Silicon
- macOS 15+ (Sequoia)
- Xcode + iOS SDK

**Dependencies:**
```bash
brew install python@3.13 aria2 wget gnu-tar openssl@3 ldid-procursus sshpass keystone cmake libusb ipsw zstd
```

<a id="install-en"></a>
### Install
```bash
brew install zqxwce/tap/vphone-cli
```

<a id="build-en"></a>
### Build
```bash
git clone --recurse-submodules https://github.com/Lakr233/vphone-cli.git
./scripts/setup_tools.sh
./scripts/build.sh
cd .build/vphone-cli.app/Contents/MacOS/
vphone-cli --help
```

<a id="quickstart-en"></a>
### Quick Start
```bash
vphone-cli vm create myphone -V jb
vphone-cli vm launch myphone
```

<a id="commands-en"></a>
### Commands
```bash
vphone-cli vm list                         # list VMs
vphone-cli vm info myphone                  # show one VM
vphone-cli vm new myphone                   # create an empty bundle
vphone-cli vm config myphone --cpu 8 --memory 8192
vphone-cli vm clone myphone myphone-2       # fast APFS clone
vphone-cli vm export myphone --out myphone.tzst
vphone-cli vm import myphone.tzst --name restored
vphone-cli vm rename myphone iphone16
vphone-cli vm delete iphone16
```

<a id="connecting-en"></a>
### Connecting
- **SSH (jailbreak):** `ssh -p 22222 mobile@<vm-ip>` (password: `alpine`)
- **SSH (regular/dev):** `ssh -p 22222 root@<vm-ip>`
- **VNC:** `vnc://<vm-ip>:5901`

---

<a id="chinese"></a>
## 🇨🇳 中文

### 📝 关于项目
本项目由 **Yaz Salaq** 开发 - AI 软件工程师和 Ollama 模型开发者。

### 🏷️ 作者
**Yaz Salaq**  
- 🐙 GitHub: [@yazsalaq](https://github.com/yazsalaq)  
- 📸 Instagram: [@yaz.salaqq](https://www.instagram.com/yaz.salaqq)  
- 📘 Facebook: [Yaz Salaq](https://www.facebook.com/YazSalaq)  
- ✈️ Telegram: [@YAZsalaq](https://t.me/YAZsalaq)  

### 📋 目录
- [前提条件](#prerequisites-zh)
- [安装](#install-zh)
- [构建](#build-zh)
- [快速开始](#quickstart-zh)
- [命令](#commands-zh)
- [连接](#connecting-zh)

<a id="prerequisites-zh"></a>
### 前提条件

**主机:**
- Apple Silicon
- macOS 15+ (Sequoia)
- Xcode + iOS SDK

**依赖:**
```bash
brew install python@3.13 aria2 wget gnu-tar openssl@3 ldid-procursus sshpass keystone cmake libusb ipsw zstd
```

<a id="install-zh"></a>
### 安装
```bash
brew install zqxwce/tap/vphone-cli
```

<a id="build-zh"></a>
### 构建
```bash
git clone --recurse-submodules https://github.com/Lakr233/vphone-cli.git
./scripts/setup_tools.sh
./scripts/build.sh
cd .build/vphone-cli.app/Contents/MacOS/
vphone-cli --help
```

<a id="quickstart-zh"></a>
### 快速开始
```bash
vphone-cli vm create myphone -V jb
vphone-cli vm launch myphone
```

<a id="commands-zh"></a>
### 命令
```bash
vphone-cli vm list                         # 列出虚拟机
vphone-cli vm info myphone                  # 显示虚拟机信息
vphone-cli vm new myphone                   # 创建新虚拟机
vphone-cli vm config myphone --cpu 8 --memory 8192
vphone-cli vm clone myphone myphone-2       # 克隆虚拟机
vphone-cli vm export myphone --out myphone.tzst
vphone-cli vm import myphone.tzst --name restored
vphone-cli vm rename myphone iphone16
vphone-cli vm delete iphone16
```

<a id="connecting-zh"></a>
### 连接
- **SSH (越狱):** `ssh -p 22222 mobile@<vm-ip>` (密码: `alpine`)
- **SSH (常规/开发):** `ssh -p 22222 root@<vm-ip>`
- **VNC:** `vnc://<vm-ip>:5901`

---

## 🛠️ التقنيات المستخدمة / Technologies Used

<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white" />
  <img src="https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white" />
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
</div>

---

## 📄 حقوق النشر / Copyright

<div align="center">
  <img src="https://img.shields.io/badge/©%202026-Yaz%20Salaq-6C63FF?style=for-the-badge" />
  <br/>
  <strong>Developed by Yaz Salaq</strong>
  <br/>
  <sub>مهندس برمجيات AI | مطور نماذج Ollama | iOS & Android Developer</sub>
  <br/>
  <sub>🇵🇸 فلسطين</sub>
</div>

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=yazsalaq&label=Profile%20Views&color=6c63ff&style=flat" alt="profile views" />
</p>
