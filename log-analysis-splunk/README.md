# 📊 Log Analysis with Splunk – Brute-Force Detection

## 📘 Summary
In this project, I used **Splunk** to upload and analyze login activity logs to detect signs of a **brute-force attack**. I discovered repeated failed login attempts by the same user, indicating a possible intrusion attempt.

---

## 🛠 Tools Used
- Splunk Enterprise (local install on Windows)
- Sample login log (`sample_login_log.csv`)

---

## 🔍 Detection Query
```spl
index=main sourcetype=csv
| stats count by username, src_ip
| sort -count
