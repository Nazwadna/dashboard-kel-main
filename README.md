# Dashboard Kelurahan

Aplikasi dashboard berbasis React + Vite.

## 1) Jalankan project di lokal

1. Install dependency:
   ```bash
   npm install
   ```
2. Copy file environment:
   ```bash
   cp .env.example .env
   ```
   Untuk Windows PowerShell:
   ```powershell
   Copy-Item .env.example .env
   ```
3. Isi `.env`:
   - `VITE_SUPABASE_URL`
   - `VITE_SUPABASE_ANON_KEY`
4. Jalankan:
   ```bash
   npm run dev
   ```

## 2) Build production

```bash
npm run build
```

Output build ada di folder `dist/`.

## 3) Deploy ke Vercel

Project ini sudah punya `vercel.json` untuk SPA rewrite. Langkah cepat:

1. Push code ke GitHub (sudah selesai).
2. Login ke Vercel lalu import repo GitHub ini.
3. Di Vercel Project Settings > Environment Variables, tambahkan:
   - `VITE_SUPABASE_URL`
   - `VITE_SUPABASE_ANON_KEY`
4. Deploy.

## 4) Keamanan secret

- Jangan commit file `.env`.
- Gunakan `.env.example` sebagai template value yang aman.
