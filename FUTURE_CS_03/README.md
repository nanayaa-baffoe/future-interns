Task 3: Wi-Fi Security Assessment – Cybersecurity Internship

This repository documents Task 3 of the Future Interns Cybersecurity Track (Track Code: CS).

Objective:
To perform a security assessment of a home Wi-Fi network using scanning tools, identify potential vulnerabilities, and provide recommendations for improving wireless network security.

Tools Used:
- Nmap (Network Mapper) – for scanning connected devices and open ports
- Windows 10 Command Prompt
- Router Admin Interface (to review Wi-Fi configuration)
- (Optional) Wireshark – for analyzing traffic

Network Details:
- Device IP: 192.168.24.184
- Router IP: 192.168.24.137

What Was Done:
1. Scanned the local network for active devices using nmap -sn
2. Scanned the router for open ports using nmap -sV
3. Logged into the router admin page to review:
   - Encryption type
   - Password strength
   - WPS status
   - List of connected devices
4. Documented all findings in a detailed report
5. Made security recommendations based on observations

Results Summary:

Scan Type     | Result
--------------|--------------------------------------------------
Device Scan   | Only one device found (intern's own PC)
Port Scan     | Only port 53 (DNS) open on the router
Router Config | Reviewed by intern manually

Repository Structure:
FUTURE_CS_03/
├── README.md
├── WiFi_Security_Report.docx
├── screenshots/
│   ├── ipconfig_output.png
│   ├── nmap_device_scan.png
│   ├── nmap_port_scan.png
│   └── router_settings.png
├── data/
│   ├── port_scan.txt


Recommendations:
- Enable WPA2 or WPA3 encryption
- Disable WPS if not in use
- Use a strong Wi-Fi password (12+ characters)
- Regularly check for unknown connected devices
- Keep router firmware up to date

Status:
Task Completed
Submitted for Certification and LoR
