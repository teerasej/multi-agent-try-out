# Exercise 03: แปลง Decision Log เป็น Task Tracker ด้วย Cowork

🔑 ต้องทำ Exercise 02 ใน Cowork task เดิมให้เสร็จก่อน

ในแบบฝึกหัดนี้ เราจะใช้ Word Decision Log ที่อยู่ใน **Output ของ task เดิม** เพื่อสร้าง Excel action tracker ไม่ต้องเปิด task ใหม่หรือพิมพ์ชื่อไฟล์ให้ Cowork เดา

---

## Practice 1: สร้าง Excel Action Tracker จาก Output เดิม

1. กลับไปที่ Cowork task ที่สร้าง Decision Log จาก Exercise 02

2. ตรวจใน Side panel ว่า Decision Log อยู่ในส่วน **Output** หากหา task ไม่เจอ ให้เปิด Tasks/Search แล้ว resume task นี้

3. ส่ง Prompt ด้านล่าง:

   ```
   ใช้ Decision Log ที่สร้างใน task นี้เพื่อสร้างไฟล์ Excel ชื่อ Action Tracker

   สร้างตารางที่มีคอลัมน์: Task, Owner, Status, Due Date และ Notes
   ดึง action item ให้ครบตามข้อมูลที่มี; ถ้า Owner หรือ Due Date ไม่มี ให้ระบุ TBD
   ตั้งค่า Status เริ่มต้นเป็น Not started และเพิ่ม conditional formatting สำหรับ Not started, In progress, Blocked และ Done
   สร้างเฉพาะไฟล์ Excel นี้ ยังไม่ต้องส่ง แชร์ หรือแก้ไขข้อมูลภายนอก task
   ```

4. สังเกตว่า Cowork โหลด Skill **Excel** และแสดงความคืบหน้าอย่างไร

5. หากนึกเงื่อนไขเพิ่มระหว่าง Cowork ทำงาน ให้ส่งข้อความต่อได้ เช่น `เพิ่ม action item ที่มี blocker ให้ Status เป็น Blocked` ข้อความจะเข้า queue และ Cowork ปรับแผนตามบริบท

---

## Practice 2: ตรวจสอบ Task Tracker

1. เปิด preview ของ Excel จาก **Output** ใน Side panel

2. ตรวจด้วย checklist นี้:

   - [ ] Action item จาก Decision Log อยู่ในตารางครบเท่าที่มี
   - [ ] คอลัมน์ Task, Owner, Status, Due Date และ Notes มีครบ
   - [ ] ค่า Owner/Due Date ที่ไม่ทราบเป็น TBD ไม่ใช่ข้อมูลที่ Cowork เดา
   - [ ] Status เริ่มต้นและ conditional formatting อ่านง่าย

3. หากมีรายการตกหล่น ให้สั่งแก้ใน task เดิม เช่น:

   ```
   เปรียบเทียบ Action Tracker กับ Decision Log ใน task นี้ แล้วเพิ่ม action item ที่ตกหล่นโดยไม่เปลี่ยนรายการเดิม
   ```

> **💡 เคล็ดลับ:** ระหว่างทำงานให้ดู Progress, Skills และ Output ใน Side panel แทนการรอผลในแชตอย่างเดียว

---

## สรุป

พวกเราได้แปลงข้อมูลจาก Word เป็น Excel ใน Cowork task เดิมแล้ว Exercise ถัดไปจะนำทั้ง Decision Log และ Action Tracker ไปสร้าง PowerPoint summary

แบบฝึกหัดถัดไป: [Exercise 04: สร้าง Presentation จาก Decision Log และ Tracker](../04-create-presentation-from-file/README.md)
