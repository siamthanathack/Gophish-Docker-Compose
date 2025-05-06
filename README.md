# Gophish‑Docker‑Compose

ติดตั้งและตั้งค่า Gophish ด้วย Docker Compose

---

## ขั้นตอน

1. สร้างโฟลเดอร์ `gophish` ขึ้นมา

   ```bash
   mkdir gophish
   cd gophish

2. จำเป็นต้องสร้างไฟล์ทั้ง 3 เพื่อเปิดใช้งาน `gophish`

   ```bash
    nano config.json
    nano .env
    nano docker-compose.yml

3. หลังจากที่สร้างครบทั้ง 3 ไฟล์แล้ว ให้ใช้คำสั่งนี้

   ```bash
    docker-compose up -d

4. ตรวจสอบว่าเปิดใช้งานแล้ว

   ```bash
    docker ps

5. ใช้คำสั่งนี้เพื่อดู `username` และ `password`

   ```bash
    docker logs gophish

6. นำข้อมูลที่ได้ไป login ที่

   ```bash
    https://<IP_SERVER>:3333
