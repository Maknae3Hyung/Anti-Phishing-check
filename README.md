# Anti-Phishing-check
This small version of the application works on the URL's and links , scans through the networks such as Google Safe Browsing, VirusTotal, Blacklists. Also scans for Outer URL Analysis, Inner Link Scanning, Network Security Checks and return whether it is safe or not!



🛡️ Advanced Anti-Phishing Python Tool

An advanced anti-phishing tool built in Python, designed to deeply inspect URLs and their inner links using multiple layers of network security, threat intelligence, and malware analysis techniques.  
It performs real-time checks through VirusTotal, Google Safe Browsing, blacklists, and even inner URL verification to ensure comprehensive threat analysis.

🚀 Features

- ✅ **URL Validation & Format Check**
- 🧩 **Inner URL Extraction & Verification**
- 🕵️‍♂️ **Google Safe Browsing API Integration**
- 🧪 **VirusTotal API Analysis**
- 🚫 **Phishing Blacklist Database Check**
- 🔎 **Malware Analysis**
- 📝 **Logging & Reporting**
- 📊 **Threat Summary Output**

📂 Project Structure


AntiPhishingTool/
│
├── main.py                # Main Python script for running the tool
├── requirements.txt       # Dependencies
├── README.md              # Project documentation
├── report.txt             # Final scan report (auto-generated)
├── assets/                # Flowchart and presentation assets
│   └── flowchart.png
│   └── presentation.pptx
└── LICENSE


🧩 Dependencies

Install the dependencies with:

bash
pip install -r requirements.txt


Dependencies include:
- requests
- beautifulsoup4
- google-api-python-client
- virustotal-python
- urllib3

🗝️ Setup & API Keys

1. Google Safe Browsing API
   - Go to [Google Cloud Console](https://console.cloud.google.com/)
   - Create new project
   - Enable **Safe Browsing API**
   - Generate and copy API key

2. VirusTotal API
   - Create an account at [VirusTotal](https://www.virustotal.com/)
   - Get your API key from the dashboard

3. Add your API keys in `main.py`:
```python
GOOGLE_API_KEY = "your_google_api_key"
VIRUSTOTAL_API_KEY = "your_virustotal_api_key"
```

⚙️ How to Use

Run the tool with:

```bash
python main.py
```

- Enter the URL when prompted.
- The tool will perform:
  - Format validation
  - Inner URL crawling and checking
  - Malware and blacklist scanning
- Results will be displayed and logged in `report.txt`.

🧭 Flowchart

![Flowchart](assets/flowchart.png)

📊 Sample Output

```
Checking main URL...
✔️ URL format is valid.
✔️ Safe Browsing: Clean
✔️ VirusTotal: Clean
✔️ Blacklist: Not found
✔️ Inner URLs extracted: 5
✔️ All inner links verified and clean.

Final Verdict: ✅ Safe
```

🎯 Project Goal

To build a robust, layered anti-phishing solution capable of detecting malicious behaviors, suspicious redirects, embedded phishing URLs, and malicious payloads — providing comprehensive protection and detailed analysis reports.

📄 License

This project is licensed under the GNU General Public License v3.0

