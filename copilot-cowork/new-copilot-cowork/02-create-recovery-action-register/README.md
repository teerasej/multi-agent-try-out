# Exercise 02: สร้าง Recovery Action Register ด้วย Cowork

🔑 ต้องทำ Exercise 01 ให้เสร็จใน **Cowork task เดิม** และเห็นไฟล์ `Executive Situation Summary` ใน Output แล้ว

ในข้อนี้จะเพิ่มข้อมูลเชิงตัวเลขจาก `service-performance-dashboard.xlsx` แล้วให้ Cowork สร้าง recovery action register ในรูปแบบไฟล์ Excel เพื่อสรุปงานกู้คืนที่ต้องดำเนินการ ระบุ owner สถานะ และสิ่งที่ต้องตัดสินใจ พร้อมตรวจสอบย้อนกลับได้จาก Word output และ dashboard

---

## Feature 1: เพิ่ม dashboard และสร้าง Excel action register

1. กลับไปที่ Cowork task เดิมจาก Exercise 01 แล้วเปิด Side panel

2. ตรวจว่า `Executive Situation Summary` ปรากฏใน **Output** แล้ว

3. เลือก **Add attachments** > **Attach cloud files** แล้วเลือก `service-performance-dashboard.xlsx` จาก OneDrive (หรืออัพโหลดจากเครื่อง) เพื่อให้ Cowork ใช้ไฟล์นี้เป็นข้อมูลประกอบกับ Word output

4. ส่ง Prompt นี้ใน task เดิม:

   ```
   จาก Executive Situation Summary และไฟล์ excel ที่แนบมา
   สร้างไฟล์ Excel ใหม่ชื่อ Recovery Action Register

   สร้างตารางที่มีคอลัมน์: Action, Owner, Status, Due Time, Dependency or Blocker, Decision Needed และ Evidence Source
   ใช้เฉพาะข้อมูลที่ยืนยันได้จาก Word output และ dashboard
   หากข้อมูลไม่มีหรือยังไม่ยืนยัน ให้ระบุ TBD หรือ Not confirmed อย่าเดา
   ตั้งค่า Status ให้ใช้สีที่อ่านง่ายสำหรับ In Progress, Not Started และ Blocked
   สร้างเฉพาะไฟล์ Excel นี้ ห้ามส่ง แชร์ โพสต์ หรือนัดหมาย

   วางแผนให้เรารีวิวก่อน ยังไม่ต้องทำอะไรเพิ่มเติม
   ```

5. ตรวจสอบแผนการที่ Cowork แสดงขึ้นมา และปรับแต่งตามต้องการ โดยใช้ prompt ด้านล่างต่อไปนี้
   ```
   ปรับแผนตามความต้องการด้านล่าง และแสดงให้รีวิว ยังไม่ต้องทำอะไร 
   ...
   ``` 
   
ุ6. เมื่อพอใจแล้ว ให้พิมพ์ prompt นี้เพื่อเริ่มดำเนินการ
   ```
   approve
   ```
7. ระหว่างทำงาน ให้สังเกตว่า Cowork โหลด Skill **Excel** และมีไฟล์ใหม่ถูกสร้างใน Output

---

## Feature 2: ตรวจสอบ Recovery Action Register

1. กดเปิด preview ของ Excel จาก **Output** ใน Side panel

2. ตรวจความถูกต้องด้วย checklist นี้:

   - [ ] มีคอลัมน์ครบตาม Prompt
   - [ ] Action ที่เกี่ยวกับ customer advisory และ vendor escalation ปรากฏครบ
   - [ ] Status อ่านง่ายและสอดคล้องกับข้อมูลต้นทาง

> 💡 เคล็ดลับ: Output ของ Cowork ถูกเก็บไว้ใน task และสามารถเปิดจาก OneDrive เพื่อใช้ต่อใน Exercise 03 ได้

---

## สรุป

พวกเราได้แปลงหลักฐาน incident เป็น Excel register ที่พร้อมติดตามงานแล้ว

แบบฝึกหัดถัดไป: [Exercise 03: สร้าง Executive Recovery Update](../03-create-executive-recovery-update/README.md)
