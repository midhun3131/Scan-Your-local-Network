# Nmap Installed
# Find Your Local IP ranges 
 Ifconfig
# Run nmap  
 Nmap -sS 10.0.2.25/24
# Open Ports found
135/tcp  open  msrpc         Microsoft Windows RPC
445/tcp  open  microsoft-ds?
1583/tcp open  psql          Pervasive.SQL Server - Relational Engine (encrypted)
3351/tcp open  psql-btrieve  Pervasive.SQL Server - Btrieve Engine
6646/tcp open  unknown
# Common ports
21	FTP	File Transfer Protocol (insecure)
22	SSH	Secure remote login
23	Telnet	Insecure remote login (deprecated)
25	SMTP	Email server (sending mail)
53	DNS	Domain Name System
80	HTTP	Web server (unsecured)
110	POP3	Email retrieval (insecure)
135	RPC	Microsoft Remote Procedure Call
139	NetBIOS	Windows file/printer sharing
143	IMAP	Email retrieval
443	HTTPS	Secure web server
445	SMB	Windows file sharing
3389	RDP	Remote Desktop Protocol
8080	HTTP-Alt/Proxy	Alternate web or proxy service
# Open Port	Potential Risk
21 (FTP)	Credentials sent in plain text → Use SFTP/FTPS
23 (Telnet)	No encryption, outdated → Replace with SSH
80 (HTTP)	Unencrypted web traffic → Switch to HTTPS
445 (SMB)	Exploitable (e.g., EternalBlue) → Restrict or patch
3389 (RDP)	Brute-force attacks possible → Enable 2FA or VPN
Any unused port	Backdoors or misconfigurations → Close it
7.-local-Network
