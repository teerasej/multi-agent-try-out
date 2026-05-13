# Exercise 05: Commit, Push และสร้าง Pull Request

🔑 ใช้ได้ทั้ง GitHub Copilot Free และ Pro

แบบฝึกหัดสุดท้ายของ Session นี้ — เราจะให้ Copilot ช่วย Commit การเปลี่ยนแปลงทั้งหมด, Push ไปยัง Repository ของเรา แล้วสร้าง Pull Request บน GitHub

---

## Feature 1: Commit การเปลี่ยนแปลงผ่าน Copilot

1. ใน Copilot Chat panel ตรวจสอบว่า Mode ยังเป็น **Agent** อยู่

2. พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   Stage all changes and create a commit with an appropriate commit message describing the features we added.
   ```

3. Copilot จะ:
   - Stage ไฟล์ที่เปลี่ยนแปลงทั้งหมด
   - สร้าง Commit message ที่สอดคล้องกับงานที่ทำ
   - แสดงคำสั่ง `git commit` ให้ Confirm

4. ถ้า Copilot ขอ Confirm ก่อนรัน Terminal command ให้กด **Continue**

---

## Feature 2: Push ไปยัง GitHub

1. พิมพ์หรือวาง Prompt ด้านล่าง แล้วกด Enter:

   ```
   Push the committed changes to the remote repository.
   ```

2. Copilot จะรัน `git push` ให้อัตโนมัติ — ถ้าขอ Confirm ให้กด **Continue**

3. สังเกต Output ใน Terminal ว่า Push สำเร็จ

---

## Feature 3: สร้าง Pull Request บน GitHub

1. เปิด Tab ใหม่ในเบราว์เซอร์ แล้วไปที่ Repository ที่คุณ Fork ไว้:

   `https://github.com/[ชื่อ Account ของคุณ]/nextjs-notes-app`

2. GitHub จะแสดง Banner **"Compare & pull request"** — กดปุ่มนั้น

   ![Compare and pull request banner](./assets/github-pr-banner.png)

3. ตรวจสอบ Title และ Description ของ Pull Request แล้วกด **Create pull request**

4. ดูหน้า Pull Request ที่สร้างขึ้น — กด Tab **Files changed** เพื่อดูไฟล์ที่มีการเปลี่ยนแปลง

> **💡 เคล็ดลับ:** ใน Copilot Chat ลองพิมพ์ `Create a pull request` — Copilot บางเวอร์ชันสามารถสร้าง PR ให้ผ่าน Chat ได้โดยตรง

---

## สรุป

เยี่ยมมาก! คุณผ่านทุกแบบฝึกหัดของ Session 1 แล้ว:

- ✅ Fork Repo และเปิด Codespaces
- ✅ ใช้ Copilot Chat อธิบาย Architecture
- ✅ ใช้ Plan Mode วางแผนฟีเจอร์
- ✅ ใช้ Agent Mode เพิ่มฟีเจอร์ Pin Note
- ✅ Commit, Push และสร้าง Pull Request

GitHub Copilot Agent Mode ช่วยให้เราโฟกัสกับ **ไอเดีย** ได้มากขึ้น โดยปล่อยให้ AI จัดการขั้นตอนที่ซ้ำซาก
