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
-  Royalty-free (RF)
-  load–store architecture
-  Its floating-point instructions use IEEE 754 floating-point
  
<br>

**Kernel** : 
-  computer program at the core of a computer's operating system(OS) 
-  Program to manage communication between software .
- generally has complete control over everything in the system
-  responsible for preventing and mitigating conflicts between different processes
-  
<br>

**DNS** :
- Domain Name System
- Turns domain names into IP addresses, which allow browsers to get to websites and other internet resources.
- 
<br>

**ISA** :
- instruction Set Architecture
- Hardware interaction
- Implemntation
  -  A device that executes instructions described by that ISA, such as a central processing unit (CPU), is called an implementation.
- ISA stands for Instruction Set Architecture.
- It refers to the set of instructions that a computer processor can execute.
- The ISA defines the operations and behavior of a processor, including the data types, registers, and memory addressing modes.
- Different processors can have different ISAs, which determine their compatibility with software and operating systems.
- The ISA serves as an interface between the hardware and software layers of a computer system.
- It defines the binary format of instructions and how they are executed by the processor.
- Common ISAs include x86, ARM, MIPS, and PowerPC.
- Software developers need to write code that is compatible with a specific ISA to ensure it can run on a particular processor or architecture.
- ISA designs can influence factors such as performance, power efficiency, and overall system design.
- outing datagrams from a source host interface to a destination host interface across one or more IP networks
<br>

**IP Address** :
- Internet Protocol (IPv4 , IPv6)
-  network layer communications protocol
-  delivering packets from the source host
-  Its routing function enables internetworking
-  defines packet structures
   - that encapsulate the data to be delivered.
- defines addressing methods
  - that are used to label the datagram with source and destination information
- addressing host interfaces, encapsulating data into datagrams
- Each datagram has two components
  - Header
    -  IP header: includes a source IP address, a destination IP address, and other metadata needed to route and deliver the datagram
  - Payload
    - IP payload : payload is the data that is transported.
    - method of nesting the data payload in a packet with a header is called encapsulation
<br>
**IPsec**
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

**VM**  
- Virtual Machine
-  Created by using Hypervisor
-  virtualization or emulation of a computer system
 
<br>

**FPGA** : 
- Field Programmable Gate Arrays
-  Array of Programmable logic block 
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
 <br>
 
**Openstack** 
-  free, open source cloud computing platform
-   deployed as infrastructure-as-a-service (IaaS)
   - n both public and private clouds where virtual servers and other resources are made available to users.

<br>

**Proxmox**
<br>
**AWS**
<br>
**Network Layer**
<br>
**Datagram**
<br>
**Helm**
<br>
**Webassembly** 
<br>
**YOTTA**
- design, build and operate infinitely scalable Data Center Parks
<br>
**HCI**
- Human-computer interaction
- four main components
  - the user
  -  task
  -   tools / interface
  -    context.
- HCI researchers analyze and design specific user interface technologies
  - e.g. pointing devices
<br>
**Kubernetes**
- K8s
- an open-source container orchestration system
  - for automating software deployment, scaling, and management
- Originally designed by Google
  -  the project is now maintained by the Cloud Native Computing Foundation
- Kubernetes works with various container runtimes
  - such as containerd and CRI-O
- Wriiten in Go
- Kubernetes defines a set of building blocks ("primitives") that collectively provide mechanisms that deploy, maintain, and scale applications based on CPU, memory or custom metrics.
- loosely coupled and extensible to meet the needs of different workloads.
<br>
**Container**
- containerization is operating system-level virtualization or application-level virtualization over multiple network resources so that software applications can run in isolated user spaces called containers in any cloud or non-cloud environment, regardless of type or vendor.
- Types of containers
  - OS containers
  - Application containers
-  the containerization technology has been widely adopted by cloud computing platforms.
   - like AWS, Microsoft Azure, Google Cloud Platform, and IBM Cloud.
- Security issues
  - Because of the shared OS, security threats can affect the whole containerized system.
  - In containerized environments, security scanners generally protect the OS but not the application containers, which adds unwanted vulnerability
<br>
**Bare-metal Server**
- used by one consumer, or tenant, only.

<br>

**OOPS**
- Object-Oriented Programming System
- Four types of OOPs
  - Abstraction
  -  encapsulation
  -   polymorphism
  -    inheritance
<br>
 
**KVM**
- Kernel-based Virtual Machine
- 
<br>

**Overlay network**
  
<br>

**Host Network**

<br>

**TUN flannel**
<br>

**OS**
  <br>
  
**ARP linux**
- Address Resolution Protocol
  <br>
  
**RARP**
<br>

**TAP**
  <br>
  
**Libvirt**
<br>

**User-Space**
  <br>
  
**Kernel-Space**
<br>

**Ovirt**
  <br>
  
  **Kubevirt**
  <br>
  
  **RAFT**
  <br>
  
  **Calico Flannel**
  <br>
  
  **RKT**
  <br>
  
  **VXLAN**
  <br>
  **Hypervisor**
  <br>
  **Type-1**
  <br>
  **Type-2**
  <br>
  **VirtualBox**
  <br>
  **VMware workstation**
<br>
**Apache Mesos**
- open-source
- project to manage computer clusters.
-  It was developed at the University of California, Berkeley.
<br>
**Vendor lock-in**
- a situation in which a client gets dependent on a certain cloud provider in order to complete their computing needs
- The client is not able to readily switch to another provider without incurring large expenditures or experiencing business disruptions
- This might occur when a customer has committed considerable resources to a certain cloud platform
  - such as building apps or transferring data there
  - and is unable to switch platforms without paying a hefty fee.
- This may restrict the ability of the customer to transfer providers and may offer the provider a powerful negotiating position when negotiating prices and other issues.
  <br>
  ![Vendor-Lock-in](https://github.com/Raveena-29/cloud-computing/assets/148243757/189813f6-f1c6-479f-9596-3907fb71f02c)
