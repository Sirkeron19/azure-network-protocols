# Network Security Groups (NSGs) and Inspecting Network Protocols

This project covers the configuration and usage of **Network Security Groups (NSGs)** in cloud environments like **Azure**, as well as the process of **inspecting network protocols** using tools such as **Wireshark** and **tcpdump**.

## Topics Covered:
- **NSGs (Network Security Groups) in Azure**: Configuring and managing rules to control network traffic.
- **Inspecting Network Traffic**: Using Wireshark and tcpdump to capture and analyze network traffic.
  
---

## Screenshots and Visuals:
You will find various screenshots demonstrating the configuration of NSGs, and examples of network protocol inspection.

---

## Getting Started:
1. Clone the repository:
   ```bash
   git clone https://github.com/username/Network-Security-Groups-and-Inspecting-Network-Protocols.git

---

### 4. **NSG Configuration Documentation**

#### 4.1 **NSG_Basics.md**

```markdown
# Understanding Network Security Groups (NSGs)

**Network Security Groups (NSGs)** are a fundamental component for managing network traffic in cloud environments. They allow users to control inbound and outbound traffic to/from resources in Azure.

### Key Features:
- **Inbound and Outbound Rules**: NSGs define rules for both inbound and outbound traffic.
- **Rule Priorities**: Each rule has a priority number; lower numbers take precedence.
- **Protocol Support**: TCP, UDP, and ICMP.

#### Example: Basic NSG Rules
In the example below, an inbound rule is created to allow HTTP traffic on port 80:

| Rule Name | Priority | Protocol | Port Range | Action  | Direction  |
|-----------|----------|----------|------------|---------|------------|
| AllowHTTP | 100      | TCP      | 80         | Allow   | Inbound    |
# Configuring Network Security Groups in Azure

To configure NSGs in Azure, follow these steps:

### Step 1: Creating an NSG
1. Go to the Azure portal.
2. Search for **Network Security Groups**.
3. Click **Add** to create a new NSG.

#### Screenshot Example:
![NSG Creation](../screenshots/nsg_config_screenshot1.png)

### Step 2: Adding Inbound and Outbound Rules
Once the NSG is created, you can add rules:
- Inbound: Allow HTTP (Port 80)
- Outbound: Allow all outbound traffic
# Managing NSG Rules

You can update or remove NSG rules at any time. Here's how:

### Step 1: Modify an NSG Rule
1. Navigate to **Network Security Groups** in Azure.
2. Select the NSG you wish to modify.
3. Under **Settings**, choose **Inbound Security Rules** or **Outbound Security Rules**.
4. Click on the rule to modify or delete.

#### Screenshot Example:
![NSG Rules Management](../screenshots/nsg_config_screenshot2.png)
# Introduction to Wireshark

Wireshark is a powerful tool for capturing and analyzing network traffic. It provides a deep dive into protocols such as HTTP, DNS, FTP, and more.

### Installation:
- Download Wireshark from [here](https://www.wireshark.org/download.html).

### Capturing Network Traffic
To capture network traffic:
1. Open Wireshark.
2. Select the network interface.
3. Click **Start** to begin capturing packets.

#### Screenshot Example:
![Wireshark Capture](../screenshots/wireshark_capture_example1.png)
# Inspecting Network Packets with Wireshark

Wireshark captures packets in real-time. Here's how to inspect them:

### Step 1: Capture Network Traffic
Once traffic is captured, you can filter it based on protocols (e.g., HTTP, DNS).

#### Example:
- Filter by protocol: `http`
- Inspect individual packets to view headers and payloads.

#### Screenshot Example:
![Wireshark Packet Capture](../screenshots/wireshark_capture_example2.png)
# Using TCPDUMP for Network Protocol Inspection

`tcpdump` is a command-line tool for network packet analysis.

### Installation:
- On Linux: `sudo apt install tcpdump`
- On macOS: `brew install tcpdump`

### Basic Usage:
Capture traffic on an interface:
```bash
sudo tcpdump -i eth0

#### 5.4 **Protocol_Analysis_Examples.md**

```markdown
# Protocol Analysis Examples

Here we discuss how to analyze various protocols captured using Wireshark or tcpdump.

### Example 1: Analyzing HTTP Traffic
Inspect HTTP request and response headers to identify web traffic patterns.

### Example 2: Analyzing DNS Traffic
View DNS query and response messages to see the name resolution process.

#### Screenshot Example:
![Wireshark HTTP Capture](../screenshots/wireshark_capture_example3.png)
6. Screenshots Folder
Make sure to include screenshots in your screenshots/ folder. These screenshots should reflect:

NSG creation and rule configuration (Azure portal screenshots).
Packet captures using Wireshark and tcpdump.
Filtered network traffic examples.
7. LICENSE
You can choose an appropriate license for your repository, such as MIT or Apache 2.0, depending on your preference.

Conclusion
This repository provides a comprehensive guide to both Network Security Groups (NSGs) and Network Protocol Inspection. The project includes step-by-step instructions, code snippets, and real-world examples of analyzing network traffic.

How to Contribute
Feel free to fork the project and submit a pull request for improvements. Contributions in the form of new examples, bug fixes, or additional screenshots are welcome!

By following this structure, you should be able to create a well-documented and informative GitHub project on NSGs and Network Protocols. Make sure to add relevant screenshots and test the code to ensure everything works as expected.



