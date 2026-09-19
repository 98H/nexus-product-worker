# Deployment & Operations Guide: Product Worker

## 🚀 Live Access & URLs
- **Live Public Access URL:** [/preview/prod-product-worker-305d2d/](/preview/prod-product-worker-305d2d/)
- **Internal Port:** `0`
- **Runtime Engine:** `python_preview`
- **Deployment Status:** `DEPLOYED / ACTIVE`
- **Timestamp:** `2026-09-19T19:05:09.818801+00:00`

## 🛠️ Management & Service Control
### Launch Command
```bash
python3 app.py --port 0
```

### Health Check Probe
```bash
curl -I http://127.0.0.1:0/
```

### Systemd Service Template
```ini
[Unit]
Description=Product Worker Service
After=network.target

[Service]
Type=simple
WorkingDirectory=/tmp/pytest-of-root/pytest-13/test_supervised_worker_lifecyc0/workspaces/prod-product-worker-305d2d
ExecStart=/usr/bin/python3 /tmp/pytest-of-root/pytest-13/test_supervised_worker_lifecyc0/workspaces/prod-product-worker-305d2d/app.py
Restart=always
RestartSec=3

[Install]
WantedBy=multi-user.target
```

## 🔒 Production Security Protocols
- HTTP-only reverse proxy via Nexus Gateway.
- Dedicated port allocation with zero port conflict.
