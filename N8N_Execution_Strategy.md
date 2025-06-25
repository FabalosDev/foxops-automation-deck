# 🧠 n8n Execution Strategy – Flow Optimization Notes

## 🔁 Pain Points

- Too many executions = high cost
- Redundant triggers reprocess same data
- Flows break on missing data / fail silently

---

## ✅ Fabaverse Execution Strategy

- Use `SplitInBatches` to minimize per-item runs
- Store `last_run` or post `status` to avoid duplicates
- Filter with `IF` nodes early to stop waste
- Add exit nodes + error handling to prevent infinite retries
