# Task 7: Monitor System Resources Using Netdata

## Objective  
Install **Netdata** and visualize **system** and **application performance metrics** in real-time.

---

## Tools Used  
- **Netdata** (Free, open-source monitoring tool)  
- **Docker**

---


## Steps Performed  

### 1. Run Netdata Using Docker  
```bash
docker run -d --name=netdata -p 19999:19999 netdata/netdata

### 2. Access the browser

Open in your browser:
http://localhost:19999

### 3. Extra Work – Simulating CPU Load

To make Netdata charts show activity, generated temporary CPU load for 30 seconds:

docker run --rm busybox sh -c "yes > /dev/null & sleep 30"