# Traffic-Analysis-Essentials (TryHackMe)

## Network Security & Network Data

The essential concern of **Network Security** focuses on two core concepts: **authentication** and **authorisation**. There are a variety of tools, technologies, and approaches to ensure and measure implementations of these two key concepts and go beyond to provide continuity and reliability. Network security operations contain three base control levels to ensure the maximum available security management.

---

### 🔒 Base Network Security Control Levels:

| Level         | Description |
|---------------|-------------|
| **Physical**  | Physical security controls prevent unauthorised physical access to networking devices, cable boards, locks, and all linked components. |
| **Technical** | Data security controls prevent unauthorised access to network data, like installing tunnels and implementing security layers. |
| **Administrative** | Administrative security controls provide consistency in security operations like creating policies, access levels and authentication processes. |

---

## 🧭 Core Approaches & Elements in Network Security

There are two main approaches and multiple elements under these control levels. The most common elements used in network security operations are explained below.

### 🔑 The Main Approaches:

| Access Control | Threat Control |
|----------------|----------------|
| The starting point of Network Security. It is a set of controls to ensure authentication and authorisation. | Detecting and preventing anomalous/malicious activities on the network. It contains both internal (trusted) and external traffic data probes. |

---

### 🛡️ Key Elements of **Access Control**:

- **Firewall Protection**  
  Controls incoming and outgoing network traffic with predetermined security rules. Designed to block suspicious/malicious traffic and application-layer threats while allowing legitimate and expected traffic.

- **Network Access Control (NAC)**  
  Controls the devices' suitability before access to the network. Designed to verify device specifications and conditions are compliant with the predetermined profile before connecting to the network.

- **Identity and Access Management (IAM)**  
  Controls and manages the asset identities and user access to data systems and resources over the network.

- **Load Balancing**  
  Controls the resource usage to distribute (based on metrics) tasks over a set of resources and improve overall data processing flow.

- **Network Segmentation**  
  Creates and controls network ranges and segmentation to isolate the users' access levels, group assets with common functionalities, and improve the protection of sensitive/internal devices/data in a safer network.

- **Virtual Private Networks (VPN)**  
  Creates and controls encrypted communication between devices (typically for secure remote access) over the network (including communications over the internet).

- **Zero Trust Model**  
  Suggests configuring and implementing the access and permissions at a minimum level (providing access required to fulfil the assigned role).  
  > _Mindset: "Never trust, always verify"._

---

### 🧨 Key Elements of **Threat Control**:

- **Intrusion Detection and Prevention (IDS/IPS)**  
  Inspects the traffic and creates alerts (IDS) or resets the connection (IPS) when detecting an anomaly/threat.

- **Data Loss Prevention (DLP)**  
  Inspects the traffic (performs content inspection and contextual analysis of the data on the wire) and blocks the extraction of sensitive data.

- **Endpoint Protection**  
  Protecting all kinds of endpoints and appliances that connect to the network by using a multi-layered approach like encryption, antivirus, antimalware, DLP, and IDS/IPS.

- **Cloud Security**  
  Protecting cloud/online-based systems resources from threats and data leakage by applying suitable countermeasures like VPN and data encryption.

- **Security Information and Event Management (SIEM)**  
  Technology that helps threat detection, compliance, and security incident management, through available data (logs and traffic statistics) by using event and context analysis to identify anomalies, threats, and vulnerabilities.

- **Security Orchestration Automation and Response (SOAR)**  
  Technology that helps coordinate and automates tasks between various people, tools, and data within a single platform to identify anomalies, threats, and vulnerabilities.  
  Also supports vulnerability management, incident response, and security operations.

- **Network Traffic Analysis & Network Detection and Response**  
  Inspecting network traffic or traffic capture to identify anomalies and threats.

---

## ⚙️ Typical Network Security Management Operation

| **Deployment** | **Configuration** | **Management** | **Monitoring** | **Maintenance** |
|----------------|-------------------|----------------|----------------|-----------------|
| • Device and software installation | • Feature configuration | • Security policy implementation | • System monitoring | • Upgrades |
| • Initial configuration | • Initial network access configuration | • NAT and VPN implementation | • User activity monitoring | • Security updates |
| • Automation |  | • Threat mitigation | • Threat monitoring | • Rule adjustments |
|  |  |  | • Log and traffic sample capturing | • Licence management |
|  |  |  |  | • Configuration updates |


---

## 📡 Managed Security Services (MSS)

Not every organisation has enough resources to create dedicated groups for specific security domains. Budget, employee skillset, and organisation size could determine how security operations are handled.

At this point, **Managed Security Services (MSS)** come in to fulfil the required effort to ensure/enhance security needs. These are services outsourced to **Managed Security Service Providers (MSSPs)**. 

Most MSS are:
- Time and cost-effective
- In-house or outsourced
- Easy to engage
- Simplifies management

### Common MSS Elements:

- **Network Penetration Testing**  
  Assessing network security by simulating external/internal attacker techniques to breach the network.

- **Vulnerability Assessment**  
  Assessing network security by discovering and analysing vulnerabilities in the environment.

- **Incident Response**  
  An organised approach to addressing and managing a security breach. It contains a set of actions to identify, contain, and eliminate incidents.

- **Behavioural Analysis**  
  Analysing system and user behaviours, creating baselines and traffic profiles for specific patterns to detect anomalies, threats, vulnerabilities, and attacks.

---

## 📊 Traffic Analysis / Network Traffic Analysis

Traffic Analysis is a method of intercepting, recording/monitoring, and analysing network data and communication patterns to detect and respond to system health issues, network anomalies, and threats.

The network is a rich data source, so traffic analysis is useful for:
- **Operational matters** (e.g., system availability, performance)
- **Security issues** (e.g., anomaly & threat detection)

Traffic analysis is part of multiple disciplines:

1. **Network Sniffing and Packet Analysis (Wireshark)**
2. **Network Monitoring (Zeek)**
3. **Intrusion Detection and Prevention (Snort)**
4. **Network Forensics (NetworkMiner)**
5. **Threat Hunting (Brim)**

---

### 🧪 Two Main Techniques in Traffic Analysis:

| Flow Analysis | Packet Analysis |
|---------------|-----------------|
| Collecting data/evidence from networking devices. Provides statistical results through summaries without in-depth packet inspection. | Collects all network data. Deep Packet Inspection (DPI) to detect and block malicious packets. |
| ✅ Easy to collect and analyse | ✅ Provides full packet details to get the root cause |
| ❌ Doesn't provide full packet-level detail | ❌ Requires time and technical skillset |

---
