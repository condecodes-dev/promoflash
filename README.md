# PromoFlash

PromoFlash is an intelligent assistant that helps users find the best grocery prices in nearby supermarkets. It interacts via platforms like Telegram (and later WhatsApp, Web), allowing users to send a list of products and receive real-time price comparisons, recommendations, and alerts.

---

## Project Goals

- Help consumers save money on grocery shopping
- Enable smart price comparison based on location
- Provide alerts when products drop in price
- Build a modular system that can scale across multiple platforms

---

## System Overview

```
[User (Telegram/WhatsApp/Web)] ⇄ [Bot Interface]
                     ⇅
          [NLP + Conversation Logic]
                     ⇅
    [Price Query System (Mock/API/Scraper)]
                     ⇅
    [Database + User Preferences + History]
                     ⇅
    [Promo & Coupon Notifier (Scheduler)]
                     ⇅
        [Future Monetization Module]
```

## Project Structure

```
promoflash/
├── app/
│   ├── interfaces/
│   ├── services/
│   ├── db/
│   ├── data/
│   ├── scraping/
│   └── scheduler/
├── tests/
├── main.py
├── requirements.txt
├── .gitignore
└── README.md
```

**Folders:**
- `interfaces/` – Telegram, WhatsApp, Web bot interfaces
- `services/` – Business logic: pricing, alerts, messages
- `db/` – SQLite setup and data models
- `data/` – Mock data (CSV)
- `scraping/` – (Future) Web scraping
- `scheduler/` – Notification and promo scheduling
- `tests/` – Unit and integration tests

---

## MVP Capabilities

- [x] Telegram bot interaction
- [x] Mocked product price search
- [x] Dynamic message generation
- [ ] Real price scraping (planned)
- [ ] Location filtering (soon)
- [ ] Scheduled promo alerts (soon)

---

## Tech Stack

- Language: Python 3.x
- Bot Platform: Telegram Bot API (python-telegram-bot)
- Framework: Flask (optional for API or admin)
- Database: SQLite (via SQLAlchemy)
- Scheduler: APScheduler
- Hosting (optional): Render / Railway / Replit

---

## Next Steps

- Implement Telegram bot interface
- Integrate mock price search
- Connect alert system
- Prepare for multi-platform support (WhatsApp, Web)

---

## License

MIT License — free to use and modify.
