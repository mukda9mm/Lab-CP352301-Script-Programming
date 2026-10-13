# Week 7 – LabsX Basic1: Introduction to Web Scraping

ดึงชื่อหนังสือและรายชื่อบททั้งหมดจากหน้าแรกของ [Automate the Boring Stuff with Python (3rd Edition)](https://automatetheboringstuff.com/3e/) ด้วย `requests` + `BeautifulSoup4`

## วิธีรัน (Windows PowerShell)

```powershell
python -m venv venv
venv\Scripts\Activate.ps1
pip install -r requirements.txt
python main.py
```

macOS / Linux: `python3 -m venv venv` แล้ว `source venv/bin/activate`

## โครงสร้างโปรเจกต์

```
web-scraping-intro/
├── src/
│   ├── __init__.py
│   └── scraper.py      # คลาส SimpleWebScraper (ดาวน์โหลด + parse HTML)
├── main.py             # จุดเริ่มต้นโปรแกรม
├── requirements.txt
├── .gitignore
└── README.md
```

## จริยธรรมในการ Scrape

ตรวจสอบ `robots.txt` และ Terms of Service ของเว็บก่อนเสมอ ไม่ส่ง request ถี่เกินไป และถ้าเว็บมี API ให้ใช้ API แทน โปรเจกต์นี้ทำเพื่อการศึกษาเท่านั้น
