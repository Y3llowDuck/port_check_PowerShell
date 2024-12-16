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
- Optional: Administrator privileges for managing Windows Firewall rules.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/check-outbound-ports.git
   cd check-outbound-ports



