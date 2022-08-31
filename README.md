# Script to run command on al Virtual Machine Scale Sets (Azure)
## Requirements
* You need to have AZ cli installed
* You need to be logged in into Azure
* You need to know your Tenant ID

## Usage
```shell
python3 main.py --command "nslookup www.google.com" --tenant <tenant-id> --filter <subscription-id>
```

### Commands
```shell
python3 main.py --command "sudo echo FallbackDNS=168.63.129.16 >> /etc/systemd/resolved.conf; sudo systemctl restart systemd-resolved.service; cat /etc/resolv.conf; nslookup www.google.com" --tenant <tenant-id> --filter <subscription-id>
```
