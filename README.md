# wic-securite-tp

**> netdiscover -r 192.168.25.0/24**

IP            At MAC Address     Count     Len  MAC Vendor / Hostname      
 -----------------------------------------------------------------------------
 192.168.25.1    00:50:56:c0:00:01      1      60  VMware, Inc.                     
 192.168.25.129  00:0c:29:b2:a9:79      1      60  VMware, Inc.                     
 192.168.25.131  00:0c:29:b5:29:86      1      60  VMware, Inc.                     
 192.168.25.254  00:50:56:f9:b7:03      1      60  VMware, Inc.               



**> nmap -v -sS  192.168.25.129**


Completed SYN Stealth Scan at 09:48, 0.08s elapsed (1000 total ports)
Nmap scan report for 192.168.25.129
Host is up (0.00037s latency).
Not shown: 990 closed ports
PORT     STATE SERVICE
22/tcp   open  ssh
25/tcp   open  smtp
80/tcp   open  http
110/tcp  open  pop3
111/tcp  open  rpcbind
139/tcp  open  netbios-ssn
143/tcp  open  imap
445/tcp  open  microsoft-ds
901/tcp  open  samba-swat
3306/tcp open  mysql
MAC Address: 00:0C:29:B2:A9:79 (VMware)


**> nmap -v -sS  192.168.25.131**

Completed SYN Stealth Scan at 09:49, 0.06s elapsed (1000 total ports)
Nmap scan report for 192.168.25.131
Host is up (0.00018s latency).
Not shown: 995 closed ports
PORT     STATE SERVICE
135/tcp  open  msrpc
139/tcp  open  netbios-ssn
445/tcp  open  microsoft-ds
1025/tcp open  NFS-or-IIS
5000/tcp open  upnp
MAC Address: 00:0C:29:B5:29:86 (VMware)


**> nmap -v -sS  192.168.25.254**

Completed SYN Stealth Scan at 09:51, 21.10s elapsed (1000 total ports)
Nmap scan report for 192.168.25.254
Host is up (0.0015s latency).
All 1000 scanned ports on 192.168.25.254 are filtered
MAC Address: 00:50:56:F9:B7:03 (VMware)

**> nmap -v -O  192.168.25.131**

MAC Address: 00:0C:29:B5:29:86 (VMware)
Device type: general purpose
Running: Microsoft Windows 2000|XP|Me
OS CPE: cpe:/o:microsoft:windows_2000::- cpe:/o:microsoft:windows_2000::sp2 cpe:/o:microsoft:windows_2000::sp4 cpe:/o:microsoft:windows_xp::- cpe:/o:microsoft:windows_xp::sp1 cpe:/o:microsoft:windows_me
OS details: Microsoft Windows 2000 SP0/SP2/SP4 or Windows XP SP0/SP1, Microsoft Windows 2000 SP2, Microsoft Windows Millennium Edition (Me)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=126 (Good luck!)
IP ID Sequence Generation: Incremental


**> nmap -v -O  192.168.25.129**

MAC Address: 00:0C:29:B2:A9:79 (VMware)
Device type: general purpose
Running: Linux 2.6.X
OS CPE: cpe:/o:linux:linux_kernel:2.6
OS details: Linux 2.6.9 - 2.6.30
Uptime guess: 0.034 days (since Fri Sep 30 09:16:42 2016)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=207 (Good luck!)
IP ID Sequence Generation: All zeros




