# cloud-computing
##**Keywords**
<br>

**Cloud computing**
- Cloud computing is the delivery of computing services
  - including servers , storage , databases , networking , software , analytics and intelligence
  - over the internet("the cloud") to offer faster innovation , flexible resources and economies of scale
<br>

**Benefits of Cloud**
- Faster time to market
- Scalability and flexibility
- Cost savings
- Better collaboration
- Advanced security
- Data loss prevention
<br>

**Disadvantages of Cloud**
- risk of vendor lock-in
- less control oer underlying cloud infrastructure
- concerns about security risks like data privacy and online threats
- integration complexity with existing systems
- unforeseen costs and unexpected expenses
<br>
**MQ** :
- Magic quadrant
- Series of market research reports published by IT consulting firm Gartner that rely on proprietary qualitative data analysis methods to demonstrate market trends, such as direction, maturity and participants.
- Their analyses are conducted for several specific technology industries and are updated every 1–2 years: once an updated report has been published, its predecessor is "retired".

  <br>
  
**Gartner's Magic Quadrant**
- The Gartner Magic Quadrant is a visual method of reporting. Magic Quadrants are used to depict which companies are leading the way within a specific market.
  ![gartner-2023](https://github.com/Raveena-29/cloud-computing/assets/148243757/7f36c2e7-0110-4cc9-bf4a-ec5460fc0734)
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

**EC2**
- Amazon Elastic Compute Cloud(EC2)
- A part of Amazon.com's cloud-computing platform, Amazon Web Services (AWS)
- Allows users to rent virtual computers on which to run their own computer applications.
- EC2 encourages scalable deployment of applications by providing a web service through which a user can boot an Amazon Machine Image (AMI) to configure a virtual machine, which Amazon calls an "instance", containing any software desired.
- A user can create, launch, and terminate server-instances as needed, paying by the second for active servers – hence the term "elastic".
- EC2 provides users with control over the geographical location of instances that allows for latency optimization and high levels of redundancy.
<br>

**Dedicated host**
- A dedicated hosting service, dedicated server, or managed hosting service is a type of Internet hosting in which the client leases an entire server not shared with anyone else.
- This is more flexible than shared hosting, as organizations have full control over the server(s), including choice of operating system, hardware, etc.
<br>

**AMI**
- Amazon Machine Image(AMI)
- a special type of virtual appliance that is used to create a virtual machine within the EC2
- It serves as the basic unit of deployment for services delivered using EC2.
<br>

**IaaS** :
<br>

**PaaS**
<br>

**SaaS**
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
-  Each instruction performs only one function
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
  - An IP Address is basically classified into two types:
    - Private IP Address
    - Public IP Address
<br>
**IPsec**
- Internet Protocol Security
- secure network protocol suite that authenticates and encrypts packets of data to provide secure encrypted communication between two computers over an Internet Protocol network.
- used in virtual private networks (VPNs)
- IPsec can control data flows between:
  - host-to-host
  - network-to-network
  - network-to-host
  
<br>

**Public IP** 
-  an IPv4 address that is reachable from the internet.
-  All public IP addresses on the Internet are unique to their host or server and cannot duplicate
-  The scope of Public IP is global.
-  Public IP Address is basically of two types:
   - Dyanamic IP address
     - addresses that change over time.
   - Static IP address
     - addresses that do not change with time
     - Mostly these are used by the DNS (Domain Name System) Servers.
-  For example
   -  google.com — 172.217. 22.14
   -   Google's DNS server — 8.8. 8.8
<br>

**Private IP** 
- IP address that is used to communicate within the same network
- Unique private IP Addresses are provided to each and every device that is present on the network.
- It is available free of cost
- The scope of Private IP is local.
<br>

**Hybrid Cloud**
- Combination of both priate and public cloud
- Shared security responsiility
- Helps maintain tighter controls over sensitive data and processes
<br>

**Port No.** 
- number assigned to uniquely identify a connection endpoint and to direct data to a specific service
- At the software level, within an operating system, a port is a logical construct that identifies a specific process or a type of network service.
- The most common transport protocols that use port numbers are:
  - the Transmission Control Protocol (TCP)
  -  the User Datagram Protocol (UDP)
  -  those port numbers are 16-bit unsigned numbers.
<br>

**SSL** 
- Secure Socket Layer
-  Used to secure communication between a web browser and a web server
-  This turns a website's address from HTTP to HTTPS, the 'S' standing for 'secure'
-  all SSL certificates are no longer in use
-  However, the industry continues to use the term SSL to refer to TLS certificates.
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

**Switch** 
- Connects devices in a network to each other
- enabling them to talk by exchanging data packets.
- Switches can be hardware devices that manage physical networks or software-based virtual devices.
- A network switch operates on the data-link layer, or Layer 2, of the Open Systems Interconnection (OSI) model.
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

![Vendor-Lock-in](https://github.com/Raveena-29/cloud-computing/assets/148243757/f0c6fee5-58ad-4d4a-94b4-1b65b1185878)
- Disadvantages of Vendor Lock-in
  - Limited Flexibility
  - Higher prices
  - Dependence on a Single Provider:
  - Limited Scalability
  - Data Migration Challenges
  - Limited Control over the Technology Stack
<br>

**NUMA**
- Non-uniform memory access
- computer memory design
  - used in multiprocessing
  -  the memory access time depends on the memory location relative to the processor
- Each processor is connected to specific memory region
- a processor can access its own local memory faster than non-local memory
- This design aims to reduce memory access latency and increase overall system performance
<br>
- Benifits
  - Non uniform access time
  - Scalability
  - Improves performance
<br>

**Cilium**
- Cilium is a networking, observability, and security solution with an eBPF-based dataplane.
- It provides a simple flat Layer 3 network with the ability to span multiple clusters in either a native routing or overlay mode.
- L7-protocol aware
<br>

**CEPH**
- Free and Open Source
-  storage platform that provides object storage, block storage, and file storage built on a common distributed cluster foundation
-  
