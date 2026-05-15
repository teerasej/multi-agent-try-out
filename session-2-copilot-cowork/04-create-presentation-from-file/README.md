# Exercise 04: สร้าง Presentation จาก Decision Log และ Tracker

🔑 ต้องการ M365 Copilot License
🔑 ต้องเปิดใช้งาน Cowork (Frontier preview)

แบบฝึกหัดนี้จะต่อ workflow จากสองข้อก่อนหน้า โดยให้ Cowork ใช้ไฟล์ Decision Log และไฟล์ action tracker เพื่อสร้าง **PowerPoint Presentation สำหรับสรุปความคืบหน้า** ที่พร้อมใช้คุยกับหัวหน้าหรือทีมต่อได้ทันที

---

## ไฟล์ที่ต้องการ

ใช้ไฟล์ 2 ชุดที่ได้จาก exercise ก่อนหน้า:

- ไฟล์ Word Decision Log จาก Exercise 02
- ไฟล์ Excel action tracker จาก Exercise 03

> **⚠️ หมายเหตุ:** ถ้าหาไฟล์ที่ Cowork สร้างไว้ไม่เจอ ให้แนบไฟล์ `meeting-notes.docx` แทนได้ แต่ถ้าใช้ไฟล์จาก exercise ก่อนหน้า จะเห็น workflow ต่อเนื่องชัดกว่า

---

## Feature 1: แนบไฟล์และสร้าง Presentation

1. เปิด Cowork Chat ใหม่

2. กดปุ่ม **+** (Add attachment) ในช่อง Prompt เพื่อแนบไฟล์ Word Decision Log และไฟล์ Excel action tracker

3. หลังจากแนบไฟล์แล้ว พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   จากไฟล์ที่แนบมา ช่วยสร้าง PowerPoint Presentation สำหรับสรุปความคืบหน้าในการประชุม โดยแบ่งเป็น 4 สไลด์: 
   1) ภาพรวม 
   2) decisions สำคัญ 
   3) action items ที่ต้องติดตาม 
   4) next steps
   ```
   หรือจะใช้วิธีพิมพ์ชื่อไฟล์ที่ได้จาก Exercise 02 และ 03 แทนแบบด้านล่างก็ได้:

   ```
   จาก [ชื่อไฟล์ที่ได้จาก Exercise 02] และ [ชื่อไฟล์ที่ได้จาก Exercise 03] ช่วยสร้าง PowerPoint Presentation สำหรับสรุปความคืบหน้าในการประชุม โดยแบ่งเป็น 4 สไลด์: 
   1) ภาพรวม 
   2) decisions สำคัญ 
   3) action items ที่ต้องติดตาม 
   4) next steps
   ```
   หรืออาจจะลองใช้วิธีพิมพ์ Prompt แบบสั้น ๆ เช่น:

   ```
   ให้นำไฟล์ทั้ง 2 ไฟล์มาสร้าง PowerPoint Presentation สำหรับสรุปความคืบหน้าในการประชุม โดยแบ่งเป็น 4 สไลด์:
   1) ภาพรวม
   2) decisions สำคัญ
   3) action items ที่ต้องติดตาม
   4) next steps
   ```

5. สังเกตการทำงานของ Cowork:
   - Cowork จะอ่านข้อมูลจากหลายไฟล์ที่เราแนบ
   - แสดงแผนการทำงาน และระบุว่ากำลังใช้ Skill **PowerPoint**
   - ถ้ามีปุ่ม **Approve** ให้กดเพื่อยืนยัน

6. เมื่อ Cowork สร้างไฟล์เสร็จ กดที่ลิงก์ไฟล์ PowerPoint เพื่อเปิดและดู Slide ทั้ง 4

7. ตรวจสอบว่าสไลด์สรุปข้อมูลจากทั้งฝั่ง narrative และฝั่ง task list ได้เข้าใจง่าย

8. จดชื่อไฟล์ PowerPoint นี้ไว้ หรือเปิดค้างไว้ก่อน เพราะเราจะใช้ต่อใน Exercise 05

> **💡 เคล็ดลับ:** สังเกตว่า Cowork จะสรุปเฉพาะประเด็นสำคัญ ไม่ได้คัดลอกทั้งเอกสาร — นี่คือประโยชน์ของ AI ที่ช่วย "กลั่น" ข้อมูล

---

## สรุป

คุณได้ใช้ Cowork รวมข้อมูลจากหลายไฟล์แล้วเปลี่ยนเป็น Presentation ที่พร้อมใช้ต่อในการสื่อสารแล้ว ในแบบฝึกหัดสุดท้าย เราจะใช้ไฟล์ที่สร้างมาทั้งหมดต่อเพื่อร่าง follow-up email แบบหลายขั้นตอน

---

แบบฝึกหัดถัดไป: [Exercise 05: งานหลายขั้นตอน — ร่าง Follow-up Email จากไฟล์ที่สร้างไว้](../05-multi-step-email/README.md)
