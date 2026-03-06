## Brute-Force Detection(Multiple Failed Attempts)

```
spl
index=ssh_logs event_type="Multiple Failed Authentication Attempts"
| stats count by id.orig_h id.resp_h
```
### Explanation:
Detects SSH brute-force attacks by identifying repeated authentication failures
from the same source IP targeting a host

## 📸 Screenshot:
screenshots/<img width="1918" height="878" alt="kali-2026-02-12-12-05-44" src="https://github.com/user-attachments/assets/5158e78c-a703-4a19-bebe-6187c5eed9d3" />
