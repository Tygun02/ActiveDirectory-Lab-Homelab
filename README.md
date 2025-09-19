# Active Directory Homelab (Windows Server)

**Hands‑on build of an on‑prem AD DS environment**: domain controller, DNS/DHCP, OUs, users/groups, baseline Group Policy, and a joined Windows client — fully documented with screenshots.

> **Elevator pitch:** I built a complete AD DS lab from scratch to practice real admin workflows and troubleshooting. This repo explains the design, steps, and rationale so hiring managers can quickly assess my skills.

---

## Highlights

- ✅ Provisioned Windows Server VM and promoted a **Domain Controller (AD DS)**
- ✅ Configured **DNS** and **DHCP** with proper scopes and reservations
- ✅ Designed **OU hierarchy**, created **users/groups**, and applied **GPO baselines**
- ✅ **Joined a Windows client** to the domain and validated policies
- ✅ Documented everything with **captions + screenshots** and troubleshooting notes

*(Adjust checkmarks to match what you actually built.)*

---

## Screenshot Gallery (quick peek)

<p>
  <img src="docs/img/01-lab-setup-01.png" alt="VMware settings summary for the DC VM" width="260" />
  <img src="docs/img/02-server-install-02.png" alt="Static IP configuration for the server" width="260" />
  <img src="docs/img/03-active-directory-ds-03.png" alt="AD DS installation progress" width="260" />
</p>

See full pages in **/docs**:
- [Lab Setup](docs/01-lab-setup.md) · [Server Install](docs/02-server-install.md) · [AD DS](docs/03-active-directory-ds.md)
- [DNS/DHCP](docs/04-dns-dhcp.md) · [Users/Groups/OUs](docs/05-users-groups-ou.md)
- [GPO Baseline](docs/06-group-policy-baseline.md) · [Join Client](docs/07-join-client.md)
- [Monitoring & Logs](docs/08-monitoring-and-logs.md)

---

## Lab Design

- **Hypervisor / VM host:** _e.g., Hyper‑V on Windows 11 / VMware Workstation / VirtualBox_
- **Server:** Windows Server _version/build_
- **Client:** Windows _version/build_
- **Domain name:** `example.local` *(redact in screenshots)*
- **IP plan:** `192.168.10.0/24` — DC: `192.168.10.10`, Client: `192.168.10.50` *(or DHCP)*
- **Services:** AD DS, DNS, DHCP, Group Policy
- **Admin tools:** Server Manager, ADUC, GPMC, PowerShell

*(Replace with your actual values.)*

---

## How I Built It (quick version)

1. Created isolated **virtual switch/network** and provisioned **Server** + **Client** VMs
2. Gave Server a **static IP**, set **DNS = self** (temporary), named the machine
3. Installed **AD DS**; ran **promotion wizard** (Server Manager → Add Roles → Promote)
4. Established new **forest/domain**; rebooted as **Domain Controller**
5. Configured **DNS zones**; installed and configured **DHCP** scope + options
6. Designed **OUs**; created **users** and **security groups**
7. Created baseline **GPOs** (password policy, firewall, RDP, NTP, audit, etc.)
8. Joined the **client** to the domain; verified **policy application** and **login**
9. Documented **troubleshooting** and **validation** steps

---

## Reproduce / Try It Yourself

- Pre-reqs: A machine capable of running 2 VMs (8–16 GB RAM recommended), Windows Server ISO
- Follow the detailed step-by-step pages under **/docs** (with screenshots)

---

## Skills Demonstrated

**Active Directory, Windows Server, DNS, DHCP, Group Policy, OU design, PowerShell, Networking (IP/DNS), Troubleshooting, Documentation.**

---

## Sanitization & Safety

Before publishing:
- Blur/redact **domain names, usernames, IPs, hostnames**, and any **keys/secrets**
- Avoid posting **production** screenshots or any PII
- Review `.gitignore` and ensure no credentials/binaries are committed

---

## About Me / Contact

- **Name:** _Your Name_
- **LinkedIn:** _URL_
- **Email:** _Email_

---

## License

Choose a license (e.g., **MIT**). Use GitHub → *Add file* → *Add license*.
