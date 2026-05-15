# Multi-Agent Try-Out

ยินดีต้อนรับสู่ **Multi-Agent Try-Out** — งาน Hands-on สำหรับสำรวจความสามารถของ AI Agent Services ด้วยตัวเองครับ 

> สำหรับผู้เข้าร่วม: ดูข้อมูลบัญชีที่เตรียมไว้ได้ที่ [provided-account.md](./provided-account.md)

Event นี้แบ่งออกเป็น 2 Track:

| Track | กลุ่มเป้าหมาย | เครื่องมือ |
|---|---|---|
| **Session 1** | นักพัฒนา (Developer) | GitHub Copilot Agent Mode + Codespaces |
| **Session 2** | ผู้ใช้งานทั่วไป (Business User) | Microsoft 365 Copilot Cowork (Frontier) |

---

## Session 1 — GitHub Copilot Agent Mode

ใช้ได้ทั้ง GitHub Copilot Free และ Pro

| # | แบบฝึกหัด | สิ่งที่จะได้เรียนรู้ |
|---|---|---|
| 00 | [Setup Checklist](./session-1-github-copilot-agent/00-setup-checklist.md) | ตรวจสอบความพร้อมก่อนเริ่ม Session |
| 01 | [Fork Repo และเริ่ม Codespaces](./session-1-github-copilot-agent/01-fork-and-codespaces/README.md) | Fork repository และเปิด VS Code ในเบราว์เซอร์ผ่าน Codespaces |
| 02 | [สำรวจโปรเจกต์ด้วย Copilot Chat](./session-1-github-copilot-agent/02-copilot-chat-explore/README.md) | เลือก Model, ปรับ Reasoning และ Prompt ให้ Copilot อธิบาย Architecture |
| 03 | [วางแผนฟีเจอร์ด้วย Plan Mode](./session-1-github-copilot-agent/03-plan-mode/README.md) | ใช้ Plan Mode วางแผนฟีเจอร์ก่อน Start Implementation |
| 04 | [พัฒนาฟีเจอร์อัตโนมัติด้วย Agent Mode](./session-1-github-copilot-agent/04-agent-mode/README.md) | ให้ Agent Mode เพิ่มฟีเจอร์ใหม่แบบ Autonomous หลายไฟล์พร้อมกัน |
| 05 | [สร้าง Custom Prompt สำหรับงานที่ทำซ้ำบ่อย](./session-1-github-copilot-agent/05-custom-prompt/README.md) | สร้าง `.prompt.md` เพื่อแปลงไอเดียสั้น ๆ ให้เป็น prompt ที่พร้อมใช้ต่อ |
| 06 | [สร้าง Skill สำหรับ workflow ของโปรเจกต์](./session-1-github-copilot-agent/06-custom-skill/README.md) | สร้าง `SKILL.md` เพื่อสอน workflow ซ้ำ ๆ ของ note app ให้ Copilot |
| 07 | [สร้าง Custom Agent สำหรับ Code Review](./session-1-github-copilot-agent/07-custom-agent/README.md) | สร้าง `.agent.md` สำหรับ review งานก่อนเปิด Pull Request |
| 08 | [Commit, Push และสร้าง Pull Request](./session-1-github-copilot-agent/08-commit-and-pr/README.md) | ให้ Copilot ช่วย Commit, Push และสร้าง Pull Request บน GitHub |

---

## Session 2 — Microsoft 365 Copilot Cowork

🔑 ต้องการ M365 Copilot License + Cowork (Frontier preview)

| # | แบบฝึกหัด | สิ่งที่จะได้เรียนรู้ |
|---|---|---|
| 00 | [Setup Checklist](./session-2-copilot-cowork/00-setup-checklist.md) | ตรวจสอบ License และความพร้อมก่อนเริ่ม Session |
| 01 | [เข้าสู่ระบบและเพิ่ม Cowork ลงใน Agent List](./session-2-copilot-cowork/01-signin-and-agent-store/README.md) | Sign in, ตรวจสอบ Plan, ดาวน์โหลดไฟล์ตัวอย่าง และเพิ่ม Cowork จาก Agent Store |
| 02 | [สร้างเอกสาร Decision Log ด้วย Cowork](./session-2-copilot-cowork/02-create-document/README.md) | ให้ Cowork แปลง meeting notes เป็น Word decision log |
| 03 | [แปลง Decision Log เป็น Task Tracker ด้วย Cowork](./session-2-copilot-cowork/03-create-spreadsheet/README.md) | ใช้ Word decision log จากข้อก่อนหน้าเพื่อสร้าง Excel action tracker |
| 04 | [สร้าง Presentation จาก Decision Log และ Tracker](./session-2-copilot-cowork/04-create-presentation-from-file/README.md) | รวมข้อมูลจาก decision log และ tracker เพื่อสร้าง PowerPoint สำหรับสรุปความคืบหน้า |
| 05 | [งานหลายขั้นตอน — ร่าง Follow-up Email จากไฟล์ที่สร้างไว้](./session-2-copilot-cowork/05-multi-step-email/README.md) | ใช้ไฟล์ที่สร้างไว้ทั้งหมดเพื่อร่าง email และเตรียม attachment พร้อม Approval controls |

---

## ไฟล์ตัวอย่างสำหรับ Session 2

ดาวน์โหลดไฟล์เหล่านี้ไว้ที่เครื่องก่อนเริ่ม Session 2 (หรือดาวน์โหลดได้จากขั้นตอนที่ 01 ด้านบน):

| ไฟล์ | ใช้ใน |
|---|---|
| 📦 [**session-2-sample-files.zip** — ทุกไฟล์รวมในครั้งเดียว](https://github.com/teerasej/multi-agent-try-out/raw/main/session-2-copilot-cowork/files/session-2-sample-files.zip) | ทุก Exercise |
| [meeting-notes.docx](https://github.com/teerasej/multi-agent-try-out/raw/main/session-2-copilot-cowork/files/meeting-notes.docx) | Exercise 02 (Decision Log) |
| [project-tasks.xlsx](https://github.com/teerasej/multi-agent-try-out/raw/main/session-2-copilot-cowork/files/project-tasks.xlsx) | Exercise 05 |
| [project-overview.pptx](https://github.com/teerasej/multi-agent-try-out/raw/main/session-2-copilot-cowork/files/project-overview.pptx) | ไฟล์อ้างอิง |
