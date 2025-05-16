
# Firebase Unity Packages (Unofficial UPM Mirror)

This repository provides an **unofficial mirror** of select Firebase Unity SDK packages—**Core (App), Analytics, and Crashlytics**—restructured for easy installation via Unity's **Package Manager (UPM)** and **OpenUPM**.

> ⚠️ This project is **not affiliated with or maintained by Google or Firebase**. It is provided for the convenience of Unity developers who prefer using UPM workflows.

---

## 📦 Available Packages

| Package              | Name                                | Description                                |
|----------------------|-------------------------------------|--------------------------------------------|
| Firebase Core        | `com.google.firebase.app`           | Core SDK required by all Firebase features |
| Firebase Analytics   | `com.google.firebase.analytics`     | Event logging and user analytics           |
| Firebase Crashlytics | `com.google.firebase.crashlytics`   | Crash reporting and diagnostics            |

---

## 🛠 Installation via Git URL

Add the following lines to your Unity `manifest.json`:

```json
"dependencies": {
  "com.google.firebase.app": "https://github.com/shirleyman/firebase-unity-packages.git?path=firebase-app",
  "com.google.firebase.analytics": "https://github.com/shirleyman/firebase-unity-packages.git?path=firebase-analytics",
  "com.google.firebase.crashlytics": "https://github.com/shirleyman/firebase-unity-packages.git?path=firebase-crashlytics"
}
```

---

## 🌐 Installation via OpenUPM

These packages are also available on [OpenUPM](https://openupm.com). To install via the CLI:

```bash
openupm add com.shirleyman.google.firebase.app
openupm add com.shirleyman.google.firebase.analytics
openupm add com.shirleyman.google.firebase.crashlytics
```

> You may need to [enable scoped registries](https://openupm.com/docs/getting-started.html#scoped-registry) in your Unity project to use OpenUPM.

---

## 📄 License

This repository redistributes the Firebase Unity SDK under the original [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). See `LICENSE` and `NOTICE` files within each package.

All original work is © Google and Firebase. This mirror is unofficial and provided for convenience only.

---

## 🙋‍♂️ Why This Exists

Google's official Firebase Unity SDK is distributed as `.tgz` tarballs which are not UPM-friendly out of the box. This repo repackages them into UPM-compliant folder structures to:

- Improve multi-project reuse
- Enable Git and OpenUPM-based workflows
- Simplify dependency management

---

## 📬 Contributions

This mirror is maintained manually as new Firebase versions release. Contributions are welcome for automation or updating to newer versions!
