# Exercise 04: พัฒนาฟีเจอร์อัตโนมัติด้วย Agent Mode

🄓 ใช้ได้ทั้ง GitHub Copilot Free และ Pro

**Agent Mode** คือโหมดที่ทรงพลังที่สุดของ Copilot — AI จะวางแผน แก้ไขไฟล์ รันคำสั่ง และแก้ Error ซ้ำ ๆ จนงานเสร็จโดยอัตโนมัติ ในแบบฝึกหัดนี้เราจะให้ Copilot เพิ่มฟีเจอร์ **"Pin Note"** ให้แอปของเรา

---

## Feature 1: เปิด Agent Mode

1. ใน Copilot Chat panel กดที่ Dropdown ชื่อ Mode ด้านล่างของช่อง Chat

2. เลือก **Agent**

   ![Agent mode selector](./assets/copilot-agent-mode.png)

---

## Feature 2: ให้ Copilot เพิ่มฟีเจอร์ Pin Note

1. ในช่อง Chat พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   Add a "pin note" feature. Each note card should have a pin icon button. Pinned notes should appear at the top of the notes list.
   ```

2. สังเกตการทำงานของ Copilot:
   - Copilot จะเริ่มอ่านไฟล์ที่เกี่ยวข้อง
   - แก้ไขหลายไฟล์พร้อมกัน เช่น `lib/notes.ts`, `components/NoteCard.tsx`, `app/page.tsx`
   - อาจรันคำสั่ง Terminal เพื่อตรวจสอบ

3. ถ้า Copilot ขอ Confirm ก่อนรันคำสั่ง ให้กด **Continue** เพื่อให้ดำเนินต่อ

4. เมื่อเสร็จแล้ว กลับไปดู Preview ของแอปในเบราว์เซอร์ และลอง:
   - กด Pin icon บนการ์ด Note
   - สังเกตว่า Note ที่ Pin แล้วจะขึ้นมาอยู่ด้านบนของ List

> **⚠️ หมายเหตุ:** ถ้า Copilot แก้ไขไฟล์ผิดพลาดหรือมี Error ให้รอ — Copilot จะพยายามแก้ Error เองก่อน

> **💡 เคล็ดลับ:** ลองกดที่ชื่อไฟล์ในคำตอบของ Copilot เพื่อกระโดดไปดูโค้ดที่มันแก้ไขได้เลย

---

## สรุป

คุณได้ใช้ Agent Mode ให้ Copilot เพิ่มฟีเจอร์ใหม่แบบ Autonomous ได้สำเร็จ ในแบบฝึกหัดสุดท้าย เราจะให้ Copilot ช่วย Commit และสร้าง Pull Request บน GitHub
