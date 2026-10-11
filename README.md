# MEPHI Session Project 2026

**Student:** 375027  
**Operating System:** RED OS 8 ARM64  
**Virtual Machine:** UTM  
**Hostname:** mephi-2026.domain.local

## 1. Network
DHCP configured. Connectivity to 8.8.8.8 verified.

## 2. Software
System packages updated. nginx, libcap-ng-utils and tcpdump installed.

## 3. Filesystem
Additional ext4 filesystem with label MEPHI_WEB mounted at /mephi-web using /etc/fstab.

## 4. Web Server
nginx enabled and running. Website root: /mephi-web.

## 5. Security
- DAC and default ACL configured for developers and curators.
- tcpdump uses cap_net_raw=ep.
- SELinux operates in Enforcing mode.

## 6. Authentication
- Local console login restricted for curators.
- Maximum password age: 90 days.
- Minimum password length: 12 characters.

## 7. Web Server Result

Hello from Student: 375027

## 8. Evidence
Configuration files, command history, system reports and screenshots are included in this repository.

**Security note:** The published shadow file is redacted to protect password hashes.

**Installation note:** The system was configured for console boot using multi-user.target; graphical packages installed previously were not removed.
