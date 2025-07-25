# 🚀 blasturl

**blasturl** is a blazing-fast and developer-friendly CLI tool for HTTP/HTTPS load testing.  
It helps you simulate traffic to any endpoint, measure performance, and view real-time latency charts — all from your terminal.

---

## how to use?

#### run:  ***npm i blasturl*** 

Current version: 1.0.0

---

## 🌟 Features

- 🔥 Simple & modern CLI
- 📦 Supports both request count and duration modes
- 📉 Real-time latency tracking and ASCII charts
- 📊 Histogram of response times
- 🧪 Error breakdown with status codes and timeouts
- ✅ Works with GET, POST, PUT, DELETE, etc.
- 🛡️ Built-in safety limits

---

## ⚙️ Options

```bash
--url, -u           Target URL to test (required)
--requests, -r      Total number of requests to send (default: 100)
--duration          Duration of test in seconds (overrides --requests)
--concurrency, -c   Number of concurrent requests (default: 10)
--method, -m        HTTP method to use (GET, POST, PUT, DELETE, etc.) [default: GET]
--header, -H        Custom headers (e.g. -H "Authorization: Bearer token")
--data, -d          Request body payload (for POST/PUT requests)

# Example:
blasturl \
  --url https://your-api.com/endpoint \
  --method POST \
  --requests 200 \
  --concurrency 20 \
  --header "Content-Type: application/json" \
  --header "Authorization: Bearer <token>" \
  --data '{"key": "value", "flag": true}'
