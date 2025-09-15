# 🔐 Kali Linux Encrypted USB with Shared Partition

This project documents how I created a **128GB bootable Kali Linux USB drive** with:

- **Encrypted Persistence** (to securely store changes and files).
- **Shared FAT32 Partition** (to exchange files between Linux and Windows).
- Step-by-step reproducible guide for anyone to try.

---

## 🚀 Steps

1. [Disable BitLocker on Windows](1-disable-bitlocker.md)  
2. [Create a Bootable Kali USB](2-create-usb.md)  
3. [Enable Encrypted Persistence](3-enable-persistence.md)  
4. [Add a Shared Partition](4-shared-partition.md)  
5. [Testing & Final Notes](5-testing.md)  

---

## 🛠️ Tools Used
- **Rufus** (for creating bootable USB)
- **Kali Linux ISO**
- **GParted** (for partitioning)
- **PowerShell** (for managing BitLocker)

---

## 📌 Notes
- Tested on a 128GB SanDisk USB 3.0 drive.
- Works on both UEFI and Legacy BIOS.
- Persistence is fully encrypted using LUKS.

---
