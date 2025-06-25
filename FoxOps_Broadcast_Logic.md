# 🛰 FoxOps – Broadcast Logic Blueprint

This doc outlines the approved-post-to-channel system inside n8n or any automation platform.

---

## 🧠 Flow Summary

1. **Trigger** – Scheduled check every 30 minutes
2. **Source** – Sheet/database with posts marked `approved`
3. **Flow**:
   - Filter posts marked `approved` and not yet posted
   - Format content
   - Send to WhatsApp API (WHAPI or Meta)
   - Log post, mark status as `posted`

---

## 🎯 Goals

- Avoid re-posting same content
- Handle multiple scheduled items gracefully
- Support delayed or future-dated posts
