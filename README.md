# User Manual for ZapFind Tool

ZapFind Tool User Manual

Version: 1.0

Date: December 20, 2024

## 1. Introduction

ZapFind is a versatile security scanning tool designed for ethical hackers and cybersecurity professionals. It integrates powerful scanning utilities such as Nmap and Nikto, enabling efficient detection of vulnerabilities and open ports in target systems.

---

## 2. Legal Disclaimer

This tool is intended strictly for authorized and ethical use. Unauthorized scanning of systems may violate laws and is strictly prohibited.

**Warning:** Users are responsible for ensuring compliance with applicable laws and obtaining proper permissions before using this tool.

---

## 3. System Requirements

- **Operating System:** Linux
- **Dependencies:**
  - Python 3.6 or higher
  - Installed utilities:
    - Nmap
    - Nikto
  - Python Libraries:
    - `rich`
    - `tqdm`

---

## 4. Installation Instructions

1. Clone the repository or download the script.
     ```bash
     git clone https://github.com/Shawky0-0/ZapFind.git
   ```
3. Install the required Python libraries:
   ```bash
   pip install rich tqdm
   ```
4. Ensure Nmap and Nikto are installed and accessible from the command line.
5. Run the script using:
   ```bash
   python zapfind
   ```

---

## 5. Features

- **Target Validation:** Ensures valid IP addresses or domain names.
- **Port Scanning:** Allows users to specify or scan all ports.
- **Concurrent Scanning:** Runs Nmap and Nikto scans simultaneously.
- **Progress Indicators:** Displays scanning progress.
- **Report Generation:** Saves detailed results to a file.
- **Help Menu:** Provides guidance on tool usage.

---

## 6. Usage Instructions

### 6.1 Starting the Tool

1. Launch the tool by executing:
   ```bash
   python zapfind
   ```
2. Read the legal disclaimer displayed at the start.

### 6.2 User Input

- **Help Menu:** Enter `yes` or `no` when prompted to display the help message.
- **Target Selection:** Input a valid IP address or domain name.
- **Scan Type Selection:**
  - [1] Nmap Scan
  - [2] Nikto Scan
  - [3] Both Nmap and Nikto
- **Ports Input:** (Optional) Specify ports as comma-separated values (e.g., `22,80,443`) or leave blank to scan all ports.

### 6.3 Viewing Results

- Scan results are displayed in a formatted panel.
- Results are saved automatically to a `scan_reports` folder with a timestamped filename.

---

## 7. Example Workflow

1. Start the tool.
2. Input a target domain, e.g., `example.com`.
3. Select scan type `3` to run both Nmap and Nikto scans.
4. Wait for the progress bar to complete.
5. View the results displayed and saved to a file.

---

## 8. Error Handling

- **Invalid Target Input:**
  - If the input does not match IP or domain patterns, the tool will prompt for re-entry.
- **Tool Unavailability:**
  - If Nmap or Nikto is missing, the tool will notify the user.
- **Scan Failures:**
  - Errors during scanning will be logged in the console output.

---

## 9. Help Menu Content

```plaintext
ZapFind Tool Help:

This tool allows you to perform security scans using Nmap and Nikto.

Usage Instructions:
1. Enter the target IP address or domain.
2. Choose the type of scan:
   - Nmap scan: Scans for open ports and services.
   - Nikto scan: Scans for vulnerabilities on web servers.
   - Both: Runs both scans sequentially.
3. View the results and save them to a file.

Disclaimer:
- This tool is for educational and authorized testing purposes only.
- Unauthorized use is strictly prohibited.
```

---

## 10. Limitations

- Requires administrative privileges to run certain scans.
- Dependent on external tools (Nmap, Nikto).
- Results accuracy depends on network conditions and tool configurations.

---

## 11. Troubleshooting

| Issue                       | Solution                                                             |
| --------------------------- | -------------------------------------------------------------------- |
| Nmap or Nikto not installed | Ensure tools are installed and accessible via command line.          |
| Invalid target input        | Verify and re-enter a valid IP or domain name.                       |
| Permission errors           | Run the script with appropriate user permissions.                    |
| Missing dependencies        | Install missing Python libraries using `pip install <library_name>`. |

---

## 12. Contact Information

For support or feedback, contact:

- **Email:** [shawkymohamd5577@gmail.com](mailto\:shawkymohamd5577@gmail.com)
- LinkedIn: [www.linkedin.com/in/shawky-mohamed-303944289](http://www.linkedin.com/in/shawky-mohamed-303944289)

