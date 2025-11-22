# ubuntu-phoneinfoga

This install allows the investigater to pull the deep details using only a phone number.

<img width="1920" height="1080" alt="Screenshot (3)" src="https://github.com/user-attachments/assets/89233f8c-e528-49eb-8bc5-18e0bb05fc5a" />

This is a there web servie that pull up a deep phone number scan.

<img width="1920" height="1080" alt="Screenshot (4)" src="https://github.com/user-attachments/assets/46d58999-329b-4742-9b92-f5dd2cd5775f" />

# PhoneInfoga on Ubuntu

PhoneInfoga is one of the most advanced tools to scan international phone numbers.  
It performs **basic reconnaissance** to discover information such as the country, carrier, line type, and possible VOIP services. It can also be extended with external APIs to gather more detailed intelligence.

This repository documents how to install and run **PhoneInfoga on Ubuntu**, with usage examples and notes for professional engagements.

---

## 🔧 Installation

1. **Update your system**
   ```bash
   sudo apt update && sudo apt upgrade -y
Install Git and cURL

bash
sudo apt install git curl -y
Clone the PhoneInfoga repository

bash
git clone https://github.com/sundowndev/phoneinfoga.git
cd phoneinfoga
Install dependencies PhoneInfoga runs as a Go application or via Docker.

Go method:

bash
sudo apt install golang -y
go build -o phoneinfoga
Docker method:

bash
sudo apt install docker.io -y
docker pull sundowndev/phoneinfoga:latest
🚀 Usage Examples
Basic scan (Go binary)

bash
./phoneinfoga scan -n +14155552671
Basic scan (Docker)

bash
docker run sundowndev/phoneinfoga scan -n +14155552671
Export results to JSON

bash
./phoneinfoga scan -n +14155552671 -o result.json
Use multiple numbers

bash
./phoneinfoga scan -n +14155552671 -n +442083661177
📂 Output
PhoneInfoga generates reconnaissance reports including:

Country and region information

Carrier and line type (mobile, landline, VOIP)

Possible reputation data (spam reports, leaks)

Exportable formats (JSON, TXT) for client delivery

⚠️ Legal Disclaimer
PhoneInfoga is intended for educational and professional security testing purposes only. Use responsibly and only on targets you have explicit permission to investigate. Unauthorized surveillance or data collection may violate privacy laws.

📚 Resources
PhoneInfoga GitHub Repository

Ubuntu Documentation

Docker Documentation

Code

This is already formatted for GitHub.  

👉 Do you want me to also add a **“Client Engagement Example” section** (like I did for Maigret) to showcase how you used PhoneInfoga professionally, so your repo doubles as a portfolio piece?
