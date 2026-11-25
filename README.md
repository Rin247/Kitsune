# Kitsune — Telemetry-Free Privacy Web Browser

Kitsune is a fast, privacy-first cross-platform web browser built on a hardened Gecko/Firefox engine and a modern Qt 6 / C++ desktop shell (`Kitsune.exe`). Designed around a **Vulkan 1.3 and DirectX 12 (Feature Level 12_1) First/Only** graphics rendering architecture, Kitsune is stripped of all telemetry, tracking, sponsored content, background telemetry pings, and bolted-on AI bloat.

---

## ⚡ Core Subsystems & Status Matrix

| Subsystem | Features & Capabilities | Status / Roadmap |
|---|---|---|
| **Graphics Engine** | **Vulkan 1.3 & DirectX 12 (Feature Level 12_1) First/Only** WebRender GPU compositor | Active |
| **Privacy Protection** | Telemetry completely stripped, zero background pings, DNS-over-HTTPS (DoH), cookie partitioning | Active |
| **Advanced Anti-Tracking** | Canvas fingerprint randomization, automatic URL tracking parameter stripping, container tabs | Roadmap |
| **Gecko Browser Engine** | Hardened Gecko rendering engine, WebExtension API support, CSS userChrome styling | Active |
| **Native Ad Blocker** | Built-in uBlock Origin native C++ ad-blocker binding, element hiding, custom filter lists | Roadmap |
| **Browser Chrome & UI** | Minimalist Qt 6 / QML browser chrome, clean tab bar, address bar autocomplete, M3 theme | Active |
| **Productivity Tools** | Vertical tabs, side-by-side split browsing, offline reading mode & article archiver | Roadmap |

---

## 🦊 Key Features & Subsystem Breakdown

### 🛡️ Privacy & Anti-Tracking Core (`privacy`)
- **Current**: Total telemetry stripped, zero telemetry pings, DNS-over-HTTPS (DoH) support, strict tracker blocking, and cookie partitioning.
- **Planned / Roadmap**: Fingerprint randomization, automatic URL tracking parameter stripping, and isolated container tabs.

### 🌐 Browser Engine & Viewport (`engine`)
- **Current**: Hardened Gecko rendering engine, WebRender GPU acceleration (Vulkan/DX12 backend), WebExtension support, and custom CSS userChrome styling.
- **Planned / Roadmap**: Custom ad-blocker engine integration (uBlock Origin native binding), vertical tab bar layout, and reading mode offline archiver.

### 🎨 Custom UI & Compact Chrome (`chrome`)
- **Current**: Minimalist Qt 6 / QML browser chrome, clean tab bar, address bar autocomplete, and dark/light Material 3 theme.
- **Planned / Roadmap**: Tab grouping, split-view side-by-side browsing, custom keyboard shortcuts, and session restore manager.

---

## 🏗️ Architecture & Technology Stack

- **Graphics APIs**: Vulkan 1.3 & DirectX 12 (Feature Level 12_1) First/Only.
- **UI Shell**: C++20, Qt 6.12, QML.
- **Browser Engine**: Pinned Gecko (Mozilla Firefox core) with WebRender Vulkan/DX12 GPU compositor.
- **Licensing**: AGPL-3.0-or-later.

---

## 🛠️ Building & Running

### Prerequisites
- **Visual Studio 2022** (C++20 MSVC compiler)
- **Qt 6.12** (`msvc2022_64`)
- **Vulkan SDK 1.3+**

### Build Commands

```bat
:: Build Release binary (Kitsune.exe)
build.bat Release

:: Run Kitsune
run.bat
```

---

## 📜 License

Kitsune is released under the **GNU Affero General Public License v3.0 or later** (AGPL-3.0-or-later). See [`LICENSE`](LICENSE) for details.
