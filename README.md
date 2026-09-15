# Hybrid Git Sync for Obsidian

[English](https://github.com/czhhbp/HybridGitSync/blob/main/README.md)｜[中文](https://github.com/czhhbp/HybridGitSync/blob/main/README_ZH.md)

> 🚀 **An adaptive, cross-platform Git synchronization solution for Obsidian.**  
> Enjoy high-performance Native Git execution on Desktop alongside a lightweight, zero-dependency Git Provider API on Mobile.

---

## 🌟 Introduction & Design Philosophy

Managing an Obsidian vault with Git across different operating systems usually requires distinct synchronization strategies due to platform-specific constraints. **Hybrid Git Sync** bridges this gap seamlessly by implementing an **Adaptive Sync Engine**.

Instead of applying a single approach to all environments, this plugin intelligently splits the synchronization workload based on the device you are currently using:

* **💻 On Desktop (Windows/Mac/Linux):** It invokes your local **Native Git client**. This guarantees maximum execution speed, reliability, and full support for complex repository histories or large assets.
* **📱 On Mobile (iOS/Android):** It bypasses mobile OS limitations by interacting directly with cloud **REST APIs (GitHub / GitLab / Gitea)**. It reads and writes changes via lightweight HTTPS requests without requiring any local Git binary environments on your phone.

---

## ✨ Key Features

* 🔄 **Adaptive Hybrid Engine:** Runs full native Git commands on your PC and shifts to clean, memory-efficient API requests on your mobile devices.
* 🔒 **Privacy Centric:** Your Personal Access Tokens (PAT) are stored locally within Obsidian's secure configuration storage. No data ever leaves your device or touches intermediate servers.
* ⚡ **Conflict Resolution:** Built-in smart synchronization logic helps track updates, reducing the risk of overwriting files during simultaneous multi-device editing.
* 💰 **100% Free & Open Source:** A reliable, customizable, and fully self-hosted alternative for universal knowledge base backups.

---

## 📦 Installation

1. Inside Obsidian, navigate to **Settings** -> **Community Plugins**.
2. Click **Browse** and search for `Hybrid Git Sync`.
3. Click **Install**, then toggle on **Enable**.

---

## ⚙️ Quick Setup Guide

Setting up Hybrid Git Sync takes less than 3 minutes:

1. **Repository Setup:** Initialize your Obsidian vault as a Git repository on your desktop and push it to your hosting platform (GitHub, GitLab, or Gitea).
2. **Generate Token:** Navigate to your Git provider's settings and create a **Personal Access Token (PAT)** with full `repo` read/write scopes.
3. **Mobile Configuration:** Open the plugin settings on your mobile device, enter your Repository URL and the generated Token. Tap **Sync** to initiate your first transfer!

---

## 🤝 Feedback & Contributing

As this is a newly released plugin, your feedback is incredibly valuable! If you encounter any bugs or have feature requests:

- Please open an **Issue** or join the discussion in the **Discussions** tab.


## License

MIT


---

---

Note: This project is a fork and modification of the original plugin [wk-obsidian/HybridGitSync](https://github.com/wk-obsidian/HybridGitSync). It preserves and improves some features and implementations.
