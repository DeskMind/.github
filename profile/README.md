# 🧠 DeskMind — Local AI Agent Framework

**DeskMind** is a modular, locally executable AI framework designed to bring **agentic intelligence** directly to your desktop.  
It enables developers to integrate local and online AI capabilities into existing software like Office, and more — all through an extensible plugin system.

---

## 🔍 Overview

DeskMind is built around three main components:

| Component | Description | License |
|------------|--------------|----------|
| **[DeskMind.SDK](https://github.com/DeskMind/DeskMind.SDK)** | Core contracts and plugin runtime used to build DeskMind-compatible extensions. | Apache 2.0 |
| **[DeskMind.Studio](https://github.com/DeskMind/DeskMind.Studio)** | Free WPF-based desktop shell that loads and manages DeskMind plugins. | Apache 2.0 |
| **[DeskMind.Plugins.Free](https://github.com/DeskMind/DeskMind.Plugins.Free)** | Collection of open-source DeskMind plugins such as Office and Web Scraper. | Apache 2.0 |
| **[DeskMind.Plugins.Pro](https://github.com/DeskMind/DeskMind.Plugins.Pro)** | Commercial plugins providing advanced integrations. | Proprietary |

---

## ⚙️ Core Concepts

- **🧩 Modular Plugins** — Each plugin is self-contained and defines its capabilities via metadata.
- **🔐 Security & Policy System** — Plugins run under a configurable local security policy.
- **🧠 Agentic Actions** — DeskMind connects UI components and tools to AI-driven agents.
- **🪶 Cross-Platform Ready** — Future versions will support Avalonia and WebAssembly.

---

## 🚀 Getting Started

1. **Install DeskMind Studio**  
   Download or build the free WPF Studio to load and test plugins.

2. **Install Free Plugins**  
   Download or build the free Plugins repo.

3. **Build Your Own Plugin**  
   Reference `DeskMind.SDK` in your project and implement:
   ```csharp
   public class MyPluginFactory : IPluginFactory
   {
       public string Name => "My Custom Plugin";
       public IPlugin CreateInstance() => new MyPlugin();
   }
4. Drop Your Plugin DLL into the Studio Plugins folder and it will appear automatically.

## 🧰 Repository Structure
DeskMind.SDK/                → Core SDK & interfaces  
DeskMind.Studio/             → WPF host application (free)  
DeskMind.Plugins.Free/       → Open-source plugins (Office, WebScraper, PythonRunner,  etc.)  
DeskMind.Plugins.Pro/        → Commercial plugins (future)  

## 📦 Build Requirements

.NET 9.0 SDK (or 8.0 for Visual Studio 2022)

Visual Studio 2022 / Rider / VS Code

Windows 10/11 (for Studio, WPF-based)

## 🪪 Licensing Summary
| Project            | License            | Summary                                    |
| ------------------ | ------------------ | ------------------------------------------ |
| SDK & Free Plugins | Apache License 2.0 | Permissive, open-source                    |
| Studio             | Free Binary (EULA) | Free for all users, source-available later |
| Pro Plugins        | Commercial         | Requires a DeskMind commercial license (Future)    |

## 💬 Contributing

Contributions are welcome for the open-source components (SDK, Free Plugins, Demo Studio).
Please open an issue or pull request in the respective repository.

📅 Roadmap

 - [x] Modular plugin system
 - [x] Python Runner plugin (Pro)
 - [x] WPF Demo Studio
 - [ ] Cross-platform Avalonia Studio
 - [ ] Local model orchestration
 - [ ] Plugin marketplace integration

🧑‍💻 Author

**Sachith Harshitha Liyanagama**  
Creator and maintainer of DeskMind  
© 2025 — All rights reserved.
