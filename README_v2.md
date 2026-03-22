# 🎓 Stipendiat Ball Tracker — Telegram Bot v2

Talabalar uchun ilmiy va ijtimoiy faoliyatlarni kuzatuvchi Telegram bot.  
**Talaba + Admin panel** bilan to'liq versiya.

---

## 👤 TALABA IMKONIYATLARI

| Funksiya | Tavsif |
|---|---|
| 📝 Ro'yxatdan o'tish | Ism, guruh, telefon raqami — qayta o'ta olmaydi |
| ⏳ Tasdiq kutish | Admin tasdiqlagunga qadar bot bloklanadi |
| ➕ Ball qo'shish | 8 ta faoliyat, hujjat/rasm bilan |
| 📊 Profil | Ball, progress bar, streak, statistika |
| 🏆 Reyting | Top 10 — barcha talabalar orasida |
| 🎖️ Yutuqlar | 9 ta achievement tizimi |
| 📅 Tarix | So'rovlar tarixi (approved/rejected/pending) |
| ⚙️ Semestr | 1–4 semestr, alohida hisoblanadi |
| ✉️ Adminga xabar | To'g'ridan-to'g'ri admin bilan bog'lanish |

---

## 🔐 ADMIN IMKONIYATLARI

| Funksiya | Buyruq/Tugma |
|---|---|
| Ro'yxatdan o'tishni tasdiqlash/rad etish | Inline tugmalar |
| Faoliyat so'rovini tasdiqlash/rad etish | Inline tugmalar (fayl bilan) |
| Barcha talabalar ro'yxati | Admin panel |
| Stipendiat ro'yxati (top 20) | Admin panel |
| Excel hisobot eksport | Admin panel → 2 ta sheet |
| Broadcast xabar | Barcha talabalarga |
| Faoliyat limitlarini o'zgartirish | Admin panel |
| Talabani o'chirish | `/del_TELEGRAM_ID` |
| Ball qo'shish/ayirish | `/adj_TELEGRAM_ID` |
| Rad etilgan talabani qayta tasdiqlash | Admin panel |

---

## 🎯 Faoliyatlar va ballar

| Faoliyat | Ball | Limit |
|---|---|---|
| 🎪 Tadbirda ishtirok | +2 | — |
| 🎓 Milliy konferensiya | +1 | 3 ta/semestr |
| 🌍 Xalqaro nashr/konferensiya | +2 | 2 ta/semestr |
| 📰 OAK jurnalida maqola | +3 | 5 ta/semestr |
| 📄 Mahalliy jurnalda maqola | +2 | 5 ta/semestr |
| 📋 Gazetaga maqola | +1 | — |
| 🤝 Volontyorlik (1 kun) | +10 | 10 ta/semestr |
| 🏅 DGU guvohnoma | +3 | — |

---

## 🚀 O'rnatish

```bash
git clone https://github.com/USERNAME/stipend-bot.git
cd stipend-bot
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
```

`bot.py` ichida sozlang:
```python
BOT_TOKEN = "YOUR_TOKEN"      # BotFather dan oling
ADMIN_IDS = [123456789]       # O'z Telegram ID ingiz
```

> Telegram ID ni bilish uchun [@userinfobot](https://t.me/userinfobot) ga yozing.

```bash
python bot.py
```

---

## 🔑 Faoliyat oqimi

```
Talaba hujjat yuboradi
        ↓
Admin ko'radi (fayl + ma'lumot)
        ↓
Tasdiqlash ✅ → ball qo'shiladi + talabaga xabar
Rad etish  ❌ → talabaga sabab + qayta yuborish imkoni
```

---

## 🗂 Fayl tuzilmasi

```
stipend-bot/
├── bot.py            # Asosiy bot (talaba + admin)
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 📝 Litsenziya

MIT — erkin foydalaning.
