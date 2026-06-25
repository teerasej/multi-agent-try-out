# Exercise 02: สร้าง Decision Log ด้วย Cowork

🔑 ต้องมี Microsoft 365 Copilot license และผู้ดูแลเปิดใช้ Cowork แล้ว

เริ่ม **Cowork task เดียว** ที่จะใช้ต่อถึง Exercise 05 ในข้อนี้ เราจะให้ Cowork อ่าน `meeting-notes.docx` แล้วสร้าง Word Decision Log ที่นำไปใช้ต่อได้จริง ไม่ใช่สรุปการประชุมแบบกว้าง ๆ

> **ต่อจาก Exercise 01:** กลับไปเปิด task เดิมจาก Tasks/Search หากยังเปิดอยู่ ห้ามเริ่ม task ใหม่ เพราะเราจะต่อยอด work context และผลลัพธ์ในบทสนทนาเดียวกัน

---

## Practice 1: เพิ่มแหล่งข้อมูลและสร้าง Decision Log

1. ตรวจสอบว่าไฟล์ `meeting-notes.docx` ปรากฏในส่วน **Input** ของ Side panel แล้ว

   - ถ้ายังไม่มี ให้เลือก **Add attachments** > **Attach cloud files** แล้วเลือกไฟล์จาก OneDrive
   - ใช้ **Add work context** ได้เมื่อมีไฟล์, บุคคล, อีเมล, Teams chat/channel หรือ meeting ในองค์กรที่ต้องการอ้างอิงเพิ่ม

2. ส่ง Prompt ด้านล่างใน **task เดิม**:

   ```
   จาก meeting-notes.docx สร้างไฟล์ Word ชื่อ Decision Log โดยใช้เฉพาะข้อมูลจากไฟล์ต้นทาง

   สำหรับแต่ละ decision ให้แสดง: การตัดสินใจ, Owner, Due date, Risks/Blockers และหลักฐานอ้างอิงจากการประชุม
   หากข้อมูลใดไม่มีในต้นทาง ให้ระบุว่า TBD หรือ Not specified แทนการคาดเดา
   สร้างเฉพาะไฟล์ Word นี้ และยังไม่ต้องส่ง แชร์ หรือแก้ไขข้อมูลอื่น
   ```

3. ระหว่าง Cowork ทำงาน ให้สังเกต thinking indicator, Skill messages และ step-by-step updates ในแชต รวมถึง Progress และ Skills ใน Side panel

4. ถ้า Cowork ถามคำถามเพิ่มเติม ให้เลือกคำตอบที่ตรงกับงาน หรือเลือก **Skip** เมื่อต้องการให้ทำต่อจากข้อมูลที่มีอยู่

5. ถ้างานกำลังไปผิดทาง ให้ใช้ Pause หรือ Cancel แล้วบอกสิ่งที่ต้องการเพิ่มได้ทันที ข้อความที่ส่งระหว่างทำงานจะถูก queue ไว้ตามลำดับ

---

## Practice 2: ตรวจสอบ Output ก่อนทำขั้นถัดไป

1. เปิดส่วน **Output** ใน Side panel แล้วเลือก preview ของไฟล์ Word ที่สร้างขึ้น

2. ตรวจด้วย checklist นี้:

   - [ ] ทุก decision มี owner หรือระบุว่าไม่พบในต้นทาง
   - [ ] Due date ที่ไม่มีในต้นทางไม่ถูกแต่งขึ้น
   - [ ] Risks/Blockers แยกจาก decision ชัดเจน
   - [ ] มีหลักฐานอ้างอิงที่ช่วยให้กลับไปตรวจ meeting notes ได้

3. หากพบข้อผิดพลาด ให้สั่งแก้ใน task เดิม เช่น:

   ```
   แก้ไข Decision Log โดยระบุ TBD ในทุกช่อง Due date ที่ไม่มีข้อมูลใน meeting notes และคงข้อมูลอื่นจากต้นฉบับไว้
   ```

> **💡 เคล็ดลับ:** ผลลัพธ์ที่ Cowork สร้างจะเปิดจาก Side panel หรือ OneDrive ได้ตลอด ไม่จำเป็นต้องจำชื่อไฟล์แล้วเริ่มแชตใหม่

---

## สรุป

พวกเรามี Word Decision Log ที่ตรวจสอบย้อนกลับได้แล้ว และยังอยู่ใน Cowork task เดิม ใน Exercise 03 เราจะใช้ output นี้สร้าง Excel action tracker ต่อทันที

แบบฝึกหัดถัดไป: [Exercise 03: แปลง Decision Log เป็น Task Tracker ด้วย Cowork](../03-create-spreadsheet/README.md)
