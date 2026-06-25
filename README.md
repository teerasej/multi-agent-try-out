# Multi-Agent Try-Out

ยินดีต้อนรับสู่ **Multi-Agent Try-Out** — งาน Hands-on สำหรับสำรวจความสามารถของ AI Agent Services ด้วยตัวเองครับ

> สำหรับผู้เข้าร่วม: ดูข้อมูลบัญชีที่เตรียมไว้ได้ที่ [provided-account.md](./provided-account.md)

Event นี้แบ่งออกเป็น 2 Track:

| Track | กลุ่มเป้าหมาย | เครื่องมือ |
|---|---|---|
| **Session 1** | นักพัฒนา (Developer) | GitHub Copilot Agent Mode + Codespaces |
| **Session 2** | ผู้ใช้งานทั่วไป (Business User) | Microsoft 365 Copilot — Cowork |

---

## Session 1 — Microsoft 365 Copilot Cowork

🔑 ต้องมี Microsoft 365 Copilot license และผู้ดูแลเปิดใช้ Cowork ให้บัญชีแล้ว

> **หมายเหตุสำหรับผู้จัดงาน:** Cowork ใช้ usage-based billing และบางความสามารถขึ้นกับนโยบาย ผู้ดูแล และภูมิภาคของ tenant ให้ทำ [Setup Checklist](./copilot-cowork/new-copilot-cowork/00-setup-checklist.md) ให้เสร็จก่อนเริ่ม Session

เวอร์ชันหลักปัจจุบัน: [Copilot Cowork — Service Recovery Workflow](./copilot-cowork/new-copilot-cowork/README.md)

| # | แบบฝึกหัด | สิ่งที่จะได้เรียนรู้ |
|---|---|---|
| 00 | [Setup Checklist](./copilot-cowork/new-copilot-cowork/00-setup-checklist.md) | ตรวจสอบ License, OneDrive และ safety boundary ของบัญชีทดสอบ |
| 01 | [เปิด Cowork และสร้าง Word output ใน OneDrive](./copilot-cowork/new-copilot-cowork/01-signin-and-agent-store/README.md) | แนบ work context, รู้จัก Side panel และแปลงคำตอบล่าสุดเป็น Word |
| 02 | [สร้าง Recovery Action Register](./copilot-cowork/new-copilot-cowork/02-create-recovery-action-register/README.md) | รวม Word output และ dashboard เพื่อสร้าง Excel action register |
| 03 | [สร้าง Executive Recovery Update](./copilot-cowork/new-copilot-cowork/03-create-executive-recovery-update/README.md) | สร้าง PowerPoint สำหรับผู้บริหารจากหลักฐานหลายไฟล์ |
| 04 | [สร้าง Custom Skill](./copilot-cowork/new-copilot-cowork/04-create-custom-skill/README.md) | กำหนดมาตรฐาน executive brief ที่ใช้ซ้ำได้ |
| 05 | [ฝึก Safe calendar action](./copilot-cowork/new-copilot-cowork/05-safe-calendar-action/README.md) | อ่าน approval card และยกเลิก action ที่ปลอดภัย |
| 06 | [ตั้ง Scheduled recovery briefing](./copilot-cowork/new-copilot-cowork/06-scheduled-recovery-briefing/README.md) | ตั้ง รัน และหยุด draft-only scheduled prompt |

---

## ไฟล์ตัวอย่างสำหรับ Session 1

ดาวน์โหลดไฟล์เหล่านี้ไว้ที่เครื่องก่อนเริ่ม Session 2 (หรือดาวน์โหลดได้จาก Exercise 01):

| ไฟล์ | ใช้ใน |
|---|---|
| 📦 [**service-recovery-files.zip** — ทุกไฟล์รวมในครั้งเดียว](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/new-copilot-cowork/files/service-recovery-files.zip) | ดาวน์โหลดและอัปโหลดขึ้น OneDrive ก่อนเริ่ม Session |
| [service-incident-timeline.docx](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/new-copilot-cowork/files/service-incident-timeline.docx) | หลักฐานเหตุการณ์และ decisions สำหรับ Exercise 01–04 |
| [service-performance-dashboard.xlsx](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/new-copilot-cowork/files/service-performance-dashboard.xlsx) | ข้อมูลตัวเลขและ recovery actions สำหรับ Exercise 02–03 |
| [executive-service-context.pptx](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/new-copilot-cowork/files/executive-service-context.pptx) | executive context สำหรับ Exercise 03 |




---


## Session 2 — GitHub Copilot Agent Mode

ใช้ได้ทั้ง GitHub Copilot Free และ Pro

| # | แบบฝึกหัด | สิ่งที่จะได้เรียนรู้ |
|---|---|---|
| 00 | [Setup Checklist](./github-copilot-agent/00-setup-checklist.md) | ตรวจสอบความพร้อมก่อนเริ่ม Session |
| 01 | [Fork Repo และเริ่ม Codespaces](./github-copilot-agent/01-fork-and-codespaces/README.md) | Fork repository และเปิด VS Code ในเบราว์เซอร์ผ่าน Codespaces |
| 02 | [สำรวจโปรเจกต์ด้วย Copilot Chat](./github-copilot-agent/02-copilot-chat-explore/README.md) | เลือก Model, ปรับ Reasoning และ Prompt ให้ Copilot อธิบาย Architecture |
| 03 | [วางแผนฟีเจอร์ด้วย Plan Mode](./github-copilot-agent/03-plan-mode/README.md) | ใช้ Plan Mode วางแผนฟีเจอร์ก่อน Start Implementation |
| 04 | [พัฒนาฟีเจอร์อัตโนมัติด้วย Agent Mode](./github-copilot-agent/04-agent-mode/README.md) | ให้ Agent Mode เพิ่มฟีเจอร์ใหม่แบบ Autonomous หลายไฟล์พร้อมกัน |
| 05 | [สร้าง Custom Prompt สำหรับงานที่ทำซ้ำบ่อย](./github-copilot-agent/05-custom-prompt/README.md) | สร้าง `.prompt.md` เพื่อแปลงไอเดียสั้น ๆ ให้เป็น prompt ที่พร้อมใช้ต่อ |
| 06 | [สร้าง Skill สำหรับ workflow ของโปรเจกต์](./github-copilot-agent/06-custom-skill/README.md) | สร้าง `SKILL.md` เพื่อสอน workflow ซ้ำ ๆ ของ note app ให้ Copilot |
| 07 | [สร้าง Custom Agent สำหรับ Code Review](./github-copilot-agent/07-custom-agent/README.md) | สร้าง `.agent.md` สำหรับ review งานก่อนเปิด Pull Request |
| 08 | [Commit, Push และสร้าง Pull Request](./github-copilot-agent/08-commit-and-pr/README.md) | ให้ Copilot ช่วย Commit, Push และสร้าง Pull Request บน GitHub |

---
