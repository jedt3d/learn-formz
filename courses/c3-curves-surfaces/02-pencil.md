---
title: "2. ดินสอหกเหลี่ยมใน 3 นาที"
parent: "C3 · โค้งแบบมือโปร: ดินสอ + กาต้มน้ำ"
nav_order: 2
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c3-curves-surfaces/02-pencil/
hook: "วัดดินสอของจริง (ระยะข้ามมุม / ข้ามด้านแบน / ความยาว) และวาด หกเหลี่ยมด้านเท่า แล้วดึงเป็น 3D Extrusion (facetted)"
---

# 2. ดินสอหกเหลี่ยมใน 3 นาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- วัดดินสอของจริง (ระยะข้ามมุม / ข้ามด้านแบน / ความยาว)
- วาด **หกเหลี่ยมด้านเท่า** แล้วดึงเป็น **3D Extrusion** (facetted)
- เตรียม "ตัวเหลา" สำหรับบทถัดไป

## 💡 ไอเดียสั้น ๆ
ดินสอไม้มาตรฐานกว้าง **ข้ามด้านแบนประมาณ 7 mm** และยาว **~175 mm** (ลองวัดของเราดู) หกเหลี่ยมที่กว้างข้ามด้านแบน 7 mm จะมีระยะข้ามมุม ≈ 8.1 mm (รัศมีถึงมุม ≈ 4.04 mm)

| ชิ้น | วิธี | ค่า |
|---|---|---|
| Hex body | Polygon 6 ด้าน + 3D Extrusion | รัศมีถึงมุม 4.04 · ยาว 195 (เผื่อไว้เหลา 20) |
| Sharpener shape | Cylinder R5 H165 + Cone R5 H30 (ไม่ตัดปลาย) | เดี๋ยวจะ Union กัน |

## 👣 ลงมือทำ (3 นาที)
1. ไฟล์ใหม่ `C3_Pencil.fmz` ระนาบ XY
2. เครื่องมือวาด **Polygon** (Draw suite) ตั้ง **6 ด้าน** แล้วเลือก object type **3D Extrusion** คลิกศูนย์กลางที่ (0, 0, 0) แล้วพิมพ์รัศมี **4.04** และ Height **195** ตั้งชื่อ `Hex`
3. **Cylinder > Preset** R **5** H **165** ที่ (0, 0, 0) แล้ววาง **Cone > Preset** R **5** H **30** ต่อบนหน้าบน (Snap to Center)
4. **Union** Cylinder กับ Cone ตั้งชื่อ `SharpenShape`

{: .shot }
[SCREENSHOT: Hex (facetted) กับ SharpenShape (smooth) ซ้อนกันใน Wire Frame]

{: .verify }
ชื่อเครื่องมือ **Polygon** และวิธีตั้งจำนวนด้าน และการวัดรัศมีถึงมุมหรือถึงกึ่งกลางด้าน ใน Draw suite ของ v10 ต้องยืนยัน (คู่มือไม่มีหน้าแยกของเครื่องมือนี้)

{: .easy }
เหมือน Polygon + Push/Pull ใน SketchUp ทุกประการ

{: .shapr }
Shapr3D: Polygon sketch → extrude · formZ: **Polygon + 3D Extrusion** ในจังหวะเดียว

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำดินสอทรงกลมกับทรงสามเหลี่ยมให้ครบ 3 แบบ
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมยาว 195 ไม่ใช่ 175?</summary>เผื่อเนื้อไว้ 20 mm สำหรับส่วนที่จะเหลาในบทถัดไป</details>
<details><summary>2. Hex เป็นวัตถุแบบไหน?</summary>Facetted (หน้าแบน 6 ด้าน + หัวท้าย)</details>
<details><summary>3. SharpenShape เป็นแบบไหน?</summary>Smooth (cylinder + cone)</details>

📚 อ้างอิง: R1 Drawing Objects, Cylinder, Cone, Union
