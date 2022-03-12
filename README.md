## Description
This repository contains a collection of systemd service files as well as systemd timers.

---

## Setup

### Installation of service files
Copy the appropriate files to /etc/systemd/system/:
```bash
cp <service_or_timer_file> /etc/systemd/system/
```

### Make file executable
Make file executable to make systemd able to execute it:
```bash
chmod 755 <service_or_timer_file>
```

### Reload systemd daemon
Reload systemd daemon in order to register new files and changes:
```bash
systemctl daemon-reload
```

---

## Optional

### Start and enable timer
```bash
systemctl enable <timer_file> --now
```

### Enable service to run at boot
```bash
systemctl enable <service_file>
```

### Manually start service
```bash
systemctl start <service_file>
```
