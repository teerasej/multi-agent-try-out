# Exercise 03: แปลง Follow-up Brief เป็น Task Tracker ด้วย Cowork

🔑 ต้องการ M365 Copilot License
🔑 ต้องเปิดใช้งาน Cowork (Frontier preview)

ในแบบฝึกหัดนี้ เราจะใช้ไฟล์ Word Follow-up Brief ที่สร้างจาก Exercise 02 แล้วให้ Cowork แปลงต่อเป็น **ตาราง Excel สำหรับติดตามงาน** (Task Tracker) เพื่อให้เห็นว่ามันช่วยพางานจากเอกสารหนึ่งไปสู่อีกแอปหนึ่งได้

---

## Feature 1: สร้าง Excel Task Tracker จากไฟล์สรุป

1. เปิด Cowork Chat ใหม่ (กดไอคอน New Chat หรือกดที่ **Cowork** ในเมนูด้านซ้ายอีกครั้ง)

2. กดปุ่ม **+** (Add attachment) แล้วแนบไฟล์ Word Follow-up Brief ที่ Cowork สร้างจาก Exercise 02

> **⚠️ หมายเหตุ:** ถ้าหาไฟล์ Word Follow-up Brief ไม่เจอ ให้แนบไฟล์ `meeting-notes.docx` เดิมแทนได้ แล้วใช้ Prompt เดียวกันนี้

3. ในช่อง Prompt พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   จากไฟล์ที่แนบมา ช่วยสร้างไฟล์ Excel สำหรับ action tracker โดยมีคอลัมน์: Task, Owner, Status, Due Date และ Notes แล้วดึง action items จากเอกสารมาใส่ให้ครบเท่าที่มี
   ```

4. สังเกตการทำงานของ Cowork:
   - Cowork จะแสดงแผนการทำงาน และระบุว่ากำลังใช้ Skill **Excel**
   - ถ้ามีปุ่ม **Approve** ให้กด เพื่อยืนยัน

5. เมื่อ Cowork สร้างไฟล์เสร็จ กดที่ลิงก์ไฟล์ Excel เพื่อเปิดและตรวจสอบว่า action items ถูกแปลงมาเป็นตารางเรียบร้อย

6. จดชื่อไฟล์ Excel นี้ไว้ หรือเปิดค้างไว้ก่อน เพราะเราจะใช้ต่อใน Exercise 04

> **💡 เคล็ดลับ:** ลองถาม Cowork ต่อว่า `เพิ่ม Conditional Formatting ให้คอลัมน์ Status ด้วย` — Cowork สามารถปรับไฟล์ Excel ที่เพิ่งสร้างได้เลย

---

## Feature 2: สังเกต Skills Panel

1. ระหว่างที่ Cowork ทำงาน ลองสังเกตที่ Panel ด้านขวาของหน้าจอ — ดูว่า Skills ใดที่ Cowork ใช้ในงานนี้

2. กดที่ Steps ที่แสดงเพื่อขยายดูรายละเอียดของแต่ละขั้นตอนที่ Cowork ทำ

---

## สรุป

คุณได้ใช้ Cowork แปลงข้อมูลจาก Word ไปเป็น Excel สำเร็จแล้ว จุดสำคัญคือเราไม่ได้เริ่มจากศูนย์ แต่ให้มันต่อยอดจาก output ของ exercise ก่อนหน้า ในแบบฝึกหัดถัดไป เราจะใช้ไฟล์ Brief และ tracker นี้ต่อเพื่อสร้าง Presentation

---

แบบฝึกหัดถัดไป: [Exercise 04: สร้าง Presentation จาก Brief และ Tracker](../04-create-presentation-from-file/README.md)
