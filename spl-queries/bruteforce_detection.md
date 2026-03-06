## Brute-Force Detection(Multiple Failed Attempts)

```
spl
index=ssh_logs event_type="Multiple Failed Authentication Attempts"
| stats count by id.orig_h id.resp_h
```
### Explanation:
Detects SSH brute-force attacks by identifying repeated authentication failures
from the same source IP targeting a host

