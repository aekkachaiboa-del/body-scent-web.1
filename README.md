# Body Scent

Static landing page สำหรับแบรนด์ Body Scent พร้อมใช้งานบน GitHub และ Vercel

## โครงสร้างไฟล์

- `index.html` หน้าแรก
- `product.html` หน้าสินค้า
- `order.html` หน้าสั่งซื้อ
- `thankyou.html` หน้าขอบคุณ
- `admin.html` หน้ารายการคำสั่งซื้อ
- `style.css` ธีมหลัก
- `script.js` JavaScript กลาง
- `products.json` ข้อมูลสินค้า
- `images/` รูปภาพสินค้า
- `vercel.json` การตั้งค่า route สำหรับ Vercel
- `404.html` หน้าไม่พบข้อมูล

## Deploy ขึ้น GitHub

1. สร้าง Repository ใหม่
2. อัปโหลด **เนื้อหาภายในโฟลเดอร์นี้ทั้งหมด** ไปไว้ที่ root ของ Repository
3. ตรวจว่า `index.html` และ `vercel.json` อยู่หน้าแรกของ Repository

## Deploy ขึ้น Vercel

1. เข้า Vercel แล้วเลือก `Add New > Project`
2. Import Repository จาก GitHub
3. Framework Preset: `Other`
4. Root Directory: `./`
5. Build Command: เว้นว่าง
6. Output Directory: เว้นว่าง
7. Install Command: เว้นว่าง
8. กด Deploy

## หมายเหตุสำคัญ

ระบบคำสั่งซื้อเวอร์ชันนี้เก็บข้อมูลใน `localStorage`
ดังนั้น `admin.html` จะเห็นเฉพาะคำสั่งซื้อที่สร้างจาก Browser/Device เดียวกัน
หากต้องการใช้งานขายจริง ควรเปลี่ยนเป็นฐานข้อมูลออนไลน์ เช่น Supabase/Firebase
