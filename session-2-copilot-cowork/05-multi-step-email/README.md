# Exercise 05: งานหลายขั้นตอน — สร้างเอกสารและร่าง Email

🔑 ต้องการ M365 Copilot License
🔑 ต้องเปิดใช้งาน Cowork (Frontier preview)

แบบฝึกหัดสุดท้ายนี้จะแสดงให้เห็นความสามารถสูงสุดของ Cowork: **การทำงานหลายขั้นตอนพร้อมกัน** — อ่านข้อมูลจากไฟล์ → สร้างเอกสารสรุป → ร่าง Email พร้อมแนบไฟล์ ทั้งหมดนี้ด้วย Prompt เดียว และที่สำคัญคือ Cowork จะขอ **Approval** ก่อนทุกขั้นตอนที่มีผลจริง

---

## ไฟล์ที่ต้องการ

📊 [project-tasks.xlsx — ดาวน์โหลดที่นี่](https://github.com/teerasej/multi-agent-try-out/raw/main/session-2-copilot-cowork/files/project-tasks.xlsx)

> ถ้ายังไม่ได้ดาวน์โหลด ให้กดลิงก์ด้านบนเพื่อดาวน์โหลดก่อน แล้วบันทึกไว้ที่ Desktop หรือ Downloads

---

## Feature 1: สั่งงานหลายขั้นตอนด้วย Prompt เดียว

1. เปิด Cowork Chat ใหม่

2. กดปุ่ม **+** (Add attachment) แล้วแนบไฟล์ **project-tasks.xlsx**

3. พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   ช่วยสร้าง Word document สรุปสถานะโปรเจกต์ Website Redesign (ใช้ข้อมูลจากไฟล์ที่แนบมา) แล้วร่าง Email ส่งให้ทีม พร้อมแนบไฟล์ที่สร้างขึ้น
   ```

4. สังเกตว่า Cowork แบ่งงานออกเป็นขั้นตอนย่อยหลายอย่าง เช่น:
   - ขั้นที่ 1: อ่านข้อมูลจาก `project-tasks.xlsx`
   - ขั้นที่ 2: สร้าง Word document สรุปสถานะโปรเจกต์
   - ขั้นที่ 3: ร่าง Email พร้อมเนื้อหาและ Attachment

---

## Feature 2: Approval Steps — ควบคุมทุกขั้นตอน

1. ระหว่างที่ Cowork ทำงาน จะมี **Approval prompt** ปรากฏขึ้นในบางขั้นตอน — โดยเฉพาะขั้นตอนที่มีผลต่อระบบจริง เช่น การส่ง Email

2. สำหรับขั้นตอน "สร้างเอกสาร Word" ให้กด **Approve** เพื่อยืนยัน

3. เมื่อถึงขั้นตอน "ส่ง Email" — **หยุดที่ Approval prompt นี้ก่อน** ลองอ่านว่า Cowork ร่าง Email ไว้ว่าอย่างไร

   ![Cowork approval prompt for email send](./assets/cowork-email-approval.png)

4. กด **Cancel** หรือ **Edit** เพื่อหยุดที่ขั้นตอนนี้ — ไม่ต้องส่ง Email จริง ๆ ในแบบฝึกหัดนี้

> **⚠️ หมายเหตุ:** ในแบบฝึกหัดนี้ขอให้ **หยุดก่อนกด Send** เพื่อไม่ให้ Email ออกไปจากบัญชีทดสอบ ลองสังเกตดูว่า Cowork ร่างเนื้อหา Email ว่าอย่างไรแทน

> **💡 เคล็ดลับ:** Approval step คือสิ่งที่ทำให้ Cowork แตกต่างจาก Automation ทั่วไป — คุณอยู่ในการควบคุมทุกขั้นตอนที่มีผลจริง

---

## สรุป

ยอดเยี่ยม! คุณผ่านทุกแบบฝึกหัดของ Session 2 แล้ว:

- ✅ Sign in และเพิ่ม Cowork จาก Agent Store
- ✅ สร้างเอกสาร Word ด้วยภาษาธรรมดา
- ✅ สร้าง Excel Task Tracker พร้อมข้อมูลตัวอย่าง
- ✅ อ่านไฟล์แล้วสร้าง PowerPoint Presentation
- ✅ สั่งงานหลายขั้นตอนด้วย Prompt เดียว พร้อม Approval controls

Cowork ช่วยให้คุณมอบหมายงานที่ต้องข้ามหลายแอปให้ AI ทำแทน โดยยังควบคุมทุกขั้นตอนที่สำคัญได้เอง
