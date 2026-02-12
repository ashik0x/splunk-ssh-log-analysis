## Vlidation of Ingested Logs

```spl
index=ssh_logs | stats count by event_type
```
## Explanation:
Validates that SSH logs are successfully ingested and properly parsed by Splunk.
This query confirms the presence and distribution of SSH event types, ensuring data readiness before advanced analysis.
## 📸 Screenshot:
screenshots/<img width="1918" height="720" alt="log validation png" src="https://github.com/user-attachments/assets/21989266-5a2b-4085-9898-ebe6f9e10d6a" />
