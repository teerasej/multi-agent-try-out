# Exercise 06: สร้าง Skill สำหรับ workflow ของโปรเจกต์

🔑 ใช้ได้ทั้ง GitHub Copilot Free และ Pro

`Skill` เหมาะกับงานที่มีขั้นตอนซ้ำ ๆ และต้องอาศัยความรู้เฉพาะของโปรเจกต์ เช่น ต้องเปิดไฟล์ไหนก่อน, ควรเปลี่ยนโค้ดแบบไหน, และควร validate อย่างไร ในแบบฝึกหัดนี้เราจะสร้าง skill ที่ช่วย Copilot เพิ่มฟีเจอร์เล็ก ๆ ให้ note app อย่างเป็นระบบ

---

## Practice 1: สร้าง SKILL.md

1. คัดลอกชื่อและที่อยู่ไฟล์ด้านล่างนี้ไว้:

   ```
   .github/skills/small-note-feature/SKILL.md
   ```
2. คลิกขวาในพื้นที่ว่างใน VS Code Explorer แล้วเลือก **New File**
3. วางชื่อไฟล์ที่คัดลอกไว้ลงไป แล้วกด Enter เพื่อสร้างไฟล์ใหม่ ตามที่อยู่ที่ระบุไว้
4. ในไฟล์ `SKILL.md` ที่สร้างขึ้นมาใหม่ ให้ copy และวางเนื้อหาด้านล่างลงไป:

   ```markdown
   ---
   name: small-note-feature
   description: "Add small features to the Next.js note app. Use for note counter, empty state message, list sorting, and small UI behavior changes."
   argument-hint: "Describe the small note app Practice you want to add"
   ---

   # Small Note Feature

   Use this skill when you need to add a small Practice to the Next.js note app without changing the overall architecture.

   ## Procedure
   1. Inspect these files first when relevant:
      - app/page.tsx
      - components/NoteCard.tsx
      - components/NoteEditor.tsx
      - lib/notes.ts
   2. Keep the existing UI and naming style consistent.
   3. Prefer the smallest possible change that satisfies the request.
   4. After editing, run `npm run lint` before finishing.
   5. Summarize what changed and how to verify it in the browser.
   ```

5. กด Save แล้วสังเกตว่า skill นี้ไม่ได้มีไว้แค่ “สั่งงาน 1 ครั้ง” แต่เป็นการสอน workflow ให้ Copilot ใช้ซ้ำกับงานแนวเดิมใน repo นี้

> **💡 เคล็ดลับ:** จุดเด่นของ skill คือเก็บทั้งคำอธิบาย ขั้นตอน และกติกาเฉพาะโปรเจกต์ไว้ด้วยกัน ทำให้เหมาะกับงานที่ทีมทำซ้ำบ่อย

---

## Practice 2: เรียกใช้ Skill กับงานจริง

1. เปิด Copilot Chat แล้วพิมพ์ `/`
2. เลือก skill ชื่อ **small-note-feature**
3. พิมพ์หรือวางตัวอย่างงานด้านล่าง:

   ```
   Add an empty state message when there are no notes. Keep the current layout and styling consistent.
   ```

4. สังเกตว่า Copilot จะมีแนวโน้ม:
   - เปิดไฟล์ที่เกี่ยวข้องก่อน
   - ทำ change แบบเล็กและตรงจุด
   - รักษา style ของโปรเจกต์เดิม
   - รัน `npm run lint` ก่อนสรุปงาน

5. เมื่อเสร็จแล้ว ลองเปิดหน้าแอปเพื่อดูว่า empty state แสดงผลถูกต้องตามที่สั่งไว้

> **⚠️ หมายเหตุ:** skill สามารถถูกเรียกแบบอัตโนมัติได้ด้วย ถ้า task ตรงกับ description ที่เราเขียนไว้ แต่ใน workshop นี้ให้เริ่มจาก slash command จะสังเกต behavior ได้ง่ายกว่า

---

## สรุป

พวกเราได้สร้าง `Skill` ที่บอก Copilot ว่าควรทำงานแบบไหนกับ note app เมื่อเจองานประเภทเดิมซ้ำอีก จุดแข็งของ skill คือเหมาะกับ workflow ที่มีหลายขั้นตอนและมีความรู้เฉพาะ repo ในแบบฝึกหัดถัดไป เราจะสร้าง `Custom Agent` เพื่อให้ Copilot รับบทบาทเฉพาะทางชัดเจนขึ้น

---

แบบฝึกหัดถัดไป: [Exercise 07: สร้าง Custom Agent สำหรับ Code Review](../07-custom-agent/README.md)
