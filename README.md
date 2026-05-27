# 👋 ยินดีต้อนรับสู่ GitHub ของฉัน! | [มรรควัฒน์ นันหน]

<div align="center">
  <img src="https://rms.bncc.ac.th/files/importpicstd/01/69319010006.jpg" alt="Profile Picture" width="150" height="150" style="border-radius: 50%;"/>
  
  <h3>"มุ่งมั่นพัฒนาทักษะ Backend เพื่อสร้างสรรค์เทคโนโลยีที่ตอบโจทย์อนาคต"</h3>
</div>

---

## 📌 จุดประสงค์และเป้าหมายการศึกษา

### 🏫 ข้อมูลการศึกษา
* **สถาบัน:** วิทยาลัยพณิชยการบางนา
* **สาขาวิชา:** เทคโนโลยีสารสนเทศ (Information Technology)

### 🎯 เป้าหมายในรายวิชา Backend
ฉันมีความตั้งใจที่จะศึกษาและพัฒนาทักษะใน**รายวิชา Backend** อย่างจริงจัง โดยมุ่งเน้นไปที่:
* เข้าใจสถาปัตยกรรมและการทำงานของระบบฝั่ง Server-side
* การออกแบบและจัดการฐานข้อมูล (Database Management)
* การสร้าง API ที่มีประสิทธิภาพ ปลอดภัย และรองรับการขยายตัวในอนาคต

---

## 🛠️ ทักษะและเครื่องมือที่กำลังศึกษา (Tech Stack)

* **Language:** JavaScript (Node.js)
* **Framework:** Express.js
* **Tools:** Git, GitHub, Postman

---

## 💻 ตัวอย่างการเขียน Code ด้วย Node.js

นี่คือตัวอย่างการสร้าง HTTP Server อย่างง่ายด้วย Node.js (Built-in Module) เพื่อเริ่มต้นแสดงคำว่า "Hello World" บนเว็บเบราว์เซอร์:

```javascript
// 1. นำเข้า http module ของ Node.js
const http = require('http');

// 2. กำหนด Hostname และ Port ที่ต้องการให้ Server ทำงาน
const hostname = '127.0.0.1';
const port = 3000;

// 3. สร้าง Server และจัดการ Request/Response
const server = http.createServer((req, res) => {
  res.statusCode = 200; // ส่ง สถานะ 200 (OK) กลับไป
  res.setHeader('Content-Type', 'text/plain; charset=utf-8');
  res.end('สวัสดีครับ! ยินดีต้อนรับเข้าสู่ Backend Server ด้วย Node.js 🚀\n');
});

// 4. สั่งให้ Server เริ่มทำงาน (Listen)
server.listen(port, hostname, () => {
  console.log(`Server กำลังทำงานที่ http://${hostname}:${port}/`);
});