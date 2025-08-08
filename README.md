# Constant Ping

Some VPN servers and clients have issues keeping the tunnel established and installed.  In some cases, a constant never ending ping across the tunnel has been able to help keep that tunnel online and running.

# Installation

1. Clone the Repo
2. Run installation command

```
# ./constant-ping -i
```

3. Modify configuration

```
$ sudo vim /etc/constant-ping/main.conf

# Configuration file for constant-ping
######################################
# Target Host to Ping
TARGET_HOST="127.0.0.1"

# Time Interval in seconds to ping
PING_INTERVAL=5
```

4. Start/Restart the service

```
# systemctl restart constant-ping.service
# systemctl status constant-ping.service
```