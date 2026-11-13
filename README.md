# Awesome Real Mobile Device Cloud

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/ishandutta2007/Awesome-Real-Mobile-Device-Cloud/pulls)

> A curated list of top **Real Mobile Device Cloud** platforms, enterprise device farms, and open-source testing infrastructure for running automated and manual tests on physical iOS and Android smartphones and tablets in the cloud.

---

## 📋 Table of Contents

- [Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
- [Open-Source Software](#-open-source-software)
- [Comparison Matrix](#-comparison-matrix)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌐 Sector Overview & Market Dynamics

The global mobile application testing and real-device cloud market is valued at approximately **$8 billion to $14 billion** and is projected to expand to **$19 billion – $35 billion** over the next decade at a CAGR of ~15–17%.

The sector exhibits a **moderately fragmented** structure driven by severe Android and iOS hardware/OEM fragmentation and rapidly evolving automation frameworks (Appium, Espresso, XCUITest). However, the infrastructure-heavy real-device cloud tier is **consolidating around hyperscale cloud providers and scaled QA leaders** (AWS, Google Firebase, BrowserStack, Sauce Labs/SmartBear) due to high capital expenditure, extensive device maintenance overhead, and enterprise CI/CD pipeline integration requirements.

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted real mobile device clouds sorted in descending order by parent company scale (revenue / market valuation).

| Platform | Company Valuation / Revenue | Starting Price | Free Tier / Trial Limits | Key Features |
|---|---|---|---|---|
| **[AWS Device Farm](https://aws.amazon.com/device-farm/)** | **Parent: $2.1T+ Market Cap** (Amazon / AWS: ~$105B+ ARR) | **$0.17 / device minute** (Pay-as-you-go) or $250/slot/mo unmetered | **1,000 device minutes** one-time free trial | Large physical iOS/Android fleet in AWS data centers, Appium/Espresso/XCUITest support, remote access interactive sessions, video/log capture. |
| **[Firebase Test Lab](https://firebase.google.com/docs/test-lab)** | **Parent: $2.1T+ Market Cap** (Alphabet / Google Cloud) | **$5.00 / physical device hour** ($0.083/min on Blaze Plan) | **Spark Plan (Free forever): 5 physical device runs/day** + 10 virtual device runs/day (resets daily) | Native Google infrastructure, instrumentation/Robo test runners, game loop support, deep Android Studio integration. |
| **[BrowserStack Real Device Cloud](https://www.browserstack.com/app-live)** | **$4 Billion Valuation** (~$230M ARR) | **$39 / month** (App Live Individual, billed annually) or $49/mo month-to-month | **30 minutes total free trial** on real devices (capped at ~1 min per device session; no permanent free plan) | 30,000+ real iOS & Android devices, App Live manual testing, App Automate, real-time debugging, network throttling, natural gestures. |
| **[BitBar](https://smartbear.com/product/bitbar/)** | **$1.8B – $2.0B Valuation** (SmartBear; ~$150M+ ARR) | **$39 / month** (Live Testing, billed annually) or $47/mo month-to-month | **14-day free trial** (No credit card required; full public cloud real-device and automation access) | SmartBear ecosystem, unlimited manual testing minutes, Appium/Selenium grid integration, AlertSite mobile monitoring hooks. |
| **[Perfecto](https://www.perfecto.io/)** | **~$1.07B+ Enterprise Value** (Perforce; ~$750M ARR) | **$300 / month** (Starting commercial tier / custom quote) | **14-day free trial** (Public real device cloud sandbox; local .apk/.ipa upload; app store downloads restricted) | Enterprise security, multi-region data centers (US/EU/APAC), biometric/sensor simulation, scriptless AI test creation, hybrid on-prem. |
| **[Sauce Labs Real Device Cloud](https://saucelabs.com/products/real-device-cloud)** | **$613M Valuation** (~$100M ARR) | **$199 / month** (Real Device Cloud, billed annually) or $249/mo month-to-month | **28-day free trial** (Includes 60 automated/live testing minutes across real devices and emulators/simulators) | Real Device Access (RDA) API with raw ADB/xcrun access, persistent sessions up to 24h, MCP-ready for AI agent test execution. |
| **[Digital.ai Testing](https://digital.ai/products/continuous-testing/)** | **~$135M – $140M ARR** (Private Equity backed) | **Custom Quote** (Enterprise-focused, historically starting ~$150/mo for base cloud packages) | **Dynamic trial upon demo request** (Typically 14 to 30 days scoped proof-of-concept; no self-serve free plan) | Formerly Experitest; enterprise mobile continuous testing, audio/biometric/network interrupt validation, on-prem/hybrid device labs. |
| **[Kobiton](https://kobiton.com/)** | **~$67M Valuation** (~$27.3M ARR; $46M total funding) | **$83 / month** (Startup Plan billed annually; includes 500 device minutes) | **15-day free trial** with **300 real-device minutes** and AI script generation included | Device-in-hand low-latency streaming, AI-assisted self-healing Appium scripts, hybrid cloud/on-prem deployment options. |
| **[HeadSpin](https://www.headspin.io/)** | **$28.2M Acquisition** (PartnerOne; ~$21M ARR) | **$39 / month** (CloudTest Lite billed annually; 40 hours manual testing) or $49/mo month-to-month | **Guided trial / demo sandbox upon request** (No permanent free tier) | Real carrier SIM testing across 50+ countries, 130+ UX/network vitals, automated AI root-cause analysis for latency and frame drops. |
| **[TestGrid](https://testgrid.io/)** | **Private / Multi-million Pre-Series A** (Bootstrapped & profitable) | **$199 / month** (AI & real-device cloud tier) | **1 to 2-week guided Proof-of-Concept (POC)** assisted by solution engineers (no self-serve free trial) | Real-time device vitals (CPU, memory, battery), AgentRx self-healing tests, AI CoTester script generator, Charles Proxy support. |

---

## 🟩 Open-Source Software

Self-hosted, community-driven device farm tools and mobile orchestration runtimes, sorted in descending order by GitHub Star count.

### [openstf/stf](https://github.com/openstf/stf) [![GitHub stars](https://img.shields.io/github/stars/openstf/stf?style=social&color=white)](https://github.com/openstf/stf/stargazers)
- **Stack:** JavaScript / Node.js / RethinkDB / ZeroMQ | **License:** Apache-2.0
- **Overview:** Smartphone Test Farm (STF) is the landmark open-source web application for debugging and managing Android smartphones, tablets, and smartwatches remotely from a browser.
- **Key Features:** Real-time screen viewing (30–40 FPS), multi-touch gesture support, keyboard input, drag-and-drop APK installation, shell execution, reverse port forwarding, and REST APIs.
- **Maintenance Note:** The original repository is unmaintained (last push 2023). Recommended to reference active forks such as DeviceFarmer for active deployments.

### [mobile-next/mobile-mcp](https://github.com/mobile-next/mobile-mcp) [![GitHub stars](https://img.shields.io/github/stars/mobile-next/mobile-mcp?style=social&color=white)](https://github.com/mobile-next/mobile-mcp/stargazers)
- **Stack:** TypeScript / Model Context Protocol (MCP) | **License:** Apache-2.0
- **Overview:** Gives AI coding agents (Claude Code, Cursor, Copilot) programmatic, direct control over iOS simulators, physical iPhones, Android emulators, and physical Android devices via 30+ MCP tools.
- **Key Features:** Accessibility tree semantic element targeting (low token consumption), tap/swipe/input simulation, biometric bypass, clipboard synchronization, screen recording, and Mobile Next Cloud integration.

### [DeviceFarmer/stf](https://github.com/DeviceFarmer/stf) [![GitHub stars](https://img.shields.io/github/stars/DeviceFarmer/stf?style=social&color=white)](https://github.com/DeviceFarmer/stf/stargazers)
- **Stack:** JavaScript / Node.js / Docker | **License:** Apache-2.0
- **Overview:** The primary community-maintained continuation of the original OpenSTF project, providing bug fixes, updated Android version support, and containerized deployment scripts.
- **Key Features:** Docker-compose setup, browser-based remote control of Android devices, remote adb connect debugging, user authorization layers, and automated device reservation.

### [SonicCloudOrg/sonic-server](https://github.com/SonicCloudOrg/sonic-server) [![GitHub stars](https://img.shields.io/github/stars/SonicCloudOrg/sonic-server?style=social&color=white)](https://github.com/SonicCloudOrg/sonic-server/stargazers)
- **Stack:** Java (Spring Cloud) / Vue 3 / Netty / Docker | **License:** Apache-2.0
- **Overview:** An enterprise-grade, distributed open-source cloud real-device platform for Android, iOS, Windows, macOS, and Web testing.
- **Key Features:** Zero-code block-based UI automation, high-performance remote control via Netty, multi-datacenter agent cluster deployment, Chrome DevTools WebView debugging, and Jenkins CI/CD plugins.

### [AppiumTestDistribution/appium-device-farm](https://github.com/AppiumTestDistribution/appium-device-farm) [![GitHub stars](https://img.shields.io/github/stars/AppiumTestDistribution/appium-device-farm?style=social&color=white)](https://github.com/AppiumTestDistribution/appium-device-farm/stargazers)
- **Stack:** Node.js / Appium 2.0 Plugin | **License:** Apache-2.0
- **Overview:** An official Appium 2.0 plugin designed to orchestrate and allocate connected physical Android & iOS devices, simulators, and emulators directly into parallel test runs.
- **Key Features:** Zero-configuration device discovery, round-robin and least-busy device scheduling, simulator leasing/spinning, dynamic session proxying, and seamless CI/CD test grid integration.

### [shamanec/GADS](https://github.com/shamanec/GADS) [![GitHub stars](https://img.shields.io/github/stars/shamanec/GADS?style=social&color=white)](https://github.com/shamanec/GADS/stargazers)
- **Stack:** Go / Appium / WebDriverAgent / Selenium Grid | **License:** AGPL-3.0 (Core)
- **Overview:** A lightweight, self-hosted device farm providing live remote control and Appium test execution across Android, iOS, and Smart TVs.
- **Key Features:** Real-time WebRTC/MJPEG video streaming, full remote interaction (touch, keyboard, clipboard), Appium 2 node integration, and Smart TV automation for Samsung Tizen OS, LG WebOS, and Android TV.

### [zebrunner/mcloud](https://github.com/zebrunner/mcloud) [![GitHub stars](https://img.shields.io/github/stars/zebrunner/mcloud?style=social&color=white)](https://github.com/zebrunner/mcloud/stargazers)
- **Stack:** Docker / Python / Shell / Selenium Grid | **License:** Apache-2.0
- **Overview:** Production-ready mobile test automation infrastructure for scalable Docker-based Android and iOS device farms with integrated Appium endpoints.
- **Key Features:** Auto-detects connected USB devices, launches isolated Appium containers per device, streams device screens via browser, and integrates natively with Selenium Grid and Zebrunner QA platforms.

---

## 📊 Comparison Matrix

| Platform / Tool | Deployment | Real Devices | Remote Control | Appium Compatible | Starting Tier | License / Model |
|---|---|---|---|---|---|---|
| **AWS Device Farm** | Cloud (AWS) | iOS & Android | ✅ Browser | ✅ Native | $0.17/min (1,000 min trial) | Commercial SaaS |
| **Firebase Test Lab** | Cloud (GCP) | iOS & Android | ✅ Test Runs | ✅ Instrumentation | Free 5 runs/day Spark ($5/hr Blaze) | Commercial SaaS / Free Tier |
| **BrowserStack** | Cloud | 30,000+ Devices | ✅ App Live | ✅ App Automate | $39/mo (30 min trial) | Commercial SaaS |
| **BitBar** | Cloud / Dedicated | iOS & Android | ✅ Live Testing | ✅ Full Grid | $39/mo (14-day trial) | Commercial SaaS |
| **Perfecto** | Cloud / On-prem | iOS & Android | ✅ Web UI | ✅ Supported | $300/mo (14-day trial) | Enterprise Commercial |
| **Sauce Labs** | Cloud / Dedicated | iOS & Android | ✅ RDA API | ✅ Extended | $199/mo (28-day trial) | Commercial SaaS |
| **Digital.ai Testing** | Cloud / On-prem | iOS & Android | ✅ Web Console | ✅ Supported | Custom quote (Guided trial) | Enterprise Commercial |
| **Kobiton** | Cloud / On-prem | iOS & Android | ✅ Real-time | ✅ Self-healing | $83/mo (15-day / 300 min trial) | Commercial SaaS |
| **HeadSpin** | Cloud / On-prem | SIM in 50+ Countries| ✅ Public Cloud | ✅ Supported | $39/mo (Guided demo/trial) | Commercial SaaS |
| **TestGrid** | Cloud / On-prem | iOS & Android | ✅ Browser | ✅ Supported | $199/mo (Guided 1-2 wk POC) | Commercial SaaS |
| **openstf/stf** | Self-hosted | Android | ✅ Browser | 🔄 Via Plugin | Free / Open-Source | Apache-2.0 (Archived) |
| **mobile-mcp** | Local / Cloud | iOS & Android | ✅ AI Agent MCP | 🔄 MCP Tooling | Free / Open-Source | Apache-2.0 |
| **DeviceFarmer/stf**| Self-hosted | Android | ✅ Browser | 🔄 Via Plugin | Free / Open-Source | Apache-2.0 |
| **Sonic** | Self-hosted | iOS & Android | ✅ Browser UI | ✅ Built-in | Free / Open-Source | Apache-2.0 |
| **Appium Device Farm** | Self-hosted / Grid | iOS & Android | ❌ CLI / Grid | ✅ Native Plugin | Free / Open-Source | Apache-2.0 |
| **GADS** | Self-hosted | iOS, Android, TVs | ✅ WebRTC/MJPEG | ✅ Supported | Free / Open-Source | AGPL-3.0 |
| **zebrunner/mcloud**| Self-hosted | iOS & Android | ✅ Browser | ✅ Native Grid | Free / Open-Source | Apache-2.0 |

---

## 🔍 SEO Keywords & Search Queries

If you're searching for testing solutions, this list covers the following topics:
`real mobile device cloud`, `mobile device farm open source`, `best cloud device farm for appium`, `browserstack alternatives`, `sauce labs alternatives`, `aws device farm pricing`, `self hosted mobile testing lab`, `android device farm docker`, `ios real device automation in cloud`, `kobiton vs browserstack vs headspin`, `model context protocol mobile testing`.

---

## 🤝 Contributing

Contributions are welcome! Please follow these guidelines:
1. Ensure the tool or platform is actively maintained and relevant to real mobile device clouds or mobile test farms.
2. For open-source tools, include the repository URL, tech stack, license, and GitHub stars badge link formatted as `[![GitHub stars](https://img.shields.io/github/stars/<owner>/<repo>?style=social&color=white)](https://github.com/<owner>/<repo>/stargazers)`.
3. Keep descriptions objective, concise, and focused on device testing capabilities.

Submit a Pull Request with your additions or updates!

---

## 📄 License

This repository and list are dedicated to the public domain under the [Creative Commons Zero v1.0 Universal](LICENSE) license.
