# Exercise 03: สร้าง Executive Recovery Update ด้วย Cowork

🔑 ต้องทำ Exercise 01 และ 02 ใน **Cowork task เดิม** ให้เสร็จก่อน

แบบฝึกหัดนี้ใช้ Word และ Excel output ที่สร้างแล้ว ร่วมกับ `executive-service-context.pptx` เพื่อสร้างสไลด์สำหรับผู้บริหารจากหลักฐานที่ตรวจสอบได้

---

## Feature 1: เพิ่ม executive context และสร้าง PowerPoint

1. กลับไปที่ Cowork task เดิม และตรวจว่าใน Output มีทั้ง `Executive Situation Summary` และ `Recovery Action Register`

2. เลือก **Add attachments** > **Attach cloud files** แล้วเลือก `executive-service-context.pptx` จาก OneDrive

3. ส่ง Prompt นี้:

   ```
   ใช้ Executive Situation Summary, Recovery Action Register และไฟล์ executive-service-context.pptx ใน task นี้
   สร้างไฟล์ PowerPoint ชื่อ Executive Recovery Update สำหรับผู้บริหาร

   สร้าง 4 สไลด์:
   1) Current situation and service status
   2) Customer and business impact
   3) Recovery actions, blockers and owners
   4) Decisions required and next steps

   ใช้เฉพาะข้อเท็จจริงจากแหล่งข้อมูล ระบุ Not confirmed หรือ TBD เมื่อข้อมูลยังไม่พอ
   สร้างเฉพาะไฟล์ PowerPoint นี้ ห้ามส่ง แชร์ หรือโพสต์ผลลัพธ์
   ```

4. ระหว่างทำงาน ให้ดู Skill **PowerPoint**, Progress และ Output ใน Side panel

---

## Feature 2: Preview และตรวจความถูกต้อง

1. เปิด PowerPoint จาก Output เพื่อดู preview แบบ split view

2. ตรวจด้วย checklist นี้:

   - [ ] มี 4 สไลด์ตามโครงสร้างที่ขอ
   - [ ] Current status เป็น AMBER และ root cause ยังไม่ถูกยืนยัน
   - [ ] ตัวเลข customer/service impact สอดคล้องกับ dashboard
   - [ ] มี decision เรื่อง customer advisory, vendor escalation และ release control
   - [ ] ไม่มีการสร้างตัวเลขหรือ timeline ใหม่

3. หากต้องการปรับ ให้ส่งคำสั่งใน task เดิม เช่น:

   ```
   ปรับสไลด์ 3 ให้แสดงเฉพาะ action ที่เป็น In Progress หรือ Blocked และคงข้อเท็จจริงเดิมไว้
   ```

---

## สรุป

พวกเราได้รวมหลักฐานจากหลาย Office files เป็น PowerPoint ที่อ่านเพื่อการตัดสินใจได้เร็วแล้ว

แบบฝึกหัดถัดไป: [Exercise 04: สร้าง Custom Skill](../04-create-custom-skill/README.md)
