Quick setup guide for A206(For IOAI 2026/07/04 only)
===
# Install ansible
```bash
sudo apt update && sudo apt install ansible -y
```
# Test network
```bash
ansible A206 -i A206.yaml -m win_ping
```
# Start uwf
```bash
ansible-playbook -i A206.yaml start-uwf.yaml
```
# Start blocking
```bash
ansible-playbook -i A206.yaml start-ioai-lockdown.yaml
```
# End
No worries, uwf will do the work
