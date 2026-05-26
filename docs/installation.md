# Installation Guide

> **DRAFT — Full guide coming soon.**

See [Getting Started](getting-started.md) for the quick installation procedure.

## Advanced Configuration

### Static IP

During the first-boot wizard, select **"2 — Static IP"** and enter:
- IP address and prefix (e.g. `192.168.1.100/24`)
- Default gateway
- DNS servers (comma-separated)

### Manual install on existing Ubuntu

```bash
git clone https://github.com/crazynet2/portguard-install.git
cd portguard-install
sudo bash install.sh
```

### Updates

```bash
portguard-update          # Update system + application
portguard-update os       # Ubuntu security updates only
portguard-update app      # PortGuard application only
```

### Diagnostics

```bash
portguard-status          # Quick service overview
portguard-health-check    # Full diagnostic report
portguard-support-bundle  # Generate support bundle
```

## Support

- Email: [info@crazynet.io](mailto:info@crazynet.io)
- Website: [portguard.crazynet.io/contact](https://portguard.crazynet.io/contact)
