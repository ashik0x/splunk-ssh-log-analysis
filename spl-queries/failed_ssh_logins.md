## Failed SSH Login Analysis

```
spl
index=ssh_logs event_type="Failed SSH Login"
| stats count by id.orig_h
```

## Explanation:
Identifies source IP addresses generating failed SSH login attempts.
Used to detect suspicious hosts and potential brute-force sources

## 📸 Screenshot:
screenshots/
