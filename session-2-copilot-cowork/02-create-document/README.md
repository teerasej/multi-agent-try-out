# Exercise 02: สร้างเอกสาร Decision Log ด้วย Cowork

🔑 ต้องการ M365 Copilot License
🔑 ต้องเปิดใช้งาน Cowork (Frontier preview)

เริ่ม workflow ต่อเนื่องของ Session 2 กันในแบบฝึกหัดนี้ เราจะให้ Cowork อ่านไฟล์ **meeting-notes.docx** แล้วแปลงเป็น **เอกสาร Word แบบ Decision Log** ที่ดึงเฉพาะการตัดสินใจ ผู้รับผิดชอบ และ risks เพื่อให้เห็นว่า Cowork ไม่ได้สรุปซ้ำ แต่แปลงข้อมูลให้เป็นรูปแบบที่ใช้งานต่อได้ทันที

---

## ไฟล์ที่ต้องการ

📄 [meeting-notes.docx — ดาวน์โหลดที่นี่](https://github.com/teerasej/multi-agent-try-out/raw/main/session-2-copilot-cowork/files/meeting-notes.docx)

> ถ้ายังไม่ได้ดาวน์โหลด ให้กดลิงก์ด้านบนเพื่อดาวน์โหลดก่อน แล้วบันทึกไว้ที่ Desktop หรือ Downloads

---

## Feature 1: เปิด Cowork

1. จากหน้า M365 Copilot Chat ให้กดที่ **Cowork** ในส่วน Agents ด้านซ้าย

   ![Cowork chat interface](../assets/cowork-chat.png)

2. หน้า Cowork จะเปิดขึ้น — สังเกตว่าต่างจาก Copilot Chat ตรงที่หน้าจอแสดงข้อความต้อนรับว่า **"What should we tackle next?"**

---

## Feature 2: อ่านบันทึกประชุมแล้วสร้าง Decision Log

1. กดปุ่ม **+** (Add attachment) ในช่อง Prompt เพื่อแนบไฟล์ **meeting-notes.docx**

2. ในช่อง "How can I help you today?" พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   จากไฟล์ meeting-notes.docx ที่แนบมา สร้างไฟล์ Word แบบ Decision Log โดยแสดง: 
   1) ผู้รับผิดชอบแต่ละข้อ 
   2) Due date (ถ้ามี) 
   3) Risks หรือ blockers ที่ต้องระวัง 
   4) ข้อมูลอ้างอิงจากการประชุม
   ```
   
   หรือจะใช้วิธีเลือกไฟล์จาก OneDrive โดยการพิมพ์ Prompt โดยใช้เครื่องหมาย `/` แบบด้านล่างก็ได้:

   
   ```
   จากไฟล์ [/meeting-notes.docx] ที่แนบมา สร้างไฟล์ Word แบบ Decision Log โดยแสดง: 1) การตัดสินใจที่เกิดขึ้นในการประชุม 
   1) ผู้รับผิดชอบแต่ละข้อ 
   2) Due date (ถ้ามี) 
   3) Risks หรือ blockers ที่ต้องระวัง 
   4) ข้อมูลอ้างอิงจากการประชุม
   ```


3. สังเกตการทำงานของ Cowork:
   - Cowork จะแสดงแผนการทำงานในขั้นตอนย่อย ๆ
   - มีการแสดงว่ากำลังใช้ Skill **Word**
   - อาจมีปุ่ม **Approve** หรือ **Confirm** ให้กดก่อนดำเนินการ — ให้กด **Approve** เพื่อยืนยัน

4. รอ Cowork สร้างเอกสาร — เมื่อเสร็จจะมีลิงก์หรือ Preview ของไฟล์ Word ปรากฏขึ้น และมีรายการไฟล์ที่เกี่ยวข้อง แสดงใน Panel ด้านขวา

5. กดที่ลิงก์เพื่อเปิดเอกสาร Word และตรวจสอบว่าเนื้อหาถูกแยกออกเป็น decision, owner, risk ได้ชัดเจน

6. จดชื่อไฟล์ Word ที่ Cowork สร้างไว้ หรือเปิดค้างไว้ก่อน เพราะเราจะใช้ไฟล์ Decision Log นี้ต่อใน Exercise 03

> **💡 เคล็ดลับ:** ลองสังเกตที่ Panel ด้านขวา — Cowork จะแสดง Skills ที่กำลัง Active เช่น "Word" จะไฮไลต์ขึ้นมาระหว่างสร้างเอกสาร

---

## สรุป

คุณได้เริ่ม workflow ของ Session 2 แล้ว โดยให้ Cowork แปลง meeting notes เป็น Decision Log ที่มีประเด็นเดียวคือ decision + owner + risk — ไม่ใช่สรุปเนื้อหาทั้งหมด แต่เป็นข้อมูลที่ใช้ทำงานต่อทันที ในแบบฝึกหัดถัดไป เราจะใช้ไฟล์นี้แปลงต่อเป็น Excel action tracker

---

แบบฝึกหัดถัดไป: [Exercise 03: แปลง Decision Log เป็น Task Tracker ด้วย Cowork](../03-create-spreadsheet/README.md)
