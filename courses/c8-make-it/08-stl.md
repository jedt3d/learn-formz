---
title: "8. STL ไม่หนักไม่หยาบ: Facetted + Simplify"
parent: "C8 · พิมพ์ 3D ให้ขันได้จริง: ขวด + ฝาเกลียว"
nav_order: 8
chapter: true
read_time: 5
do_time: 4
track: "📐 Engineering"
permalink: /courses/c8-make-it/08-stl/
edition: pro
hook: "เข้าใจว่า STL = สามเหลี่ยมล้วน และ Smooth object จะถูกแปลงเป็นสามเหลี่ยมตอน export"
---

# 8. STL ไม่หนักไม่หยาบ: Facetted + Simplify
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เข้าใจว่า **STL = สามเหลี่ยมล้วน** และ Smooth object จะถูกแปลงเป็นสามเหลี่ยมตอน export
- คุมความละเอียด (จำนวนสามเหลี่ยม) และใช้ **Simplify Mesh** เมื่อไฟล์ใหญ่เกิน
- Export **STL** โดยใช้ **Scale** และ **Position In Positive XYZ Octant**

## 💡 ไอเดียสั้น ๆ
STL รับเฉพาะ **หน้าสามเหลี่ยม** formZ จะแตกทุกหน้าเป็นสามเหลี่ยมก่อน export (R1: STL)
- สามเหลี่ยม **น้อยไป** → เกลียวเป็นเหลี่ยม ขันฝืด
- สามเหลี่ยม **มากไป** → ไฟล์ใหญ่ slicer ทำงานช้า
- ขวดจิ๋วนี้ควรอยู่ที่ **~50k–200k สามเหลี่ยม** ต่อชิ้น

| เครื่องมือ | ใช้ทำอะไร |
|---|---|
| **Convert Object Type** (Smooth → Facetted) | แปลงเป็น facetted ด้วยความละเอียดที่กำหนด |
| **Triangulate** | แตกหน้าเป็นสามเหลี่ยม (ดูหน้าตาก่อน export) |
| **Simplify Mesh** (Keep Percentage / Target Number Triangles) | ลดจำนวนสามเหลี่ยมแต่คงรูปทรงหลักไว้ |
| **Reduce Mesh** (Face Angle) | รวมหน้าที่เกือบอยู่ในระนาบเดียวกัน |

## 👣 ลงมือทำ (4 นาที)
1. **บันทึกไฟล์ smooth ไว้ก่อน** แล้ว Save As `C8_Bottle_print.fmz`
2. **Convert Object Type** → Facetted (ความละเอียดสูงพอให้เกลียวกลม) แล้ว **Measure Quantities** ดูจำนวน face
3. ถ้าเกิน 200k ให้ใช้ **Simplify Mesh** → Target Number Triangles **150000**
4. เลือก `Bottle` → **File › Export...** → **STL** (ตั้งให้ export เฉพาะชิ้นที่เลือก)
5. ตัวเลือก: Scale Factor **1**, เปิด **Position In Positive XYZ Octant** → `bottle.stl` แล้วทำซ้ำกับ `cap.stl`
6. **กลับหัวฝา** (หลังคาลงพื้น) ก่อน export เพื่อไม่ต้องใช้ support

{: .shot }
[SCREENSHOT: Modeling Export Options: STL]
{: .shot }
[SCREENSHOT: เกลียวแบบ Facetted ความละเอียดต่ำเทียบสูง]

{: .verify }
- การ export เฉพาะชิ้นที่เลือก (Export Selected) และหน่วยใน STL (mm) ใน v10 ต้องยืนยัน
- Smooth object ที่ export ตรง ๆ จะใช้ Display Resolution หรือค่า tessellation ใด

{: .shapr }
Shapr3D export STL โดยมี slider ความละเอียด formZ ให้คุมเองแบบละเอียดกว่า (Convert / Simplify / Reduce)

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** export STL 2 ความละเอียด แล้วเทียบขนาดไฟล์
</div>

## ✅ เช็คตัวเอง
<details><summary>1. STL เก็บหน้าแบบไหน?</summary>สามเหลี่ยมล้วน</details>
<details><summary>2. ทำไมต้องกลับหัวฝาก่อนพิมพ์?</summary>ให้หลังคาฝาวางบนพื้นเตียงพิมพ์ จะได้ไม่มี overhang ใหญ่</details>
<details><summary>3. Simplify Mesh ต่างจาก Reduce Mesh อย่างไร?</summary>Simplify Mesh ลดสามเหลี่ยมตามเป้าหมายแต่คงรูปทรงหลัก ส่วน Reduce Mesh รวมหน้าที่มุมระหว่างกันน้อยกว่าค่าที่กำหนด</details>

📚 อ้างอิง: R1 STL, Simplify Mesh, Reduce Mesh, Triangulate, Convert Object Type · R15
