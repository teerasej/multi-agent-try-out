# Exercise 02: สร้างเอกสาร Follow-up Brief ด้วย Cowork

🔑 ต้องการ M365 Copilot License
🔑 ต้องเปิดใช้งาน Cowork (Frontier preview)

เริ่ม workflow ต่อเนื่องของ Session 2 กันในแบบฝึกหัดนี้ เราจะให้ Cowork อ่านไฟล์ **meeting-notes.docx** แล้วแปลงเป็น **เอกสาร Word แบบ Follow-up Brief** สำหรับส่งต่อให้คนที่ไม่ได้เข้าประชุม เพื่อให้เห็นว่ามันไม่ได้แค่สรุปซ้ำ แต่ช่วยปรับข้อมูลให้เหมาะกับการใช้งานต่อ

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

## Feature 2: อ่านบันทึกประชุมแล้วสร้าง Follow-up Brief

1. กดปุ่ม **+** (Add attachment) ในช่อง Prompt เพื่อแนบไฟล์ **meeting-notes.docx**

2. ในช่อง "How can I help you today?" พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   จากไฟล์ meeting-notes.docx ที่แนบมา ช่วยสร้างไฟล์ Word แบบ Follow-up Brief สำหรับส่งให้หัวหน้าที่ไม่ได้เข้าประชุม โดยแบ่งเป็น 4 ส่วน: 1) ภาพรวมสั้น ๆ 2) decisions สำคัญ 3) issues หรือ risks ที่ต้องติดตาม 4) action items พร้อม owner และ due date ถ้ามีข้อมูลในไฟล์
   ```

3. สังเกตการทำงานของ Cowork:
   - Cowork จะแสดงแผนการทำงานในขั้นตอนย่อย ๆ
   - มีการแสดงว่ากำลังใช้ Skill **Word**
   - อาจมีปุ่ม **Approve** หรือ **Confirm** ให้กดก่อนดำเนินการ — ให้กด **Approve** เพื่อยืนยัน

4. รอ Cowork สร้างเอกสาร — เมื่อเสร็จจะมีลิงก์หรือ Preview ของไฟล์ Word ปรากฏขึ้น

5. กดที่ลิงก์เพื่อเปิดเอกสาร Word และตรวจสอบว่าเนื้อหาถูกเรียบเรียงใหม่ให้อ่านเร็วและพร้อมส่งต่อ

6. จดชื่อไฟล์ Word ที่ Cowork สร้างไว้ หรือเปิดค้างไว้ก่อน เพราะเราจะใช้ไฟล์ Follow-up Brief นี้ต่อใน Exercise 03

> **💡 เคล็ดลับ:** ลองสังเกตที่ Panel ด้านขวา — Cowork จะแสดง Skills ที่กำลัง Active เช่น "Word" จะไฮไลต์ขึ้นมาระหว่างสร้างเอกสาร

---

## สรุป

คุณได้เริ่ม workflow ของ Session 2 แล้ว โดยให้ Cowork อ่าน meeting notes แล้วแปลงเป็น Follow-up Brief ที่พร้อมส่งต่อและพร้อมใช้งานต่อทันที ในแบบฝึกหัดถัดไป เราจะใช้ไฟล์นี้แปลงต่อเป็น Excel action tracker

---

แบบฝึกหัดถัดไป: [Exercise 03: แปลง Follow-up Brief เป็น Task Tracker ด้วย Cowork](../03-create-spreadsheet/README.md)
