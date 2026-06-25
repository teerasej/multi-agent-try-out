# Exercise 03: สร้าง Executive Recovery Update ด้วย Cowork

🔑 ต้องทำ Exercise 01 และ 02 ใน **Cowork task เดิม** ให้เสร็จก่อน

แบบฝึกหัดนี้ใช้ Word และ Excel output ที่สร้างแล้ว ร่วมกับ `executive-service-context.pptx` เพื่อให้ Cowork วางแผนสไลด์สำหรับผู้บริหารก่อน จากนั้นบันทึก outline เป็น Markdown แล้วค่อยสร้าง PowerPoint จากแผนที่รีวิวแล้ว

---

## Practice 1: เพิ่ม executive context และวางแผน PowerPoint

1. กลับไปที่ Cowork task เดิม และตรวจว่าใน Output มีทั้ง `Executive Situation Summary` และ `Recovery Action Register`

2. *(ถ้ายังไม่มีไฟล์ `service-performance-dashboard.xlsx`)* เลือก **Add attachments** > **Upload image or files** แล้วเลือก `service-performance-dashboard.xlsx` จาก OneDrive (หรืออัพโหลดจากเครื่อง) เพื่อให้ Cowork ใช้ไฟล์นี้เป็นข้อมูลประกอบ

3. เลือก **Add attachments** > **Upload image or files** แล้วเลือก `executive-service-context.pptx` จาก OneDrive (หรืออัพโหลดจากเครื่อง) เพื่อให้ Cowork ใช้ไฟล์นี้เป็นข้อมูลประกอบ
   
4. ส่ง Prompt นี้เพื่อให้ Cowork วางแผนก่อน ยังไม่ต้องสร้าง PowerPoint:

   ```
   ใช้ Executive Situation Summary, Recovery Action Register, และไฟล์ powerpoint ใน task นี้

   วางแผนสำหรับไฟล์ PowerPoint ชื่อ Executive Recovery Update สำหรับผู้บริหาร
   แสดงแผนให้รีวิวก่อน โดยระบุ:
   - Slide outline จำนวน 4 สไลด์
   - Key message ของแต่ละสไลด์
   - ข้อมูลที่จะใช้จาก Word output, Excel register และ executive-service-context.pptx
   - Theme/style direction ที่เหมาะกับ executive-service-context.pptx
   - จุดที่ยังเป็น Not confirmed หรือ TBD

   ใช้เฉพาะข้อเท็จจริงจากแหล่งข้อมูล ห้ามสร้างตัวเลขหรือ timeline ใหม่
   ```

5. รีวิวแผนที่ Cowork แสดงขึ้นมา โดยดูว่า outline, key message, evidence sources และ theme/style direction เหมาะกับผู้บริหารหรือไม่

6. *(optional)* หากต้องการปรับแผน ให้ส่งคำสั่งใน task เดิม เช่น:

   ```
   ปรับแผนให้ slide 4 เน้น decision required มากขึ้น และคง theme/style direction แบบ executive
   แสดงแผนใหม่ให้รีวิวก่อน ยังไม่ต้องสร้างไฟล์
   ```

7. เมื่อพอใจกับแผนแล้ว ให้ส่ง Prompt นี้เพื่อบันทึก outline เป็น Markdown:

   ```
   บันทึกแผนที่รีวิวแล้วเป็นไฟล์ Markdown ชื่อ Executive Recovery Update Outline.md

   ในไฟล์ให้มีหัวข้อ:
   - Purpose
   - Theme Style
   - Slide Outline
   - Evidence Sources
   - Open Questions or TBD

   สร้างเฉพาะไฟล์ Markdown นี้ ยังไม่ต้องสร้าง PowerPoint
   ```

8. ตรวจว่า `Executive Recovery Update Outline.md` ปรากฏใน **Output** แล้ว
9. กด preview ไฟล์ Markdown เพื่อดูว่า outline, key message, evidence sources และ theme/style direction ตรงกับสิ่งที่รีวิวแล้วหรือไม่ 
10. กดดู code จากด้านบนของหน้าต่าง preview เพื่อให้แน่ใจว่า Markdown ถูกบันทึกครบถ้วนและถูกต้อง

11. ส่ง Prompt นี้เพื่อให้ Cowork สร้าง PowerPoint จาก outline ที่บันทึกแล้ว:

   ```
   จากแผนใน Executive Recovery Update Outline.md
   ให้สร้างไฟล์ PowerPoint ชื่อ Executive Recovery Update สำหรับผู้บริหาร

   ใช้โครงสร้าง slide, key message, evidence sources และ theme/style direction ตาม outline
   ใช้เฉพาะข้อเท็จจริงจากแหล่งข้อมูล ระบุ Not confirmed หรือ TBD เมื่อข้อมูลยังไม่พอ
   สร้างเฉพาะไฟล์ PowerPoint นี้ ห้ามส่ง แชร์ หรือโพสต์ผลลัพธ์
   ```

12. ระหว่างทำงาน ให้ดู Skill **PowerPoint**, Progress และ Output ใน Side panel

---

## Practice 2: Preview outline และตรวจความถูกต้องของ PowerPoint

1. เปิด `Executive Recovery Update Outline.md` จาก **Output** เพื่อตรวจว่าแผนตรงกับสิ่งที่รีวิวแล้ว

2. เปิด PowerPoint จาก Output เพื่อดู preview แบบ split view

3. ตรวจด้วย checklist นี้:

   - [ ] มี 4 สไลด์ตามโครงสร้างที่ขอ
   - [ ] PowerPoint ทำตาม outline ที่กำหนดไว้
   - [ ] Theme/style มีการอ้างอิงจาก `executive-service-context.pptx`
   - [ ] Current status เป็น AMBER และ root cause ยังไม่ถูกยืนยัน
   - [ ] ตัวเลข customer/service impact สอดคล้องกับ dashboard
   - [ ] มี decision เรื่อง customer advisory, vendor escalation และ release control
   - [ ] ไม่มีการสร้างตัวเลขหรือ timeline ใหม่ และใช้ `Not confirmed` หรือ `TBD` เมื่อหลักฐานยังไม่พอ

---

## สรุป

พวกเราได้ฝึกให้ Cowork วางแผนและบันทึก outline ก่อนสร้าง PowerPoint เพื่อให้ผู้ใช้รีวิวทิศทาง เนื้อหา และ style ก่อนลงมือสร้างไฟล์จริง

แบบฝึกหัดถัดไป: [Exercise 04: สร้าง Custom Skill](../04-create-custom-skill/README.md)
