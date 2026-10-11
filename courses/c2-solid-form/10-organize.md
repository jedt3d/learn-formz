---
title: "10. Symmetry + จัดระเบียบ + แกนหมุน"
parent: "C2 · ฟอร์มสวยด้วย Solid"
nav_order: 10
chapter: true
read_time: 4
do_time: 6
permalink: /courses/c2-solid-form/10-organize/
---

# 10. Symmetry + จัดระเบียบ + แกนหมุน
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใส่ **Object Symmetry** ให้ชิ้นงาน แก้ข้างหนึ่งอีกข้างก็ตามไปด้วย
- จัดชิ้นส่วนลง **Layers** และรวมด้วย **Group**
- ใส่ **แกนหมุน (hinge pin)** เตรียมไว้ทำ animation ใน C5 แล้วเรนเดอร์ภาพ

## 💡 ไอเดียสั้น ๆ
**Object Symmetry** ใส่ "ระนาบสมมาตร" ให้วัตถุ หลังจากนั้นทุกการแก้จะสมมาตรตลอด และระนาบจะแสดงเป็นเส้นประเมื่อเลือกวัตถุ (R1: Symmetry)
**Layers** ใช้แยกกลุ่มชิ้นงาน เปิดปิด ล็อก หรือห้าม snap ได้ ส่วน layer ที่ active (จุดแดง) คือ layer ที่วัตถุใหม่จะไปอยู่ (R1: Layers)

## 👣 ลงมือทำ (6 นาที)
### A. Symmetry (2 นาที)
1. เลือก **Object Symmetry** แล้วคลิก `Base` จะมีระนาบสมมาตรเริ่มต้นขึ้นมา ใช้ปุ่มใน Tool Options จัดให้อยู่ **กึ่งกลางความกว้าง** (ระนาบ XZ ที่ผ่านกลางฐาน)
2. ลองใช้ **Reshape** ดึงหน้าข้างซ้ายออก 2 mm หน้าข้างขวาจะขยับตาม แล้ว Undo

### B. แกนหมุน (2 นาที)
3. สลับเป็นระนาบ **ZX** แล้วใช้ **Cylinder > Preset** Radius **2**, Height **30** คลิกที่ (18, 20) แกนจะวิ่งตามแนว Y
4. ใช้ **Align / Distribute** (Y = Center) กับ Base ตั้งชื่อ `HingePin`

### C. จัดระเบียบ + เรนเดอร์ (2 นาที)
5. ที่ **Layers** palette สร้าง layer `Stapler_Parts` และ `Helpers` แล้วย้ายตัวตัดหรือเส้นช่วยไปไว้ใน Helpers และซ่อนไว้
6. ใส่ material: Base เทาเข้ม (ยาง), Magazine โลหะ, Cover สีสด แล้วใช้ **Group** รวมทุกชิ้นเป็น `Stapler`
7. ใช้ฉากสตูดิโอจาก template (C1) แล้ว **RenderZone** 1 ภาพ ตั้งชื่อ `C2_Stapler_Hero.png`

{: .shot }
[SCREENSHOT: Object Symmetry ระนาบเส้นประบน Base]
{: .shot }
[SCREENSHOT: Layers palette ที่มี Stapler_Parts + Helpers]
{: .shot }
[SCREENSHOT: ภาพเรนเดอร์แม็กเย็บ 3 ชิ้นบนพื้น Catcher]

{% include homework.html id="c2-workshop" title="C2 · Stapler 3 ชิ้น" what="ภาพถ่ายแม็กเย็บจริง + ภาพเรนเดอร์ + ภาพหน้าจอที่เห็น Layers / Objects palette" %}

{: .power }
Symmetry ของ formZ **ยังทำงานต่อหลังแก้งาน** (แก้ทีหลังได้) และรองรับทั้ง NURBS และ SubD ส่วน SketchUp ต้องใช้วิธีกลับด้าน component (flip) ซึ่งใช้ได้แค่บางกรณี

{: .shapr }
Shapr3D: Mirror body · formZ: **Object Symmetry** (แบบ live) หรือ **Mirror** (ใน Transform suite แบบครั้งเดียว)

## ✅ เช็คตัวเอง
<details><summary>1. รู้ได้อย่างไรว่าวัตถุมี symmetry อยู่?</summary>เมื่อเลือกวัตถุจะเห็นระนาบสมมาตรเป็นเส้นประ</details>
<details><summary>2. วัตถุใหม่จะไปอยู่ layer ไหน?</summary>layer ที่ active (มีจุดแดง)</details>
<details><summary>3. ทำไมต้องใส่แกนหมุนเป็นชิ้นแยก?</summary>เพื่อใช้เป็นจุดหมุนตอนทำ animation เปิดฝาใน C5</details>

📚 อ้างอิง: R1 Symmetry, Layers, Separating Grouping and Ungrouping
