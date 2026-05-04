# Post History

The daily agent reads this file before selecting a content angle. It enforces freshness ceilings AND the Deduplication Protocol defined in `LinkedIn post.md`.

**Column guide:**
- **Hook (first line):** The exact first line of the post — used to enforce hook differentiation (no two similar hooks within 3 posts)
- **Hook Formula:** Which formula was used (Bold claim / Stat hook / Pattern interrupt / Problem/pain / Question) — must differ from last post
- **Key Themes:** 3–5 comma-separated keywords capturing the core argument — used for the theme keyword overlap check (max 1 shared keyword within 3 posts)
- **Image Style:** The V1–V8 style code — must differ from last post
- **Image Subject:** The primary visual subject (e.g., "robot at desk," "split-screen office") — must differ from last 3 posts

After each draft is sent to Telegram, the agent appends a row here. Update the **Approved** column to `Yes` once the post goes live on LinkedIn.

---

| Date | Angle | Hook (first line) | Hook Formula | Topic Summary | Key Themes | CTA Type | Image Style | Image Subject | Approved |
|------|-------|-------------------|--------------|---------------|------------|----------|-------------|---------------|----------|
| 2026-05-01 | A6 | "We tried AI and it didn't work." | Bold claim | Busting the myth that failed AI pilots mean AI doesn't work — the real culprit is bad process and no rollout ownership. | myth-bust, AI-failure, process, implementation | Question CTA | V4 | Robot shrugging at a whiteboard of tangled flowcharts | Yes |
| 2026-05-03 | A14 | Stop losing leads to slow follow-up. | Pattern interrupt | A 20-minute Make.com automation that instantly follows up with leads on form submission, boosting response rates for service businesses. | lead-follow-up, Make.com, automation, response-rate | Save prompt | V2 | Four-node automation pipeline infographic (form → gear → email → calendar) | No |
| 2026-05-04 | A3 | $3.70 returned for every $1 invested in AI automation. | Stat hook | ROI data post showing $3.70 returned per $1 invested in AI automation, illustrated with a professional services client story, reinforcing that AI processes — not just AI tools — drive measurable returns for SMBs. | ROI, data, business-case, investment | Resource offer | V1 | Business owner reviewing upward-trending ROI bar chart at a modern desk (editorial illustration) | No |
