# Network Scanner

## Introduction

This script, `network_scanner.py`, is a simple tool for scanning a target IP or IP range and discovering the corresponding MAC addresses of devices on the network. It utilizes the Scapy library for crafting and sending ARP requests.

## Usage

### Prerequisites

Make sure you have Scapy installed. You can install it using:

```bash
pip install scapy
```

### Running the Script

1. Clone the repository:

```bash
git clone https://github.com/TUR14CUS/Network-Scanner.git
cd Network-Scanner
```

2. Run the script with the following command:

```bash
python network_scanner.py -t [TARGET_IP_OR_RANGE]
```

Replace `[TARGET_IP_OR_RANGE]` with the IP address or IP range you want to scan.

## Options

- `-t, --target`: Specifies the target IP address or IP range.

## Example

```bash
python network_scanner.py -t 192.168.1.1/24
```

## Output

The script will display a list of devices on the network along with their IP addresses and MAC addresses.

```
IP                MAC Address
------------------------------------
192.168.1.1       00:1a:2b:3c:4d:5e
192.168.1.2       00:aa:bb:cc:dd:ee
192.168.1.3       00:11:22:33:44:55
...
```

## Disclaimer

This tool is intended for educational and informational purposes only. Ensure that you have the necessary permissions before scanning any network.

