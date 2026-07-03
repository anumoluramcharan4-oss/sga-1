# Q5 Explanation

- `lsblk` identified the available block devices and showed which ones were mounted in the container environment.
- `mount | head -5` confirmed the active filesystem types and mount points without dumping the full table.
- `df -h` measured capacity usage in human-readable units, which is the easiest way to judge free storage space.
- `df -i` checked inode usage, which matters because a filesystem can run out of inodes even when disk space is still available.
- The results show that the environment is generally healthy, but `/vscode` deserves monitoring because it has noticeably higher usage than the other mounts.
