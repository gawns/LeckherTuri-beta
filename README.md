# PROJECT-WEB-PWP — Pizza Lecker Thury (versi awal)

Versi awal aplikasi web pemesanan Pizza Lecker Thury: Flask + MySQL dengan template Jinja.

## Halaman

- `/` — beranda menu.
- `/order` — pemesanan; `/checkout` — pembayaran (QRIS).
- `/login`, `/register`, `/profile` — autentikasi dan profil pengguna.
- `/admin` dan turunannya — CRUD menu, pesanan, statistik, dan pengguna.

## API JSON

Endpoint `/api/*` (antara lain `/api/pizzas`, `/api/checkout`, `/api/admin/stats`) untuk konsumsi dari JavaScript.

## Struktur

- `app.py` — seluruh route web dan API dalam satu berkas.
- `templates/` — template Jinja.
- `static/` — CSS per komponen, JavaScript, dan gambar QRIS.

## Menjalankan

```bash
pip install flask mysql-connector-python
python app.py          # http://127.0.0.1:5000
```

Konfigurasi MySQL ada di `app.py` (database `db_pizza_thury`).

## Status

Repositori ini adalah versi awal sebelum penambahan 2FA. Versi terbaru ada pada repositori `Leckers-Turi-Project`.