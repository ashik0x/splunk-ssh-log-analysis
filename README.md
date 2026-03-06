# Log Analysis & Threat Detection using Splunk SIEM

## 📌 Project Overview
This project demonstrates hands-on security monitoring and threat detection using **Splunk SIEM** by analyzing **SSH authentication logs**. The goal is to identify brute-force attacks, unauthorized access attempts, and suspicious login behavior.

## 🔍 Use Case
- Detect SSH brute-force attacks
- Identify unauthorized and suspicious login attempts
- Monitor SSH access trends and attacker IPs
- Generate real-time security alerts

## 🛠️ Tools & Technologies
- Splunk SIEM
- SPL (Search Processing Language)
- Linux SSH Authentication Logs
- Security Monitoring & Incident Detection

## 📊 Data Ingestion
- Ingested SSH authentication logs using:
  - Custom Index: `ssh_logs`
  - Source Type: `linux_secure`

## 🧠 Detection Techniques
- Correlated multiple failed SSH login attempts within defined time windows
- Identified suspicious IPs and users based on login behavior
- Detected unauthenticated SSH connection attempts indicating scanning/probing

## 🚨 Alerts & Dashboards
- Real-time alert for excessive failed login attempts
- Interactive dashboards showing:
  - Failed vs successful logins
  - Top attacking IPs
  - SSH login trends

## 🔎 SPL Detection Queries

All detection queries used for SSH security monitoring are stored in the **`spl-queries/`** folder.

| Detection Use Case | File |
|--------------------|------|
| SSH Brute Force Detection | [bruteforce_detection.md](spl-queries/bruteforce_detection.md) |
| SSH Connection Without Authentication | [connection without authentication.md](spl-queries/connection%20without%20authentication.md) |
| Failed SSH Login Analysis | [failed_ssh_logins.md](spl-queries/failed_ssh_logins.md) |
| SSH Log Validation | [log_validation.md](spl-queries/log_validation.md) |
| SSH Timechart Monitoring | [ssh_timechart_monitoring.md](spl-queries/ssh_timechart_monitoring.md) |
| Successful SSH Login Monitoring | [successful ssh login.md](spl-queries/successful%20ssh%20login.md) |
