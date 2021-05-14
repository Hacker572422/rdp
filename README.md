# Windows2019RDP-US
Windows Server 2019 Github พร้อมการเข้าถึง RDP (ngrok US) 

ต้นฉบับ : https://github.com/docefio/Windows2019RDP-Github/ 

สร้าง RDP ฟรีพร้อม 2cpu-7gb Ram ฟรีด้วย Github:
(แนะนำให้โหลดลงไปนะครับ)

+ clone ไฟล์ไป
+ สร้าง repository ขึ้นมาเปิดเป็น public
+ ทำไฟล์ทั้ง 9 ไฟล์ลากใส่ลงใน repository ก่อน
+ จากนั้นกด commit
+ จากนั้นกลับมาที่หน้าแรกของ repository 
+ เลือก Add File แล้วเลือก Create New file
+ จากนั้นพิมพ์ path ลงในช่อง Name your file... ว่า
.github/workflows/main.yml
+ เมื่แกำหนด path เสร็จแล้ว ให้ทำการคัดลอกโค้ดที่อยู่ใน .github/workflows/main.yml ที่ทำการ clone มาเพื่อมาแก้ path
+ โดยให้เปลี่ยน 
[ชื่อผู้ใช้] คือชื่อ github ของท่าน 
[ชื่อ repository] คือชื่อ repository ที่ท่านสร้าง
เช่น
[ชื่อผู้ใช้] คือ watchakorn
[ชื่อ repository] คือ vps-test
+ จากนั้นกด commit
+ ไปที่ https://dashboard.ngrok.com เพื่อไปเอา NGROK_AUTH_TOKEN
+ จากนั้นไปใน repository ที่สร้างขึ้นไปที่ Settings จากนั้นไป    Secrets เลือก New repository secret
+ จากนั้นจริง Name ใส่ตัวแปร NGROK_AUTH_TOKEN ลงไป
+ ไปที่เว็บไซต์ https://dashboard.ngrok.com/auth/your-authtoken คัดลอก authtoken มา
+ แล้วเอาไปวางที่ Value
+ ไปที่ Action เลือก CI จากนั้นกด Run workflow
+ รีโหลดหน้าหนึ่งครั้งแล้วกด CI จากนั้นคลิก build
+ จากนั้นรอมันโหลดจนเสร็จ
+ *อย่าลองขุด บิทคอยนะครับ ไม่งั้นจะโดนลบได้
+ *แนะนำเพิ่มเติมหลังจาก เข้าใช้งานได้แล้วให้ปิดเป็น ส่วนตัวทันที ตัว vps จะอยู่ได้ 6 ชั่วโมง
