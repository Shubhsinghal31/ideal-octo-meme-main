# 📚 Smart Attendance System

A **secure and automated web-based attendance system** that uses **QR Code + OTP verification** for real-time, proxy-proof attendance logging — built with **Supabase**, **TypeScript**, and **TailwindCSS**.

---

## 🚀 Features

### 👨‍🏫 For Teachers
- Generate QR codes with auto-refreshing OTP (every 20s)
- Live dashboard with real-time student attendance updates
- Manual override for attendance
- Export to Excel/PDF

### 👨‍🎓 For Students
- Secure login via Supabase Auth
- Scan QR and enter OTP for attendance
- View attendance history
- Notifications for expired sessions or invalid OTP

### 🔐 Security
- OTP retry limit (3 attempts)
- Session auto-expiry
- Time-based QR invalidation
- JWT-based route protection

---

## 🛠️ Tech Stack

| Layer        | Tech Used                          |
|--------------|-------------------------------------|
| **Frontend** | HTML, TailwindCSS, TypeScript, Bun  |
| **Backend**  | Node.js, Express, TypeScript        |
| **Database** | Supabase (PostgreSQL + Auth)        |
| **Other**    | QR Code Generator, OTP System       |

---

## 🧩 Project Structure

```
ideal-octo-meme-main/
├── frontend/         # UI using Tailwind + TS + Bun
│   └── index.html    # Entry point
├── backend/          # Supabase-integrated Node backend
│   └── src/          
│       ├── index.ts
│       └── supabaseClient.ts
```

---

## 📦 Installation & Run

### 📍 Backend

```bash
cd backend
npm install
npm run dev
```

Make sure your Supabase credentials are set properly in `.env`.

### 📍 Frontend

```bash
cd frontend
bun install
bun run dev
```

Visit `http://localhost:3000` to view the app.

---

## 📈 Future Enhancements

- Real-time animations for QR display
- Admin panel to track batch-wise stats
- Facial recognition integration (optional module)
