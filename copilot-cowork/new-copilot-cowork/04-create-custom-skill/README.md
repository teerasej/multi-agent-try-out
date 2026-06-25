# Exercise 04: สร้าง Custom Skill สำหรับ Executive Brief

🔑 ทำข้อนี้เมื่อเมนู **Customize** และการสร้าง Skills ปรากฏใน tenant

ในแบบฝึกหัดนี้ เราจะสร้าง Custom Skill ชื่อ `Service Recovery Executive Brief` เพื่อกำหนดรูปแบบ executive brief ที่ใช้ซ้ำได้ แทนการเริ่มเขียน Prompt ใหม่ทุกครั้ง

> ⚠️ Skill ที่สร้างจะพร้อมใช้งานใน **conversation ใหม่** ดังนั้น Exercise นี้จบ workflow task เดิมอย่างตั้งใจ

---

## Feature 1: สร้าง Skill ผ่าน Customize

1. เปิด **Customize** จากเมนู Cowork แล้วเลือก **Skills**

2. เลือก **Add** > **Create new**

3. เมื่อตัวช่วยถามรายละเอียด ให้ใช้ข้อมูลนี้:

   ```
   Name: Service Recovery Executive Brief

   Description: Creates a concise Thai executive brief from service incident evidence.

   Instructions:
   When the user provides service incident documents, create a Thai executive brief with these sections:
   - Current situation and service status
   - Customer and business impact
   - Confirmed actions, owners and due times
   - Decisions required
   - Facts, working hypotheses and unknowns

   Use only supplied evidence. Never present a working hypothesis as a confirmed root cause.
   Use TBD or Not confirmed when evidence is missing.
   Do not send email, post Teams messages, create meetings, or change external systems.
   ```

4. ตรวจชื่อ คำอธิบาย และ instructions ก่อนยืนยันให้ Cowork บันทึก Skill

---

## Feature 2: เปิด conversation ใหม่และทดลองใช้ Skill

1. เลือก **+ New Task** เพื่อเริ่ม conversation ใหม่

2. แนบ `service-incident-timeline.docx` แล้วส่ง Prompt นี้:

   ```
   ใช้ Service Recovery Executive Brief กับไฟล์ที่แนบมา
   สร้าง executive brief ภาษาไทยไม่เกิน 1 หน้า สำหรับผู้บริหาร
   ```

3. เปิด Side panel และตรวจว่า Skill ปรากฏในส่วน **Skills**

4. ตรวจผลลัพธ์:

   - [ ] มี 5 ส่วนตามรูปแบบที่กำหนด
   - [ ] แยก Facts, Working hypotheses และ Unknowns ชัดเจน
   - [ ] ไม่มี action ภายนอกเกิดขึ้นเอง

> หากไม่มี Customize หรือองค์กรปิดการสร้าง custom skill ให้ Facilitator สาธิตจากหน้าจอของตน และข้ามไป Exercise 05 โดยไม่ต้องสร้าง Skill แบบ manual

---

## สรุป

พวกเราได้สร้างมาตรฐานการเขียน executive brief ที่ Cowork ค้นพบและใช้ซ้ำได้ใน conversation ใหม่

แบบฝึกหัดถัดไป: [Exercise 05: ฝึก Safe calendar action](../05-safe-calendar-action/README.md)
