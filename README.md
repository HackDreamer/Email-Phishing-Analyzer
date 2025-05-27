# Email-Phishing-Analyzer
📧 Email Phishing Analyzer (Python)

   A lightweight command-line tool to analyze email content for potential phishing indicators. This analyzer checks for spoofed domains, suspicious URLs, urgency language, and common 
   phishing grammar errors.

🚀 Features

  - ✅ Detect spoofed/suspicious sender domains: Identifies email addresses that may be impersonating legitimate sources.

  - 🔗 Extract and analyze URLs: Scans embedded links for mismatches and hidden threats.

  - ⚠️ Identify urgency or threatening language: Detects phrases commonly used in phishing attempts to create a sense of urgency.

  - 📝 Spot common spelling and grammar mistakes: Flags errors typically found in phishing emails.

  - 🧠 Simple, rule-based engine: No machine learning required; utilizes a straightforward heuristic approach.

  - 📋 CLI tool for fast and interactive use: Designed for quick analysis through the command line.


🧰 Requirements

  - Python 3.x

  - No external libraries needed (uses Python standard library)

🛠️ How to Use

1.Clone the repository or download the script.
  
2.Run the script:
  ```
   python email_phishing_analyzer.py
```
 3.Paste the full email content when prompted. Press Enter twice to analyze.

🔍 Example Output
```python

  📧 Paste the full email content below (press Enter twice to finish):

  From: support@secure-paypal.com
  Subject: Urgent! Your account has been suspended!
  Click here to verify: http://paypal-secure.com/verify

  === Phishing Email Analyzer ===
  [+] Spoofed sender domain detected: Yes
  [+] URLs found: ['http://paypal-secure.com/verify']
  [+] Mismatched/malicious URLs: ['http://paypal-secure.com/verify']
  [+] Urgent language found: ['your account has been suspended']
  [+] Spelling/grammar issues found: None
  🚨 Potential phishing email detected!
```
📁 File Structure

  - `email_phishing_analyzer.py`

  - `README.md`

  - `Sample phishing email.txt`

✨ Customization

 You can update these lists in the script to adapt detection:

- SPOOFED_DOMAINS: Add known fake domains.

- URGENT_PHRASES: Expand with additional phishing phrases.

- COMMON_ERRORS: Add frequent spelling/grammar issues.

📌 Disclaimer

  This tool uses basic rule-based heuristics and does not guarantee 100% accurate detection. For enterprise-grade solutions, consider machine learning and threat intelligence 
  integrations.
