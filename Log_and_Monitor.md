# Sound the Alarm: Detection and Response

## Module 1: Introduction to Detection and Incident Response

### The Incident Response Lifecycle
- **Detect, Respond, Recover**: Critical stages during incident response.
- **Incident**: An occurrence jeopardizing confidentiality, integrity, or availability of information.
- **Event**: An observable occurrence on a network, system, or device.
- **Five W's of an Incident**: Who, What, When, Where, Why.

### Incident Response Operations
- **CSIRTs (Computer Security Incident Response Teams)**: Specialized groups managing incidents.
- **Security Analyst**: Monitors for threats, analyzes alerts, performs root-cause investigations.
- **Technical Lead**: Manages technical aspects like applying patches.
- **Incident Coordinator**: Tracks and manages response activities.
- **SOC (Security Operations Center)**: Monitors networks, systems, and devices for threats.
- **Incident Response Plan**: Outlines procedures for each step of incident response.

### Tools
- **Detection and Management Tools**: Monitor system activity.
- **Documentation Tools**: Collect and compile evidence.
- **Investigative Tools**: Analyze events (e.g., packet sniffers).

### Intrusion Detection and Prevention
- **IDS (Intrusion Detection System)**: Monitors and alerts on intrusions.
- **IPS (Intrusion Prevention System)**: Monitors and stops intrusions.
- **EDR (Endpoint Detection and Response)**: Monitors endpoints for malicious activity.

### SIEM and SOAR
- **SIEM Tools**: Collect, normalize, and analyze data.
- **SOAR (Security Orchestration, Automation, and Response)**: Uses automation to respond to security events.
- **Parsing**: Maps data according to fields and values.

---

## Module 2: Network Monitoring and Analysis

### Network Traffic and Data
- **Network Traffic**: Data moving across a network.
- **Network Data**: Data transmitted between devices.
- **Indicators of Compromise (IoCs)**: Observable evidence of potential incidents.
- **Flow**: Movement of network communications (packets, protocols, ports).
- **Command and Control (C2)**: Techniques used by attackers to maintain access.
- **Lateral Movement**: Attackers exploring a network to expand access.

### Defensive Measures
- Prevent attacker access.
- Monitor network activity.
- Protect assets.
- Detect and stop exfiltration.

### Capture and View Network Traffic
- **Network Protocols**: Rules for data transmission.
- **Packet Sniffer**: Captures and analyzes network traffic.
- **Packet Capture (P-cap)**: File containing intercepted data packets.
- **NIC (Network Interface Card)**: Hardware connecting computers to a network.
- **tcpdump**: Command-line packet capture tool.
- **Wireshark**: Graphical packet capture tool.

### IPv4 Header Fields
- **Version**: IP version (e.g., IPv4).
- **IHL (Internet Header Length)**: Length of the header.
- **ToS (Type of Service)**: Packet priority.
- **Total Length**: Length of the entire packet.
- **Identification**: Unique identifier for fragmented packets.
- **Flags**: Information about packet fragmentation.
- **Fragment Offset**: Sequence of fragments.
- **TTL (Time to Live)**: Limits packet circulation time.
- **Protocol**: Protocol used for data.
- **Header Checksum**: Error-checking value.
- **Source Address**: Sender's address.
- **Destination Address**: Receiver's address.
- **Options**: Optional security options.

### Packet Inspection
- **tcpdump Commands**:
  - `-i eth0`: Capture from eth0 interface.
  - `-v`: Display detailed packet data.
  - `-c5`: Capture 5 packets.
  - `-nn`: Do not resolve IPs or ports.
  - `-w capture.pcap`: Save captured data.
  - `&`: Run command in the background.
  - `-X`: Display hexadecimal and ASCII output.
  - `-r`: Read capture data from a file.

---

## Module 3: Incident Investigation and Response

### Threat Hunting and Cyber Deception
- **Threat Hunting**: Proactive search for threats.
- **Cyber Deception**: Techniques to deceive attackers.
- **Honeypots**: Decoy systems to attract intruders.

### Indicators and Documentation
- **IoCs (Indicators of Compromise)**: Observable evidence of incidents.
- **IoAs (Indicators of Attack)**: Behavioral evidence of attackers.
- **Crowdsourcing**: Gathering information through public input.
- **Documentation**: Ensures transparency, standardization, and clarity.
- **Chain of Custody**: Documents evidence possession and control.
- **Custody Log**: Details evidence transfers.
- **Broken Chain of Custody**: Inconsistencies in evidence logging.

### Playbooks and Triage
- **Automated Playbooks**: Automate incident response tasks.
- **Semi-Automated Playbooks**: Combine human action with automation.
- **Triage**: Prioritize incidents by importance or urgency.
  - **Functional Impact**: Impact on operations.
  - **Information Impact**: Impact on data.
  - **Recoverability**: Ease of recovery.

### Containment, Eradication, and Recovery
- **Containment**: Limit additional damage.
- **Eradication**: Remove threats (e.g., patching vulnerabilities).
- **Recovery**: Restore systems to normal operations.

### Final Report
- Comprehensive review of an incident.
- Includes timeline, event details, and prevention recommendations.

---

## Module 4: Network Traffic and Logs Using IDS and SIEM Tools

### Logs and Log Analysis
- **Logs**: Record details of network events.
- **Log Analysis**: Identify events of interest.
- **Types of Logs**:
  - **Network Logs**: Generated by routers, switches, etc.
  - **System Logs**: Generated by operating systems.
  - **Application Logs**: Related to software applications.
  - **Security Logs**: Generated by IDS/IPS.
  - **Authentication Logs**: Record login attempts.

### Log Management
- **Log Management**: Collect, store, analyze, and dispose of log data.
- **Syslog**: Protocol and log format.
- **JSON (JavaScript Object Notation)**: Text-based format for data.
- **XML (eXtensible Markup Language)**: Language for storing and transmitting data.
- **CSV (Comma Separated Values)**: Uses separators like commas.

### Intrusion Detection Systems
- **HIDS (Host-Based Intrusion Detection System)**: Monitors host activity.
- **NIDS (Network-Based Intrusion Detection System)**: Monitors network traffic.
- **Signature Analysis**: Detects patterns associated with malicious activity.
- **Anomaly-Based Analysis**: Identifies abnormal behavior.

### Suricata
- **Suricata**: Can function as IDS, IPS, or NSM.
- **EVE (Extensible Event Format)**: JSON-based log format.
  - **Alert Logs**: Relevant to security investigations.
  - **Network Telemetry Logs**: Record network traffic flows.
- **Custom Rules**: Modify existing rules for specific security needs.

### SIEM Tools
- **Splunk**: Uses SPL (Search Processing Language).
- **Chronicle**: Uses YARA-L for detection rules.

---

## Practice

### Wireshark
- Open saved packet capture files.
- View high-level packet data.
- Use filters to inspect detailed packet data.

### tcpdump
- Identify network interfaces.
- Capture network data for inspection.
- Interpret packet information.
- Save and load packet data for analysis.

### Suricata
- Create custom rules.
- Monitor traffic in packet capture files.
- Examine `fast.log` and `eve.json` output.