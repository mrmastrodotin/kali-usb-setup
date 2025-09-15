# Step 3: Create Encrypted Persistence Partition

Now that Kali is booting from USB, we will partition the USB to add **encrypted persistence** and a **shared storage partition**.

---

## 🧩 Partition Setup (using `fdisk`)

### 1. List all disks
```bash
sudo fdisk -l
