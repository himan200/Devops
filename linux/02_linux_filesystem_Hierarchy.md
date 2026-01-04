# Linux File Structure

To see the top-level directories, run the command:

`ls -l /`

While your system might have minor differences, the core Linux file hierarchy structure is very similar to the one described below.

---

## The Root Directory

- `/` – This is the root directory, the starting point for the entire filesystem. Every single file and directory on your system is located under this directory.

---

## Essential System Directories

The file hierarchy in Linux includes several directories critical for the system's operation.

- `/bin` – Contains essential command-line programs (binaries) available to all users, such as `ls`, `cp`, and `mv`.
- `/sbin` – Holds essential system binaries, primarily intended for system administration and typically run by the root user.
- `/etc` – The core system configuration directory. It contains configuration files but no executable binaries.
- `/lib` – Contains essential shared library files required by binaries in `/bin` and `/sbin`.
- `/boot` – Stores files required for the system boot process, including the Linux kernel and boot loader files.

---

## User and Application Data

- `/home` – Contains personal directories for each user, including documents and application settings.
- `/root` – The home directory for the root user, kept separate so root can log in even if `/home` is unavailable.
- `/opt` – Reserved for optional or third-party application software packages.
- `/usr` – Contains user-installed software and utilities. Common subdirectories include:
  - `/usr/bin` – Non-essential user binaries
  - `/usr/local` – Software compiled from source

---

## Dynamic and Temporary Data

- `/var` – Stores variable data such as logs (`/var/log`), caches, and spool files.
- `/tmp` – A world-writable directory for temporary files, often cleared on reboot.
- `/run` – Stores runtime information such as process IDs (PIDs) since the last boot.

---

## Device and Mount Points

- `/dev` – Contains device files representing hardware components.
- `/media` – Mount point for removable media like USB drives and CDs.
- `/mnt` – Temporary mount point for filesystems.

---

## System Information

- `/proc` – A virtual filesystem providing real-time process and kernel information.
- `/srv` – Contains data served by system services, such as web server files.

