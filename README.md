
# System Health Check Script

This Python script is designed to monitor and check the system's health by performing various checks on the machine's disk space, CPU usage, network connectivity, and reboot status. If any of the checks fail, it will display an appropriate message and exit with a non-zero status. This can be used as part of automated monitoring or alerting systems to ensure that the system is running smoothly.

## Features:
- **Disk Space Check**: Verifies if the root partition has sufficient free space (at least 2GB and 10% free).
- **CPU Usage Check**: Monitors the CPU load and raises a warning if the CPU usage exceeds 75%.
- **Reboot Check**: Detects if there is a pending system reboot.
- **Network Connectivity Check**: Tests if the system is able to resolve Google's URL (used to check for network connectivity).

## Requirements:
- Python 3.x
- `psutil` library for CPU and disk usage information.
- Works for Linux based systems

You can install `psutil` using pip:


## How It Works:
1. The script checks the system for issues in the following areas:
   - Pending reboot
   - Full root partition
   - Network connectivity (Google URL resolution)
   - High CPU load
2. If any issue is found, the script prints the corresponding message.
3. If no issues are found, it prints "Everything ok" and exits successfully.
4. If any issues are found, the script exits with a status code of 1, indicating failure.

## Usage:
Simply run the script in your terminal:


