# ShareFile RCE (CVE-2023-24489)

This is a Python script that exploits a remote code execution vulnerability in the ShareFile application (CVE-2023-24489). This vulnerability allows an attacker to execute arbitrary commands on the target system.

## Usage

To use the script, follow the instructions below:

1. Install the required dependencies:
   ```bash
   pip install requests
   ```

2. Run the script with the desired options:

   ```bash
   python cve.py --host <target URL> [--windows | --linux] [--cmd <command>] [--mass-check <wordlist file>]
   ```

   The available options are:

   - `--host`: Specifies the URL of the target to exploit.
   - `--windows`: Specifies that the target system is running Windows.
   - `--linux`: Specifies that the target system is running Linux.
   - `--cmd`: Specifies the command to execute during exploitation (optional).
   - `--mass-check`: Specifies the path to the wordlist file for mass checking (optional).

   Note: Either the `--host` option or the `--mass-check` option must be provided.

## References
[https://blog.assetnote.io/2023/07/04/citrix-sharefile-rce/](https://blog.assetnote.io/2023/07/04/citrix-sharefile-rce/)

## Disclaimer

This script is provided for educational purposes only. You are responsible for using this script in compliance with applicable laws and regulations. The author assumes no responsibility for any unauthorized or malicious use of this script. You should only use this script on systems that you have proper authorization to access. Using this script on unauthorized systems is strictly prohibited and may result in legal consequences. Use it responsibly and at your own risk.