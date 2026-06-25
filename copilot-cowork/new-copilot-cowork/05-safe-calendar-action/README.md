# Exercise 05: ฝึกตรวจ Safe Calendar Action และ Approval

🔑 ใช้เฉพาะบัญชีทดสอบของผู้จัดงาน และห้ามเพิ่มผู้เข้าร่วมประชุม

ในข้อนี้จะใช้ Cowork เตรียม action ที่มีผลกับปฏิทินของตนเอง เพื่อเรียนรู้การอ่าน approval card อย่างปลอดภัย โดยจะ **Cancel** ก่อนสร้าง event จริง

---

## Feature 1: เตรียม private calendar event

1. เปิด Cowork task ใหม่

2. ส่ง Prompt นี้:

   ```
   เตรียมสร้าง private calendar event ชื่อ Service Recovery Review
   พรุ่งนี้เวลา 09:00 นาน 15 นาที
   ไม่มีผู้เข้าร่วมประชุม และไม่ต้องสร้าง Teams meeting link

   แสดงรายละเอียด event ให้ฉันตรวจ และรอ approval จากฉันก่อนสร้าง
   ```

3. เมื่อ Cowork แสดง preview หรือ approval card ให้ตรวจ:

   - [ ] ชื่อ event ถูกต้อง
   - [ ] วัน เวลา และระยะเวลา 15 นาทีถูกต้อง
   - [ ] ไม่มีผู้เข้าร่วมประชุม
   - [ ] ไม่มี Teams link หรือข้อความที่จะส่งออก

4. เลือก **Show parameters** หากปรากฏ เพื่อดูรายละเอียด action

5. เลือก **Cancel** เสมอ ห้ามเลือก Create และห้ามเลือก Don't ask again

---

## สรุป

พวกเราได้เห็นว่า Cowork จะหยุดรอให้ตรวจและอนุมัติก่อนทำ action ที่มีผลจริงกับ calendar

แบบฝึกหัดถัดไป: [Exercise 06: ตั้ง Scheduled recovery briefing](../06-scheduled-recovery-briefing/README.md)
