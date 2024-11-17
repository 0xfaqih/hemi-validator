### Install

```
curl -O https://raw.githubusercontent.com/0xfaqih/hemi-validator/refs/heads/main/hemi.sh && chmod +x hemi.sh && ./hemi.sh
```
### Restart Node and Check Log

```
sudo journalctl -u heminetwork -f
```

```
sudo systemctl restart heminetwork
```

### Delete Node

```
sudo systemctl stop heminetwork && \
sudo systemctl disable heminetwork && \
sudo rm /etc/systemd/system/heminetwork.service && \
sudo systemctl daemon-reload
```
