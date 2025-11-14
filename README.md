# 🚨 Azure Honeypot & Global Attack Map  
### *Cloud SOC | Threat Telemetry | KQL Detection Engineering*

This project simulates a real-world SOC workflow by deploying a honeypot in Microsoft Azure, capturing attacker traffic, enriching logs with geolocation data, and visualizing live attacks on a world map using an Azure Sentinel workbook.

It demonstrates skills in threat detection, cloud security, log analysis, watchlists, and KQL.

---
![Azure](https://img.shields.io/badge/Microsoft%20Azure-0089D6?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Sentinel](https://img.shields.io/badge/Azure%20Sentinel-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![KQL](https://img.shields.io/badge/KQL-4B275F?style=for-the-badge)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-FF0000?style=for-the-badge)

---

## ⚙️ Technologies Used
- **Microsoft Azure:** VM, VNet, NSG/Firewalls, Workspace, Azure Sentinel  
- **Kusto Query Language (KQL)**  
- **Azure Workbooks & Watchlists**  
- **Windows Event Logging**  
- **Threat Telemetry & Attack Visualization**  

---

## 🗂️ Project Workflow

### 🔹 **1. Cloud Infrastructure Setup**
- Created a resource group  
- Built a VNet + subnets  
- Deployed a Windows honeypot VM  

### 🔹 **2. Exposing the Honeypot**
- Disabled Windows Firewall  
- Added “Allow Any” rule in NSG  
- Confirmed public internet reachability  

### 🔹 **3. Log Ingestion & Sentinel Integration**
- Added Sentinel to Workspace
- Installed Sentinel agent on VM
- Verified logs flowing into Sentinel  

### 🔹 **4. Threat Detection (KQL)**
- Queried brute-force attempts  
- Extracted attacker IPs  
- Filtered 4625 failed-logins 

### 🔹 **5. Threat Intelligence Enrichment**
- Built a Watchlist mapping IP → Geolocation
- Joined logs with geolocation metadata  

### 🔹 **6. Attack Map Workbook**
- Built a real-time world map  
- Plotted attacker coordinates  
- Visualized global login failures  

---

## 📸 Screenshots

### **Created Resource Group**  
![Created Resource Group](Azure-Honeypot-Sentinel-Lab/screenshots/created_resource_group.png.png)

### **Created Virtual Network**  
![Created Virtual Network](Azure-Honeypot-Sentinel-Lab/screenshots/created_virtual_network.png.png)

### **Created Honeypot VM**  
![Created Honeypot](Azure-Honeypot-Sentinel-Lab/screenshots/created_honeypot.png.png)

### **Allow Any Rule in NSG**  
![Allow All Traffic](Azure-Honeypot-Sentinel-Lab/screenshots/add_allow_all_traffic_rule_to_v-firewall.png.png)

### **Disabled Windows Firewall on Honeypot**  
![Turned Off Firewall](Azure-Honeypot-Sentinel-Lab/screenshots/turned_off_honeypot_firewall.png.png)

### **Ping: Confirm Public Reachability**  
![Ping Test](Azure-Honeypot-Sentinel-Lab/screenshots/pinged_honeypot_to_ensure_it_is_reachable_from_the_public_internet.png.png)

### **Queried Failed Login Attempts**  
![Failed Logins](Azure-Honeypot-Sentinel-Lab/screenshots/searched_for_failed_logins_in_honeypot_log.png.png)

### **Added Sentinel to Workspace**  
![Sentinel Added](Azure-Honeypot-Sentinel-Lab/screenshots/added_sentinel_to_log_analysis_workspace.png.png)

### **Installed Sentinel Agent**  
![Sentinel Agent](Azure-Honeypot-Sentinel-Lab/screenshots/installed_sentinel_agent_on_honeypot.png.png)

### **Filtered Logs with KQL**  
![Filtered Logs](Azure-Honeypot-Sentinel-Lab/screenshots/filtered_logs_using_KQL.png.png)

### **Created Watchlist**  
![Watchlist](Azure-Honeypot-Sentinel-Lab/screenshots/created_watchlist_in_sentinel.png.png)

### **Attack Map Workbook**  
![Attack Map](Azure-Honeypot-Sentinel-Lab/screenshots/created_attack_map_workbook_to_show_geolocation_of_attackers.png.png)

### **Attack Map JSON Configuration**  
![Attack Map JSON](Azure-Honeypot-Sentinel-Lab/screenshots/attach_map_with_json.png.png)

