# Partitioning

- [Partitioning - ArchWiki](https://wiki.archlinux.org/title/partitioning)

```bash
# fdisk -l
```

## Types

```bash
# fdisk /dev/sdb

Command (m for help): t
Partition type or alias (type L to list all): 11
Command (m for help): w
```

- [Microsoft basic data partition - Wikipedia](https://en.wikipedia.org/wiki/Microsoft_basic_data_partition)
- [command line - How do you know, using the CLI, the type of partition that corresponds to its id? - Ask Ubuntu](https://askubuntu.com/questions/330780/how-do-you-know-using-the-cli-the-type-of-partition-that-corresponds-to-its-id)
- [Using the GPT Linux Filesystem Data Type Code](https://www.rodsbooks.com/linux-fs-code/)
- [[Solved] linux ext4 partitions show up as "Microsoft basic data" type / Newbie Corner / Arch Linux Forums](https://bbs.archlinux.org/viewtopic.php?id=191163)
- [[SOLVED] Exfat Partitions created in Linux not readable in Windows or Mac OS X](https://www.linuxquestions.org/questions/linux-software-2/exfat-partitions-created-in-linux-not-readable-in-windows-or-mac-os-x-4175575119/)
- [Solutions for an ExFat drive not mounted on Mac : r/editors](https://www.reddit.com/r/editors/comments/oln12b/solutions_for_an_exfat_drive_not_mounted_on_mac/)
- [filesystems - Mac OS cannot mount exFAT disk created on (Ubuntu) linux - Unix & Linux Stack Exchange](https://unix.stackexchange.com/questions/460155/mac-os-cannot-mount-exfat-disk-created-on-ubuntu-linux)
- [Can't mount exFAT external drive in macOS - Ask Different](https://apple.stackexchange.com/questions/293390/cant-mount-exfat-external-drive-in-macos)

## Recovery

- [File recovery - ArchWiki](https://wiki.archlinux.org/title/file_recovery)

## Partition table schemes

- Master Boot Record (MBR, sometimes called DOS)

### GUID Partition Table (GPT)

```bash
# fdisk /dev/sdb

Command (m for help): g
Command (m for help): n
Command (m for help): w
```

## Sizes

[Default cluster size for NTFS, FAT, and exFAT - Microsoft Support](https://support.microsoft.com/en-us/topic/default-cluster-size-for-ntfs-fat-and-exfat-9772e6f1-e31a-00d7-e18f-73169155af95)

- Sector size (physical)
- Cluster size (file-system)

## exFAT

Using [exfatprogs](https://github.com/exfatprogs/exfatprogs) [(Arch)](https://archlinux.org/packages/extra/x86_64/exfatprogs/), similar with [exfat-utils](https://man.archlinux.org/listing/exfat-utils).

- Get cluster size: `# dump.exfat /dev/sdb1` (output in [bytes](https://en.wikipedia.org/wiki/Byte#Multiple-byte_units)) ([dump.exfat(8)](https://man.archlinux.org/man/dump.exfat.8))
- Set cluster size: `# mkfs.exfat -c 128K /dev/sdb1` ([mkfs.exfat(8)](https://man.archlinux.org/man/mkfs.exfat.8))
