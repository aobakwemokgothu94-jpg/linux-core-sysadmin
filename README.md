# linux-core-sysadmin
Hands-on Linux core system administration and security engineering portfolio. Covers automated Bash scripting, user/group privilege management, SSH hardening, and deep-dive system log auditing.

# 🐧 Linux Core System Administration & Security Engineering

A production-focused engineering repository documenting core Linux system operations, user authorization modeling, scripting automation, and telemetry log auditing.

---

## 🛠️ Module 1: Automated System Scripting & Task Scheduling
* **Objective:** Automate routine infrastructure maintenance, backup tasks, and user alerting scripts using native shells.
* **Core Skills Implemented:** 
  * Written modular Bash scripts using robust error handling (`set -e`) and conditional logic pipelines.
  * Configured system-wide scheduling profiles using `cron` jobs (`crontab -e`) to execute background telemetry sweeps.
  * Managed environment variables and shell configurations inside profiles like `.bashrc` and `.profile`.

---

## 🔐 Module 2: Access Control, Permissions & Hardening
* **Objective:** Enforce standard security baselines and secure local environment access vectors.
* **Core Skills Implemented:**
  * Configured user creation accounts and administrative privilege sets via the `/etc/sudoers` file and `visudo`.
  * Managed strict directory security matrices utilizing absolute and relative permissions (`chmod`, `chown`, `chgrp`).
  * Hardened remote connections via SSH configurations (`/etc/ssh/sshd_config`) by disabling root password access and enforcing key-based authentication.

---

## 📊 Module 3: System Telemetry & Log Investigation
* **Objective:** Audit system events, troubleshoot process terminations, and parse active connection footprints.
* **Core Skills Implemented:**
  * Investigated system authorization sequences and failed access logs within `/var/log/auth.log` or `/var/log/secure`.
  * Tracked live system performance metrics, memory allocations, and process trees using `top`, `htop`, and `ps aux`.
  * Filtered massive plain-text unstructured data streams efficiently using `grep`, `awk`, and `sed` regex operations.

---

## 🛡️ Recommended Production System Baselines
1. **Enforce Least Privilege:** Restrict root execution vectors by forcing standard operations to happen through individual user accounts using granular `sudo` configurations.
2. **Implement Regular Auditing:** Schedule routine automation checks via system log monitors to capture anomalous access failures before they scale.
3. **Keep Packages Managed:** Ensure continuous system vulnerability patching by setting up automated package management updates (`apt-get upgrade` or `yum update`).
