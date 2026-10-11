---
title: "10. Title block + PDF"
parent: "C7 · วัดขนาดและเขียนแบบ"
nav_order: 10
chapter: true
read_time: 4
do_time: 5
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/10-titleblock/
---

# 10. Title block + PDF
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใส่ **dimension บน layout** (บนภาพฉาย 2D) ด้วยเครื่องมือชุดเดียวกับบท 6–7
- สร้าง **title block** แบบง่ายที่มุมขวาล่าง
- ส่งออก **PDF** แบบที่พร้อมส่งโรงงานหรือร้านพิมพ์ 3D

## 💡 ไอเดียสั้น ๆ
**Title block มาตรฐานแบบย่อ** สำหรับนักเรียน

| ช่อง | ตัวอย่าง |
|---|---|
| ชื่อชิ้นงาน | PENCIL SHARPENER – BODY |
| เลขแบบ / รุ่น | PD-C7-001 · Rev A |
| วัสดุ | ABS (Body), Steel (Blade) |
| มาตราส่วน / หน่วย | 2:1 · mm |
| Tolerance ทั่วไป | ±0.2 |
| ระบบภาพฉาย | First-angle (สัญลักษณ์กรวย) |
| ผู้เขียน / วันที่ | ชื่อเล่น · 2026-10-12 |

## 👣 ลงมือทำ (5 นาที)
1. ใส่ dimension บนภาพฉายใน layout: ความยาว ความกว้าง ความสูง Ø รูเข้า และมุมกรวย (บนภาพตัด) ใช้ style `PD_mm_3.5`
2. วาด title block ด้วย **Rectangle** + **Vector Line** แบ่งช่อง แล้วใส่ **Place Text** ตามตาราง
3. ใส่ Text Note "ขอบทั้งหมด R1.5 · Tolerance ทั่วไป ±0.2" และน้ำหนักโดยประมาณจากบทที่ 5
4. **Print → PDF** ตั้งชื่อ `C7_Sharpener_Drawing.pdf`

{: .shot }
[SCREENSHOT: title block มุมขวาล่าง]
{: .shot }
[SCREENSHOT: แบบ A4 ที่เสร็จสมบูรณ์]

{: .verify }
Dimension ที่วางบน frame ใน Layout ผูก (associative) กับเส้นของ frame ไหม เมื่อ regenerate frame แล้ว dimension ยังอยู่ไหม ต้องทดสอบใน v10

{% include homework.html id="c7-workshop" title="C7 · Sharpener Drawing" what="PDF แบบ A4 + ภาพร่างด้วยมือจากบทที่ 1 (เทียบกัน)" %}

## ✅ เช็คตัวเอง
<details><summary>1. Title block ต้องบอกอะไรบ้างอย่างน้อย?</summary>ชื่อชิ้นงาน วัสดุ มาตราส่วน หน่วย tolerance ระบบภาพฉาย ผู้เขียน และวันที่</details>
<details><summary>2. Rev A หมายถึงอะไร?</summary>รุ่นแก้ไขครั้งแรกของแบบ (revision)</details>
<details><summary>3. ทำไมต้องบอก tolerance ทั่วไป?</summary>เพื่อให้ผู้ผลิตรู้ว่าทุกขนาดที่ไม่ได้ระบุคลาดได้เท่าไร</details>

📚 อ้างอิง: R1 Dimensions, Layout, Place Text
