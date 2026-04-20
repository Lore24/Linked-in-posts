# Cherry Hill AI — LinkedIn Post Scheduler

## What This Does
This project runs a daily Claude agent that researches trending AI-in-business topics, selects the best content angle, writes a LinkedIn post, generates an image via kie.ai, and sends the draft to Telegram for approval. Once approved, Make.com posts it to LinkedIn.

The agent runs every day at 9:00 AM ET via a scheduled Claude routine.

---

## Who This Is For
**Lauren Fernandez** — founder of Cherry Hill AI, an AI automation consultancy for small and medium-sized businesses.

**Brand voice:** Confident and direct. Practitioner, not academic. Speaks to operators and owners, not engineers. Short sentences, no passive voice. Never use: leverage, synergy, unlock, revolutionize, game-changer, empower, seamless.

**Goal of every post:** Move SMB owners closer to booking a discovery call with Cherry Hill AI.

---

## Files in This Repo

| File | Purpose |
|------|---------|
| `LinkedIn post.md` | Full content strategy: angle library (A1–A15), post framework, hashtag rules, tone guide |
| `post-history.md` | Running log of every post sent. Agent reads this to enforce freshness ceilings. |
| `.env.example` | Template for required API keys. Copy to `.env` locally (never commit `.env`). |

---

## How the Daily Agent Works

1. **Research** — Searches for AI-in-business news from the last 7 days
2. **Check freshness** — Reads `post-history.md` to see which angles have been used recently and enforces freshness ceilings from `LinkedIn post.md`
3. **Score angles** — Rates the top 3 candidates on Freshness + Engagement + Conversion (1–5 each, max 15), picks the winner
4. **Write post** — Follows the framework in `LinkedIn post.md` exactly: hook, body, CTA, hashtags
5. **Generate image** — Creates a Flux Nano prompt and calls kie.ai to generate the image
6. **Send to Telegram** — Delivers the draft post, image, and scoring rationale to the Telegram bot
7. **Log** — Adds a row to `post-history.md`

---

## Approval & Publishing Flow

1. Agent sends draft to Telegram
2. Lauren reviews and replies **APPROVED** (or gives revision notes)
3. Make.com watches the Telegram bot for "APPROVED"
4. Make.com posts to LinkedIn automatically

---

## Adding New Content Angles
Open `LinkedIn post.md` and add a new angle block at the bottom of the Angle Library section following the same format as A1–A15. Include: theme, hook direction, value, variations, best CTA type, and freshness ceiling.

---

## Environment Variables Required

```
KIE_API_KEY          — kie.ai API key for Flux Nano image generation
TELEGRAM_BOT_TOKEN   — Telegram bot token from BotFather
TELEGRAM_CHAT_ID     — Your Telegram chat ID where drafts are sent
MAKE_WEBHOOK_URL     — Make.com webhook URL (optional — for direct LinkedIn trigger)
```

Store these in `.env` locally. In the scheduled cloud routine, they are injected as secrets in the task prompt.
