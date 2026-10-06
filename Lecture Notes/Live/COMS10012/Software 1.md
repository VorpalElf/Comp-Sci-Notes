---
Date & Time: 22-09-2026 11:11
Lecturer:
  - Gretchen Hallett
Course Name:
  - COMS10012
Lecture Name: System Admin
---
## Permission
```bash
-rwxr-x--- root wheel nigel.txt
```
<mark style="background: #FFB86CA6;">user group others</mark> <mark style="background: #BBFABBA6;">userName groupName</mark> filename

![[Pasted image 20260922114934.png]]

## OpenSSH
- Secure Shell
- Runs on port 22
- Remotely login to another machine
- `-i FILENAME` for identity file
### SSH Keys
- Private Key: `id_CIPHER`
- Public Key: `id_CIPHER.pub`
- Generate `ssh-keygen -t ed25519`, -t: Type of crypt algorithm
- `known_hosts`: where SSH stores public keys computers you've already connected to
- `authorized_keys`: Server side, only accept public key if in the file
### SSH Config
In `~/.ssh/config`
```
Host lab

  HostName rd-mvb-linuxlab.bristol.ac.uk

  User USERNAME
  
  # Optional
  IdentityFile FILENAME 
```
## File Transfer
```bash
# Send
scp FILEPATH username@dest
# Receive
scp username@source:FILEPATH username@dest:DESTPATH
```

## Linux File System
Binary: `bin/`
Bootloader: `boot/`
Device files: `/dev/`
Config: `etc/`
Programs for root: `sbin/`
Temporary files, lives in RAM: `/tmp`
Files being served: `srv/` or `var/`
Runtime: `run/`
User: `/usr`
User installed programs: `/usr/local`
System-wide config: `/opt`
Dynamic libraries: `/lib`



---
#Incomplete