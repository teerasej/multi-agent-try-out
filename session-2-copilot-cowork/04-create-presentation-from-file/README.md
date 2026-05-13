# Exercise 04: สร้าง Presentation จากไฟล์เอกสาร

🔑 ต้องการ M365 Copilot License
🔑 ต้องเปิดใช้งาน Cowork (Frontier preview)

แบบฝึกหัดนี้จะแสดงให้เห็นความสามารถของ Cowork ในการ **อ่านไฟล์ที่เราแนบ** แล้วสร้าง PowerPoint Presentation สรุปเนื้อหาให้อัตโนมัติ

---

## ไฟล์ที่ต้องการ

📄 [meeting-notes.docx — ดาวน์โหลดที่นี่](https://github.com/teerasej/multi-agent-try-out/raw/main/session-2-copilot-cowork/files/meeting-notes.docx)

> ถ้ายังไม่ได้ดาวน์โหลด ให้กดลิงก์ด้านบนเพื่อดาวน์โหลดก่อน แล้วบันทึกไว้ที่ Desktop หรือ Downloads

---

## Feature 1: แนบไฟล์และสร้าง Presentation

1. เปิด Cowork Chat ใหม่

2. กดปุ่ม **+** (Add attachment) ในช่อง Prompt เพื่อแนบไฟล์

3. เลือกไฟล์ **meeting-notes.docx** ที่ดาวน์โหลดมา

4. หลังจากแนบไฟล์แล้ว พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   จากไฟล์ที่แนบมา ให้สร้าง PowerPoint Presentation สรุปประเด็นสำคัญ พร้อม action items โดยแบ่งเป็น 4 สไลด์
   ```

5. สังเกตการทำงานของ Cowork:
   - Cowork จะอ่านเนื้อหาในไฟล์ `meeting-notes.docx`
   - แสดงแผนการทำงาน และระบุว่ากำลังใช้ Skill **PowerPoint**
   - ถ้ามีปุ่ม **Approve** ให้กดเพื่อยืนยัน

6. เมื่อ Cowork สร้างไฟล์เสร็จ กดที่ลิงก์ไฟล์ PowerPoint เพื่อเปิดและดู Slide ทั้ง 4

> **💡 เคล็ดลับ:** สังเกตว่า Cowork จะสรุปเฉพาะประเด็นสำคัญ ไม่ได้คัดลอกทั้งเอกสาร — นี่คือประโยชน์ของ AI ที่ช่วย "กลั่น" ข้อมูล

---

## สรุป

คุณได้ให้ Cowork อ่านเอกสารและสร้าง Presentation สรุปสำเร็จแล้ว ในแบบฝึกหัดสุดท้าย เราจะลองสั่งงานที่ซับซ้อนขึ้น — ให้ Cowork ทำงานหลายขั้นตอนพร้อมกัน

---

แบบฝึกหัดถัดไป: [Exercise 05: งานหลายขั้นตอน — สร้างเอกสารและร่าง Email](../05-multi-step-email/README.md)
