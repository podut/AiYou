<div align="center">

<img src="docs/logo.png" alt="AiYou" width="120" />

# AiYou

### Turn any video into a set of actionable ideas and strategies

An Android app that automatically extracts the key ideas from videos (YouTube),
organizes them by category and generates an **AI Resume** of the essential strategies —
so you learn faster without watching everything end to end.

[![Download APK](https://img.shields.io/badge/⬇️_Download-AiYou.apk-6C5CE7?style=for-the-badge)](../../releases/latest/download/AiYou.apk)
![Platform](https://img.shields.io/badge/Android-6.0%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Version](https://img.shields.io/badge/version-1.0-blue?style=for-the-badge)

</div>

---

## 📲 Installation

1. Download **[`AiYou.apk`](../../releases/latest/download/AiYou.apk)** (the link starts the download right away — or grab it [from the repo](AiYou.apk)).
2. On your phone, open the downloaded file.
3. If a warning appears, allow installation from *unknown sources* for the app you opened the APK with (browser / file manager).
4. Tap **Install** and open **AiYou**.

> Requires Android 6.0 (API 26) or newer. Debug APK, developer-signed — for internal distribution / demo.

---

## ✨ What the app does

| Feature | Description |
|---|---|
| 🎬 **Idea extraction** | Analyzes videos and automatically pulls out the key ideas, with a relevance score. |
| 🧠 **AI Resume** | Generates a summary of the strategies (investing, marketing, etc.) from the processed content. |
| 🏷️ **Categories** | Ideas are grouped by topic: *Investing strategies*, *Marketing strategies*, and so on. |
| 🔖 **Saved** | Bookmark and keep the important ideas for later. |
| 📊 **Dashboard** | Live stats: processed videos, extracted ideas, time saved. |
| ⭐ **Feedback** | Rate the usefulness of each idea to improve the results. |

---

## 📸 Screenshots

<div align="center">

<table>
  <tr>
    <td align="center" width="50%">
      <img src="docs/screenshot-resume.png" alt="AI Resume" width="280" /><br/>
      <b>AI Resume</b><br/>
      <sub>Key ideas extracted, by category, with rating</sub>
    </td>
    <td align="center" width="50%">
      <img src="docs/screenshot-dashboard.png" alt="Dashboard" width="280" /><br/>
      <b>Dashboard</b><br/>
      <sub>Overview with stats and recent videos</sub>
    </td>
  </tr>
</table>

<br/>

<img src="docs/screenshot-tablet.png" alt="Tablet view" width="640" /><br/>
<b>Tablet view</b> — adaptive layout with side navigation

</div>

---

## ☸️ Infrastructure & Deployment

The AiYou backend runs on **Kubernetes**, delivered **GitOps**-style via **Argo CD** —
every component (API, Elasticsearch, Istio, observability, security) is an application
synced automatically from Git, with *Healthy / Synced* status.

<div align="center">
<img src="docs/screenshot-argocd.png" alt="Argo CD Applications" width="860" /><br/>
<sub>Argo CD — platform applications (AiYou API, Elasticsearch, Istio, Gatekeeper, Vault, Grafana/Loki/Prometheus, Velero) synced via GitOps</sub>
</div>

---

## 🛠️ Tech stack

- **Kotlin** + **Jetpack Compose** (declarative UI)
- Clean **multi-module** architecture (`core` / `feature`)
- **MVVM**, Coroutines & Flow
- **Adaptive** layout for phone and tablet

| | |
|---|---|
| Package | `com.podut.aiyou` |
| minSdk | 26 (Android 6.0) |
| targetSdk / compileSdk | 35 (Android 15) |
| Version | 1.0 |

---

<div align="center">
<sub>© AiYou — built by <a href="https://github.com/podut">podut</a></sub>
</div>
