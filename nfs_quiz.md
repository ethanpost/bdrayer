## Network File System (NFS) Issues and Solutions

> Import this file into [Mochi](https://mochi.cards/) or give it to your favorite AI tool and have it proxy a quiz and check your answers. When importing make sure you select Markdown as the format, "Multiple cards per .md file", and a ```triple backslash``` as the string delimiter. You can use the link to the raw file in GitHub instead of downloading and importing if you prefer.

### Application Impact
- Application hangs or freezes
- Processes waiting indefinitely for I/O operations
- Potential application failures

### System Performance Issues
- Increased CPU and memory usage
- System slowdown
- Resource consumption by waiting processes

### Technical Problems
- Stale file handles (ESTALE errors)
- I/O errors during read/write operations
- Process blocking with "hard" mount option
- Timeouts and retries with "soft" mounts
- Data loss or corruption during server crashes
- Zombie processes consuming resources
- System crashes in severe cases

### User Impact
- Productivity loss
- Downtime
- User frustration
- Mount point inaccessibility
- Log flooding with error messages

### Mitigation Strategies
- Use soft mounts with timeo options
- Set appropriate timeouts
- Implement NFS health monitoring
- Use Autofs for on-demand mounting
- Set up redundant NFS servers
- Tune mount options (intr, noac)
- Ensure stable network connectivity

### Terms
- NFS (Network File System) - A distributed file system protocol that allows a user to access files over a network as if they were on the local machine.
- Hard Mount - An NFS mount option that causes processes to block and wait indefinitely for the server to respond.
- Soft Mount - An NFS mount option that allows operations to time out after a set period, returning errors to applications.
- Stale File Handle - An error condition where a file handle becomes invalid due to server unavailability or mount point disruption.
- Autofs - A system that automatically mounts NFS shares only when needed.
- Zombie Process - A defunct process that continues to consume system resources while waiting on an unresponsive NFS mount.

///

## What happens to applications when an NFS mount point is not responding?

---

A) They continue to function normally

B) They may hang or freeze

C) They automatically switch to local storage

D) They create backup copies of files

---

They may hang or freeze

///

## Which of the following is a characteristic of a "hard" mount option in NFS?

---

A) Processes will time out after a set period

B) Processes will block and wait indefinitely

C) Operations will automatically retry

D) Files will be cached locally

---

Processes will block and wait indefinitely

///

## What is a potential consequence of an NFS server crash during write operations?

---

A) Files will be automatically recovered

B) Data may be lost or corrupted

C) The system will switch to read-only mode

D) All processes will be terminated

---

Data may be lost or corrupted

///

## Which mitigation strategy involves mounting NFS shares only when needed?

---

A) Using soft mounts

B) Implementing Autofs

C) Setting up redundant servers

D) Tuning mount options

---

Implementing Autofs

///

## What is a "stale file handle" in the context of NFS?

---

A) A file that hasn't been accessed recently

B) An invalid file handle due to server unavailability

C) A corrupted file system

D) A file with incorrect permissions

---

An invalid file handle due to server unavailability

///

## Which of the following is NOT a recommended mitigation strategy for NFS issues?

---

A) Using soft mounts with timeo options

B) Setting appropriate timeouts

C) Disabling all network monitoring

D) Implementing NFS health monitoring

---

Disabling all network monitoring

///

## What can happen to system performance when multiple processes are waiting on an unresponsive NFS mount?

---

A) Performance improves

B) System speeds up

C) System slows down

D) No impact on performance

---

System slows down

///

## What is the purpose of the "intr" mount option in NFS?

---

A) To increase file transfer speed

B) To allow interrupting stuck operations

C) To enable automatic failover

D) To improve caching performance

---

To allow interrupting stuck operations

///

## Which of the following is a user impact of NFS mount issues?

---

A) Increased productivity

B) System optimization

C) Productivity loss

D) Better file organization

---

Productivity loss

///

## What is a zombie process in the context of NFS?

---

A) A process that has completed successfully

B) A defunct process consuming system resources

C) A process that has been terminated

D) A process running in the background

---

A defunct process consuming system resources
