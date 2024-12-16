# Check Outbound Ports

A PowerShell script to test outbound TCP connectivity from your Windows machine. This script dynamically prompts the user to validate outbound communication to specific ports on a target server, helping troubleshoot network configurations and firewall rules.

## Features

- Dynamically prompts the user for:
  - Target server (IP address or hostname).
  - Number of ports to test.
  - Ports to check.
- Validates target server and port inputs.
- Uses PowerShell's built-in `Test-NetConnection` cmdlet for efficient and accurate testing.
- Provides clear results for each port: **open** or **blocked**.
- Includes instructions for simulating blocked ports using Windows Firewall rules.

## Prerequisites

- A Windows system with **PowerShell 5.1** or later installed.
- Optional: Administrator privileges for managing Windows Firewall rules, if we want to test blocked ports.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/check-outbound-ports.git
   .\check-outbound-ports.ps1
   ## Example Output

Here’s an example of what running the script looks like:

```plaintext
Enter the target server (default: portquiz.net): portquiz.net
How many ports would you like to check? 3
Enter port number 1: 80
Enter port number 2: 443
Enter port number 3: 8080

Checking outbound connectivity to portquiz.net...
Outbound connection successful on port 80
Outbound connection successful on port 443
Outbound connection blocked on port 8080
All ports checked!




