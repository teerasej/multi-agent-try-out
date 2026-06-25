# Exercise 07: สร้าง Custom Agent สำหรับ Code Review

🔑 ใช้ได้ทั้ง GitHub Copilot Free และ Pro

`Custom Agent` เหมาะกับงานที่ต้องมีบทบาทชัดเจน ขอบเขตชัดเจน และอาจจำกัดเครื่องมือที่ใช้ได้ ในแบบฝึกหัดนี้เราจะสร้าง agent แบบ read-only สำหรับ review งานก่อนเปิด Pull Request เพื่อให้เห็นความต่างจาก prompt และ skill อย่างชัดเจน

---

## Feature 1: สร้างไฟล์ .agent.md

1. คัดลอกชื่อและที่อยู่ไฟล์ด้านล่างนี้ไว้:

   ```
   .github/agents/code-reviewer.agent.md
   ```
2. คลิกขวาในพื้นที่ว่างใน VS Code Explorer แล้วเลือก **New File**
3. วางชื่อไฟล์ที่คัดลอกไว้ลงไป แล้วกด Enter เพื่อสร้างไฟล์ใหม่ ตามที่อยู่ที่ระบุไว้
4. วางเนื้อหาด้านล่างลงไป:

   ```markdown
   ---
   name: "Code Reviewer"
   description: "Review code changes for bug risk, naming consistency, UI regressions, and missing tests before opening a pull request"
   tools: [read, search]
   ---

   You are a careful code reviewer for the Next.js note app.

   ## Constraints
   - Do not edit files.
   - Do not suggest unrelated refactors.
   - Focus only on the current change.

   ## Review Focus
   1. Bug risk
   2. Naming consistency
   3. UI regressions
   4. Missing test coverage or missing validation steps

   ## Output Format
   - List findings from most important to least important.
   - If no issues are found, say that explicitly.
   - Write the summary in Thai.
   ```

5. กด Save แล้วสังเกตว่า agent นี้มี persona ชัด และจำกัด tools ไว้แค่ `read` กับ `search` เพื่อให้มันทำหน้าที่ reviewer อย่างเดียว

> **💡 เคล็ดลับ:** จุดเด่นของ custom agent คือเรากำหนดบทบาทและขอบเขตให้ชัดได้ เช่น reviewer, tester, doc writer หรือ security reviewer

---

## Feature 2: ใช้ Agent ตรวจงานก่อนเปิด PR

1. เปิด Copilot Chat แล้วคลิก dropdown สำหรับเลือก agent
2. เลือก **Code Reviewer**
3. พิมพ์หรือวาง prompt ด้านล่าง:

   ```
   Review the current note app changes before I open a pull request. Focus on bug risk, naming consistency, UI regressions, and missing tests.
   ```

4. สังเกตผลลัพธ์ที่ได้:
   - Copilot จะทำหน้าที่ reviewer ไม่ลงมือแก้ไฟล์
   - รายงานสิ่งที่ควรระวังเป็นลำดับ
   - ถ้าไม่พบปัญหา จะบอกชัดว่าไม่พบ issue สำคัญ

5. ลองใช้ผล review นี้ปรับงานให้เรียบร้อยก่อนเข้าสู่ขั้นตอน Commit และเปิด Pull Request

> **⚠️ หมายเหตุ:** ถ้า agent ยังไม่แสดงใน dropdown ให้ลองเริ่ม chat ใหม่ หรือเปิด agents menu ใหม่อีกครั้งหลังจาก Save ไฟล์

---

## สรุป

พวกเราได้สร้าง `Custom Agent` ที่มีบทบาทเฉพาะสำหรับ review งานก่อนเปิด PR แล้ว จุดแข็งของวิธีนี้คือเราสามารถทำให้ Copilot รับผิดชอบงานเฉพาะทางได้อย่างสม่ำเสมอ และลดโอกาสที่มันจะออกนอกขอบเขต ในแบบฝึกหัดถัดไป เราจะใช้ Copilot ช่วย Commit, Push และสร้าง Pull Request จริง

---

แบบฝึกหัดถัดไป: [Exercise 08: Commit, Push และสร้าง Pull Request](../08-commit-and-pr/README.md)
