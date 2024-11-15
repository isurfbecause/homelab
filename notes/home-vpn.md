# Homelab / Home VPN

## Purpose

- The primary use is for access outside the home network.
- Ensure traffic from public/free Wi-Fi appears to originate from my home ISP.
- Some services only work within the US.
- Avoid IP blacklisting often associated with VPNs hosted on cloud providers.

## ALB

- Purpose: Distribute requests across WireGuard servers.
- Technology: nginx
- Role: Redundancy and failover to WireGuard servers.

### Resources

- VMs: 1
- vCPUs: 1
- RAM: 1 GB
- Storage: 10 GB

---

## WireGuard Servers

- Purpose: Provide fast VPN performance.
- Technology: WireGuard
- Role: VPN servers for secure remote access.

### Resources (Per VM)

- VMs: 2
- vCPUs: 1
- RAM: 1 GB
- Storage: 10 GB
