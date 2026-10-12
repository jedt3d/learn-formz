---
title: "9. แบบ 3 ด้านใน Layout"
parent: "C7 · เขียนแบบให้โรงงานอ่านออก: กบเหลา 3 ด้าน"
nav_order: 9
chapter: true
read_time: 5
do_time: 4
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/09-views/
edition: pro
hook: "วางภาพฉาย Front / Top / Left แบบ first-angle ด้วย Place Multi-Frame ที่มาตราส่วน 2:1"
---

# 9. แบบ 3 ด้านใน Layout
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- วางภาพฉาย **Front / Top / Left** แบบ **first-angle** ด้วย **Place Multi-Frame** ที่มาตราส่วน **2:1**
- วางภาพตัดจาก **Section** view ของ frame (ใช้ clipping plane `SEC_A`)
- ตั้งให้ **เส้นที่ถูกบังเป็นเส้นประ** (hidden line options)

## 💡 ไอเดียสั้น ๆ
**First-angle** (ISO): ภาพ **Top วางใต้** ภาพ Front และภาพ **Left วางขวา** ของภาพ Front (ตรงข้ามกับ third-angle) ของชิ้นเล็กอย่างกบเหลา (26 mm) ใช้ **2:1** (ขยาย 2 เท่า) จะอ่านง่าย

| ตำแหน่งบน A4 แนวนอน | Frame View |
|---|---|
| ซ้ายบน | **Front** |
| ซ้ายล่าง | **Top** (first-angle) |
| ขวาบน | **Left** |
| ขวาล่าง | **Section** → `SEC_A` |

## 👣 ลงมือทำ (4 นาที)
1. **File > New Layout Project**: A4 Landscape, Margin 10, Border ✅
2. **Place Multi-Frame** 2 × 2 · File = `C7_Sharpener.fmz` · Scale **2:1** + **Apply To All Frames**
3. ตั้ง View ของแต่ละกรอบตามตาราง (กรอบ Section: View = **Section** แล้วเลือก Section Plane = `SEC_A`)
4. Graphics: Object Type = **Lines, Splines and Arcs** → **Options** (Hidden Line) ให้แสดงเส้นที่ถูกบังเป็น **เส้นประ**
5. ตรวจว่าภาพ Front กับ Top **อยู่ในแนวเดียวกัน** (ใช้ Align ถ้าจำเป็น)

{: .shot }
[SCREENSHOT: Multiple Frame Parameters ที่ตั้ง Section = SEC_A]
{: .shot }
[SCREENSHOT: A4 ที่มี 3 ภาพฉาย + ภาพตัด]

{: .verify }
ตัวเลือกให้เส้นที่ถูกบังแสดงเป็น **เส้นประ** ใน Hidden Line Options และรายการ **Left** ใน View menu ต้องยืนยันใน v10 (คู่มือระบุ Top, Bottom, Right, Left, Back, Front)

{: .note }
ถ้าวาง Multi-Frame แล้วตำแหน่งไม่ตรงตามระบบ first-angle ให้วางทีละ frame ด้วย **Place Frame** แทน แล้วจัดแนวด้วย Align

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** เพิ่มมุม iso มุมที่ 4 ลงในแบบ
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ใน first-angle ภาพ Top อยู่ตรงไหน?</summary>ใต้ภาพ Front</details>
<details><summary>2. 2:1 หมายถึงอะไร?</summary>ภาพบนกระดาษใหญ่เป็น 2 เท่าของของจริง</details>
<details><summary>3. ภาพตัดใน Layout ใช้อะไรเป็นตัวกำหนดระนาบ?</summary>clipping plane ในไฟล์โมเดล</details>

📚 อ้างอิง: R1 Layout (Place Frame — Section, Place Multi-Frame), Hidden Line
