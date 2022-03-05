# Red Team: Summary of Operations

## Table of Contents
- Exposed Services
- Critical Vulnerabilities
- Exploitation

### Exposed Services

Nmap scan results for each machine reveal the below services and OS details:

```bash
$ nmap ... -sV -oN namp_scan.txt 192.168.1.0/24
```
[NMAP Scan Output](/Doc/nmap_scan.txt)

This scan identifies the services below as potential points of entry:
- Target 1
  - Service Info: Host: TARGET1; OS: Linux; CPE: cpe:/o:linux:linux_kernel
    - Port 22 OpenSSH 6.7p1
    - Port 80 HTTP Apache httpd 2.4.10 (Debian)
    - Port 111 RPCBind 2-4 (RPC #1000000)
    - Port 139 NetBios-SSN Samba smb 3.X - 4.X (workgroup: Workgroup)
    - Port 445 NetBios-SSN Samba smb 3.X - 4.X (workgroup: Workgroup)

_TODO: Fill out the list below. Include severity, and CVE numbers, if possible._

The following vulnerabilities were identified on each target:
- Target 1
  - List of
  - Critical
  - Vulnerabilities

_TODO: Include vulnerability scan results to prove the identified vulnerabilities._

### Exploitation
_TODO: Fill out the details below. Include screenshots where possible._

The Red Team was able to penetrate `Target 1` and retrieve the following confidential data:
- Target 1
  - `flag1{b9bbcb33e11b80be759c4e844862482d}`:
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      -  ```
      -  cd /var/www/html 
      -  grep -r flag 
      -  ```
  - `flag2{fc3fd58dcdad9ab23faca6e9a36e581c}`: 
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_
  - `flag3{afc01ab56b50591e7dccf93122770cd2}`: 
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_
  - `flag4{715dea6c055b9fe3337544932f2941ce}`: 
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_