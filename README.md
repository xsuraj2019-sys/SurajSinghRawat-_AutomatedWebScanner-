Automated Web Scanner
Project Overview
This project is an Automated Web Scanner developed as part of the IBM SkillsBuild Cyber Security BootCamp 2026. It is a Python-based tool designed to audit websites for missing HTTP security headers and overly permissive Cross-Origin Resource Sharing (CORS) configurations.
Technologies Used
Language: Python 3.x
Libraries: requests (for handling HTTP GET requests to target websites)
Project Description
Many common web vulnerabilities (like Clickjacking, XSS, and MIME-sniffing) can be mitigated by configuring web servers to return specific security headers. This tool automates the process of checking a target URL for the presence of these crucial headers:
Strict-Transport-Security (HSTS)
Content-Security-Policy (CSP)
X-Frame-Options
X-Content-Type-Options
Additionally, it checks for insecure CORS policies by looking for the Access-Control-Allow-Origin: * header, which can expose site data to unauthorized domains.
Setup and Run Instructions
Prerequisites: Ensure you have Python installed on your computer.
Install Dependencies: Open your terminal or command prompt and run the following command to install the required library: pip install -r requirements.txt
Run the Script: Execute the Python script using the following command: python YourName_AutomatedWebScanner.py
Usage: When prompted, enter a website URL (e.g., example.com or https://google.com) and press Enter to view the security audit results.
Key Information / Dataset
Dataset: This project performs live, active checks against user-supplied URLs. It does not require a static, pre-downloaded dataset.
Disclaimer: This tool relies entirely on publicly available HTTP response headers and performs no intrusive scanning or exploitation.
