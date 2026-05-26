# Getting Started with PortGuard

## Prerequisites

- x86_64 bare metal or VM with **30 GB disk minimum**
- 2 GB RAM minimum (4 GB recommended)
- 1 network interface
- UEFI or BIOS boot

## Installation

1. **[Sign up](https://portguard.crazynet.io/signup)** to get download access and your trial license key.
2. Download the ISO from your account dashboard.
3. Boot the ISO on your target machine.
4. Select **"PortGuard Appliance Install (automatic)"** — the installer partitions the disk and installs everything automatically.
5. Reboot. The **first-boot wizard** launches on the console:
   - Set hostname, network (DHCP or static), timezone, organization name, admin password.
6. Access the dashboard at `https://<appliance-ip>` with user `admin`.

## SSH Access

```bash
ssh pgadmin@<appliance-ip>
# Initial password: admin (you will be prompted to change it)
```

The `pgadmin` shell is a restricted console (`portguard-cli`) with commands for network testing, service management and diagnostics.

## Partition Layout

| Partition | Size | Mount | Purpose |
|-----------|------|-------|---------|
| sda1 | 512 MB | /boot/efi | EFI |
| sda2 | 512 MB | /boot | Kernel |
| sda3 | 8 GB | / | OS + PortGuard core |
| sda4 | 11 GB | /data | Runtime data, DB, config |
| sda5 | 5 GB | /backup | Dedicated backups |
| sda6 | 3 GB | /var/log | Logs |
| sda7 | ~2 GB | swap | Virtual memory |

## Next Steps

- See [Installation Guide](installation.md) for advanced configuration.
- Visit [portguard.crazynet.io/docs](https://portguard.crazynet.io/docs) for full documentation.
