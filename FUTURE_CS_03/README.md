# FUTURE_CS_03 – Wi-Fi Security Assessment  

This project was part of the **Cybersecurity Track (CS)** during the Future Interns Internship.  

---

## 🎯 Objective  
To perform a **security assessment of a home Wi-Fi network** by:  
- Scanning connected devices.  
- Identifying open ports on the router.  
- Reviewing Wi-Fi configuration for vulnerabilities.  
- Providing recommendations for improvement.  

---

## 🛠️ Tools Used  
- **Nmap** → Network & port scanning  
- **Windows 10 Command Prompt**  
- **Router Admin Interface** → Reviewing configuration  
- *(Optional)* Wireshark → Traffic analysis  

---

## 🌐 Network Details  
- Device IP: `192.168.24.184`  
- Router IP: `192.168.24.137`  

---

## 🔎 What Was Done  
- Ran device discovery using `nmap -sn`  
- Performed port scanning on router with `nmap -sV`  
- Logged into router admin panel to review:  
  - Encryption type  
  - Password strength  
  - WPS status  
  - Connected devices list  
- Documented all findings and provided security recommendations  

---

## 📊 Results Summary  

| Scan Type      | Result                                |
|----------------|---------------------------------------|
| Device Scan    | Only one device found (intern's PC)   |
| Port Scan      | Only port 53 (DNS) open on router     |
| Router Config  | Reviewed manually                     |

---

## 📂 Project Structure  
