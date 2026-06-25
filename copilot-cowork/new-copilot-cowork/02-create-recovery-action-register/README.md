# Exercise 02: สร้าง Recovery Action Register ด้วย Cowork

🔑 ต้องทำ Exercise 01 ให้เสร็จใน **Cowork task เดิม** และเห็นไฟล์ `Executive Situation Summary` ใน Output แล้ว

ในข้อนี้จะเพิ่มข้อมูลเชิงตัวเลขจาก `service-performance-dashboard.xlsx` แล้วให้ Cowork สร้าง Excel recovery action register ที่ตรวจสอบย้อนกลับได้จาก Word output และ dashboard

---

## Feature 1: เพิ่ม dashboard และสร้าง Excel action register

1. กลับไปที่ Cowork task เดิมจาก Exercise 01 แล้วเปิด Side panel

2. ตรวจว่า `Executive Situation Summary` ปรากฏใน **Output** แล้ว

3. เลือก **Add attachments** > **Attach cloud files** แล้วเลือก `service-performance-dashboard.xlsx` จาก OneDrive

4. ส่ง Prompt นี้ใน task เดิม:

   ```
   ใช้ Executive Situation Summary ที่สร้างใน task นี้ และไฟล์ service-performance-dashboard.xlsx ที่แนบมา
   สร้างไฟล์ Excel ชื่อ Recovery Action Register

   สร้างตารางที่มีคอลัมน์: Action, Owner, Status, Due Time, Dependency or Blocker, Decision Needed และ Evidence Source
   ใช้เฉพาะข้อมูลที่ยืนยันได้จาก Word output และ dashboard
   หากข้อมูลไม่มีหรือยังไม่ยืนยัน ให้ระบุ TBD หรือ Not confirmed แทนการคาดเดา
   ตั้งค่า Status ให้ใช้สีที่อ่านง่ายสำหรับ In Progress, Not Started และ Blocked
   สร้างเฉพาะไฟล์ Excel นี้ ห้ามส่ง แชร์ โพสต์ หรือนัดหมาย
   ```

5. ระหว่างทำงาน ให้สังเกตว่า Cowork โหลด Skill **Excel** และมีไฟล์ใหม่ใน Output

---

## Feature 2: ตรวจสอบ Recovery Action Register

1. เปิด preview ของ Excel จาก **Output** ใน Side panel

2. ตรวจด้วย checklist นี้:

   - [ ] มีคอลัมน์ครบตาม Prompt
   - [ ] Action ที่เกี่ยวกับ customer advisory และ vendor escalation ปรากฏครบ
   - [ ] Root cause ยังระบุว่า Not confirmed หรือ Working hypothesis
   - [ ] ไม่มี owner, deadline หรือ evidence ที่ Cowork สร้างขึ้นเอง
   - [ ] Status อ่านง่ายและสอดคล้องกับข้อมูลต้นทาง

3. หากต้องการแก้ไข ให้สั่งใน task เดิม เช่น:

   ```
   เปรียบเทียบ Recovery Action Register กับ Executive Situation Summary และ dashboard แล้วเพิ่มเฉพาะ action ที่ตกหล่น โดยไม่เปลี่ยนข้อเท็จจริงเดิม
   ```

> 💡 เคล็ดลับ: Output ของ Cowork ถูกเก็บไว้ใน task และสามารถเปิดจาก OneDrive เพื่อใช้ต่อใน Exercise 03 ได้

---

## สรุป

คุณได้แปลงหลักฐานเชิงข้อความและตัวเลขเป็น Excel register ที่พร้อมติดตามงานแล้ว

แบบฝึกหัดถัดไป: [Exercise 03: สร้าง Executive Recovery Update](../03-create-executive-recovery-update/README.md)
