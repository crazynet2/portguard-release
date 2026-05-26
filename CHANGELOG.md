# Changelog

All notable changes to PortGuard are documented here.

## [v0.1.0-trial] — 2026-05-26

### Initial public release

- Ubuntu 26.04 LTS base, automated installer (autoinstall/subiquity)
- Appliance partition layout: EFI / boot / root / data / backup / logs / swap
- 802.1X RADIUS authentication (FreeRADIUS, PEAP-MSCHAPv2, EAP-TLS)
- Web dashboard (React + FastAPI)
- Captive portal with voucher management
- Dynamic VLAN assignment
- Multi-tenant MSP support
- Compliance exports (NIS2, PCI DSS)
- First-boot setup wizard (console)
- PortGuard CLI restricted shell for SSH admin access
- Plymouth boot splash
- Diagnostic and maintenance scripts (`portguard-status`, `portguard-health-check`, etc.)
