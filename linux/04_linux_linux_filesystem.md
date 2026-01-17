[200~# Filesystem Types

Linux supports many **filesystem types**, each optimized for different needs—speed, large storage, or smaller devices. Every filesystem organizes data in its own way.

## Virtual File System (VFS)
The **VFS** is an abstraction layer in the Linux kernel that provides a **uniform interface** for applications, allowing them to access any filesystem seamlessly. This enables multiple filesystem types on the same system, often across different partitions.

## Journaling for Data Integrity
Most modern filesystems use **journaling** to prevent data corruption. Before writing data, changes are recorded in a **journal**. If a crash occurs, the system can use the journal to restore consistency quickly, avoiding long filesystem checks.

## Common Linux Filesystem Types
- **ext4** – Default for many Linux distros; reliable, supports large volumes and files.
- **Btrfs** – Modern FS with snapshots, incremental backups, and performance improvements.
- **XFS** – High-performance, ideal for large files and parallel I/O operations.
- **NTFS / FAT** – Windows filesystems; Linux can read/write them, useful for dual-boot.
- **HFS+** – macOS filesystem; mostly read-only in Linux, write possible with extra tools.

## Checking Filesystem Types
Use the `df -T` command to see disk usage and filesystem types:

```bash
pete@icebox:~$ df -T
Filesystem     Type     1K-blocks    Used Available Use% Mounted on
/dev/sda1      ext4       6461592 2402708   3707604  40% /
udev           devtmpfs    501356       4    501352   1% /dev
tmpfs          tmpfs       102544    1068    101476   2% /run
/dev/sda6      xfs       13752320  460112  13292208   4% /home

- The `-T` flag shows the filesystem type.


This version keeps the **essential points**: VFS, journaling, common FS types, and a practical command example.  

If you want, I can also make your **Filesystem notes visually structured like a table**, which makes it even quicker to study. Do you want me to do that?

