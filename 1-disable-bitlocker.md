# Step 1: Disable BitLocker on Windows

Before creating the Kali Linux bootable USB, I had to **disable BitLocker** on my Windows system.  
This ensures Windows does not block or encrypt the USB drive during formatting and partitioning.

---

## Disable BitLocker for All Drives

Run PowerShell as **Administrator** and enter:

```powershell
# Get all BitLocker volumes
$BLV = Get-BitLockerVolume

# Disable BitLocker for all detected volumes
Disable-BitLocker -MountPoint $BLV
