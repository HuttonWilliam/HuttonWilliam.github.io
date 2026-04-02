# HuttonWilliam.github.io
# Lubuntu System Tools 🛠️

A professional-grade maintenance suite designed to optimize **Lubuntu 24.04** for high-performance on older hardware. This project was refined based on community feedback to ensure safe, efficient, and "fail-fast" execution.

## 📂 Project Structure
*   **backups/**: Destination folder for system snapshots.
*   **scripts/**: Automated tools for system monitoring, security, and maintenance.

---

## 📜 Available Scripts

### 🔄 System Update (`update-system.sh`)
**Feature:** Performs a full system refresh, including kernel updates and security patches.
*   Uses `full-upgrade` to ensure no packages are held back.
*   Automatically runs `autoremove` to reclaim disk space.
*   **How to use:** `bash scripts/update-system.sh`

### 💾 Backup Manager (`backup-manager.sh`)
**Feature:** High-speed `rsync` mirroring of your entire Home directory.
*   Safely mirrors your Documents, Photos, and Configs to `~/Backups`.
*   Highly efficient: only copies files that have changed.
*   **How to use:** `bash scripts/backup-manager.sh`

### 📊 System Information & Topology (`sys-info.sh`)
**Feature:** A real-time "Cockpit" view of your machine.
*   Displays **Disk Topology** (all connected drives/USB) using `lsblk`.
*   Shows live RAM usage and CPU stats.
*   **How to use:** `bash scripts/sys-info.sh`

### 🧹 Disk Cleanup Utility (`disk-cleanup.sh`)
**Feature:** Aggressive space reclamation for small SSDs/HDDs.
*   Clears APT cache, system logs (>30 days), and thumbnail cache.
*   Includes a `--dry-run` mode to see savings before deleting.
*   **How to use:** `bash scripts/disk-cleanup.sh`

---

## 🚀 Quick Start

1. **Clone the repo:**
   ```bash
   git clone [https://github.com/HuttonWilliam/lubuntu-system-tools.git](https://github.com/HuttonWilliam/lubuntu-system-tools.git)
   cd lubuntu-system-tools
