<div align="center">

<img src="docs/logo.png" alt="AiYou" width="120" />

# AiYou

### Transformă orice videoclip într-un set de idei și strategii acționabile

Aplicație Android care extrage automat ideile cheie din videoclipuri (YouTube),
le organizează pe categorii și generează un **AI Resume** cu strategiile esențiale —
ca să înveți mai repede și să nu pierzi timpul cu vizionarea integrală.

[![Descarcă APK](https://img.shields.io/badge/⬇️_Descarcă-AiYou.apk-6C5CE7?style=for-the-badge)](../../releases/latest)
![Platform](https://img.shields.io/badge/Android-6.0%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Version](https://img.shields.io/badge/versiune-1.0-blue?style=for-the-badge)

</div>

---

## 📲 Instalare

1. Descarcă **[`AiYou.apk`](../../releases/latest)** din secțiunea Releases (sau direct [din repo](AiYou.apk)).
2. Pe telefon, deschide fișierul descărcat.
3. Dacă apare un avertisment, permite instalarea din *surse necunoscute* pentru aplicația cu care deschizi APK-ul (browser / file manager).
4. Apasă **Instalează** și deschide **AiYou**.

> Necesită Android 6.0 (API 26) sau mai nou. APK debug, semnat de dezvoltator — pentru distribuție internă / demo.

---

## ✨ Ce face aplicația

| Funcție | Descriere |
|---|---|
| 🎬 **Extragere idei** | Analizează videoclipuri și scoate automat ideile cheie, cu scor de relevanță. |
| 🧠 **AI Resume** | Generează un rezumat al strategiilor (investiții, marketing etc.) din conținutul procesat. |
| 🏷️ **Categorii** | Ideile sunt grupate pe teme: *Strategii de investiții*, *Strategii de marketing* ș.a.m.d. |
| 🔖 **Salvate** | Marchează și păstrează ideile importante pentru mai târziu. |
| 📊 **Dashboard** | Statistici live: videoclipuri procesate, idei extrase, timp economisit. |
| ⭐ **Feedback** | Evaluează utilitatea fiecărei idei pentru a îmbunătăți rezultatele. |

---

## 📸 Capturi de ecran

<div align="center">

<table>
  <tr>
    <td align="center" width="50%">
      <img src="docs/screenshot-resume.png" alt="AI Resume" width="280" /><br/>
      <b>AI Resume</b><br/>
      <sub>Idei cheie extrase, pe categorii, cu rating</sub>
    </td>
    <td align="center" width="50%">
      <img src="docs/screenshot-dashboard.png" alt="Dashboard" width="280" /><br/>
      <b>Dashboard</b><br/>
      <sub>Overview cu statistici și videoclipuri recente</sub>
    </td>
  </tr>
</table>

<br/>

<img src="docs/screenshot-tablet.png" alt="Vedere tabletă" width="640" /><br/>
<b>Vedere pe tabletă</b> — layout adaptiv cu navigație laterală

</div>

---

## ☸️ Infrastructură & Deploy

Backend-ul AiYou rulează pe **Kubernetes**, livrat **GitOps** prin **Argo CD** —
fiecare componentă (API, Elasticsearch, Istio, observabilitate, securitate) este o aplicație
sincronizată automat din Git, cu status *Healthy / Synced*.

<div align="center">
<img src="docs/screenshot-argocd.png" alt="Argo CD Applications" width="860" /><br/>
<sub>Argo CD — aplicațiile platformei (API AiYou, Elasticsearch, Istio, Gatekeeper, Vault, Grafana/Loki/Prometheus, Velero) sincronizate GitOps</sub>
</div>

---

## 🛠️ Tehnologii

- **Kotlin** + **Jetpack Compose** (UI declarativă)
- Arhitectură **multi-modul** (`core` / `feature`) curată
- **MVVM**, Coroutines & Flow
- Layout **adaptiv** pentru telefon și tabletă

| | |
|---|---|
| Package | `com.podut.aiyou` |
| minSdk | 26 (Android 6.0) |
| targetSdk / compileSdk | 35 (Android 15) |
| Versiune | 1.0 |

---

<div align="center">
<sub>© AiYou — dezvoltat de <a href="https://github.com/podut">podut</a></sub>
</div>
