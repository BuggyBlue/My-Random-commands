# My Recon Tool that i made with AI
# Reconnaissance Assistant

A minimal Python tool to automate initial reconnaissance for a **single domain** – intended **solely for use in authorized security assessments**.

## Features

- Asks for a domain name (or takes as argument).
- Runs lightweight recon commands:
  - `whois <domain>`
  - `nslookup <domain>`
  - `nmap` service scan on ports 80 and 443
- Saves each command's raw results to separate files in a `results/` directory.
- Generates a short, human-readable summary report from outputs.

---

## Ethical Use Limitation

> **IMPORTANT:**  
> This tool must **only** be used on domains/systems where you have **explicit, written permission** to test.  
> Unauthorized use is illegal and unethical.

---

## Dependencies

- **Python 3.7+**
- System utilities available in your `PATH`:
  - [`whois`](https://linux.die.net/man/1/whois)
  - [`nslookup`](https://linux.die.net/man/1/nslookup)
  - [`nmap`](https://nmap.org/)

*On Windows, you may need to install these tools separately.*

---

## Usage

1. **Install dependencies** if needed (see above).

2. **Run the script**:

  
   python recon_assistant.py example.com
      or simply:

  
   python recon_assistant.py
      (and you will be prompted for a domain)

3. **Results** will be stored in the `results/` folder.  
   A summary report will be shown in your terminal.

4. For help, use:

  
   python recon_assistant.py --help
   ---

## Disclaimer

- This tool is for **authorized testing only**.
- The authors are **not responsible for misuse**.
