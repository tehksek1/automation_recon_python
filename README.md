🕵️ AI-Recon Tool

**AI-Recon** is a powerful automation tool for reconnaissance tasks including subdomain enumeration, live host checking, port scanning, and CMS/technology fingerprinting.  
Built for bug bounty hunters, penetration testers, and OSINT researchers.

---

## 🚀 Features

- 🔍 Fast **Subdomain Enumeration** using `subfinder`
- 🌐 **Live Host Detection** via parallel HTTP/HTTPS requests
- 🛡️ Fast **Port Scanning** using `nmap`
- 🧠 **Technology & CMS Detection** using `python-Wappalyzer` and `WhatWeb`
- 📁 Organized reporting and summaries saved to your desktop
- ✅ Auto-installs Python modules (unless blocked by PEP 668)

---

## 📸 Screenshot

[1] Finding subdomains for: example.com
[✓] Found 132 subdomains.

[2] Checking live subdomains...
[✓] Live: https://api.example.com [Status: 200]
[✓] Live: http://shop.example.com [Status: 301]

[✓] Starting Nmap scan on 2 hosts...
[→] Scanning api.example.com
[✓] Port 443/tcp open

[+] Starting CMS detection...
[✓] Wappalyzer: Apache, WordPress, PHP

yaml
Copy
Edit

---
<img width="461" height="368" alt="image" src="https://github.com/user-attachments/assets/9a4fd0e5-fd09-4d94-9faf-9441de3c7549" />


## 📦 Requirements

### ✅ Python 3.x (recommended 3.8+)





https://github.com/user-attachments/assets/bf2e6ce0-0eac-4272-b975-db4192e205f3



### 📚 Python Modules

Installed automatically (or use `pip install -r requirements.txt`):
- `requests`
- `python-Wappalyzer`

### 🛠 External Tools (Install Manually)

These are required in your system `PATH`:

```bash
sudo apt install subfinder nmap whatweb
🔧 Installation
🧰 Option 1: Manual Setup
bash
Copy
Edit
git clone https://github.com/yourusername/ai-recon-tool.git
cd ai-recon-tool

# Create virtual environment
python3 -m venv reconenv
source reconenv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run the tool
python3 main.py
⚙️ Option 2: One-Click Setup (Linux)
bash
Copy
Edit
git clone https://github.com/yourusername/ai-recon-tool.git
cd ai-recon-tool
chmod +x setup.sh
./setup.sh
🚀 Usage
Just run the script:

bash
Copy
Edit
python3 main.py
Then enter your target domain when prompted:

text
Copy
Edit
Enter the target domain (e.g. example.com): certinia.com
📁 Output Files
All results are saved to:

javascript
Copy
Edit
~/Desktop/AI-Recon-Results/
Inside this folder, for each domain:

File	Description
example.com_subs.txt	List of discovered subdomains
example.com_live_basic.txt	Live (200/301) HTTP/HTTPS endpoints
example.com_summary.txt	Summary including nmap and tech info
example.com_cms_results.txt	Technologies & CMS detected
nmap/*.txt	Nmap scan results for each live host

🧠 Tech Stack Used
subfinder

nmap

WhatWeb

python-Wappalyzer

⚠️ Notes
PEP 668 Warning: On newer Kali systems, auto-install may be blocked. If so, use:

bash
Copy
Edit
python3 -m venv reconenv && source reconenv/bin/activate
pip install -r requirements.txt
This script is designed for Linux (Kali, Ubuntu, Parrot). It may not work on Windows without WSL or Docker.

🧾 License
This project is licensed under the MIT License – see the LICENSE file for details.

👨‍💻 Author
Hacker Abdul
Bug Bounty Hunter | Python Automation Developer

GitHub: hacker abdul

Twitter: @yourhandle

🌟 Support & Contributions
If you like the project, please ⭐ the repo.
Issues and pull requests are welcome!

yaml
Copy
Edit

---

Would you like this README saved into a file and sent to you? I can also generate the a
