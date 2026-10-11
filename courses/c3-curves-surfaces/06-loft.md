---
title: "6. พวยกา: NURBS by Lofting"
parent: "C3 · ผิวโค้งแบบมือโปร"
nav_order: 6
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c3-curves-surfaces/06-loft/
---

# 6. พวยกา: NURBS by Lofting
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- สร้างผิวที่ผ่านหน้าตัดหลายอันด้วย **NURBS by Lofting**
- รู้ความต่างของ **Loose Lofting** กับ **Tight Lofting**
- รู้จักเครื่องมือ loft ตระกูลอื่น (Ruled / Tangent / Guided / Path Loft) และ **Skin**

## 💡 ไอเดียสั้น ๆ
**Loft** คือ "ขึงผิว" ผ่านหน้าตัดที่เรียงกัน เหมือนการหุ้มผ้าบนโครงลวด ใช้ทำของที่ **หน้าตัดเปลี่ยนไปเรื่อย ๆ** เช่น พวยกา ด้ามแปรงสีฟัน หรือหัวฉีด (R1: NURBS by Lofting)

| แบบ | ผล |
|---|---|
| **By Tight Lofting** | ผิว **ผ่าน** ทุกเส้น |
| **By Loose Lofting** | ใช้ control points ของเส้น ผิวนุ่มกว่าแต่ไม่ผ่านเส้นเป๊ะ |

**หน้าตัดพวย** (วงกลมแนวนอนวางทีละระดับ)

| เส้น | ศูนย์กลาง (x, y, z) | Ø |
|---|---|---|
| S1 | (60, 0, 120) | 26 (อยู่ในตัวกา) |
| S2 | (85, 0, 150) | 18 |
| S3 | (100, 0, 172) | 12 |

## 👣 ลงมือทำ (4 นาที)
1. ระนาบ XY ใช้ **Circle** (type 2D) วาดวงกลม S1 แล้ว **Move** ขึ้นไปที่ z = 120 (หรือพิมพ์ z ใน Input palette ตอนคลิกศูนย์กลาง) ทำซ้ำกับ S2 และ S3
2. ถ้า NURBS by Lofting ไม่ยอมรับวงกลม ให้ใช้ **Convert Object Type** แปลงเป็น NURBS curve ก่อน
3. **NURBS by Lofting** ตั้ง **By Tight Lofting** แล้ว **Shift-คลิก** S1 → S2 → S3 ตามลำดับ ปล่อย Shift แล้วคลิกที่ว่าง
4. **Thicken** 2 mm ตั้งชื่อ `Spout`
5. หมุนดู: ส่วน S1 ควรจมอยู่ในผนังตัวกา (บทถัดไปจะรวมและตรวจผิว)

{: .shot }
[SCREENSHOT: วงกลม 3 วงลอยในอากาศก่อน loft]
{: .shot }
[SCREENSHOT: พวยหลัง NURBS by Lofting (Tight)]

{: .verify }
ชื่อเครื่องมือ **Circle** ใน Draw suite และการที่ NURBS by Lofting รับวงกลมแบบ 2D ได้เลยหรือต้องแปลงก่อน ให้ยืนยันใน v10

{: .note }
ตระกูล Loft อื่นใน formZ: **Ruled Loft**, **Tangent Loft** (ให้ผิวสัมผัสกับหน้าตัดหัวท้าย), **Guided Loft**, **Perpendicular Loft**, **Path Loft**, **Branched Loft** และ **Skin** (หน้าตัด + path หลายเส้น) จะได้ใช้อีกครั้งใน C8 และ C9

{: .power }
SketchUp **ไม่มี loft** ในตัวเลย ส่วน formZ มี loft มากกว่า 7 แบบ

{: .shapr }
Shapr3D: **Loft** ผ่าน profiles · formZ: **NURBS by Lofting** (ผิว NURBS) หรือ **Loft tools** (ทำ solid ได้)

## ✅ เช็คตัวเอง
<details><summary>1. อยากให้ผิวผ่านทุกหน้าตัด เลือกแบบไหน?</summary>By Tight Lofting</details>
<details><summary>2. ลำดับการคลิกหน้าตัดสำคัญไหม?</summary>สำคัญ ผิวจะเรียงตามลำดับที่คลิก</details>
<details><summary>3. ถ้ามีหน้าตัด + เส้น path หลายเส้น ใช้เครื่องมืออะไร?</summary>Skin</details>

📚 อ้างอิง: R1 NURBS by Lofting, Lofting tools, Skin
