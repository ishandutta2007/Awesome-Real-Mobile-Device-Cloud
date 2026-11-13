# Awesome-Real-Mobile-Device-Cloud

# Awesome Real Mobile Device Cloud

> A curated list of top Real Mobile Device Cloud platforms — both SaaS/Hosted commercial device farms and open-source alternatives for running manual and automated tests on physical Android and iOS devices hosted in the cloud.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [BrowserStack Real Device Cloud](#browserstack-real-device-cloud)
  - [Sauce Labs Real Device Cloud](#sauce-labs-real-device-cloud)
  - [Kobiton](#kobiton)
  - [AWS Device Farm](#aws-device-farm)
  - [HeadSpin](#headspin)
  - [BitBar](#bitbar)
  - [Perfecto](#perfecto)
  - [TestGrid](#testgrid)
  - [Firebase Test Lab](#firebase-test-lab)
  - [Digital.ai Testing](#digitalai-testing)
- [Open-Source Software](#-open-source-software)
  - [Sonic](#sonic)
  - [GADS](#gads)
  - [OpenSTF (archived)](#openstf-archived)
  - [mobile-mcp](#mobile-mcp)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Real Mobile Device Cloud platforms. These are not open-source but are included as reference points for feature comparison.

### BrowserStack Real Device Cloud
**Type:** Large-scale real device cloud with App Live and App Automate
BrowserStack provides access to **30,000+ real devices** and 3,500+ browser combinations, with a free forever plan available . App Live enables interactive manual testing with natural gestures, real-time debugging, crash logs, and network throttling (2G/3G/Edge) . Devices are pristine and data is wiped clean after each session . It is the most widely adopted commercial device cloud, trusted by 50,000+ customers .  
**Best for:** Teams wanting the broadest device coverage and a mature manual testing experience with a free entry point.

### Sauce Labs Real Device Cloud
**Type:** Extensive real device cloud with programmable API and AI-ready workflows
Sauce Labs provides real devices across iPhone, iPad, Samsung Galaxy, Google Pixel, Oppo, Huawei, and Xiaomi . The **Real Device Access API** offers deep, framework-agnostic device control with raw adb and xcrun commands, persistent sessions up to 24 hours on private devices, and live WebSocket streams of logs, network traffic, and video . It is **MCP-ready**, allowing AI agents to treat devices as native tools, with IDE plugins for VS Code, Cursor, and IntelliJ . Private devices support unrestricted ADB shell and custom Appium drivers .  
**Best for:** Teams wanting deep device-level control for AI-driven workflows, soak tests, and custom automation beyond standard frameworks.

### Kobiton
**Type:** Real device cloud with AI automation and on-prem options
Kobiton offers a device-in-hand experience from anywhere, with a secure and scalable device lab that can run in the cloud or on-premises . Its AI engine delivers **3x faster script execution**, Appium script generation, self-healing execution, and no-code testing . The Startup plan starts at **$83/month for 500 minutes**, making it the lowest entry price among major automation platforms, though minutes are capped . Larger plans scale to $399/month for 3,000 minutes .  
**Best for:** Small teams testing in occasional bursts wanting AI-assisted automation at a low entry price, or teams wanting to manage their own device lab.

### AWS Device Farm
**Type:** Pay-per-minute real device testing within AWS
AWS Device Farm provides access to a large fleet of physical devices in AWS data centers, with pay-per-minute pricing at **$0.17 per device minute** after a one-time 1,000-minute trial . It supports Appium, Espresso, XCUITest, and a built-in test suite that requires no scripting . Each run returns videos, logs, and performance data . Private device labs are available for dedicated iOS and Android devices with persistent settings across sessions . Unmetered testing costs $250 per device slot per month .  
**Best for:** Teams already on AWS with uneven testing schedules wanting pay-as-you-go pricing and native AWS integration.

### HeadSpin
**Type:** Performance-focused real device cloud across 50+ countries
HeadSpin focuses on **performance** as well as functionality, tracking **130+ performance metrics** across UI, network, and device . Its SIM-enabled devices sit in more than 50 countries, making it valuable for validating app performance on local carriers in different markets . AI-driven issue cards automatically detect freezes, crashes, and latency before they impact users . The low-priced CloudTest Lite plan starts at $39/month for one user and 40 hours of manual testing, but automation and performance features are add-ons on higher tiers .  
**Best for:** Teams where slow load times are costing users or shipping in many countries needing real-world performance validation.

### BitBar
**Type:** Real device cloud with AlertSite monitoring integration
BitBar (SmartBear) provides real device cloud testing with support for Appium, XCTest, XCUITest, and mobile browser testing . A key differentiator is integration with **AlertSite** for mobile monitoring: BitBar test configurations can be scheduled as AlertSite monitors with automated alerts on failures or performance thresholds . Devices can be dedicated or shared, with options to run on currently idle devices .  
**Best for:** Teams wanting to convert functional tests into scheduled production monitoring with automated alerts.

### Perfecto
**Type:** Enterprise device cloud with on-prem and hybrid deployment
Perfecto (Perforce) provides real device cloud testing with support for iOS and Android, integrating with IBM DevOps Test UI and other enterprise frameworks . It offers SaaS, on-premises, and hybrid deployment options, with multi-region hosting across the US, UK, Europe, and Asia . Biometrics, sensor testing, network logs, and device vitals are supported .  
**Best for:** Enterprises needing flexible deployment (including air-gapped on-premises) and multi-region hosting.

### TestGrid
**Type:** Real device cloud with AI CoTester and device vitals
TestGrid provides real Android and iOS devices with its AI **CoTester** assistant that generates, runs, and maintains test flows, plus **AgentRx** for self-healing automation . It supports GPS simulation, biometric login, gesture automation, camera input, orientation changes, and network throttling . Real-time device vitals (CPU, memory, battery, network) are available during testing, along with Appium Inspector, ADB commands, and Charles Proxy workflows . A mobile banking case study reported 3x expanded regression coverage and 42% fewer device-specific production defects .  
**Best for:** Teams wanting AI-assisted test creation with strong real-world scenario simulation and device vitals.

### Firebase Test Lab
**Type:** Google-hosted device testing within Firebase
Firebase Test Lab provides cloud-based app testing infrastructure on devices hosted in Google data centers, including virtual Android test devices that run quickly on Arm hosts . It supports instrumentation tests, Robo tests (no pre-written tests required), game loop tests for iOS and Android, and XCTest for iOS .  
**Best for:** Teams already in the Firebase/Google ecosystem wanting automated testing without managing infrastructure.

### Digital.ai Testing
**Type:** Enterprise mobile testing with multi-region deployment
Digital.ai Testing (formerly Experitest) provides manual and automated testing on real and virtual iOS and Android devices across data centers in the US, UK, Europe, and Asia . It supports SaaS, on-premises, and hybrid deployment, with biometrics (Face ID, fingerprint), sensor testing, network logs, crash analysis, and interrupt testing . Dedicated or shared devices are available, with enterprise-grade security for sensitive data and builds .  
**Best for:** Enterprises needing multi-region hosting, air-gapped on-premises options, and comprehensive non-functional testing.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Real Mobile Device Cloud tools. The open-source ecosystem is **limited and fragmented**, with most projects either archived, in early-stage development, or focused on specific platforms.

### Sonic
**Stack:** Spring Cloud / Vue 3 / Docker / Netty | **License:** Open Source  
Sonic is an open-source cloud real-device platform positioned as an affordable alternative for small and mid-sized teams . Key features include:
- **Zero-code UI automation** with a block-based interface for building test flows and distributing tasks across devices
- **Cross-platform support**: Android, iOS, Web, Windows, and macOS
- **Remote control and debugging** across networks via Agent nodes, with integrated Chrome DevTools for WebView debugging and one-click proxy packet capture
- **Distributed cluster** supporting multi-datacenter deployment for global testing
- **CI/CD integration** with Jenkins plugin support and scheduled tasks
- **Visual reports** with screenshots, logs, and recordings

Deploys via Docker Compose with Java 17+, MySQL 8.0+, and ADB for Android devices . The backend uses Spring Cloud microservices with a Netty-based custom protocol for high-concurrency device communication .  
**Best for:** Small to mid-sized teams wanting a self-hosted cloud device platform with UI automation, remote debugging, and CI/CD integration without commercial licensing.

### GADS
**Stack:** Go / Appium / Selenium Grid / WebDriverAgent | **License:** AGPL-3.0 (open source) / Proprietary (hub-ui)  
GADS is a simple device farm for remote control of devices and Appium test execution on iOS and Android . Key features include:
- **Real-time video streaming** (MJPEG/WebRTC) for both iOS (via WebDriverAgent) and Android
- **Remote interactions**: tap, swipe, text input, clipboard, keyboard typing
- **App installation/uninstallation**, high-quality screenshots, device reservation system
- **Appium-compatible** with optional Selenium Grid 4 node registration
- **Smart TV automation** for Samsung Tizen OS and LG WebOS (automation only, no remote control)
- **Workspace management** with user access control per workspace

Platform support: full Android and iOS on macOS; limited iOS on Linux/Windows (Xcode dependency). The project is **dual-licensed** with the core under AGPL-3.0 and the `hub-ui` directory under a separate proprietary license (obfuscated, not modifiable) .  
**Best for:** Teams wanting a self-hosted device farm with Appium compatibility and remote control across Android, iOS, and even Smart TVs, accepting the dual-license arrangement.

### OpenSTF (archived)
**Stack:** JavaScript / Node.js / MongoDB | **License:** Other (open source)  
OpenSTF (Smartphone Test Farm) was the original open-source Android device farm, allowing control and management of Android devices from a browser . It had **13,958 GitHub stars** and 2,995 forks, with real-time screen viewing at 30-40 FPS, multitouch, drag-and-drop APK installation, reverse port forwarding, device inventory monitoring, and booking/partitioning systems . **Critical status:** The original project was **last pushed in May 2023** and has 464 open issues, making it effectively unmaintained . Forks and derivatives (like vkcom/devicehub) exist with MongoDB support and extended features, but the original OpenSTF is not recommended for new deployments .  
**Best for:** Historical reference only; evaluate maintained forks or alternatives like GADS for new projects.

### mobile-mcp
**Stack:** TypeScript / MCP (Model Context Protocol) | **License:** Apache-2.0  
mobile-mcp gives AI agents (Claude Code, Cursor, Copilot) direct access to iOS simulators, iOS real devices (USB), Android emulators, and Android real devices (ADB) through **30+ MCP tools** . It reads UI elements from the native accessibility tree rather than screenshots, reducing token usage and enabling deterministic interactions across screen sizes . Tools cover device management (orientation, GPS, clipboard), app lifecycle (install, launch, terminate), screen interaction (tap, swipe, long press), input (type text, hardware buttons), and diagnostics (logs, crash reports, screen recording). It also supports **cloud device access** via Mobile Next Cloud, billed per device-minute, and a Streamable HTTP mode for CI environments .  
**Best for:** Developers using AI coding agents wanting device access within the same session, or teams integrating mobile verification into CI/CD pipelines with agent-driven workflows.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Real Devices | Remote Control | Self-Hosted | Best For |
|----------|---------|-------|--------------|----------------|-------------|----------|
| **BrowserStack** | Proprietary | Cloud | ✅ 30,000+ | ✅ App Live | ❌ | Broadest coverage + free plan |
| **Sauce Labs** | Proprietary | Cloud | ✅ Extensive | ✅ RDA API | (Private) | Deep device control + AI |
| **Kobiton** | Proprietary | Cloud/On-prem | ✅ | ✅ | (On-prem) | Low entry price + AI |
| **AWS Device Farm** | Proprietary | Cloud | ✅ | ✅ Remote access | (Private lab) | AWS-native pay-per-minute |
| **HeadSpin** | Proprietary | Cloud/On-prem | ✅ 50+ countries | ✅ | (On-prem) | Real-world performance |
| **Sonic** | Open Source | Spring/Vue/Docker | ✅ Android/iOS | ✅ | ✅ | Self-hosted cloud device |
| **GADS** | AGPL-3.0 | Go/Appium | ✅ Android/iOS | ✅ MJPEG/WebRTC | ✅ | Appium-compatible farm |
| **mobile-mcp** | Apache-2.0 | TypeScript/MCP | ✅ (Local/cloud) | ✅ Agent-driven | ✅ | AI agent device access |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Real Mobile Device Cloud tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem for **full cloud device farms** is **limited and fragmented**. **Sonic** is the most comprehensive actively maintained open-source option for self-hosted cloud device testing with UI automation and remote debugging . **GADS** offers a focused Appium-compatible device farm with iOS/Android/Smart TV support under AGPL-3.0 . **OpenSTF**, the original Android device farm, is effectively unmaintained since May 2023 and should only be referenced or replaced with maintained forks . **mobile-mcp** represents a newer paradigm: AI-agent-driven device access via MCP rather than a traditional web console, filling a different gap than full device farms.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
