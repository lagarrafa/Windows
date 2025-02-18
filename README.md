# 🖥️ Common Windows Issues & Fixes

## Overview
This document outlines some of the most frequently encountered Windows errors, their causes, and how to resolve them.

---

## 1️⃣ Blue Screen of Death (BSOD)
- **Cause:** Hardware failure, driver issues, or system file corruption.
- **Fix:**
  - Note the error code and search for specific solutions.
  - Update or roll back drivers in Device Manager.
  - Run `sfc /scannow` to repair system files.
  - Check for Windows updates and install the latest patches.

## 2️⃣ Slow Performance
- **Cause:** High resource usage, background applications, or malware.
- **Fix:**
  - Check resource usage in Task Manager (`Ctrl + Shift + Esc`).
  - Disable startup programs in Task Manager > Startup.
  - Run `Windows Defender` or a trusted antivirus scan.
  - Clear temporary files using `Disk Cleanup`.

## 3️⃣ Application Crashes
- **Cause:** Incompatible software, insufficient system resources, or corrupt files.
- **Fix:**
  - Update the application to the latest version.
  - Run the application in compatibility mode.
  - Check Event Viewer (`eventvwr.msc`) for error logs.
  - Reinstall the application.

## 4️⃣ Network Connectivity Issues
- **Cause:** Incorrect network settings, driver issues, or ISP problems.
- **Fix:**
  - Restart router and modem.
  - Run `ipconfig /flushdns` in Command Prompt.
  - Update network adapter drivers in Device Manager.
  - Run the Windows network troubleshooter.

## 5️⃣ Windows Update Failures
- **Cause:** Corrupt update files, insufficient disk space, or system misconfiguration.
- **Fix:**
  - Run `Windows Update Troubleshooter`.
  - Free up disk space if necessary.
  - Reset Windows Update components with `net stop wuauserv && net start wuauserv`.

## 6️⃣ Disk Errors (`CHKDSK` Required)
- **Cause:** Bad sectors, file system corruption, or improper shutdowns.
- **Fix:**
  - Run `chkdsk /f /r` and restart the system.
  - Use `S.M.A.R.T.` diagnostics to check disk health.
  - Backup important files and consider replacing the disk if issues persist.

## 7️⃣ Printer Not Working
- **Cause:** Driver issues, connectivity problems, or spooler service failure.
- **Fix:**
  - Restart the Print Spooler service (`services.msc`).
  - Update or reinstall printer drivers.
  - Check printer connections and ensure it's set as the default printer.

## 8️⃣ File Explorer Not Responding
- **Cause:** Corrupt system files, background processes, or excessive cache buildup.
- **Fix:**
  - Restart `explorer.exe` from Task Manager.
  - Clear File Explorer history in Folder Options.
  - Run `sfc /scannow` to fix system files.

---

This document serves as a quick reference for troubleshooting common Windows issues. Contributions and updates are welcome! 🖥️
