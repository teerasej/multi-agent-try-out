# Exercise 06: ตั้ง Scheduled Recovery Briefing แบบ Draft-only

🔑 ทำข้อนี้เมื่อเมนู **Scheduled** ปรากฏใน tenant และ Facilitator อนุมัติให้ทดลองแล้ว

Cowork สามารถตั้ง prompt ให้ทำงานตามเวลาได้ ในแบบฝึกหัดนี้จะสร้าง schedule ที่เตรียม draft briefing จาก Office outputs เดิม แต่ห้ามส่งหรือโพสต์ข้อมูลออกไป

---

## Practice 1: สร้าง scheduled prompt

1. เปิด Cowork และเริ่ม task ใหม่

2. ส่ง Prompt นี้:

   ```
   ทำงานเวลา 08:30 ทุกวันท
   ใช้ Executive Situation Summary, Recovery Action Register และ Executive Recovery Update ใน OneDrive 
   เพื่อสร้าง Daily Service Recovery Brief ใน Cowork ไม่เกิน 5 bullet

   สรุปเฉพาะ current status, blockers, owner, due time และ decision needed
   หากข้อมูลยังไม่ยืนยัน ให้ระบุ Not confirmed หรือ TBD
   ห้ามส่งอีเมล โพสต์ Teams สร้างนัดหมาย หรือแก้ไขไฟล์ต้นทาง
   ตั้ง schedule นี้ แล้วเลือก Activate and run now เพื่อทดสอบการทำงานครั้งแรก
   ```

3. ตรวจชื่อ เวลา ความถี่ และขอบเขต draft-only ก่อน Activate

4. เมื่อ run แรกเสร็จ ให้ตรวจว่า:

   - [ ] briefing อยู่ใน Cowork และไม่มี email/Teams/calendar action
   - [ ] เนื้อหาใช้ผลลัพธ์เดิมและไม่เดาข้อเท็จจริง
   - [ ] schedule แสดงใน Side panel หรือหน้า Scheduled

---

## Practice 2: หยุด Scheduled task

1. เปิด **Scheduled** หรือส่วน **Schedule** ใน Cowork panel

2. เลือก **Pause** เพื่อหยุด schedule ก่อนถึงเวลารันครั้งถัดไป

3. หากต้องการลบ ให้เลือก **Delete** หลังตรวจรายละเอียด

> หากไม่เห็น Scheduled ให้ข้ามแบบฝึกหัดนี้ เพราะความสามารถอาจถูกปิดโดย tenant policy

---

## สรุป

พวกเราได้สร้าง ตรวจสอบ และควบคุม recurring prompt โดยคงผลลัพธ์ไว้เป็น draft-only
