# Deployment & Operations Guide: Product Worker

## 🚀 Live Access URLs
- **Public Preview URL:** [https://river-alternatives-isolated-parker.trycloudflare.com/preview/prod-product-worker-305d2d/](https://river-alternatives-isolated-parker.trycloudflare.com/preview/prod-product-worker-305d2d/)
- **Local Gateway Path:** [/preview/prod-product-worker-305d2d/](/preview/prod-product-worker-305d2d/)
- **Internal Port:** `8104`
- **Process PID:** `587238`
- **Runtime Engine:** `python_preview`
- **Health Status:** `HEALTHY (HTTP 200)`
- **Deployed Timestamp:** `2026-09-19T19:05:13.643361+00:00`

## 📋 Execution Command
```bash
/usr/local/lib/hermes-agent/venv/bin/python3 app.py --port 8104
```

## 🩺 Health Check Verification
```bash
curl -I http://127.0.0.1:8104/
```

## 📜 Live Deployment Logs
Logs are stored at `/tmp/pytest-of-root/pytest-13/test_supervised_worker_lifecyc0/workspaces/prod-product-worker-305d2d/logs/deploy.log`.
