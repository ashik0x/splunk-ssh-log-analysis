
### Splunk Query – Suspicious SSH Connections Without Authentication

```spl
index=ssh_logs event_type="Connection Without Authentication"
| stats count by id.orig_h
```
## Explanation:
This query searches the ssh_logs index for SSH connections where authentication did not occur. It counts the number of such attempts by source IP (id.orig_h), which helps identify hosts making suspicious or incomplete SSH connection attempts

## 📸 Screenshot:
screenshots/<img width="1918" height="878" alt="kali-2026-02-12-12-08-09" src="https://github.com/user-attachments/assets/383e338f-acdf-4161-8117-648aacd69b56" />
