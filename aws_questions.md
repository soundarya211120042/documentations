---

## 📌 **Storage Questions**

1. **What is Snapshot?**
   - A snapshot is a point-in-time backup of a storage volume. In AWS, EBS snapshots are stored in S3 and used for backup, restore, and cloning volumes.

2. **What is EBS?**
   - EBS (Elastic Block Store) is AWS's block storage for EC2 instances, providing persistent, high-performance storage.

3. **EBS vs EBS (Elastic Block Store vs Elastic Beanstalk)**
   - EBS: Block storage for EC2.
   - Elastic Beanstalk: Platform-as-a-Service for deploying and managing applications.

4. **EFS**
   - EFS (Elastic File System) is a scalable, managed NFS file system for Linux workloads in AWS, mountable on multiple EC2s.

5. **NFS**
   - NFS (Network File System) is a protocol for sharing files over a network, allowing multiple clients to access files remotely.

6. **NFS vs EFS vs EBS**
   - NFS: Protocol for network file sharing.
   - EFS: AWS-managed NFS file system.
   - EBS: Block storage for a single EC2 instance.

7. **What is S3?**
   - S3 (Simple Storage Service) is AWS's object storage service, storing data as objects in buckets.

8. **S3 bucket versioning**
   - Enables multiple versions of objects in a bucket, helping with recovery and protection against accidental deletion.

9. **How to create new EBS and how to attach it on running instance**
   - Create EBS in AWS Console, attach to EC2, use `lsblk` to verify, format and mount.

10. **How to take a snapshot of running instance and how to create a new EBS based on snapshot**
    - Create snapshot from volume, create new EBS from snapshot, attach to instance.

11. **What is mount point?**
    - A directory where a storage device or partition is attached and accessible.

12. **What is LVM?**
    - Logical Volume Manager for flexible disk management, allowing creation and resizing of logical volumes.

13. **What is NVME?**
    - High-speed storage protocol for SSDs, faster than SATA.

14. **What is LSBLK?**
    - Linux command to list block devices (disks, partitions).

15. **Using the attached new EBS volume, how to increase the root volumes (/, /tmp, /var)**
    - Attach EBS, use LVM to extend volumes, resize file systems.

16. **What is partition in root volume?**
    - A section of a disk; root partition contains OS and system files.

17. **Explain the functionality of fstab**
    - `/etc/fstab` configures how disk partitions and volumes are mounted at boot.

18. **What is Shared Volume?**
    - Storage accessible by multiple servers/instances, useful for distributed apps.

19. **What is Persistent Data?**
    - Data that remains after reboots or restarts.

20. **What is PV?**
    - Physical Volume in LVM, the physical storage device for volume groups.

---

## 📌 **Networking Questions**

1. **What is VPC?**
   - Virtual Private Cloud, a logically isolated network in AWS for resources.

2. **What is Security Group?**
   - Virtual firewall controlling inbound/outbound traffic for AWS resources.

3. **What is Routing Table?**
   - Set of rules that determine network traffic direction in a VPC.

4. **What is Subnet?**
   - Subdivision of a VPC's IP range, used to organize resources.

5. **What is Region and Availability Zone?**
   - Region: Geographical area. AZ: Isolated data center within a region.

6. **What is Inbound and Outbound?**
   - Inbound: Traffic coming into a resource. Outbound: Traffic going out.

7. **What is Port?**
   - Logical endpoint for network communication (e.g., 22 for SSH).

8. **What is IP?**
   - Internet Protocol address, unique identifier for devices on a network.

9. **Difference between Private and Public IP**
   - Private IP: Used within VPC, not accessible from internet. Public IP: Accessible from internet.

10. **Explain EIP**
    - Elastic IP, a static public IPv4 address for AWS resources.

11. **What is difference between Public and Private Subnet?**
    - Public subnet: Has route to internet via IGW. Private subnet: No direct internet access.

12. **Explain IGW**
    - Internet Gateway, enables communication between VPC and internet.

13. **What is Load Balancer?**
    - Distributes incoming traffic across multiple targets for high availability.

14. **What are the types of Load Balancer?**
    - Classic, Application (ALB), Network (NLB), Gateway Load Balancer.

15. **Explain DNS**
    - Domain Name System, translates domain names to IP addresses.

16. **What is Target Group in AWS?**
    - Group of resources (EC2, Lambda) for load balancer to route traffic.

17. **What is Auto Scaling Group?**
    - Automatically adjusts number of EC2 instances based on demand.

18. **Explain VPC Peering**
    - Connects two VPCs for private communication.

19. **What is Domain and Subdomain?**
    - Domain: Main address (example.com). Subdomain: Subsection (app.example.com).

20. **What are the records in DNS, Explain it**
    - A (Address), CNAME (Alias), MX (Mail), TXT (Text), NS (Name Server), PTR (Pointer).

---

## 📌 **Linux / Security Questions**

1. **How to use sendmail service in Linux environment?**
   - Install sendmail, configure `/etc/mail/sendmail.cf`, use `mail` command to send emails.

2. **What is Key Pair in AWS?**
   - SSH key pair (public/private) for secure access to EC2 instances.

3. **Difference between Public and Private Key**
   - Public key: Shared, used for encryption. Private key: Kept secret, used for decryption.

4. **What is User and Group?**
   - User: Individual account. Group: Collection of users for permission management.

5. **How to set ownership of the file system?**
   - Use `chown user:group filename` command.

6. **How to set the permissions in files?**
   - Use `chmod` command (e.g., `chmod 755 filename`).

7. **What is SCP?**
   - Secure Copy Protocol for transferring files over SSH.

8. **What is the purpose of sshpass?**
   - Tool to provide password for SSH in scripts/non-interactive sessions.

9. **How to use ssh-keygen command?**
   - Run `ssh-keygen` to generate SSH key pairs for authentication.

10. **Explain UFW**
    - Uncomplicated Firewall, a simple tool to manage firewall rules in Linux.

---
