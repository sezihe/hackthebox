# HackTheBox Starting Point - Redeemer

IP: 10.129.227.37


## Nmap
```bash
nmap -sC -sV -oN nmap/initial 10.129.227.37
```

Ports Open
```
PORT   STATE SERVICE VERSION
135/tcp open  msrpc         Microsoft Windows RPC
139/tcp open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp open  microsoft-ds?
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows
```

Questions
```
Q: What does the 3-letter acronym SMB stand for?
A: Server Message Block

Q: What port does SMB use to operate at?
A: 445

Q: What is the service name for port 445 that came up in our Nmap scan?
A: microsoft-ds

Q: What is the 'flag' or 'switch' we can use with the SMB tool to 'list' the contents of the share?
A: -L

Q: What is the name of the share we are able to access in the end with a blank password?
A: WorkShares

Q: What is the command we can use within the SMB shell to download the files we find?
A: get
```
