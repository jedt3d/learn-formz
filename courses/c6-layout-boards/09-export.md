---
title: "9. ส่งออก PDF + อัปเดตโมเดล"
parent: "C6 · Brand & Presentation Boards"
nav_order: 9
chapter: true
read_time: 4
do_time: 5
permalink: /courses/c6-layout-boards/09-export/
---

# 9. ส่งออก PDF + อัปเดตโมเดล
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทดลอง **แก้โมเดล → board อัปเดต** (เวทมนตร์ของ frame ที่ลิงก์อยู่)
- พิมพ์หรือบันทึกเป็น **PDF** 2 หน้า
- เตรียมไฟล์ภาพ PNG สำหรับ portfolio ออนไลน์

## 👣 ลงมือทำ (5 นาที)
### A. แก้แล้วอัปเดต (2 นาที)
1. เปิด `C3_Kettle.fmz` แล้วแก้ฟอร์มเล็กน้อย (เช่น ยืด Spout ด้วย Move จุดของหน้าตัด S3 หรือเปลี่ยน diameter ของหูแก้ว) แล้ว **บันทึก**
2. กลับไปที่ layout: frame ที่ลิงก์ไฟล์นั้นจะต้อง **regenerate** ใช้คำสั่ง update/regenerate ของ frame (คลิกขวาที่ frame)
3. ดูว่า Front/Right/Top เปลี่ยนตาม ส่วน **ภาพเรนเดอร์ (Place Image)** จะไม่เปลี่ยน จนกว่าจะเรนเดอร์ใหม่

### B. PDF (3 นาที)
4. ส่วนพิมพ์ของ Layout → **Print Settings** เลือก A3 → **Print** → ในหน้าต่างพิมพ์ของระบบ เลือก **Save as PDF** (macOS) หรือ **Microsoft Print to PDF** (Windows)
5. ตั้งชื่อ `C6_KitchenSet_Boards.pdf` (2 หน้า)
6. สำหรับเว็บ/social: เปิด PDF แล้ว export หน้าละ 1 PNG

{: .shot }
[SCREENSHOT: คำสั่ง update/regenerate frame ใน context menu]
{: .shot }
[SCREENSHOT: หน้าพิมพ์ (Print Settings / Print)]

{: .verify }
ชื่อคำสั่ง **regenerate/update frame** และเมนูที่เปิดหน้าพิมพ์ของ Layout (File > Print... หรือคำสั่งอื่น) ใน v10 ต้องยืนยัน (คู่มือบอกปุ่ม Print Settings และ Print ที่ส่งไปเครื่องพิมพ์หรือ PDF)

{% include homework.html id="c6-workshop" title="C6 · Kitchen Set Boards" what="PDF/PNG ของ board 2 แผ่น + ภาพ thumbnail ที่ร่างด้วยมือ" %}

## ✅ เช็คตัวเอง
<details><summary>1. อะไรอัปเดตเองเมื่อแก้โมเดล และอะไรไม่อัปเดต?</summary>frame (หลัง regenerate) อัปเดต ส่วนภาพเรนเดอร์ต้องเรนเดอร์ใหม่</details>
<details><summary>2. ทำ PDF จาก Layout อย่างไร?</summary>Print → เลือก PDF ในหน้าต่างพิมพ์ของระบบ</details>
<details><summary>3. ทำไมต้องบันทึกโมเดลก่อน regenerate?</summary>เพราะ frame อ่านจากไฟล์ที่บันทึกแล้ว</details>

📚 อ้างอิง: R1 Layout (Editing Frames, Print)
