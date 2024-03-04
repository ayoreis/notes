# Disks

- Bad blocks

---

I had three HDDs formated HFS+ to fix (recover/restore), this is what I learned while doing it:

im on arch btw but most of theese tips should waork on any \*nix as long as you can compile the tools and some on anything else.

## Start when it starts

I noticed that the disks where starting to not work about 6 months ago, and I only started to work on them a few weeks back

## Backup, BACKUP!

I've heard this so many times and I've always thought, nah...

But yeah...

Some disks where still mounting when I started but when I reached them thay were not anymore, not sure why but I think the [[#Bad blocks]] spread

- CloneZilla
- DD
- DDresuce
- [Disk cloning - ArchWiki](https://wiki.archlinux.org/title/Disk_cloning)
- only partition table

## S.M.A.R.T.

It is a protocol to check disk health, I used GNOME Disks but there is also smartctl

- SMART

## Ask help from a SATA to USB adaptors but also don't trust them

- [How do you reset a USB device from the command line? - Ask Ubuntu](https://askubuntu.com/questions/645/how-do-you-reset-a-usb-device-from-the-command-line)
- UAS, [Linux keeps connecting and disconnecting USB mounted external drives - Linux Mint Forums](https://forums.linuxmint.com/viewtopic.php?t=320801)

- usb addaptors

## TestDisk

## HFS+ Rescue

## disable journaling

## Dolphin

## hdd witohout partitions if not used with usb

## `fsck`

## `fsck`

| Label           | Size | Space    | Format   | Notes                              | Writable   | Mountable     | TODO                        | Journal |
| --------------- | ---- | -------- | -------- | ---------------------------------- | ---------- | ------------- | --------------------------- | ------- |
| WD              | 2.5  | 40/320GB | GPT/HFS+ |                                    | yes        | yes           |                             | no      |
| Backup (travel) | 2.5  | 0.5/1TB  | MBR/HFS+ | fdisk does not list any partitions | only macOS | yes, manually |                             | ?       |
| Backup (office) | 3.5  | 0.5/1TB  | GPT/HFS+ |                                    | N/A        | no            | Backup disk image, testdisk | ?       |
