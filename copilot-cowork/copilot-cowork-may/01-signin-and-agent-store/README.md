# Exercise 01: เปิด Cowork และสำรวจ Interface

🔑 ต้องมี Microsoft 365 Copilot license และผู้ดูแลเปิดใช้ Cowork แล้ว

ในแบบฝึกหัดแรกนี้ เราจะ Sign in ด้วยบัญชีที่ Event จัดเตรียมไว้, เปิด **Cowork** จาก Microsoft 365 Copilot, เตรียมไฟล์ตัวอย่างไว้เป็น work context และสำรวจส่วนสำคัญของหน้าจอที่จะใช้ตลอด Session

---

## ไฟล์ที่ต้องดาวน์โหลดก่อนเริ่ม

กดลิงก์ด้านล่างเพื่อดาวน์โหลดไฟล์ตัวอย่างสำหรับ Session นี้ แล้วอัปโหลดขึ้น **OneDrive** ของบัญชีทดสอบในโฟลเดอร์ที่หาเจอง่าย เช่น `Cowork workshop` ก่อนเริ่ม Exercise 02

หรือดาวน์โหลดทั้งหมดในคราวเดียว:

- 📦 **[sample-files.zip — ดาวน์โหลดทุกไฟล์ในครั้งเดียว](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/copilot-cowork-may/files/sample-files.zip)**

หรือดาวน์โหลดทีละไฟล์:

- 📄 [meeting-notes.docx — บันทึกการประชุม Q2 Planning](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/copilot-cowork-may/files/meeting-notes.docx)
- 📊 [project-tasks.xlsx — Task Tracker โปรเจกต์ Website Redesign](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/copilot-cowork-may/files/project-tasks.xlsx)
- 📑 [project-overview.pptx — Project Overview Presentation](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/copilot-cowork-may/files/project-overview.pptx)

> **💡 เคล็ดลับ:** Cowork รับไฟล์จากเครื่องได้ แต่การเก็บไฟล์ตัวอย่างไว้ใน OneDrive ทำให้เลือกเป็น work context, เปิด preview และใช้ต่อใน task ได้สะดวกกว่า

---

## Feature 1: Sign In และเปิด Cowork

1. เปิด Microsoft Edge หรือ Google Chrome แล้วไปที่ **[https://m365.cloud.microsoft](https://m365.cloud.microsoft)**

2. กด **Sign in** แล้วใช้บัญชีที่ Event จัดเตรียมให้ (รับจากผู้ดูแล) เพื่อเข้าสู่ระบบ

3. ที่ด้านบนของหน้าจอ เลือก tab **Cowork** ที่อยู่ข้าง **Chat**

4. ถ้าไม่เห็น tab Cowork ให้แจ้งผู้จัดงานทันที ไม่ต้องค้นหาใน **Agents** หรือ **Agent Store** เพราะ Cowork เป็น tab หลักของ Microsoft 365 Copilot แล้ว

## Feature 2: รู้จักหน้า Cowork

เมื่อหน้า Cowork เปิดขึ้น ให้ใช้เวลา 2–3 นาทีสังเกตส่วนต่อไปนี้:

![alt text](images/overview-cowork-workspace.png)

1. ช่องพิมพ์งานและ Suggested prompts เช่น Catch me up หรือ Prep for a meeting
2. ตัวเลือก model ที่มุมบนซ้าย — ใช้ **Auto** ตลอด workshop นี้
3. My Task: แสดงงานล่าสุดและ task ที่คุณสร้างไว้เพื่อกับไปทำต่อได้
4. Scheduled สำหรับงานที่ตั้งเวลา และ Customize สำหรับ Plugins/Skills (อาจไม่แสดงในทุก tenant)

> **⚠️ หมายเหตุ:** อย่าเปลี่ยน model, เพิ่ม Plugin หรือเปิด Browser use ใน workshop นี้ เว้นแต่ Facilitator ประกาศให้ทำ

## Feature 3: เพิ่ม Work Context และดู Side panel

1. กดปุ่ม **+ New Task** จากเมนู Cowork ด้านซ้ายบน เพื่อสร้าง task สั้น ๆ จากช่องพิมพ์ prompt บนหน้า Cowork
   ![alt text](images/cowork-new-task.png)
2. กดปุ่ม **Add attachments** แล้วเลือกไฟล์ `meeting-notes.docx` จาก OneDrive ที่เตรียมไว้ (หรืออัปโหลดจากเครื่องก็ได้) เพื่อให้ Cowork ใช้เป็น work context
   ![alt text](images/cowork-add-attachement-upload-image-files.png)
   จะมีตตัวเลือกดังนี้
   - เลือก **Add work context** เมื่อจะอ้างอิงไฟล์, บุคคล, อีเมล, Teams chat/channel หรือ meeting ในองค์กร
   - เลือก **Attach cloud files** เมื่อต้องการเลือกจาก OneDrive, SharePoint หรือ Teams
   - เลือก **Upload images and files** เมื่อต้องการแนบจากเครื่องโดยตรง

3. คัดลอกข้อความทดสอบด้านล่างมาใช้:

   ```
   จากไฟล์ที่แนบมา สรุป 3 ประเด็นสำคัญเป็นรายการ bullet 
   ```

4. ระหว่าง Cowork ทำงาน ให้เปิด Side panel ด้านขวาและสังเกต:
   ![alt text](images/cowork-side-panel.png)
   - **Reference** สำหรับไฟล์ที่แนบมา
   - **Progress** และขั้นตอนการทำงาน
   - **Input** สำหรับไฟล์ต้นทาง และ **Output** สำหรับไฟล์ที่ Cowork สร้าง
   - **Skills** ที่ Cowork โหลดมาใช้
   - **Permissions** และ **Schedule** ถ้ามี

5. เมื่อได้ผลลัพธ์แล้ว ให้เปิด task นี้จาก Tasks/Search อีกครั้ง เพื่อยืนยันว่าคุณสามารถกลับมาทำงานต่อจาก task เดิมได้
   ![alt text](images/cowork-my-task.png)
---

## สรุป

คุณได้เปิด Cowork จาก tab ที่ถูกต้อง, เตรียม work context และรู้จัก Side panel แล้ว **ให้เก็บ task นี้ไว้** เพราะ Exercise 02–05 จะทำต่อใน task เดียวกัน

---

แบบฝึกหัดถัดไป: [Exercise 02: สร้างเอกสาร Decision Log ด้วย Cowork](../02-create-document/README.md)
