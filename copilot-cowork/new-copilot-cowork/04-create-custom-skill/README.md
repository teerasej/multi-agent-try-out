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

5. หลังจาก Cowork สร้าง Skill เสร็จ ให้กดดูไฟล์ Markdown ของ Skill ที่ปรากฏใน **Output** เพื่อยืนยันว่า instructions ถูกบันทึกครบถ้วน

6. กด Open in OneDrive เพื่อดูไฟล์ Markdown ของ Skill ใน OneDrive 
7. ตรวจสอบว่า Cowork บันทึก Skill ไว้ในโฟลเดอร์ `My Files/Document/Cowork/Skills` แล้ว
---

## Feature 2: เปิด conversation ใหม่และทดลองใช้ Skill

1. เลือก **+ New Task** เพื่อเริ่ม conversation ใหม่

2. แนบ `service-incident-timeline.docx` แล้วส่ง Prompt นี้:

   ```
   สร้าง executive brief ภาษาไทยไม่เกิน 1 หน้า สำหรับผู้บริหาร
   ```
   
> 💡 Tips #1: เราสามารถใช้ prompt ชี้นำเพื่อให้ Cowork เลือกใช้ skill ได้ เช่น 
> ```
> ใช้ Service Recovery Executive Brief กับไฟล์ที่แนบมา
> ```

> 💡 Tips #2: หรือเราสามารถพิมพ์ `/` เพื่อเลือก skill ลงในช่อง prompt โดยตรงก็ได้

1. เปิด Side panel และตรวจว่า Skill ที่เราสร้างขึ้น ถูกใช้ และปรากฏในส่วน **Skills**

2. ตรวจผลลัพธ์:

   - [ ] มี 5 ส่วนตามรูปแบบที่กำหนด
   - [ ] แยก Facts, Working hypotheses และ Unknowns ชัดเจน
   - [ ] ไม่มี action นอกเหนือจากการทำงาน

> หากไม่มี Customize หรือองค์กรปิดการสร้าง custom skill ให้ดูผมสาธิต และข้ามไป Exercise 05 โดยไม่ต้องสร้าง Skill แบบ manual

---

## สรุป

พวกเราได้สร้าง skill การเขียน executive brief ที่ Cowork ค้นพบและใช้ซ้ำได้ใน conversation ใหม่

แบบฝึกหัดถัดไป: [Exercise 05: ฝึก Safe calendar action](../05-safe-calendar-action/README.md)
