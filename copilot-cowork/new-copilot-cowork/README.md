# Copilot Cowork — Service Recovery Workflow

Workshop นี้ใช้สถานการณ์จำลอง **Customer Digital Platform service recovery** เพื่อให้เห็นการทำงานแบบต่อเนื่องของ Cowork ตั้งแต่หลักฐานที่กระจัดกระจาย ไปจนถึง Word, Excel, PowerPoint, Custom Skill, Action approval และ Scheduled prompt

> ข้อมูล ชื่อบุคคล และองค์กรใน workshop นี้เป็นข้อมูลสมมติทั้งหมด ใช้เพื่อการเรียนรู้เท่านั้น

## กำหนดการแนะนำ

| เวลา | กิจกรรม |
|---|---|
| 09:30–09:40 | Welcome และภาพรวม Cowork |
| 09:40–10:00 | Exercise 01 — Work context และ Word output ใน OneDrive |
| 10:00–10:15 | Exercise 02 — Excel Recovery Action Register |
| 10:15–10:30 | Exercise 03 — Executive Recovery Update |
| 10:30–10:45 | Break |
| 10:45–11:00 | Exercise 04 — Custom Skill |
| 11:00–11:10 | Exercise 05 — Safe calendar action และ approval |
| 11:10–11:20 | Exercise 06 — Scheduled recovery briefing |
| 11:20–11:25 | Review และ next steps |

## ลำดับแบบฝึกหัด

| # | แบบฝึกหัด | สิ่งที่จะได้เรียนรู้ |
|---|---|---|
| 00 | [Setup Checklist](./00-setup-checklist.md) | ตรวจสิทธิ์ Cowork และความพร้อมของบัญชีทดสอบ |
| 01 | [เปิด Cowork และสร้าง Word output ใน OneDrive](./01-signin-and-agent-store/README.md) | แนบ work context, ดู Side panel และแปลงคำตอบล่าสุดเป็น Word |
| 02 | [สร้าง Recovery Action Register](./02-create-recovery-action-register/README.md) | ใช้ Word output และ dashboard เพื่อสร้าง Excel action register |
| 03 | [สร้าง Executive Recovery Update](./03-create-executive-recovery-update/README.md) | รวม Word, Excel และ PowerPoint context เป็นสไลด์ผู้บริหาร |
| 04 | [สร้าง Custom Skill](./04-create-custom-skill/README.md) | กำหนดมาตรฐาน executive brief ที่ใช้ซ้ำได้ |
| 05 | [ฝึก Safe calendar action](./05-safe-calendar-action/README.md) | ตรวจ approval card ของ action ที่ไม่มีผู้รับภายนอก |
| 06 | [ตั้ง Scheduled recovery briefing](./06-scheduled-recovery-briefing/README.md) | ตั้ง รัน และควบคุม draft-only schedule |

## ไฟล์ตัวอย่าง

ดาวน์โหลดไฟล์ทั้งหมดและอัปโหลดขึ้น OneDrive ของบัญชีทดสอบในโฟลเดอร์ `Cowork workshop` ก่อนเริ่ม Exercise 01

- 📦 [service-recovery-files.zip — ดาวน์โหลดทุกไฟล์](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/new-copilot-cowork/files/service-recovery-files.zip)
- 📄 [service-incident-timeline.docx](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/new-copilot-cowork/files/service-incident-timeline.docx)
- 📊 [service-performance-dashboard.xlsx](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/new-copilot-cowork/files/service-performance-dashboard.xlsx)
- 📑 [executive-service-context.pptx](https://github.com/teerasej/multi-agent-try-out/raw/main/copilot-cowork/new-copilot-cowork/files/executive-service-context.pptx)

## Safety boundary

- ใช้บัญชีทดสอบที่ผู้จัดงานกำหนดเท่านั้น
- ห้ามส่งอีเมล โพสต์ Teams หรือเชิญผู้เข้าร่วมประชุมจริง
- ให้ตรวจ preview และ approval ทุกครั้ง แล้วเลือก Cancel ใน Exercise 05
- Scheduled prompt ต้องเป็น draft-only และต้อง pause/delete หลังทดลอง

Microsoft guidance was validated on 25 June 2026: [Get started with Cowork](https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/get-started) and [Use Cowork](https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/use-cowork).
