# cloud-computing
##**Keywords**
<br>

**etcd** : 
- Open source key value data store
- Manage and store data that help keep distributed systems running
- Well known for being one of core components of kubernetes
  - manages and stored kubernetes State Data , configuration data and meta data

**Features of etcd**
1. Fully replicated
   - every node in an etcd cluster has access to the full data store.
1. Reliably consistent
   - every data read in an etcd cluster is going to return the most recent data right
1. Highly Available
   - can tolerate network partitions and hardware failure too
1. Fast
   - bendmarked at 10,000 writes per second
1. Secure
   - Uses transport layer security with SSL client certificate authentication.
1. Simple to use
   - A web app can read and write data to etcd using simple http JSON tools.
1. Watch Function
   - If configuration and store data of kubernetes ever go out of sync, etcd will let the kubernetes API know and the kubernetes API will reconfigure the cluster acccordingly.
   
<br>

**CISC** :
- Complex instructiion set computer
-  closed source - Intel , AMD
-  single instructions can execute several low-level operations
   - such as a load from memory, an arithmetic operation, and a memory store
<br>

**RISC** : 
- Reduced Instruction Set Computer
-  Closed sourse-ARM
-  computer architecture designed to simplify the individual instructions given to the computer to accomplish tasks
-  require more instructions (more code) in order to accomplish a task
   - the individual instructions are written in simpler code
-  each instruction performs only one function
   - Example : copy a value from memory to a register
  
<br>

**RISC-V** : 
- It is an ISA based on reduced instruction set computer(RISC) principles
-  Open source
<br>

**Kernel** : 
- Program to manage communication between software .
-  User-level applications and hardware.
-   CPU and disk memory
<br>

**DNS** :
- Turns domain names into IP addresses, which allow browsers to get to websites and other internet resources.
<br>
**ISA** : instruction Set Architecture , Hardware interaction , input - outputs , registers , data types 
<br>
**IP Address** : Internet Protocol (IPv4 , IPv6)
<br>
**Public IP** : B/W Internet and Device, assigned by internet service provider to the device
<br>
**Private IP** : Private network addresses are not allocated to any specific organization(can use without approval from regional or local internet registries).In a private network (starts with 10,17.16 , 192.168).
<br>
**Port No.** : a way to identify a specific process to which an internet or other network message is to be forwarded when it arrives at a server.(For HTTP- 80 , SSH-22 , SMTP- 25 , Telnet-23 , HHTPS - 443)
<br>
**SSL** - Secure Socket Layer - IP Address+Port Number 
<br>
**Seven Layers of OSI** (Open Systems Interconnection)

 - L7 : Application 
 + L6 : Presentation
 * L5 : Cryptography 
 - L4 : Port Number (16 Bits)
 + L3 : IP[ Address(32 Bits) , Router
 * L2 - Hardware Address, NIC , MAC Address(48 Bits) , Ethernet , Switch 
 - L1 : Digiital (1 and 0)
   
<br> 
**Switch** : Connects devices in a network to each other , enabling them to talk by exchanging data packets.
<br>
**Virtual Machine** : 
- Created by using Hypervisor
+ virtualization or emulation of a computer system
* 
<br>
**FPGA** : Field Programmable Gate Arrays . Array of Programmable logic block 
<br>
**Libvirt** : 
-Open source API 
*managing platform virtualization
+Used to manage KVM , Xen, VMware ESXI , QEMU 
-C Library with binding in other languages.
<br>
**LXC** : lightweight Linux container system 
<br>
**OpenVZ** : lightweight Linux container system  
<br>
**Helm** 
- Helps in managing Kubernetes applications 
+ It renders your templates and communicates with the kubernetes API 
* Charts are Helm packages

<br>

**Docker**
1. A set of PaaS products
   - OS level irtualization to deliver software in packages (Containers)
2. Software that hosts the containers is called Docker Engine
   - Released in 2013
     - Developed by Docker , Inc 
 
