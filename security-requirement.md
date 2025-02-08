## 12.4.1 File Storage

Verify that files obtained from untrusted sources are stored outside the web
root, with limited permissions.

ChatGPT : การจัดเก็บไฟล์จากแหล่งที่ไม่น่าเชื่อถือ (Untrusted Sources) เป็นประเด็นสำคัญด้านความปลอดภัยของระบบ โดยเฉพาะเว็บแอปพลิเคชันที่อนุญาตให้ผู้ใช้ อัปโหลดไฟล์ เช่น รูปภาพ เอกสาร หรือไฟล์อื่นๆ ซึ่งหากไม่มีมาตรการรักษาความปลอดภัยที่ดี อาจเปิดช่องให้เกิด การโจมตีทางไซเบอร์ เช่น Remote Code Execution (RCE), File Inclusion Attacks และอื่นๆ
Web Root คือไดเรกทอรีที่เว็บเซิร์ฟเวอร์ใช้ให้บริการไฟล์ เช่น /var/www/html/ (สำหรับ Apache บน Linux) หรือ C:\inetpub\wwwroot\ (สำหรับ IIS บน Windows) ซึ่งหากมีไฟล์ที่อัปโหลดไปอยู่ภายในโฟลเดอร์นี้โดยตรง อาจถูกเข้าถึงและรันได้โดยตรงจาก URL

Gemini :

My self :
