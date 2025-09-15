# Step 4: Add a Shared Partition

In addition to the encrypted persistence, you can create a **shared partition** on the USB.  
This partition allows you to easily transfer files between **Linux** and **Windows** systems.

---

## 1. Create Shared Partition

We already created `/dev/sda3` during the partitioning step (see Step 3).  
If not, repeat the process:

```bash
sudo fdisk /dev/sda
