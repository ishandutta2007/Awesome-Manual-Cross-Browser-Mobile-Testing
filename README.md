# Awesome-Manual-Cross-Browser-Mobile-Testing

# Awesome Manual Cross-Browser & Mobile Testing

> A curated list of top Manual Cross-Browser and Mobile Testing platforms — both SaaS/Hosted commercial device clouds and open-source alternatives for interactive testing on real browsers and physical devices.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [BrowserStack Live & App Live](#browserstack-live--app-live)
  - [Sauce Labs Live Testing](#sauce-labs-live-testing)
  - [LambdaTest Real Time Testing](#lambdatest-real-time-testing)
  - [Kobiton](#kobiton)
  - [HeadSpin CloudTest Lite](#headspin-cloudtest-lite)
  - [TestingBot Live](#testingbot-live)
  - [TestGrid Real Device Cloud](#testgrid-real-device-cloud)
  - [Browserling](#browserling)
  - [Appetize.io](#appetizeio)
  - [Comparium](#comparium)
- [Open-Source Software](#-open-source-software)
  - [Selenium Grid](#selenium-grid)
  - [Playwright Codegen & UI Mode](#playwright-codegen--ui-mode)
  - [GADS](#gads)
  - [Device Farmer STF](#device-farmer-stf)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Manual Cross-Browser and Mobile Testing platforms. These are not open-source but are included as reference points for feature comparison.

### BrowserStack Live & App Live
**Type:** Real browser and device cloud for interactive manual testing
BrowserStack provides two distinct manual testing products: **Live** for websites on real desktop and mobile browsers, and **App Live** for native mobile apps on real Android and iOS devices . Key capabilities include cross-browser testing, responsive testing, local testing, screenshot capture, and session debugging for web; and app upload/install, gesture testing, network simulation, device logs, screenshots, and video recording for mobile . A free trial is available.  
**Best for:** Teams wanting the broadest real device and browser coverage for manual exploratory testing without maintaining an in-house lab.

### Sauce Labs Live Testing
**Type:** Interactive manual testing on real browsers and devices
Sauce Labs provides live testing for evaluating usability and user experience aspects that are difficult to assess through automation—such as clunky design or subjective UX issues that a script would not catch . It is also positioned for exploratory testing, where testers access the application unscripted and use their skill set to discover edge cases .  
**Best for:** Teams already using Sauce Labs for automation wanting to extend into manual UX and exploratory testing on the same platform.

### LambdaTest Real Time Testing
**Type:** Live interactive testing with debugging tools
LambdaTest (TestMu AI) provides Real Time Testing for both web and native mobile apps . For mobile, you can upload `.apk` files up to 1GB and test on Android emulators and iOS simulators, with a "Mark As Bug" feature that captures screenshots and integrates with issue trackers like YouTrack . The left panel includes **DevTools** for viewing Network, App, and Device logs, a **UI Inspector** for viewing XML details and properties, **video recording**, and **device controls** for keyboard language, orientation, sleep mode, and volume .  
**Best for:** Teams wanting a feature-dense interactive testing console with integrated debugging, screenshots, and bug logging.

### Kobiton
**Type:** Real device manual testing with root cause analysis
Kobiton provides manual testing on real cloud devices with best-in-class responsiveness for near zero-latency "device in hand" feel, including complex gestures like pinch-to-zoom and natural swipes . Key differentiators include **session video recording** with discrete step-by-step breakdowns and screenshots for interactive debugging, full device logs, and system metrics (memory, battery) captured alongside the session .  
**Best for:** Teams needing detailed root cause analysis and step-by-step session evidence during manual testing.

### HeadSpin CloudTest Lite
**Type:** Affordable real device manual testing for emerging teams
HeadSpin's CloudTest Lite is explicitly positioned for individual testers and emerging teams, offering **unlimited session durations** (up to 40 hours per month) rather than the 5-10 minute limits common on other platforms . Features include ADB shell for advanced debugging, a mini remote control for precise gesture testing, support for all major mobile formats (APK, APK+, OBB, IPA, XAPX), and **automatic device cleaning** after each session for data security .  
**Best for:** Startups and individual testers needing long, uninterrupted manual testing sessions without session time limits.

### TestingBot Live
**Type:** Budget-friendly live manual testing
TestingBot offers a Live plan for manual testing of websites and apps at **€20/month (billed annually)** or €30 month-to-month, with access to 6,100+ real browsers and devices . It is positioned as an affordable entry point for teams needing live cross-browser testing without enterprise contracts.  
**Best for:** Cost-conscious teams wanting access to a broad real device/browser matrix for manual testing.

### TestGrid Real Device Cloud
**Type:** Real device testing with AI-assisted debugging
TestGrid provides real Android and iOS devices with **AI CoTester** for generating and maintaining test flows, and **AgentRx** for self-healing automation . For manual testing, it offers Appium Inspector, ADB commands, browser DevTools, Charles Proxy workflows, network capture, HAR files, logs, crash reports, screenshots, and video playback . **Real-time device vitals** (CPU, memory, battery, network) are available during testing . A mobile banking case study reported 3x expanded regression coverage and 42% fewer device-specific production defects .  
**Best for:** Teams wanting AI-assisted debugging and real-time device vitals alongside manual testing.

### Browserling
**Type:** Real browser testing with full OS control
Browserling provides live interactive browser testing on real Windows, Android, macOS, and iOS environments . The **Developer Pro plan ($29/month billed annually)** adds macOS and iOS platform browsers (including native Safari on iPhone and iPad), Linux via WSL, geobrowsing in 50+ countries, mobile and residential IPs, Tor exit nodes, unlimited file uploads/downloads, admin rights, VM reboot, and BIOS access . A free plan is available for limited occasional testing.  
**Best for:** Developers needing deep OS-level control, native Safari on iOS, and advanced networking options during manual testing.

### Appetize.io
**Type:** Browser-based mobile app testing without downloads
Appetize lets you run native iOS and Android apps directly in a web browser with no downloads, plugins, or extra permissions required . It is positioned for live app previews, training and support, sales and marketing demos, and testing and automation . You upload your app, then run or embed it, with query parameters for customization.  
**Best for:** Teams wanting to share runnable mobile app demos or perform quick manual checks without installing anything.

### Comparium
**Type:** Chrome extension for instant cross-browser screenshots
Comparium's Chrome extension allows you to capture screenshots of a web page and run real-time tests with a single click, checking appearance across multiple browsers and operating systems without installing a device lab . It supports unlimited screenshots per session, manual and automatic comparison modes, and screenshot-to-mockup comparison. A Comparium account is required.  
**Best for:** Quick visual cross-browser checks directly from Chrome without a full testing platform.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Manual Cross-Browser and Mobile Testing tools. The open-source ecosystem spans **grid-based browser automation (with interactive debugging)**, **browser-native codegen and UI modes**, **self-hosted Appium-compatible device farms**, and **Android device farm managers**.

### Selenium Grid
**Stack:** Java / Docker / Kubernetes | **License:** Apache-2.0
Selenium Grid is the foundational open-source infrastructure for distributed browser testing, enabling parallel test runs across multiple browsers and machines. While primarily used for automation, Grid 4's **interactive session support** via its web console allows manual inspection of running sessions, and the grid can be used to provide remote browser access for manual testers. Grid 4.41.0 ships 167+ Docker image variants across Chrome, Edge, and Firefox, with a **Kubernetes Dynamic Grid** that provisions one browser Pod per session request .  
**Best for:** Teams wanting full control over a distributed browser grid that can serve both automated and interactive manual testing, accepting the operational overhead of managing browser versions and scaling.

### Playwright Codegen & UI Mode
**Stack:** Node.js / Python / Java / .NET | **License:** Apache-2.0
Playwright includes **Codegen** for recording interactions and generating test code in real time, and **UI Mode** for interactive test exploration with time-travel debugging, watch mode, and a trace viewer. While Codegen is automation-focused, UI Mode provides a rich interactive environment for exploring application behavior across Chromium, Firefox, and WebKit from a single API. The recorder analyzes the rendered page and recommends resilient locators (role, text, test ID) to reduce flakiness .  
**Best for:** Developers wanting a free, built-in interactive environment for exploring web app behavior and generating automation from manual interactions.

### GADS
**Stack:** Go / Appium / WebDriverAgent | **License:** AGPL-3.0 (core) / Proprietary (hub-ui)
GADS is a self-hosted device farm for **remote control of Android and iOS devices** and Appium test execution . Key manual testing capabilities include **real-time video streaming** (MJPEG/WebRTC) for both iOS and Android, remote interactions (tap, swipe, text input, clipboard, keyboard typing), app installation/uninstallation, and a device reservation system with workspace-level access control . Platform support: full Android and iOS on macOS; limited iOS on Linux/Windows due to Xcode dependency. The core is AGPL-3.0, with the `hub-ui` directory under a separate proprietary license .  
**Best for:** Teams wanting a self-hosted device farm with genuine remote control across Android and iOS for manual testing, accepting the dual-license arrangement.

### Device Farmer STF
**Stack:** Node.js / TypeScript / RethinkDB / ADB | **License:** Apache-2.0
Device Farmer STF is the leading actively maintained open-source **Android device farm**, allowing teams to share and control physical devices remotely via a web interface . It supports the full ADB workflow including shell, logcat, and file management through the web UI, with a **Remote Debug panel** that exposes an `adb connect` command for connecting a remote device to your workstation for Chrome DevTools inspection . It is a maintained fork/derivative of the original OpenSTF project.  
**Best for:** Android QA teams wanting to share physical devices across a distributed team with genuine remote ADB debugging access for manual testing.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Real Browsers | Real Devices | OS-Level Control | Self-Hosted | Best For |
|----------|---------|-------|--------------|--------------|------------------|-------------|----------|
| **BrowserStack** | Proprietary | Cloud | ✅ | ✅ | (Limited) | ❌ | Broadest manual coverage |
| **Sauce Labs** | Proprietary | Cloud | ✅ | ✅ | ❌ | ❌ | UX + exploratory on existing platform |
| **LambdaTest** | Proprietary | Cloud | ✅ | (Emulators) | ❌ | ❌ | Debugging + bug logging |
| **Kobiton** | Proprietary | Cloud | ❌ | ✅ | ❌ | ❌ | Step-by-step session evidence |
| **HeadSpin Lite** | Proprietary | Cloud | ❌ | ✅ | ✅ ADB shell | ❌ | Long uninterrupted sessions |
| **Browserling** | Proprietary | Cloud | ✅ | ✅ iOS | ✅ Full VM | ❌ | OS-level control + native Safari |
| **Appetize.io** | Proprietary | Cloud | ❌ | Virtual | ❌ | ❌ | Browser-based app demos |
| **Selenium Grid** | Apache-2.0 | Java/Docker | ✅ | ❌ | ❌ | ✅ | Distributed browser access |
| **Playwright** | Apache-2.0 | Node/Python | ✅ | ❌ | ❌ | ✅ (Built-in) | Interactive exploration + codegen |
| **GADS** | AGPL-3.0 | Go/Appium | ❌ | ✅ Android/iOS | (Check) | ✅ | Self-hosted device remote control |
| **Device Farmer STF** | Apache-2.0 | Node.js/ADB | ❌ | ✅ Android | ✅ ADB | ✅ | Shared Android device access |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Manual Cross-Browser or Mobile Testing tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The open-source landscape for **manual cross-browser and mobile testing** is **anchored by infrastructure** rather than dedicated manual testing consoles. **Selenium Grid** and **Playwright** provide the browser execution layer that manual testers can use interactively, though neither is purpose-built for manual session management . For **mobile device access**, **GADS** and **Device Farmer STF** are the strongest open-source options—GADS provides remote control across Android and iOS with video streaming, while Device Farmer STF focuses on Android with deep ADB integration . No open-source project replicates BrowserStack Live's polish, HeadSpin Lite's unlimited session durations, or Kobiton's step-by-step session breakdowns, but these tools cover the core remote access and debugging workflows for self-hosted manual testing.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
