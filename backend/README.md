# FloraGift – Sistem Pemesanan Bucket Bunga Custom Online

Back-end: Express.js + SQLite (REST API). Front-end: React (Vite). Keduanya terpisah.

## Menjalankan di lokal
```bash
git clone <URL-REPO-KAMU>
cd floragift

# Terminal 1 – API (http://localhost:3000)
cd backend && npm install && npm start

# Terminal 2 – Web (http://localhost:5173)
cd frontend && npm install && cp .env.example .env && npm run dev
```
Data contoh terisi otomatis saat API pertama kali jalan.

## Endpoint utama
GET /api/products, /api/products/:id, /api/categories · POST/PUT/DELETE /api/products
POST /api/orders · GET /api/orders · GET /api/orders/:code · PATCH /api/orders/:code/status

## Deploy
- API: Render/Railway (root `backend`, start `npm start`).
- Web: Vercel/Netlify (root `frontend`, build `npm run build`, output `dist`), set `VITE_API_URL` ke URL API.
