# Exercise 05: งานหลายขั้นตอน — ร่าง Follow-up Email และตรวจ Approval

🔑 ต้องใช้ **test mailbox ที่ผู้จัดงานกำหนดเท่านั้น**

แบบฝึกหัดสุดท้ายของ core workflow นี้จะใช้ output ทั้งหมดใน Cowork task เดิมเพื่อร่าง follow-up email แล้วฝึกตรวจ approval card โดย **ห้ามส่งอีเมลจริง**

---

## Feature 1: ร่าง Email จาก Output เดิม

1. กลับไปที่ Cowork task เดิม และตรวจใน Side panel ว่ามี Decision Log, Action Tracker และ PowerPoint summary อยู่ใน **Output**

2. ส่ง Prompt ด้านล่าง โดยแทน `[test mailbox]` ด้วยอีเมลทดสอบที่ Facilitator ให้มา:

   ```
   ใช้ Decision Log, Action Tracker และ PowerPoint summary ใน task นี้
   ร่าง follow-up email ถึง [test mailbox] โดยสรุป 3 ประเด็นสำคัญ, ระบุ action items ที่ต้องติดตาม และแนบ PowerPoint กับ Excel ที่เกี่ยวข้อง

   แสดง draft และรายการไฟล์แนบให้ฉันตรวจสอบก่อน ยังไม่ต้องส่งอีเมล
   ```

3. ตรวจ draft ในแชตและ preview/output ก่อนทำขั้นถัดไป:

   - [ ] ผู้รับเป็น test mailbox ที่ถูกต้อง
   - [ ] เนื้อหาสรุปตรงกับ output ก่อนหน้า
   - [ ] Action items สำคัญอยู่ครบ
   - [ ] รายการไฟล์แนบเป็น PowerPoint และ Excel ที่ถูกต้อง

---

## Feature 2: ฝึกอ่าน Approval card โดยไม่ส่งจริง

1. เมื่อ draft ถูกต้องแล้ว ให้ส่งข้อความนี้ **เฉพาะเมื่อ Facilitator ยืนยันว่าเป็น test mailbox**:

   ```
   เตรียมส่งอีเมล draft นี้ไปยัง [test mailbox] พร้อมไฟล์แนบตามที่แสดง แล้วรอ approval จากฉัน
   ```

2. เมื่อ Cowork แสดง approval card:

   - อ่าน preview ของผู้รับ เนื้อหา และไฟล์แนบ
   - ดู risk indicator หากปรากฏ
   - เลือก **Show parameters** เพื่อดูรายละเอียดการกระทำ
   - ทำความเข้าใจว่าปุ่ม Send/Action อนุมัติครั้งนี้เท่านั้น ส่วน **Don't ask again** ใช้ข้าม approval ที่คล้ายกันใน conversation ปัจจุบัน

3. เลือก **Cancel** เสมอในแบบฝึกหัดนี้ ห้ามกด Send และห้ามเลือก Don't ask again

4. หาก Cowork ไปผิดทางก่อนถึง approval ให้ใช้ Pause หรือ Cancel และแก้คำสั่งใน task เดิมได้

> **⚠️ หมายเหตุ:** Cowork ขอ approval สำหรับการกระทำที่มีผลจริง เช่น ส่งอีเมล โพสต์ Teams หรือสร้างนัดหมาย ไม่ได้หมายความว่าทุกขั้นตอนสร้างเอกสารจะต้องมี approval

---

## สรุป

คุณได้ทำ workflow ข้าม Word, Excel, PowerPoint และ Email ใน Cowork task เดียว พร้อมตรวจข้อมูลและหยุดการกระทำที่มีผลจริงก่อนส่งออกไป

หากต้องการทดลองความสามารถแบบตั้งเวลา ให้ทำต่อที่ [Exercise 06 (Optional): ตั้ง Scheduled Briefing](../06-scheduled-briefing/README.md)
