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
| 2026-05-05 | A9 | Most home service businesses are running $500K+ in annual revenue on a spreadsheet and a gut feeling. | Problem/pain | Three automations for HVAC and home service businesses — quoting, scheduling, and review collection — that eliminate 12+ hours of manual work per week. | trades, home-services, quoting-automation, scheduling | Soft sell | V3 | HVAC service van at suburban home with floating isometric workflow panel | No |
| 2026-05-06 | A10 | The pilot phase is over. | Bold claim | Lauren's take on why 2026 marks the end of AI experimentation and the start of AI as permanent operating infrastructure for SMBs. | agentic-AI, infrastructure, 2026, systems | Perspective challenge | V1 | Divided cityscape — scaffolded pilot structures left, solid modern infrastructure right | No |
| 2026-05-07 | A4 | Nobody hired their ops manager to copy-paste data between tools every Friday morning. | Pattern interrupt | Anonymized consulting firm client story: ops manager freed 4.5 hours/week by automating Friday report assembly via Make.com, recapturing roughly $11K/month in billable time. | client-story, ops-automation, Friday-reporting, recaptured-time | Question CTA | V6 | Split-screen: cluttered ops desk with spreadsheets and sticky notes (left) vs. clean desk with automated report email arriving at 7 AM (right) | No |
| 2026-05-08 | A13 | Bad data beats good AI every time. | Bold claim | Contrarian take: AI projects fail not because of bad tools but because of bad data — SMBs must audit and clean their data before building any AI automation. | data-quality, processes, automation-failure, implementation | Perspective challenge | V4 | Cartoon robot presenting a perfect bar chart while a chaotic data back-room is visible through the open door behind it | No |
