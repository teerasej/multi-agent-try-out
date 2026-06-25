# Exercise 02: สำรวจโปรเจกต์ด้วย Copilot Chat

🔑 ใช้ได้ทั้ง GitHub Copilot Free และ Pro

แบบฝึกหัดนี้จะใช้ **Copilot Chat** เพื่อถามให้ AI อธิบายสถาปัตยกรรมของโปรเจกต์ให้ฟัง — เหมาะมากสำหรับการทำความเข้าใจ Codebase ใหม่ ๆ อย่างรวดเร็ว

---

## Feature 1: เปิด Copilot Chat และเลือก Model

1. ใน Codespaces กดไอคอน **GitHub Copilot** ที่ Sidebar ด้านซ้าย (ไอคอนรูปดาวหรือฟองคำพูด) เพื่อเปิด Chat panel

2. ในช่อง Chat กดที่ชื่อ Model (Auto) ด้านล่างสุด เพื่อเปิด Dropdown เลือก Model

3. คลิกเลือก Model ที่ต้องการ เช่น **Claude Haiku**, **Claude Sonnet** หรือ **GPT-4o** 

> **💡 เคล็ดลับ:** ถ้าเห็น **Reasoning** option ให้ลองเปิดดู — Copilot จะคิดวิเคราะห์ลึกขึ้น เหมาะกับโจทย์ที่ซับซ้อน

---

## Feature 2: ถามให้ Copilot อธิบาย Architecture

1. ในช่อง Chat ให้พิมพ์หรือวาง Prompt ด้านล่างแล้วกด Enter:

   ```
   Explain the overall architecture of this project. What are the main files and what does each one do? Response in Thai
   ```

2. รอสักครู่ — Copilot จะอ่านไฟล์ในโปรเจกต์และอธิบายให้ฟัง

3. ลองอ่านคำอธิบาย สังเกตว่า Copilot จะระบุชื่อไฟล์และหน้าที่ของแต่ละส่วน เช่น `app/page.tsx`, `components/NoteCard.tsx`, `lib/notes.ts`

> **💡 เคล็ดลับ:** ถ้าอยากรู้เพิ่มเติมเกี่ยวกับไฟล์ใดไฟล์หนึ่ง ลองถามต่อได้เลย เช่น `What does lib/notes.ts do exactly?`

---

## สรุป

พวกเราได้ทดลองใช้ Copilot Chat เพื่อสำรวจโปรเจกต์ใหม่แบบรวดเร็วสำเร็จแล้ว ในแบบฝึกหัดถัดไป เราจะลองใช้ **Plan Mode** เพื่อวางแผนการเพิ่มฟีเจอร์ใหม่กัน

---

แบบฝึกหัดถัดไป: [Exercise 03: วางแผนฟีเจอร์ด้วย Plan Mode](../03-plan-mode/README.md)
