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
screenshots/<img width="1918" height="728" alt="kali-2026-02-12-12-03-05" src="https://github.com/user-attachments/assets/e0472cd9-8125-47f1-9ae7-934f0f49a760" />

