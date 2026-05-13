# Exercise 03: สร้าง Task Tracker ด้วย Cowork

🔑 ต้องการ M365 Copilot License
🔑 ต้องเปิดใช้งาน Cowork (Frontier preview)

ในแบบฝึกหัดนี้ เราจะให้ Cowork สร้าง **ตาราง Excel สำหรับติดตามงาน** (Task Tracker) พร้อมข้อมูลตัวอย่าง — โดยใช้แค่การอธิบายสิ่งที่ต้องการ

---

## Feature 1: สร้าง Excel Task Tracker

1. เปิด Cowork Chat ใหม่ (กดไอคอน New Chat หรือกดที่ **Cowork** ในเมนูด้านซ้ายอีกครั้ง)

2. ในช่อง Prompt พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   สร้างไฟล์ Excel สำหรับ Task Tracker ของโปรเจกต์ "Website Redesign" โดยมีคอลัมน์: Task, Owner, Status (Not Started/In Progress/Done), Due Date และใส่ข้อมูลตัวอย่าง 5 แถว
   ```

3. สังเกตการทำงานของ Cowork:
   - Cowork จะแสดงแผนการทำงาน และระบุว่ากำลังใช้ Skill **Excel**
   - ถ้ามีปุ่ม **Approve** ให้กด เพื่อยืนยัน

4. เมื่อ Cowork สร้างไฟล์เสร็จ กดที่ลิงก์ไฟล์ Excel เพื่อเปิดและตรวจสอบข้อมูล

> **💡 เคล็ดลับ:** ลองถาม Cowork ต่อว่า `เพิ่ม Conditional Formatting ให้คอลัมน์ Status ด้วย` — Cowork สามารถแก้ไขไฟล์ที่เพิ่งสร้างได้เลย

---

## Feature 2: สังเกต Skills Panel

1. ระหว่างที่ Cowork ทำงาน ลองสังเกตที่ Panel ด้านขวาของหน้าจอ — ดูว่า Skills ใดที่ Cowork ใช้ในงานนี้

2. กดที่ Steps ที่แสดงเพื่อขยายดูรายละเอียดของแต่ละขั้นตอนที่ Cowork ทำ

---

## สรุป

คุณได้สร้าง Excel Task Tracker พร้อมข้อมูลตัวอย่างด้วย Cowork สำเร็จแล้ว ในแบบฝึกหัดถัดไป เราจะลองให้ Cowork อ่านไฟล์ที่เราอัปโหลดเองเพื่อสร้าง Presentation

---

แบบฝึกหัดถัดไป: [Exercise 04: สร้าง Presentation จากไฟล์เอกสาร](../04-create-presentation-from-file/README.md)
