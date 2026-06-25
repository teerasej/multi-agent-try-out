# Exercise 08: Commit, Push และสร้าง Pull Request

🔑 ใช้ได้ทั้ง GitHub Copilot Free และ Pro

แบบฝึกหัดสุดท้ายของ Session นี้ — หลังจากเราได้ลองทั้ง Agent Mode, `Custom Prompt`, `Skill` และ `Custom Agent` แล้ว เราจะให้ Copilot ช่วย Commit การเปลี่ยนแปลงทั้งหมด, Push ไปยัง Repository ของเรา แล้วสร้าง Pull Request บน GitHub

---

## Practice 1: Commit การเปลี่ยนแปลงผ่าน Copilot

1. ใน Copilot Chat panel ตรวจสอบว่า Mode ยังเป็น **Agent** อยู่
2. กดปุ่ม (←) ด้านบนซ้ายของช่อง Chat เพื่อย้อนกลับไปยังหน้ารวม Session จะเห็นรายการของ Session Chat ที่เราคุยกับ Copilot มาแล้วทั้งหมด 

3. ลงมาในช่อง Prompt ด้านล่าง พิมพ์หรือก้อปปี้ และวาง Prompt ด้านล่างลงไป แล้วกด Enter:

   ```
   1. Create a branch
   2. Stage all changes and create a commit with an appropriate commit message describing the features we added.
   ```

4. Copilot จะ:
   - สร้าง Branch ใหม่ให้โดยอัตโนมัติ (เช่น `feature/pin-note`)
   - Stage ไฟล์ที่เปลี่ยนแปลงทั้งหมด
   - สร้าง Commit message ที่สอดคล้องกับงานที่ทำ
   - แสดงคำสั่ง `git commit` ให้ Confirm

5. ถ้า Copilot ขอ Confirm ก่อนรัน Terminal command ให้กด **Continue**

---

## Practice 2: Push ไปยัง GitHub

1. พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   Push the committed changes to the remote repository.
   ```

2. Copilot จะรัน `git push` ให้อัตโนมัติ — ถ้าขอ Confirm ให้กด **Continue**

3. สังเกต Output ใน Terminal ว่า Push สำเร็จ

---

## Practice 3: สร้าง Pull Request บน GitHub

1. กลับไปที่ Copilot Chat panel แล้วพิมพ์หรือวาง Prompt ด้านล่าง จากนั้นกด Enter:

   ```
   Create pull request to merge this branch into the origin repo's main branch. Summarize a useful information for its description in Thai
   ```

2. Copilot จะเตรียมการสร้าง Pull Request ให้ โดยอาจแสดงรายละเอียด Title และ Description ที่สรุปจากงานที่เราทำไว้

3. ถ้า Copilot ขอ Confirm ก่อนดำเนินการ ให้กด **Continue**

4. เมื่อสร้างเสร็จแล้ว Copilot มักจะแสดงลิงก์หรือแจ้งว่า Pull Request ถูกสร้างเรียบร้อย ให้สังเกตหมายเลข PR หรือ URL ที่ได้


> **💡 เคล็ดลับ:** ถ้า Copilot แสดงลิงก์ PR มาให้แล้ว พวกเราสามารถกดลิงก์นั้นเพื่อเปิดหน้า Pull Request บน GitHub ได้ทันที

---

## สรุป

เยี่ยมมาก! พวกเราผ่านทุกแบบฝึกหัดของ Session 1 แล้ว:

- ✅ Fork Repo และเปิด Codespaces
- ✅ ใช้ Copilot Chat อธิบาย Architecture
- ✅ ใช้ Plan Mode วางแผนฟีเจอร์
- ✅ ใช้ Agent Mode เพิ่มฟีเจอร์ Pin Note
- ✅ สร้าง Custom Prompt สำหรับงานที่ทำซ้ำบ่อย
- ✅ สร้าง Skill สำหรับ workflow ของโปรเจกต์
- ✅ สร้าง Custom Agent สำหรับ Code Review
- ✅ Commit, Push และสร้าง Pull Request

GitHub Copilot Agent Mode ช่วยให้เราโฟกัสกับ **ไอเดีย** ได้มากขึ้น โดยปล่อยให้ AI จัดการขั้นตอนที่ซ้ำซาก
