# 🧠 GPT Editorial Flow

How AI is used to enhance scraped content before publishing.

---

## 🧠 Flow Structure

1. Scrape source (RSS or HTML)
2. Check for new article (via hash or timestamp)
3. Store in Sheet or DB for human review
4. If approved:
   - Clean with GPT
   - Generate headline, summary
   - Image generation
   - Format for WhatsApp or social

---

## 🛡 Challenges Solved

- Broken links → fixed by pre-validation
- Outdated content → filtered by timestamp
- Overuse of GPT → only on approved items
