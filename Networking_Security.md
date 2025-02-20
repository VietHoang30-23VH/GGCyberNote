# Connect and Protect: Networks and Network Security

## MODULE 1:
- A local area network, or LAN, spans a small area like an office building, a school, or a home.
- A wide area network or WAN spans a large geographical area like a city, state, or country.
- A hub is a network device that broadcasts information to every device on the network.
- A switch makes connections between specific devices on a network by sending and receiving data between them. A switch connects the network to devices like phones, tablets, workstations, and desktops.
- A router is a network device that connects multiple networks together. A router connects the internet, firewall, and server to the rest of the network.
- A modem is a device that connects your router to the internet, and brings internet access to the LAN.
- A firewall is a network security device that monitors traffic to or from your network.
- Servers provide information and services for devices like computers, smart home devices, and smartphones on the network.
- A wireless access point sends and receives digital signals over radio waves creating a wireless network.
- Cloud computing is the practice of using remote servers, applications, and network services that are hosted on the internet instead of on local physical devices.
- A cloud network is a collection of servers or computers that stores resources and data in a remote data center that can be accessed via the internet.
- Software as a service (SaaS) refers to software suites operated by the CSP that a company can use remotely without hosting the software.
- Infrastructure as a service (IaaS) refers to the use of virtual computer components offered by the CSP.
- Platform as a service (PaaS) refers to tools that application developers can use to design custom applications for their company.
- **SDNs:**
  + Reliability in cloud computing is based on how available cloud services and resources are, how secure connections are, and how often the services are effectively running.
  + Cost
  + Scalability
- A data packet is a basic unit of information that travels from one device to another within a network.
- Bandwidth refers to the amount of data a device receives every second.
- Header the IP address, and the media access control, or MAC, address of the destination device.
- Body includes messages.
- Footer includes signature on a letter.
- IP has a set of standards used for routing and addressing data packets as they travel between devices on a network.
- The network access layer deals with creation of data packets and their transmission across a network. This includes hardware devices connected to physical cables and switches that direct data to its destination.
- The internet layer is where IP addresses are attached to data packets to indicate the location of the sender and receiver.
- The transport layer includes protocols to control the flow of traffic across a network.
- **Application layer**, protocols determine how the data packets will interact with receiving devices. Functions that are organized at application layer include file transfers and email services. (HTTP,SMTP,SSH,FTP,DNS)
- The ICMP reports information about packets that were dropped or that disappeared in transit, issues with network connectivity, and packets redirected to other routers. (internet layer)
- The Transmission Control Protocol (TCP) is an internet communication protocol that allows two devices to form a connection and stream data. It ensures that data is reliably transmitted to the destination service. TCP contains the port number of the intended destination service, which resides in the TCP header of a TCP/IP packet. (transport layer)
- The User Datagram Protocol (UDP) is a connectionless protocol that does not establish a connection between devices before transmissions. It has performance-sensitive applications that operate in real time, such as video streaming. (transport)
- An internet protocol address, or IP address, is a unique string of characters that identifies a location of a device on the internet.
- An IPv4 header format is determined by the IPv4 protocol and includes the IP routing information that devices use to direct the packet.
  + The first 20 bytes are a fixed set of information containing data such as the source and destination IP address, header length, and total length of the packet. The last set of bytes can range from 0 to 40 and consists of the options field.
- Public IP Address kết nối với geographic location.

## MODULE 2:
- Network protocols are a set of rules used by two or more devices on a network to describe the order of delivery and the structure of the data.
- TCP isn’t limited to just two devices. It establishes a direct connection between two endpoints, but the underlying network infrastructure can handle routing data packets across multiple devices. TCP uses a three-way handshake process.
- The Address Resolution Protocol, or ARP, is used to determine the MAC address of the next router or device on the path. This ensures that the data gets to the right place.
- The Hypertext Transfer Protocol Secure, or HTTPS, is a network protocol that provides a secure method of communication between client and website servers.
- Domain Name System, or DNS, is a network protocol that translates internet domain names into IP addresses.
- So just by visiting one website, the devices on your network are using four different protocols: TCP, ARP, HTTPS, and DNS.
- **Communication protocols**: TCP, UDP, HTTP-80. DNS-UDP 53,
- **Management protocols**: SNMP(app), ICMP(internet)-ping
- **Security protocols**: HTTPS-443, SFTP-22 (app)
- **Other**: NAT, DHCP, ARP, Telnet-23, SSH-22, Post Office Protocol(POP3)-995, IMAP-993, SMTP-587
- IEEE802.11, commonly known as Wi-Fi, is a set of standards that define communications for wireless LANs.
- WPA is a wireless security protocol for devices to connect to the internet.
- **Vulnerability of WPA**: Despite the security improvements of WPA, it still has vulnerabilities. Malicious actors can use a key reinstallation attack (KRACK attack) to decrypt transmissions using WPA.
- WPA2 improves upon WPA by using the Advanced Encryption Standard (AES) (KRACK attacks).
- WPA3 addresses the authentication handshake vulnerability to KRACK attacks, which is present in WPA2. Using Simultaneous Authentication of Equals (SAE), a password-authenticated, cipher-key-sharing agreement. WPA3 has increased encryption to make passwords more secure by using 128-bit encryption, with WPA3-Enterprise mode offering optional 192-bit encryption.

## MODULE 3:
- A firewall is a network security device that monitors traffic to and from your network. It either allows traffic or it blocks it based on a defined set of security rules.
- Firewalls can use port filtering, which blocks or allows certain port numbers to limit unwanted communication.
- A hardware firewall is considered the most basic way to defend against threats to a network; it inspects each data packet before it's allowed to enter the network.
- A software firewall is installed on a computer, it will analyze all the traffic received by that computer.
- Cloud-based firewalls also protect any assets or processes that an organization might be using in the cloud.
- **Stateful** refers to a class of firewall that keeps track of information passing through it and proactively filters out threats.
- A next-generation firewall (NGFW) provides even more security than a stateful firewall. It performs more in-depth security functions like deep packet inspection and intrusion protection.
- Virtual Private Networks (VPNs) is a network security service that changes your public IP address and hides your virtual location so that you can keep your data private when you're using a public network like the internet.
- **Encapsulation** is a process performed by a VPN service that protects your data by wrapping sensitive data in other data packets.
- VPN also uses an encrypted tunnel between your device and the VPN server. The encryption is unhackable without a cryptographic key.
- **Security zones** are a segment of a network that protects the internal network from the internet, acting as a barrier to maintain privacy and prevent issues from spreading.
- On the outer layer is the demilitarized zone (DMZ), which contains public-facing services.
- The restricted zone protects highly confidential information accessible only to certain employees.
- **Classless Inter-Domain Routing (CIDR)** is a method of assigning subnet masks to IP addresses to create a subnet.
- **Proxy Servers**: A server that forwards client requests to other servers.
  + **Forward Proxy**: Hides a user's IP address and approves outgoing requests.
  + **Reverse Proxy**: Accepts traffic from external parties, forwards it to internal servers.
  + **Email Proxy**: Filters spam emails and reduces phishing attacks.

## MODULE 4:
- **Security Hardening**: Strengthens a system to reduce its vulnerability and attack surface.
  + OS hardening includes patch updates, baseline configuration, and MFA.
  + **Networking Hardening**: Involves port filtering, encryption over networks, network log analysis, and firewall configuration.
  + **Cloud Hardening**: Includes IAM, zero-day attacks, shared responsibility model, and modern encryption methods like TPM and CloudHSM.
