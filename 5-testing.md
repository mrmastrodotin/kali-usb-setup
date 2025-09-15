# Step 4: Testing, Verification & Usage

Now that the partitions and encrypted persistence are set up, it’s time to **verify everything works** and give some usage tips.

---

## 1. Boot with Encrypted Persistence

1. Insert the USB and boot using your BIOS/Boot Menu key.
2. Select: **Live system (encrypted persistence)**.
3. Enter the **LUKS passphrase** when prompted.
4. Once logged in, confirm that the persistence partition is mounted:

```bash
lsblk -o NAME,SIZE,FSTYPE,LABEL,MOUNTPOINT
