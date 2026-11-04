
# Best Magisk Modules & Root Projects for Android

> A hand-picked showcase of useful Magisk modules, Zygisk frameworks, LSPosed modules, systemless tools, root utilities, audio mods, privacy tools, and Android customization projects.

**Author / researched by:** Sidharth S (@zidhuxd)  
**Use this list as:** A discovery index. Open the GitHub source, read the project README and release notes, and confirm compatibility with your device before installing anything.

[![Android](https://img.shields.io/badge/platform-Android-3DDC84?logo=android&logoColor=white)](https://www.android.com/)
[![Magisk](https://img.shields.io/badge/root-Magisk-8A2BE2)](https://github.com/topjohnwu/Magisk)
[![Projects](https://img.shields.io/badge/showcase-100%20projects-1f6feb)](#-the-100-project-showcase)
[![ZidhuXD](https://img.shields.io/badge/curated%20by-ZidhuXD-111827)](#about-zidhuxd)

## Contents

- [How to read the list](#how-to-read-the-list)
- [The 100-project showcase](#-the-100-project-showcase)
  - [Root management and module infrastructure](#1-root-management-and-module-infrastructure)
  - [Zygisk and LSPosed frameworks](#2-zygisk-and-lsposed-frameworks)
  - [Play Integrity and environment tools](#3-play-integrity-and-environment-tools)
  - [Privacy, ad blocking, and networking](#4-privacy-ad-blocking-and-networking)
  - [Debloating and system customization](#5-debloating-and-system-customization)
  - [Security, certificates, and root utilities](#6-security-certificates-and-root-utilities)
  - [Audio and media](#7-audio-and-media)
  - [Performance and gaming](#8-performance-and-gaming)
  - [Classic and legacy projects](#9-classic-and-legacy-projects)
- [Simple installation flow](#simple-installation-flow)
- [About ZidhuXD](#about-zidhuxd)
- [Source directories](#source-directories)

## How to read the list

| Label | Meaning |
|---|---|
| `Module` | Normally flashed as a Magisk-compatible ZIP or loaded by a root manager. |
| `Zygisk` | Injects into Android app processes and usually needs a compatible Zygisk implementation. |
| `LSPosed` | A framework or app module for Xposed-style hooks; not every entry is a flashable Magisk ZIP. |
| `Utility` | A root app, manager, recovery tool, or companion project used with Magisk. |
| `Conditional` | Useful for a specific device, ROM, app, or workflow; not a default install. |
| `Legacy` | Kept for reference because it appears in older lists, but check maintenance carefully before using it. |

## 🔥 The 100-project showcase

### 1. Root management and module infrastructure

| # | Project | Type | Description | Direct GitHub link |
|---:|---|---|---|---|
| 1 | **Magisk** | Core | Systemless root framework with MagiskSU, boot-image tools, modules, and Zygisk. | <a href="https://github.com/topjohnwu/Magisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 2 | **KernelSU** | Core | Kernel-based Android root solution with a module ecosystem that overlaps with Magisk tooling. | <a href="https://github.com/tiann/KernelSU" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 3 | **APatch** | Core | Android kernel and system patching framework with module support and a root manager. | <a href="https://github.com/bmax121/APatch" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 4 | **MMRL** | Utility | Open-source module manager for browsing and managing Magisk, KernelSU, and APatch modules. | <a href="https://github.com/DerGoogler/MMRL" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 5 | **Magisk Manager for Recovery Mode** | Utility | Terminal-based recovery tool for inspecting and managing Magisk modules when Android will not boot normally. | <a href="https://github.com/Rikj000/Magisk-Manager-for-Recovery-Mode" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 6 | **Mountify** | Module | OverlayFS and mount infrastructure intended to change how systemless modules are mounted. | <a href="https://github.com/backslashxx/mountify" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 7 | **NoMount** | Module | Mountless module injection using kernel VFS redirection, per-app isolation, and WebUI controls. | <a href="https://github.com/maxsteeel/nomount" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 8 | **ZeroMount** | Module | Mountless module loading with VFS redirection, SUSFS integration, WebUI, and bootloop safeguards. | <a href="https://github.com/Enginex0/zeromount" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 9 | **Magic Mount Metamodule** | Module | Metamodule implementation that provides an alternative Magic Mount-based module engine. | <a href="https://github.com/Tools-cx-app/meta-magic_mount-rs" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 10 | **Magisk Bootloop Protector** | Module | Attempts to protect the device from bootloops caused by problematic Magisk modules. | <a href="https://github.com/Magisk-Modules-Alt-Repo/abootloop" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 11 | **YetAnotherBootloopProtector** | Module | Monitors boot and SystemUI failures and provides another recovery-oriented module option. | <a href="https://github.com/Magisk-Modules-Alt-Repo/YetAnotherBootloopProtector" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |

### 2. Zygisk and LSPosed frameworks

| # | Project | Type | Description | Direct GitHub link |
|---:|---|---|---|---|
| 12 | **LSPosed** | Zygisk / LSPosed | ART hooking framework that exposes Xposed-compatible APIs for app and system customization. | <a href="https://github.com/LSPosed/LSPosed" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 13 | **Vector** | Zygisk / LSPosed | Open-source LSPosed fork focused on dynamic module loading and framework improvements. | <a href="https://github.com/JingMatrix/Vector" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 14 | **ZygiskNext** | Zygisk | Standalone Zygisk implementation for Magisk, KernelSU, and APatch configurations. | <a href="https://github.com/Dr-TSNG/ZygiskNext" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 15 | **NeoZygisk** | Zygisk | Alternative Zygisk implementation using ptrace-based injection and a minimalist design. | <a href="https://github.com/JingMatrix/NeoZygisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 16 | **ReZygisk** | Zygisk | C-based Zygisk implementation with custom linker work and support for modern Android setups. | <a href="https://github.com/PerformanC/ReZygisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 17 | **OnyxZygisk** | Zygisk | Ptrace-powered Zygisk implementation with WebUI controls and configurable module behavior. | <a href="https://github.com/OnyxZygisk/OnyxZygisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 18 | **VexZygisk** | Zygisk | Standalone Zygisk implementation aimed at KernelSU and APatch environments. | <a href="https://github.com/Lxiaoyao077/VexZygisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 19 | **YukiZygisk** | Zygisk | Kernel-oriented Zygisk implementation with status and settings controls. | <a href="https://github.com/Rouyashiki/YukiZygisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 20 | **Zygisk Assistant** | Zygisk | Root-environment management and hiding helper for Magisk, KernelSU, and APatch setups. | <a href="https://github.com/snake-4/Zygisk-Assistant" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 21 | **Shamiko** | Zygisk | Zygisk-based root-visibility tool distributed through the LSPosed project release channel. | <a href="https://github.com/LSPosed/LSPosed.github.io/releases" target="_blank" rel="noopener noreferrer">GitHub Releases ↗</a> |

> **Do not install all Zygisk entries together.** Pick the implementation required by your root setup and follow its own README.

### 3. Play Integrity and environment tools

| # | Project | Type | Description | Direct GitHub link |
|---:|---|---|---|---|
| 22 | **PlayIntegrityFix** | Conditional module | Attempts to obtain a valid Play Integrity device verdict; the project states that it is not a general root-hiding tool. | <a href="https://github.com/KOWX712/PlayIntegrityFix" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 23 | **Play Integrity Fork** | Conditional module | Maintained fork that works with configurable build fields and system properties for integrity troubleshooting. | <a href="https://github.com/osm0sis/PlayIntegrityFork" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 24 | **TrickyStore** | Conditional module | Advanced keystore and certificate-chain tooling for specialized attestation setups. | <a href="https://github.com/5ec1cff/TrickyStore" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 25 | **TrickyStore OSS** | Conditional module | Open-source TrickyStore alternative for users who need a different implementation. | <a href="https://github.com/beakthoven/TrickyStoreOSS" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 26 | **TEESimulator** | Conditional module | Software-based Trusted Execution Environment simulator for key-attestation testing. | <a href="https://github.com/JingMatrix/TEESimulator" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 27 | **TEESimulator-RS** | Conditional module | Rust-oriented TEESimulator fork with certificate generation and persistence features. | <a href="https://github.com/Enginex0/TEESimulator-RS" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 28 | **Tricky Addon — Update Target List** | Utility | WebUI helper for configuring TrickyStore target lists on supported root managers. | <a href="https://github.com/KOWX712/Tricky-Addon-Update-Target-List" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 29 | **Specter** | Conditional module | Unified Play Integrity and root-environment configuration project for advanced users. | <a href="https://github.com/dpejoh/specter" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 30 | **YuriKey** | Conditional module | Systemless approach to advanced integrity and key-attestation experiments. | <a href="https://github.com/dpejoh/yurikey" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 31 | **Sensitive Props** | Conditional module | Applies device-property changes and device-specific fixes for integrity experiments. | <a href="https://github.com/Pixel-Props/sensitive-props" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |

> **Integrity warning:** A temporary verdict is not a guarantee. App developers can use additional checks, and attempts to alter attestation may violate an app’s terms.

### 4. Privacy, ad blocking, and networking

| # | Project | Type | Description | Direct GitHub link |
|---:|---|---|---|---|
| 32 | **bindhosts** | Module | Systemless hosts manager for Magisk, KernelSU, and APatch with multiple redirect methods. | <a href="https://github.com/bindhosts/bindhosts" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 33 | **Re-Malwack** | Module / utility | Root and non-root ad-blocking suite with configurable hosts and filtering workflows. | <a href="https://github.com/ZG089/Re-Malwack" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 34 | **AdGuardHome Magisk** | Module | Runs AdGuard Home as a Magisk-compatible DNS filtering module on Android. | <a href="https://github.com/410154425/AdGuardHome_magisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 35 | **AdGuard Certificate Module** | Module | Adds the AdGuard certificate path needed for system-wide HTTPS filtering in supported setups. | <a href="https://github.com/AdguardTeam/adguardcert" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 36 | **Magisk Ad Blocking Module** | Module | Hosts-based Android ad blocking through a systemless Magisk installation. | <a href="https://github.com/pantsufan/Magisk-Ad-Blocking-Module" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 37 | **StevenBlock** | Module | Advanced ad-blocking module compatible with Magisk, KernelSU, and APatch. | <a href="https://github.com/mikropsoft/StevenBlock" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 38 | **10007** | Module | Hosts-based blocking project with Android ad-blocking lists and systemless integration. | <a href="https://github.com/lingeringsound/10007" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 39 | **box for Magisk** | Module | Transparent proxy and network-routing module for rooted Android devices. | <a href="https://github.com/taamarin/box_for_magisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 40 | **NetProxy-Magisk** | Module | sing-box-based transparent proxy module with one-click controls. | <a href="https://github.com/Fanju6/NetProxy-Magisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 41 | **magisk-tailscaled** | Module | Runs Tailscale on rooted Android for private mesh networking and secure remote access. | <a href="https://github.com/anasfanani/magisk-tailscaled" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 42 | **ZeroTier Magisk** | Module | Adds ZeroTier networking support and an Android controller workflow for rooted devices. | <a href="https://github.com/eventlOwOp/zerotier-magisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 43 | **zaprett** | Module | Android port of zapret-style network filtering and censorship-bypass tooling. | <a href="https://github.com/egor-white/zaprett" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |

> Pick one primary hosts or DNS workflow. Multiple hosts modules can overwrite the same files or redirect layer.

### 5. Debloating and system customization

| # | Project | Type | Description | Direct GitHub link |
|---:|---|---|---|---|
| 44 | **De-Bloater** | Root utility | Creates a systemless debloat module for removing or hiding selected preinstalled packages. | <a href="https://github.com/sunilpaulmathew/de-bloater" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 45 | **SystemlessDebloater** | Module | Hides selected system apps using systemless overlays and configurable package lists. | <a href="https://github.com/Magisk-Modules-Alt-Repo/SystemlessDebloater" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 46 | **Scalpel** | Root utility | Precision debloat and systemize tool for rooted Android devices. | <a href="https://github.com/Enginex0/Scalpel" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 47 | **System App Nuker** | Module | WebUI-driven system-app debloating module for supported Magisk, KernelSU, and APatch setups. | <a href="https://github.com/ChiseWaguri/systemapp_nuker" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 48 | **PixelXpert-Next** | Module / LSPosed | Pixel-oriented system customization project for newer Android builds. | <a href="https://github.com/anirudhgupta109/PixelXpert-Next" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 49 | **Pixel Launcher Extended** | Module | Adds extra Pixel Launcher customization and behavior options through a systemless module. | <a href="https://github.com/saitamasahil/Pixel-Launcher-Extended" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 50 | **HyperOS Launcher** | Module | Extends HyperOS Launcher with additional blur, widget, dock, and recent-app options. | <a href="https://github.com/Mods-Center/HyperOS-Launcher" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 51 | **HyperOS Theme Manager** | Module / utility | Expands HyperOS theme and customization features on compatible Xiaomi devices. | <a href="https://github.com/Mods-Center/HyperOS-Theme-Manager" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 52 | **HyperUnlocked** | Module | Unlocks selected high-end Xiaomi or HyperOS features on supported devices. | <a href="https://github.com/ukriu/HyperUnlocked" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 53 | **WebView Manager Module** | Module | Helps switch or manage the Android WebView implementation used by the device. | <a href="https://github.com/Androidacy/WebviewManager-Module" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 54 | **PixelFeatureDrops** | Module | Adds selected Pixel feature files and related device-property configuration. | <a href="https://github.com/ayush5harma/PixelFeatureDrops" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 55 | **MakeFontsGreatAgain** | Module | System-wide font override with Unicode-range filtering and masking options. | <a href="https://github.com/Numbersf/MakeFontsGreatAgain" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 56 | **Noto CJK** | Module | Installs Noto Sans CJK and Noto Serif CJK font coverage through a systemless module. | <a href="https://github.com/simonsmh/notocjk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |

### 6. Security, certificates, and root utilities

| # | Project | Type | Description | Direct GitHub link |
|---:|---|---|---|---|
| 57 | **DisableFlagSecure** | LSPosed | Enables screenshots or recording in apps that use Android’s `FLAG_SECURE` when compatible. | <a href="https://github.com/LSPosed/DisableFlagSecure" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 58 | **FlagSecurePatcher** | Module | Patches supported system services to change secure-window and screenshot behavior. | <a href="https://github.com/j-hc/FlagSecurePatcher" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 59 | **Zygisk Cacerts** | Zygisk | Replaces or manages the local root certificate store for supported testing workflows. | <a href="https://github.com/vvb2060/zygisk_cacerts" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 60 | **CertBridge** | Module | Merges custom certificates into the system trust store with WebUI and Android-version support. | <a href="https://github.com/Eikeitsu/CertBridge" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 61 | **AntiSafetyCore** | Module | Holds selected Google SafetyCore and Key Verifier package names using systemless placeholders. | <a href="https://github.com/Astoritin/AntiSafetyCore" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 62 | **Simple Flag Secure** | Module | Toggleable secure-flag behavior for screenshot and recording experiments on rooted devices. | <a href="https://github.com/ShivamXD6/Simple-Flag-Secure" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 63 | **Built-in BusyBox** | Module | Exposes Magisk’s BusyBox applets for scripts, terminal commands, and module compatibility. | <a href="https://github.com/Magisk-Modules-Alt-Repo/BuiltIn-BusyBox" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 64 | **Rclone FUSE3 Magisk** | Module | Integrates rclone and FUSE support for mounting or managing remote storage. | <a href="https://github.com/NewFuture/rclone-fuse3-magisk" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 65 | **Docker Magisk** | Module | Experimental Docker support for rooted Android environments. | <a href="https://github.com/mgksu/dockerd" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 66 | **TermuxRootMods** | Module | Adds extra root-oriented Termux capabilities and shell helpers. | <a href="https://github.com/rompelhd/TermuxRootMods" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 67 | **Android Subsystem for GNU/Linux** | Module | Linux subsystem module for Android with Magisk, KernelSU, and APatch support. | <a href="https://github.com/RuriOSS/asl" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 68 | **NetHunter Wi-Fi Firmware** | Module | Adds firmware needed for selected external wireless adapters and NetHunter workflows. | <a href="https://github.com/rithvikvibhu/nh-magisk-wifi-firmware" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 69 | **Call Recorder Axet** | Module | Installs the axet call-recorder app and its root module components. | <a href="https://github.com/di72nn/callrecorder-axet" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 70 | **USB Mass Storage** | Module | Turns a rooted Android device into a USB mass-storage device in supported configurations. | <a href="https://github.com/Enginex0/UsbMassStorage" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 71 | **StorageRedirect** | LSPosed | Redirects app external-storage paths to work around selected Android storage restrictions. | <a href="https://github.com/AcE77505/storage-redirect-module" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 72 | **No Photo Picker API** | LSPosed | Lets selected apps use the classic document picker instead of the Android Photo Picker API. | <a href="https://github.com/yureitzk/NoPhotoPickerAPI" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 73 | **CleanShare** | LSPosed | Removes suggested contacts and conversations from the Android share sheet. | <a href="https://github.com/hxreborn/cleanshare" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 74 | **Remember My Sort** | LSPosed | Makes the native Android file picker remember sorting preferences. | <a href="https://github.com/hxreborn/remember-my-sort" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 75 | **ShiroSU Utils** | Utility | Multi-platform Android modding and tweaking utility for rooted-device workflows. | <a href="https://github.com/ShIroRRen/ShiroSU-Utils" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 76 | **Compatible Magisk Mirroring** | Module | Compatibility layer for installing pure Magisk modules on selected alternative root managers. | <a href="https://github.com/Magisk-Modules-Alt-Repo/compatible-magisk-mirroring" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |

### 7. Audio and media

| # | Project | Type | Description | Direct GitHub link |
|---:|---|---|---|---|
| 77 | **ViPER4Android FX** | Module | Classic system audio-effects module with equalizer, profiles, and driver installation. | <a href="https://github.com/Magisk-Modules-Repo/ViPER4Android-FX" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 78 | **ViPERFX RE** | Module | Reverse-engineered modern ViPER audio implementation with separate Android audio integration paths. | <a href="https://github.com/likelikeslike/ViPERFX_RE" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 79 | **NLSound** | Module | System-level Android audio enhancement module for Magisk, KernelSU, and APatch. | <a href="https://github.com/Briclyaz/NLSound" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 80 | **Audio Misc Settings** | Module | Adjusts audio configuration values such as volume steps, resampling, and effects behavior. | <a href="https://github.com/Magisk-Modules-Alt-Repo/audio-misc-settings" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 81 | **Audio Jitter Silencer** | Module | Attempts to reduce selected digital-audio jitter and related processing behavior. | <a href="https://github.com/Magisk-Modules-Alt-Repo/audio-jitter-silencer" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 82 | **USB Sample Rate Unlocker** | Module | Removes selected USB audio sample-rate limits on compatible Android audio stacks. | <a href="https://github.com/Magisk-Modules-Alt-Repo/usb-samplerate-unlocker" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 83 | **DRC Remover** | Module | Targets dynamic-range compression behavior on selected devices and audio paths. | <a href="https://github.com/Magisk-Modules-Alt-Repo/drc-remover" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 84 | **HiFi Maximizer Mod** | Module | Audio-fidelity tuning module aimed at USB DAC, Bluetooth, DLNA, and other digital outputs. | <a href="https://github.com/yzyhk904/hifi-maximizer-mod" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 85 | **V4A QSSI Patch** | Module | Patches Qualcomm QSSI audio-effect configuration so ViPER4Android can detect its driver. | <a href="https://github.com/TKtheDEV/V4A-ODM-ETC-AUDIO-Patch" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |

> Audio modules are mutually sensitive. Test one audio stack at a time and keep the original vendor audio configuration.

### 8. Performance and gaming

| # | Project | Type | Description | Direct GitHub link |
|---:|---|---|---|---|
| 86 | **Encore Tweaks** | Module | Device performance and gaming-session tuning with an emphasis on returning to normal behavior afterward. | <a href="https://github.com/Rem01Gaming/encore" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 87 | **AsoulOpt** | Module | Game-thread tuning module intended for selected Android games and device profiles. | <a href="https://github.com/nakixii/Magisk_AsoulOpt" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 88 | **Uperf-Game-Turbo** | Module | Userspace performance controller for gaming and foreground-app scenarios. | <a href="https://github.com/yinwanxi/Uperf-Game-Turbo" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 89 | **iUnlocker GLTool** | Module | Spoofs GPU information for graphics testing and selected game-compatibility experiments. | <a href="https://github.com/i-Taylo/iUnlockerGL" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 90 | **FPS Limitation Patcher** | Module | Removes selected FPS limitations in HyperOS system apps and games. | <a href="https://github.com/Mods-Center/FPS-Limitation-Patcher" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 91 | **MAGNETAR** | Module | Device performance optimizer with scenario-based tuning goals. | <a href="https://github.com/Kyliekyler/MAGNETAR" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 92 | **PerfMTK** | Module | MediaTek-focused performance module for devices with Mali graphics. | <a href="https://github.com/JUANIMAN/PerfMTK" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 93 | **Wi-Fi Bonding** | Module | Qualcomm-oriented Wi-Fi channel and bandwidth experiment module. | <a href="https://github.com/Magisk-Modules-Repo/wifi-bonding" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 94 | **Magisk Autoboot** | Module | Enables automatic boot or power-on behavior when the device is connected to power. | <a href="https://github.com/anasfanani/magisk-autoboot" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |

### 9. Classic and legacy projects

These projects remain useful references or may still work on specific devices, but their repository status or compatibility should be checked before installation.

| # | Project | Type | Description | Direct GitHub link |
|---:|---|---|---|---|
| 95 | **MagiskHide Props Config** | Legacy module | Older system-property and device-fingerprint configuration tool; not a universal Play Integrity solution. | <a href="https://github.com/Magisk-Modules-Repo/MagiskHidePropsConf" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 96 | **EdXposed** | Legacy framework | Earlier Xposed implementation for Android root environments; newer setups usually investigate LSPosed instead. | <a href="https://github.com/ElderDrivers/EdXposed" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 97 | **Pixelify** | Legacy module | Older Pixel-feature and UI-enablement module for selected Android ROMs. | <a href="https://github.com/Kingsman44/Pixelify" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 98 | **Detach** | Legacy module | Older Play Store detach tool for keeping selected apps from automatic updates. | <a href="https://github.com/Magisk-Modules-Repo/Detach" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 99 | **Open WebView** | Legacy module | Replaces the system WebView implementation on compatible Android builds. | <a href="https://github.com/Magisk-Modules-Alt-Repo/open_webview" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |
| 100 | **ViperFX RE Releases** | Legacy archive | Archived release repository for a redesigned ViPER4Android application and driver workflow. | <a href="https://github.com/WSTxda/ViperFX-RE-Releases" target="_blank" rel="noopener noreferrer">GitHub ↗</a> |

## Simple installation flow

1. Check the project’s README and Releases page.
2. Confirm your Android version, architecture, ROM, root manager, and required framework.
3. Download the ZIP or APK from the direct GitHub source above.
4. Back up your data and keep a stock boot or init_boot image.
5. Install one module from Magisk or the project’s documented manager.
6. Reboot, test, and record what changed before adding another module.
7. If the device bootloops, use the project’s recovery steps or Magisk’s module-removal workflow; do not delete random directories from `/data/adb/`.

## About ZidhuXD

**ZidhuXD** is the identity and SEO label for this Android root and Magisk module showcase. This collection is intended to help rooted Android users discover project sources quickly, compare module categories, and avoid downloading unofficial repacks.

Search topics covered by this README include **Magisk modules**, **best Magisk modules for rooted Android**, **useful root modules**, **Zygisk**, **LSPosed**, **KernelSU**, **APatch**, **systemless Android customization**, **Android debloating**, **root privacy tools**, **Android audio mods**, and **Magisk troubleshooting**.

## Source directories

- <a href="https://github.com/topjohnwu/Magisk" target="_blank" rel="noopener noreferrer">Magisk</a> — upstream root framework and documentation.
- <a href="https://github.com/awesome-android-root/awesome-android-root" target="_blank" rel="noopener noreferrer">Awesome Android Root</a> — community-curated root apps, modules, and guides used for discovery.
- [Supplied Android / KernelSU / LSPosed module list](https://gist.githubusercontent.com/supermarsx/26a1ace8dd4fa9bb88c482e28d51de35/raw/4c492b6815627e6215c08abfab8078fda6beeece/curated-list-android-ksu-lsposed-module.md) — source list supplied for comparison.

---

**Collected by Sidharth S ( ZidhuXD ) • Discover the module. Read the source. Keep a recovery path.**
