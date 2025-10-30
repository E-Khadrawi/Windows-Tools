# 🖥️ Windows Maintenance Tool

![Version](https://img.shields.io/badge/version-v5.0.0-green)  
![Platform](https://img.shields.io/badge/platform-Windows-blue)  
![License: MIT](https://img.shields.io/badge/license-AL%20Khadrawi-blue)  

A powerful, all-in-one Windows maintenance toolkit built entirely in Batch & PowerShell.  
Designed for power users, sysadmins, and curious tinkerers – now smarter, safer, and fully offline-compatible.  

---

## 📸 Screenshot  
<img width="958" height="878" alt="2025-10-19 01_47_11-NVIDIA GeForce Overlay" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjCkzbOSOeO-n1J4vzZ-rdHELA73jCfU03g5AWTjAiKT_TmhQhyphenhyphenx_Ui8trbZPfX_83iXfwNGOQX1p8MrdsqJ_0MKPQf7y38NCuLeENSlSxmRRBU-CQ3OSOoHq8H1JxQHpx5S1AFkUqzn4BESfrAdE3zoSrQe4GfhuGjXnAwpRvmwuyRfBYEM7spf_Qi8qZv/s1180/Windows-Maintenance-Tool.png" />


---

## ✅ Features  

**Run essential repair tools:**  
- Quick access to SFC, DISM, and CHKDSK for core Windows repairs  

**Optimize SSD drives:**  
- TRIM and compatible defrag for faster, healthier drives  

**Windows Update management:**  
- Use winget to install, upgrade, and repair system packages  
- Automatically installs winget if missing  
- Flexible package handling: View, search, and upgrade individual apps/packages by entering their ID directly  
- **Improved in v5.0.0:** Windows Update Repair Tool now supports **full nuke & rebuild** with more repair options  

**Network diagnostics & repair:**  
- Includes ipconfig, routing table viewer, DNS config, adapter reset, and more  

**Privacy & temp cleanup:**  
- Clean temp files, logs, and browser cache  
- Privacy cleanup for extra traces (history, cookies, etc.)  

**Save detailed reports:**  
- Export System Info, Network Info, and Driver List to your Desktop or a custom folder  

**Registry tools:**  
- Safe cleanup, backup, and corruption scan  
- Menu-driven, stable registry cleaning:  
  - List “safe to delete” entries (IE40, IE4Data, DirectDrawEx, etc.)  
  - Bulk delete all safe entries  
  - Easy backup & restore with versioned .reg files  

**DNS-Adblock management:**  
- Block ad/tracker domains with hosts file (adblock/mirrors included)  
- Improved handling of locked files, better messaging, multiple backup/restore  

**Firewall Manager:**  T runtimes  

**Shortcut Fixer (New in v5.0.0):**  
- Automatic shortcut repair  
- Menu reorganized (options 30 and 0 moved to the end for better structure)  

**Menu-driven and user-friendly:**  
- More return-to-menu options added (v5.0.0)  
- All functions accessible from a clear main menu—no PowerShell experience needed  
- Support/help, Discord/GitHub contact, openable with a single key press  
 
**Windows Activation:**
- Thanks to the [MAS (Microsoft Activation S
- Built-in menu-driven PowerShell Firewall Manager  
- Manage firewall rules, enable/disable Windows Firewall directly from the tool  

**.NET RollForward Settings (New in v5.0.0):**  
- Lets the system use a specific .NET version (SDK/runtime)  
- Reduces the need to install multiple .NEcript)](https://massgrave.dev) project, Windows and Office activation support is now integrated into this tool.  
- Full credit goes to the Massgrave team for maintaining and developing MAS. This project does not modify or redistribute MAS — it only provides a convenient way to access it.  
- A clear warning and confirmation step has been added to ensure that users review the documentation and accept responsibility before running the script.

**Portable & safe:**  
- Runs from USB, no install or admin deployment required  
- No third-party dependencies or internet downloads required (except optional winget)  

---

## ⚙️ Installation  

1. Start `Start_Windows_Maintenance_Tool.bat`.  
2. Follow the interactive menu.  
3. Ensure that both `Start_Windows_Maintenance_Tool.bat` and `Windows_Maintenance_Tool.ps1` are in the same folder.  

> ⚠️ Script output may appear in your system language (e.g. English, Danish, etc). This is normal.  

---

## 📁 Output Files  

Saved directly to your chosen folder (default: Desktop\SystemReports):  

- `System_Info_YYYY-MM-DD.txt` – full system information  
- `Network_Info_YYYY-MM-DD.txt` – detailed network configuration  
- `Driver_List_YYYY-MM-DD.txt` – list of all installed drivers  
- `routing_table_YYYY-MM-DD.txt` – network routing table  
- `RegistryBackup_YYYY-MM-DD_HH-MM.reg` – registry backup files with date/time  

---

## 🧪 Troubleshooting & FAQ  

**Q: The script didn’t run with administrator rights?**  
A: For the tool to work properly, administrator rights are required.  
Right-click the `.bat` file and choose "Run as administrator".  

If nothing happens, check that UAC is enabled and try again.  

Run manually with PowerShell if needed:  
```powershell
Start-Process powershell -Verb RunAs -ArgumentList "-NoProfile -ExecutionPolicy Bypass -File 'Path\To\Windows_Maintenance_Tool.ps1'"
```  

**Q: Why does it crash when selecting registry cleanup?**  
A: This was fixed in v5.0.0. The tool now safely lists and deletes registry keys with auto-backup.  

**Q: Why was Registry Defrag removed?**  
A: It depended on NTREGOPT, which is no longer accessible. The script is now fully offline and native to Windows.  

---

## 📜 Credits  

This release (**5.0.0**) was fully contributed by **[@Chaython]([https://github.com/E-Khadrawi/Windows-Tools/releases])**.  
All new features, fixes, and improvements are thanks to his work.  

---

## 📜 License  

MIT License

Copyright (c) 2025 AL Khadrawi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

