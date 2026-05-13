# Exercise 05: สร้าง Custom Prompt สำหรับงานที่ทำซ้ำบ่อย

🔑 ใช้ได้ทั้ง GitHub Copilot Free และ Pro

`Custom Prompt` ช่วยให้เราเก็บ prompt ที่ใช้ซ้ำบ่อยไว้เป็นไฟล์ `.prompt.md` แล้วเรียกใช้จาก slash command ได้ทันที ในแบบฝึกหัดนี้เราจะสร้าง prompt ที่ช่วยแปลงไอเดียฟีเจอร์สั้น ๆ ให้กลายเป็น prompt ที่พร้อมใช้ต่อกับ Plan Mode หรือ Agent Mode

---

## Feature 1: สร้าง Prompt file

1. ใน root ของ note app สร้างโฟลเดอร์ `.github/prompts`
2. สร้างไฟล์ `.github/prompts/feature-request-refiner.prompt.md`
3. วางเนื้อหาด้านล่างลงไปในไฟล์:

   ```markdown
   ---
   name: "Feature Request Refiner"
   description: "Turn a short feature idea into a build-ready implementation prompt for the Next.js note app"
   argument-hint: "Describe the feature idea"
   agent: "ask"
   ---

   Turn the user's short feature request into a build-ready prompt for GitHub Copilot.

   Return these sections:
   1. Goal
   2. User-facing behavior
   3. Files to inspect first
   4. Acceptance criteria
   5. Validation checklist

   Keep the result concise and tailored to this Next.js note app.
   Prefer inspecting these files first when relevant:
   - app/page.tsx
   - components/NoteCard.tsx
   - components/NoteEditor.tsx
   - lib/notes.ts
   ```

4. กด Save แล้วสังเกตว่าเราได้ reusable prompt ที่เรียกใช้ซ้ำได้จาก Chat โดยไม่ต้องพิมพ์ prompt ยาวใหม่ทุกครั้ง

> **💡 เคล็ดลับ:** จุดเด่นของ `.prompt.md` คือเหมาะกับงานเดี่ยวที่ชัดเจนมาก ๆ เช่น ช่วย refine requirement, สร้าง test cases, หรือเขียน README จากข้อมูลตั้งต้น

---

## Feature 2: เรียกใช้ Prompt ผ่าน slash command

1. เปิด Copilot Chat แล้วพิมพ์ `/`
2. เลือก prompt ชื่อ **Feature Request Refiner**
3. เมื่อ Copilot ขอ input ให้พิมพ์หรือวางตัวอย่างด้านล่าง:

   ```
   Add note color labels with 4 preset colors and show the selected color on each note card.
   ```

4. สังเกตผลลัพธ์ที่ได้:
   - มี Goal ชัดเจน
   - บอกไฟล์ที่ควรเปิดดูก่อน
   - มี Acceptance criteria
   - มี Validation checklist พร้อมใช้ต่อ

5. ลอง copy ผลลัพธ์ที่ได้ไปใช้ต่อใน Plan Mode หรือ Agent Mode แล้วเปรียบเทียบกับการพิมพ์ prompt สดเอง

> **⚠️ หมายเหตุ:** ถ้า prompt ยังไม่แสดงในรายการ slash command ให้ลอง Save ไฟล์อีกครั้ง หรือเริ่ม chat ใหม่หนึ่งรอบ

---

## สรุป

คุณได้สร้าง `Custom Prompt` สำหรับงานที่ทำซ้ำบ่อยแล้ว จุดแข็งของวิธีนี้คือเราสามารถเก็บ prompt คุณภาพดีไว้ใช้ซ้ำทั้งทีมได้ และช่วยให้การเริ่มต้นงานใหม่เร็วขึ้นมาก ในแบบฝึกหัดถัดไป เราจะขยับไปอีกระดับด้วยการสร้าง `Skill` สำหรับ workflow ที่ซ้ำกันทั้งโปรเจกต์

---

แบบฝึกหัดถัดไป: [Exercise 06: สร้าง Skill สำหรับ workflow ของโปรเจกต์](../06-custom-skill/README.md)
