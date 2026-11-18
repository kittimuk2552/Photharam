# 🌿 โพธาราม Second Market

**ตลาดของเหลือใช้ชุมชน — Photharam Green Eco Community Marketplace**

เว็บแอปตลาดซื้อขายของเหลือใช้ในชุมชนโพธาราม จ.ราชบุรี  
รองรับ 9 ภาษา · แผนที่จุดนัดรับสินค้า · ระบบแชท & วิดีโอคอล · ธีมสีญี่ปุ่น Eco Minimal

---

## 🚀 เปิดใช้งานเว็บไซต์

### วิธีที่ 1: เปิดบน GitHub Pages (แนะนำ)
เพียงเปิด URL ของ GitHub Pages โดยตรง — ไม่ต้องติดตั้งอะไรเพิ่มเติม

### วิธีที่ 2: เปิดบนเครื่องตัวเอง (Local)

> ⚠️ **สำคัญ**: แผนที่ OpenStreetMap **ต้องรันผ่าน HTTP Server** เท่านั้น  
> การดับเบิลคลิก `index.html` โดยตรงจะทำให้แผนที่ไม่แสดงผล

**วิธีเปิด Local Server:**

**ตัวเลือก A — ใช้ `start.bat` (Windows, ง่ายที่สุด):**
```
ดับเบิลคลิก start.bat → เบราว์เซอร์จะเปิดอัตโนมัติที่ http://localhost:8085
```

**ตัวเลือก B — Python (ทุก OS):**
```bash
cd photharam-second-market
python -m http.server 8080
# เปิดเบราว์เซอร์ที่ http://localhost:8080
```

**ตัวเลือก C — Node.js / npx:**
```bash
cd photharam-second-market
npx serve .
# เปิดเบราว์เซอร์ที่ URL ที่แสดงในเทอร์มินัล
```

**ตัวเลือก D — VS Code Live Server Extension:**
คลิกขวาที่ `index.html` → "Open with Live Server"

---

## 📁 โครงสร้างไฟล์

```
photharam-second-market/
├── index.html          ← หน้าหลักของเว็บแอป
├── style.css           ← ธีมสี, Layout, Responsive
├── app.js              ← ระบบทั้งหมด (ไม่ต้องการ server-side)
├── lib/                ← ไลบรารี local (ไม่ต้องการ internet)
│   ├── leaflet.css
│   ├── leaflet.js      ← แผนที่ OpenStreetMap
│   ├── lucide.js       ← ไอคอน
│   └── images/         ← Marker icons สำหรับแผนที่
└── public/
    └── images/         ← รูปภาพสินค้า
```

---

## ✨ ฟีเจอร์

| ฟีเจอร์ | รายละเอียด |
|---------|-----------|
| 🌍 9 ภาษา | ไทย, อังกฤษ, ญี่ปุ่น, จีน, เกาหลี, เยอรมัน, ฝรั่งเศส, สเปน, พม่า |
| 🗺️ แผนที่ | OpenStreetMap + Leaflet.js (พื้นที่จริงโพธาราม) |
| 💬 แชท | ระบบ Chat ในแอป |
| 📹 วิดีโอคอล | WebRTC Video/Voice Call |
| 🎨 ธีม | 4 ธีมสี (ครีมมินต์, ฟ้าสกาย, เขียว Sage, คลื่นปอลล์) |
| 🌙 Dark Mode | สลับโหมดมืด/สว่าง |
| 🔔 แจ้งเตือน | ระบบการแจ้งเตือน |
| 🛒 ลงประกาศ | เพิ่ม/ลบสินค้า พร้อมราคา |
| 👑 Admin | ระบบแอดมินจัดการสินค้า |

---

## 🌐 Deploy บน GitHub Pages

1. Fork หรือ Upload โปรเจกต์นี้ไป GitHub Repository
2. ไปที่ **Settings → Pages**
3. เลือก **Source: Deploy from a branch**
4. เลือก **Branch: main** และ **folder: / (root)**
5. กด **Save** → รอ 1-3 นาที
6. เว็บจะ live ที่: `https://[username].github.io/[repo-name]/`

> ✅ เว็บนี้เป็น **Static HTML/CSS/JS ล้วน** — ไม่ต้องการ PHP หรือฐานข้อมูล  
> สามารถ deploy ได้บน GitHub Pages, Netlify, Vercel, หรือ Hosting ทั่วไป

---

## 🛠️ เทคโนโลยีที่ใช้

- **HTML5 / CSS3 / Vanilla JavaScript** (ไม่มี Framework)
- **Leaflet.js 1.9.4** — แผนที่ Interactive
- **OpenStreetMap** — ข้อมูลแผนที่
- **Lucide Icons** — ไอคอน
- **Google Fonts** — Prompt, Kanit, Noto Sans (JP/KR/SC)
- **WebRTC** — Video/Voice Call

---

## 📝 License

สร้างเพื่อชุมชนโพธาราม จ.ราชบุรี 🌿  
Photharam, Ratchaburi, Thailand
