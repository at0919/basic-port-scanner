# 👁️ VigilantEye Port Scanner

A simple and efficient network port scanner built in Python using the `socket` library. This tool scans a target host for open ports and helps identify potential services running on a system.

---

## Features
- Scan common ports quickly
- Identify open ports on a target host
- Clean and structured console output
- Lightweight and easy to use
- Built using core Python (no external dependencies)

---

## Tech Stack
- **Language:** Python  
- **Library:** socket
- **NOTE:** As more things are added, the tech stack is likely to change. This is just a low-level implementation for now.

---

## How It Works
The scanner attempts to establish a TCP connection to a list of specified ports on a target IP or domain. If a connection is successful, the port is marked as **OPEN**, helping identify active services on the system.

---

## Installation & Setup
1. Clone the repository:
```bash
git clone https://github.com/yourusername/port-scanner.git
cd port-scanner
```
2. Ensure Python is installed:
```bash
python --version
```
3. (Optional but recommended) Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate # On Windows: venv\Scripts\activate
```

---

## Usage
1. Run the script:
```bash
python scanner.py
```
Then enter a target (IP or Domain) when prompted.

---

## Example Output
```text
--------------------------------------------------
-- [X] HOST: example.com
-- [X] SCANNING TARGET: 93.184.216.34
-- [X] Scan Started At: 2026-03-17 12:00:00
--------------------------------------------------

TARGET: 93.184.216.34 | PORT: 80  | CONNECTION: OPEN
TARGET: 93.184.216.34 | PORT: 443 | CONNECTION: OPEN
```

---

## ⚠️ Disclaimer
This tool is built STRICTLY for educational and ethical use and is part of my learning journey in Cybersecurity.
  - Only scan systems that you own or have explicit permission to test
  - Do not use this tool against networks without authorization
  - Misuse of this tool may violate laws and regulations

I am not responsible for any misuse or damage caused by this project.

---

## Future Improvements
This project will likely continue to evolve as I learn more about networking and Cybersecurity.
  - Support custom port ranges and targeted scans
  - Export results to CSV for reporting and analysis
  - Implement banner grabbing for service detection
  - Add smarter detection (open vs. filtered vs. closed ports)
  - Build a CLI interface with flags (`-t`, `-p`, `--threads`)
  - Create a simple web dashboard to visualize scan results
  - Improve error handling and timeout controls
