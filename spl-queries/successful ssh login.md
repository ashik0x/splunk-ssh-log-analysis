
### Splunk Query – Successful SSH Login Analysis

```spl
index=ssh_logs event_type="Successful SSH Login"
| stats count by id.orig_h, id.resp_h

```
## Explanation:
This query searches the ssh_logs index for successful SSH login events and counts the number of logins grouped by source IP (id.orig_h) and destination IP (id.resp_h). It helps identify which hosts are initiating SSH connections and which servers are receiving them.

## 📸 Screenshot:
screenshots/<img width="1918" height="878" alt="kali-2026-02-12-12-06-30" src="https://github.com/user-attachments/assets/124f0011-a7e8-4cfa-bdbe-96d0683595f4" />
