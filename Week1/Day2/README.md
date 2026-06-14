# Day 2 – Operating Systems & Linux Fundamentals

## Block 1 Theory: How Operating Systems Work
An operating system is the master manager of a computer. Its five key jobs are:

1. **Process Management** – Starts, pauses, and ends programs; multitasks so many apps can run at once.
2. **Memory Management** – Allocates RAM to processes and frees it when done; prevents one program from reading another's memory.
3. **File System Management** – Organises, reads, writes, and protects files on storage devices.
4. **Device Management** – Controls hardware like keyboards, disks, and network cards through drivers.
5. **Security & Access Control** – Authenticates users, enforces permissions, and isolates processes.

## Block 2 Theory: Linux Filesystem & Permissions

### Important Directories
- `/etc` – System-wide configuration files (think "editable text config").
- `/var/log` – Log files that record what the system and applications are doing.
- `/home` – Personal home directories for each user.
- `/tmp` – Temporary files; world-writable, often cleaned on reboot. A common security risk if misconfigured.

### Permissions
Linux files have three permission groups: **owner**, **group**, and **others**. Each group can have read (`r`), write (`w`), and execute (`x`) permissions.

- `chmod 600 file` sets permissions so that **only the owner** can read and write the file. Group and others get zero access.
- `chmod 644 file` gives the owner read/write, while group and others can only read.

View permissions with `ls -l`. The output string like `-rw-r--r--` maps to owner/group/others.
