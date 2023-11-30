# Partitioning

- [Partitioning - ArchWiki](https://wiki.archlinux.org/title/partitioning)

```bash
# fdisk -l
```

## Partition table schemes

- Master Boot Record (MBR, sometimes called DOS)

## GUID Partition Table (GPT)

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

- Get cluster size: `# dump.exfat /dev/sdb1` (output in [bytes](https://en.wikipedia.org/wiki/Byte#Multiple-byte_units)) ([dump.exfat(8)](https://man.archlinux.org/man/dump.exfat.8))
- Set cluster size: `# mkfs.exfat -c 128K /dev/sdb1` ([mkfs.exfat(8)](https://man.archlinux.org/man/mkfs.exfat.8))
