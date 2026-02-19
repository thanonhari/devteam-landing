# DevTeam Landing Page

หน้าเว็บสำหรับบริการรับทำเว็บไซต์

## 🚀 วิธี Deploy

### ตัวเลือกที่ 1: Vercel (แนะนำ)

```bash
# 1. ติดตั้ง Vercel CLI
npm i -g vercel

# 2. Deploy
cd landing-page
vercel

# 3. ตอบคำถาม:
# - Set up and deploy? Yes
# - Which scope? (เลือก account ของคุณ)
# - Link to existing project? No
# - Project Name? devteam-landing
# - Directory? ./
# - Want to modify settings? No
```

### ตัวเลือกที่ 2: GitHub Pages

```bash
# 1. สร้าง GitHub repository ใหม่
# 2. Push โค้ดขึ้น GitHub
git init
git add .
git commit -m "Initial landing page"
git remote add origin https://github.com/YOUR_USERNAME/devteam-landing.git
git push -u origin main

# 3. ไปที่ Settings > Pages
# 4. เลือก branch: main, folder: / (root)
# 5. กด Save
```

### ตัวเลือกที่ 3: Netlify

```bash
# 1. ไปที่ https://app.netlify.com/drop
# 2. ลาก folder "landing-page" ลงไป
# 3. รอ deploy เสร็จ
```

## 📧 ตั้งค่าส่งอีเมล

### ใช้ Formspree (ฟรี)

1. ไปที่ https://formspree.io
2. สร้าง account และสร้าง form ใหม่
3. จะได้ FORM_ID มา
4. แก้ไข `index.html` บรรทัด 370:
   ```javascript
   fetch('https://formspree.io/f/YOUR_FORM_ID', {
   ```

### ใช้ EmailJS

1. สมัคร https://www.emailjs.com
2. สร้าง Email Service
3. แก้ไข JavaScript ให้ส่งผ่าน EmailJS

## 🎨 การแก้ไข

### เปลี่ยนข้อมูลติดต่อ

แก้ไขใน `index.html`:
- ชื่อบริษัท: บรรทัด 91 ("DevTeam")
- อีเมล: แก้ใน form action

### เปลี่ยนราคา

แก้ไขใน `index.html`:
- Landing Page: บรรทัด 174
- Business Website: บรรทัด 188
- E-commerce: บรรทัด 202

## 📱 Responsive

หน้าเว็บรองรับ:
- Desktop
- Tablet
- Mobile

## 🛠️ เทคโนโลยี

- HTML5
- CSS3 (CSS Grid, Flexbox)
- Vanilla JavaScript
- ไม่ต้องใช้ framework

## 📄 License

MIT
