# PortGuard

**Open-source-friendly Network Access Control for SMB and MSP**

PortGuard is a modern, lightweight NAC solution designed for small and medium businesses and Managed Service Providers. It integrates RADIUS authentication, captive portal, VLAN management, and a full web dashboard — all in one appliance.

## Key Features

- 802.1X / RADIUS authentication (EAP-PEAP, EAP-TLS)
- Captive portal with voucher management
- Multi-tenant MSP support
- Dynamic VLAN assignment
- FortiGate and Palo Alto integration
- Compliance exports (NIS2, PCI DSS)
- Self-contained ISO appliance (Ubuntu-based, 30 GB disk)

## Website

→ [portguard.crazynet.io](https://portguard.crazynet.io)

## Download

Releases are published on this repository. Every release includes:
- ISO image (bootable appliance)
- SHA256 checksum
- GPG signature

**[→ Latest Release](https://github.com/crazynet2/portguard-release/releases/latest)**

Download is gated — [sign up](https://portguard.crazynet.io/signup) to get access.

## GPG Signing Key

All releases are signed with the PortGuard release key:

```
Key: releases@portguard.crazynet.io
Fingerprint: see docs/gpg-signing-key.asc
```

Verify a release:
```bash
gpg --import docs/gpg-signing-key.asc
gpg --verify portguard-v0.1.0.iso.asc portguard-v0.1.0.iso
```

## Documentation

- [Getting Started](docs/getting-started.md)
- [Installation Guide](docs/installation.md)
- [Full EULA](https://portguard.crazynet.io/legal/eula)

## License

Proprietary — see [LICENSE.txt](LICENSE.txt)

Commercial license required for production use.  
Trial use permitted only for evaluation purposes, time-limited.

---

*CrazyNet / PortGuard — [crazynet.io](https://crazynet.io)*
