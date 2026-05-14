# Exercise 05: งานหลายขั้นตอน — ร่าง Follow-up Email จากไฟล์ที่สร้างไว้

🔑 ต้องการ M365 Copilot License
🔑 ต้องเปิดใช้งาน Cowork (Frontier preview)

แบบฝึกหัดสุดท้ายนี้จะปิด workflow ต่อเนื่องของ Session 2 โดยใช้ไฟล์ที่เราสร้างไว้จาก Exercise 02 ถึง 04 มาให้ Cowork **ร่าง Follow-up Email พร้อมเตรียมไฟล์แนบ** ทั้งหมดนี้ด้วย Prompt เดียว และที่สำคัญคือ Cowork จะขอ **Approval** ก่อนขั้นตอนที่มีผลจริง

---

## ไฟล์ที่ต้องการ

ใช้ไฟล์ที่สร้างจาก exercise ก่อนหน้า:

- ไฟล์ Word Follow-up Brief จาก Exercise 02
- ไฟล์ Excel action tracker จาก Exercise 03
- ไฟล์ PowerPoint summary จาก Exercise 04

> **⚠️ หมายเหตุ:** ถ้าหาไฟล์ที่ Cowork สร้างไว้ไม่เจอ ให้ใช้ไฟล์ที่มีอยู่เท่าที่หาเจอได้ จุดสำคัญของแบบฝึกหัดนี้คือดูว่า Cowork เตรียม email และ attachment ให้เราอย่างไร

---

## Feature 1: สั่งงานหลายขั้นตอนด้วย Prompt เดียว

1. เปิด Cowork Chat ใหม่

2. กดปุ่ม **+** (Add attachment) แล้วแนบไฟล์ Word Follow-up Brief, Excel action tracker และ PowerPoint summary ที่สร้างไว้

3. พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   จากไฟล์ที่แนบมา ช่วยร่าง follow-up email ถึง [email address] โดยสรุป 3 ประเด็นสำคัญจากการประชุม, ระบุ action items ที่ต้องติดตาม, และเตรียมแนบไฟล์ PowerPoint กับ Excel ที่เกี่ยวข้องไปด้วย 
   ```

4. สังเกตว่า Cowork แบ่งงานออกเป็นขั้นตอนย่อยหลายอย่าง เช่น:
   - ขั้นที่ 1: อ่านข้อมูลจากไฟล์ที่เราแนบ
   - ขั้นที่ 2: สรุปสาระสำคัญสำหรับเนื้อหาอีเมล
   - ขั้นที่ 3: ร่าง Email พร้อมเนื้อหาและ Attachment

---

## Feature 2: Approval Steps — ควบคุมทุกขั้นตอน

1. ระหว่างที่ Cowork ทำงาน จะมี **Approval prompt** ปรากฏขึ้นในบางขั้นตอน — โดยเฉพาะขั้นตอนที่มีผลต่อระบบจริง เช่น การส่ง Email

2. สำหรับขั้นตอนเตรียมเนื้อหา หรือเตรียมไฟล์แนบ ให้กด **Approve** เพื่อให้ workflow เดินต่อ

3. เมื่อถึงขั้นตอน "ส่ง Email" — **หยุดที่ Approval prompt นี้ก่อน** ลองอ่านว่า Cowork ร่าง Email ไว้ว่าอย่างไร

   ![Cowork chat interface](../assets/cowork-chat.png)

4. กด **Cancel** หรือ **Edit** เพื่อหยุดที่ขั้นตอนนี้ — ไม่ต้องส่ง Email จริง ๆ ในแบบฝึกหัดนี้

> **⚠️ หมายเหตุ:** ในแบบฝึกหัดนี้ขอให้ **หยุดก่อนกด Send** เพื่อไม่ให้ Email ออกไปจากบัญชีทดสอบ ลองสังเกตดูว่า Cowork ร่างเนื้อหา Email และเลือกไฟล์แนบไว้อย่างไรแทน

> **💡 เคล็ดลับ:** Approval step คือสิ่งที่ทำให้ Cowork แตกต่างจาก Automation ทั่วไป — คุณอยู่ในการควบคุมทุกขั้นตอนที่มีผลจริง

---

## สรุป

ยอดเยี่ยม! คุณผ่านทุกแบบฝึกหัดของ Session 2 แล้ว:

- ✅ Sign in และเพิ่ม Cowork จาก Agent Store
- ✅ อ่าน meeting notes แล้วสร้าง Word Follow-up Brief
- ✅ แปลง Follow-up Brief เป็น Excel action tracker
- ✅ รวมข้อมูลจากหลายไฟล์เป็น PowerPoint summary
- ✅ ร่าง follow-up email พร้อม Approval controls

Cowork ช่วยให้คุณมอบหมายงานที่ต้องข้ามหลายแอปให้ AI ทำแทนได้จริง ตั้งแต่สรุปข้อมูล, แปลงเป็นตาราง, ทำสไลด์ ไปจนถึงเตรียมอีเมล โดยยังควบคุมทุกขั้นตอนที่สำคัญได้เอง
