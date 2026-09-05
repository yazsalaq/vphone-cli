<div align="right">
  <strong><a href="./docs/README_ko.md">🇰🇷한국어</a></strong> | 
  <strong><a href="./docs/README_ja.md">🇯🇵日本語</a></strong> | 
  <strong><a href="./docs/README_zh.md">🇨🇳中文</a></strong> | 
  <strong>🇬🇧English</strong> |
  <strong><a href="#arabic">🇸🇦 العربية</a></strong>
</div>

---

# 📱 vphone-cli

> Boot a virtual iPhone via Apple's Virtualization.framework using PCC research VM infrastructure.

![poc](./docs/demo.jpeg)

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

## 📝 عن المشروع / About

هذا المشروع من تطوير **Yaz Salaq** - مهندس برمجيات متخصص في الذكاء الاصطناعي وتطوير نماذج Ollama.

This project is developed by **Yaz Salaq** - AI Software Engineer & Ollama Model Developer.

---

## 🏷️ المؤلف / Author

**Yaz Salaq**  
- 🐙 GitHub: [@yazsalaq](https://github.com/yazsalaq)  
- 📸 Instagram: [@yaz.salaqq](https://www.instagram.com/yaz.salaqq)  
- 📘 Facebook: [Yaz Salaq](https://www.facebook.com/YazSalaq)  
- ✈️ Telegram: [@YAZsalaq](https://t.me/YAZsalaq)  

---

## 📋 Table of Contents

- [Prerequisites](#prerequisites)
- [Install](#install)
- [Build](#build)
- [Quick Start](#quick-start)
- [Commands](#commands)
- [Firmware Variants](#firmware-variants)
- [Running & Connecting](#running--connecting)
- [Locations](#locations)
- [SIP/AMFI Relaxation](#sipamfi-relaxation)
- [Tested Environments](#tested-environments)
- [FAQ](#faq)
- [Automation](#automation)
- [Acknowledgements](#acknowledgements)

---

## Prerequisites

**Host:**

- Apple Silicon
- macOS 15+ (Sequoia)
- Xcode + iOS SDK (cross-compiles the guest daemon)
- [SIP/AMFI relaxation to allow private PV=3 entitlements with unsigned-binary](#sipamfi-relaxation)

**Dependencies:**

```bash
brew install python@3.13 aria2 wget gnu-tar openssl@3 ldid-procursus sshpass keystone cmake libusb ipsw zstd
