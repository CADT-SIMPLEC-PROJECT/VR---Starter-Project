# Unity VR Starter Project 🎮

A starter template for building Virtual Reality (VR) applications in Unity using XR Interaction Toolkit. This project provides a basic setup for VR development, including locomotion, interaction, and controller support.

---

## 📌 Features

- XR Interaction Toolkit setup
- Support for Meta Quest / OpenXR devices
- Basic locomotion (Teleport / Smooth Move)
- Grab and interactable objects
- Hand/controller tracking
- Optimized project settings for VR
- Sample scene for testing

---

## 🛠️ Requirements

Most required XR packages are already installed and configured in this project.

Make sure you have the following:

- **Unity Version:** 6000.0.028f1 LTS or later (recommended)
- **XR Interaction Toolkit** (Pre-installed)
- **XR Plugin Management** (Pre-installed)
- **Input System Package** (Pre-installed)
- **OpenXR Plugin** (Configured for Meta Quest)
- **Meta Quest Headset (Primary Target Device)**
- USB-C Cable (for Link / Debugging)

---


## 📥 Installation

1. Clone this repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
```

2. Open Unity Hub
3. Click **Open Project**
4. Select the cloned project folder
5. Wait for Unity to import packages

---

## ⚙️ Project Setup

### Enable XR Plugin

1. Go to **Edit → Project Settings → XR Plug-in Management**
2. Enable **OpenXR** (or Oculus if required)
3. Select target platform (PC / Android)

### Input System

1. Go to **Edit → Project Settings → Player**
2. Under **Other Settings → Active Input Handling**
3. Select **Input System Package** (or Both)
4. Restart Unity if prompted

### XR Interaction Toolkit

Ensure the following are enabled:

- XR Origin
- Interaction Manager
- Locomotion System
- Action-based Controllers

---

## ▶️ How to Run

### PC VR (Link / SteamVR)

1. Connect headset to PC
2. Enable OpenXR runtime
3. Click **Play** in Unity

### Standalone (Meta Quest)

1. Switch platform to Android
2. Build & Run
3. Install APK on headset

---

## 📁 Project Structure

```
Assets/
 ├── Resources/      # Contain material, prefab, shader etc...
 ├── Sample/         # Sample Package from OpenXR
 ├── Scripts/        # C# scripts
 ├── Scenes/         # Main VR scenes
 └── XR/             # XR configurations
```

---

## 🧩 Main Components

| Component | Description |
|-----------|-------------|
| XR Origin | Player camera and tracking |
| Interactors | Ray and Direct interactors |
| Grab Interactable | Grabbable objects |
| Locomotion Provider | Movement system |
| Input Actions | Controller mapping |

---

## 🧪 Testing

- Use Unity Play Mode for quick tests
- Use Link / AirLink for Meta Quest
- Build to device for performance testing
- Enable XR Device Simulator for debugging

---

## 🐞 Troubleshooting

### VR Not Detected
- Check XR Plugin settings
- Verify headset connection
- Restart Unity and headset

### Controllers Not Working
- Check Input Action Asset
- Verify Action-based Controller setup
- Re-import XR Toolkit samples

### Build Errors
- Clear Library folder
- Rebuild project
- Check Android SDK/NDK paths

---

## 🔌 Meta Quest External Tools Setup

To build, deploy, and debug on Meta Quest devices, install the following tools:

### 1. Meta Quest Developer Hub (MQDH)

- Download from Meta Developer website
- Used for device management, APK installation, and performance monitoring
- Enable Developer Mode on your headset

### 2. Android SDK / NDK / JDK

Unity requires Android development tools for Quest builds.

Steps:
1. Open **Unity Hub**
2. Go to **Installs → Your Unity Version → Add Modules**
3. Install:
   - Android Build Support
   - OpenJDK
   - Android SDK & NDK Tools

### 3. ADB (Android Debug Bridge)

ADB is used to communicate with the headset.

Verify connection:

```
adb devices
```

Your Quest device should appear in the list.

### 4. Enable Developer Mode

1. Open Meta Quest mobile app
2. Go to **Menu → Devices → Developer Mode**
3. Turn on Developer Mode
4. Restart headset

---

## 📚 References

- Unity XR Toolkit Docs: https://docs.unity3d.com
- OpenXR Documentation
- Meta Developer Hub

---

## ✉️ Contact

Maintained by: **CADT**  
Institution: CADT IDT

---

> This project is intended for educational and research purposes.

