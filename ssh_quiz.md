## SSH (Secure Shell) Overview

### SSH Basics
- Purpose: Secure remote access and management over untrusted networks
- Default port: 22 (customizable)
- Authentication methods:
  - Password-based
  - Key-based
  - Multi-factor authentication (MFA)

### SSH Key Management
- Key generation using `ssh-keygen`
  - Key types: RSA, ED25519
  - Key size options (e.g., 4096 for RSA)
  - Passphrase protection
- Authorized keys file (`~/.ssh/authorized_keys`)
  - Proper permissions (600 for file, 700 for directory)
  - Key restrictions (IP, commands)
- Key management tools
  - `ssh-agent` for key caching
  - `ssh-add` for key management
  - `known_hosts` file for server verification

### SSH Tools
- PuTTY (Windows)
  - GUI configuration
  - Key management via PuTTYgen
  - Session saving
- MobaXterm (Windows)
  - Built-in X server
  - Tabbed interface
  - Integrated SFTP
- OpenSSH (Linux/macOS)
  - Native command-line tools
  - Full SSH feature support

### X-Windows Forwarding
- Purpose: Run graphical applications remotely
- Requirements:
  - Local X server
  - Server X11Forwarding enabled
- Usage with -X (untrusted) or -Y (trusted)
- Performance and security considerations

### SSH Tunneling
- Local Port Forwarding (-L)
- Remote Port Forwarding (-R)
- Dynamic Port Forwarding (-D)
- Configuration and security considerations

### File Transfer Commands
- SCP (Secure Copy)
  - Basic syntax and options
  - Performance limitations
- Rsync
  - Efficient synchronization
  - Incremental transfers
  - Resume capability
- SFTP
  - Interactive file management
  - Basic commands

### Remote Command Execution
- Basic command execution
- Environment sourcing issues
- TTY requirements
- Quoting and exit codes

### Common Issues and Troubleshooting
- Connection refused
- Permission denied
- Host key verification
- Slow connections
- Broken pipe
- Environment variables

### SSH Configuration
- `~/.ssh/config` file
- Host-specific settings
- Command simplification

### Security Best Practices
- Disable password authentication
- Change default port
- Use strong keys
- Restrict access
- Enable MFA
- Regular updates
- Log monitoring

### Advanced Use Cases
- SSH over proxy
- Reverse SSH
- Automation
- Port knocking

### Debugging
- Verbose mode
- Server logs
- Configuration testing
- Network tools

### Terms
- SSH (Secure Shell) - A cryptographic network protocol for secure remote access and management of systems
- Public/Private Key Pair - A set of cryptographic keys used for authentication, where the public key is shared and the private key is kept secret
- X-Windows Forwarding - A feature that allows running graphical applications on a remote server and displaying them locally
- SSH Tunneling - Creating encrypted tunnels to forward network traffic through an SSH connection
- SCP (Secure Copy) - A command-line tool for securely transferring files between systems
- Rsync - A utility for efficiently transferring and synchronizing files between systems
- SFTP (Secure File Transfer Protocol) - An interactive file transfer protocol that provides secure file management
- SSH Agent - A program that holds private keys in memory to avoid repeated passphrase entry
- Known Hosts - A file containing public keys of SSH servers for host verification
- Port Forwarding - Redirecting network traffic from one port to another through an SSH connection

///

Now, I'll create a quiz based on this content:

## What is the default port used by SSH?

---

A) 21

B) 22

C) 23

D) 80

---

22

///

## Which of the following is NOT a valid SSH authentication method?

---

A) Password-based

B) Key-based

C) Token-based

D) Multi-factor authentication

---

Token-based

///

## What command is used to generate SSH keys?

---

A) ssh-keygen

B) ssh-key

C) keygen

D) generate-key

---

ssh-keygen

///

## What is the recommended permission setting for the authorized_keys file?

---

A) 644

B) 600

C) 755

D) 777

---

600

///

## Which Windows SSH client includes built-in X server support?

---

A) PuTTY

B) MobaXterm

C) OpenSSH

D) WinSCP

---

MobaXterm

///

## What flag is used for untrusted X-Windows forwarding?

---

A) -X

B) -Y

C) -W

D) -F

---

-X

///

## Which type of SSH tunneling creates a SOCKS proxy?

---

A) Local Port Forwarding

B) Remote Port Forwarding

C) Dynamic Port Forwarding

D) Static Port Forwarding

---

Dynamic Port Forwarding

///

## What is the main advantage of using rsync over scp?

---

A) Better security

B) Incremental transfers

C) Simpler syntax

D) Faster initial transfer

---

Incremental transfers

///

## What is the purpose of the ssh-agent?

---

A) To generate new SSH keys

B) To cache decrypted private keys

C) To manage server configurations

D) To forward X-Windows sessions

---

To cache decrypted private keys

///

## Which file stores the public keys of known SSH servers?

---

A) authorized_keys

B) known_hosts

C) config

D) id_rsa.pub

---

known_hosts

///

## What is the recommended key size for RSA keys?

---

A) 1024 bits

B) 2048 bits

C) 4096 bits

D) 8192 bits

---

4096 bits

///

## Which of the following is NOT a security best practice for SSH?

---

A) Disable password authentication

B) Use default port 22

C) Enable MFA

D) Keep software updated

---

Use default port 22

///

## What command is used to test SSH server configuration?

---

A) sshd -t

B) ssh -t

C) ssh-test

D) test-sshd

---

sshd -t

///

## What is the purpose of the ~/.ssh/config file?

---

A) To store SSH keys

B) To define host-specific settings

C) To configure the SSH server

D) To store known hosts

---

To define host-specific settings

///

## Which of the following is NOT a common SSH troubleshooting step?

---

A) Check server logs

B) Use verbose mode

C) Test network connectivity

D) Reinstall the operating system

---

Reinstall the operating system
