# Network Automation (IT-AUTOMATION)

An enterprise-grade repository for multi-vendor network automation workflows, Ansible playbooks, and modern Python NetDevOps toolchains targeting Cisco, Arista, and Linux network topologies.

---

## Repository Structure

```
Automation/
├── ANSIBLE/                        # Ansible playbooks, inventory, and roles
│   └── .gitkeep
└── PYTHON/                         # Python network automation toolchains
    ├── 0-Python-Basics/            # Foundational Python scripts for network engineers
    ├── 1-Telnet/                   # Legacy switch & router Telnet automation & config backup
    └── 2-SSH/                      # Production SSH automation frameworks
        ├── a-Paramiko/             # Low-level SSH socket automation
        ├── b-Netmiko/              # Multi-vendor CLI automation (Cisco IOS-XE, Nexus, Arista)
        │   ├── 0-Basics-Single-Device.py
        │   ├── 1-Erorr-Handling.py
        │   ├── 2-SingleL2Switch.py
        │   ├── 3-Multiple-SW-Same-config.py
        │   ├── 4-Multiple-SW-Differnet-config.py
        │   ├── 5-Device-Backup.py
        │   ├── 6a-Replace-password-with-vairable.py
        │   └── 6b-encrypt-devices.py
        └── c-Napalm/               # Cross-vendor declarative network manipulation
            ├── 1-Basics/           # State validation and structured JSON data extraction
            ├── 2-BGP/              # Dynamic BGP neighbor inspection & large-scale deployment
            └── c-Audit/            # Network compliance, ACL validation, and diff-based merging
```

---

## Toolchains & Frameworks

### 1. Python Automation Modules
* **Netmiko**: Handles multi-vendor SSH connections with robust error handling, device credential abstraction, and concurrent multi-device provisioning.
* **Paramiko**: Direct SSHv2 client library handling low-level terminal channel interactions.
* **NAPALM**: Vendor-neutral network automation library used for configuration auditing, ACL deployments, and declarative state verification.

### 2. Ansible Playbooks
* Automated orchestration of network state, configuration compliance checks, and scheduled backups across enterprise switches and routers.

---

## Related Repositories

* **[AzamLabs](https://github.com/azambasha1987/AzamLabs)**: Self-hosted virtual network emulation platform engine, hypervisor orchestration, and satellite clusters.
* **[GNS3](https://github.com/azambasha1987/GNS3)**: AzamGNS3 3.1 enterprise edition, unified server daemon, and web management interface.

---

## License

Internal Enterprise Repository — All rights reserved.
