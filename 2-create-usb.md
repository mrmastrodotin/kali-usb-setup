# Step 2: Create Bootable Kali USB

Now that BitLocker is disabled, the next step is to create a **bootable Kali Linux USB drive** using **Rufus**.

---

## 🛠️ Requirements

- A **128GB USB drive** (I used [SanDisk 128GB USB 3.0](https://amzn.in/d/9W1WVJv)).
- [Rufus](https://github.com/pbatard/rufus/releases/download/v4.9/rufus-4.9.exe) (Windows tool for creating bootable USBs).
- [Kali Linux Live ISO](https://www.kali.org/get-kali/#kali-live).

---

## ⚙️ Steps in Rufus

1. Open **Rufus** (run as Administrator).
2. Select your **USB drive** under *Device*.
3. Under *Boot selection*, choose the **Kali Linux ISO** file.
4. Configure as follows:
   - **Partition scheme**: `MBR`
   - **Target system**: `BIOS or UEFI`
   - **File system**: `FAT32`
   - **Persistence**: At least a few GB (we will later re-partition for more persistence).
5. Click **Start** and wait for the process to finish.

---

## 🖥️ BIOS / Boot Menu Keys

After the USB is ready, reboot your system.  
Depending on your laptop/PC brand, press the right key during startup:

| Brand      | BIOS Key | Boot Menu Key |
|------------|----------|---------------|
| ASUS       | F2       | ESC           |
| Acer       | F2       | F12           |
| Dell       | F2       | F12           |
| HP         | ESC/F10  | F9            |
| Lenovo     | F1/F2    | F12           |
| MSI        | DEL      | F11           |
| Toshiba    | F2       | F12           |

- Enter **BIOS setup** → Disable **Secure Boot**.  
- Restart and press the **Boot Menu Key** continuously → Select your **USB drive**.

---

## 🔑 Booting Options

When Kali boots, you’ll see a menu. Choose:

- `Live system` → Runs without saving changes.
- `Live system (persistence)` → Saves changes (unencrypted).
- `Live system (encrypted persistence)` → Secure option (we’ll configure in next step).

👉 For now, select **Live system** to proceed with partition setup.
