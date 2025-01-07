# HAProxy Load Balancer Setup Guide

This guide demonstrates how to install, configure, and use HAProxy as a load balancer for HTTP traffic on a Linux system.


## **Installation**

1. Update system packages:
```bash
sudo apt update && sudo apt upgrade -y
```
2. Install HAProxy:   
```bash
sudo apt install haproxy -y
```
3.Verify installation:
```bash
haproxy -v
```

## **Configuration**
Copy config file in :
```bash
sudo nano /etc/haproxy/haproxy.cfg
```

## **Starting HAProxy**

1.	Start HAProxy:
```bash
sudo systemctl start haproxy
```
2.Enable HAProxy to start on boot:
```bash
sudo systemctl enable haproxy
```
3.Verify the status of the HAProxy service:
```bash
sudo systemctl status haproxy
```
## **LOGS**
```bash
tail -f /var/log/haproxy.log
```
