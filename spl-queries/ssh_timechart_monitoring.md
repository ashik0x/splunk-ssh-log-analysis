
### Splunk Query – Timechart for SSH Connections Without Authentication

```spl
index=ssh_logs event_type="Connection Without Authentication"
| timechart count by id.orig_h
```
## Explanation:
This query searches for SSH connections where authentication did not occur and creates a time-based chart of the events. It shows the number of unauthenticated SSH attempts over time grouped by source IP (id.orig_h), helping analysts detect spikes or suspicious activity patterns.

## 📸 Screenshot:
screenshots/<img width="1918" height="878" alt="kali-2026-02-12-12-08-41" src="https://github.com/user-attachments/assets/66dec87e-a9c4-409b-a6d8-1e23fe072b2d" />
