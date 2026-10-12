---
title: "SP1 · พวงกุญแจชื่อเรา → พิมพ์ 3D ใน 10 นาที"
parent: "⭐ Special Projects"
nav_order: 1
chapter: true
read_time: 2
do_time: 8
hook: "ทำพวงกุญแจที่มีชื่อเรานูน แล้ว export STL ไปพิมพ์ 3D ได้เลย"
track: "📐 Engineering"
permalink: /projects/sp1-keychain/
---

# SP1 · พวงกุญแจชื่อเรา → พิมพ์ 3D ใน 10 นาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- สร้างแผ่นมุมมน + ตัวอักษรนูนด้วย **Text** + **3D Extrusion**
- รวมชิ้นด้วย **Union** เจาะรูด้วย **Difference**
- ตรวจด้วย **Print Preparation** แล้ว **Export STL**

## 💡 ไอเดียสั้น ๆ
ของชิ้นแรกที่จับได้จริงควร **เล็ก เร็ว และเป็นของเรา** พวงกุญแจขนาด 50 × 20 × 3 mm พิมพ์ใช้เวลาประมาณ 15–20 นาที 🔍 (ขึ้นกับเครื่อง)

## 👣 ลงมือทำ (8 นาที)
1. **Rectangle** 50 × 20 → **3D Extrusion** สูง **3**
2. **Controlled Round** ขอบแนวตั้ง 4 เส้น R**4** แล้วขอบบน R**0.8**
3. **Text** พิมพ์ชื่อเรา (ฟอนต์หนา สูง ~8) วางบนหน้าบน → **3D Extrusion** สูง **1.2**
4. **Union** ตัวอักษรกับแผ่น
5. **Cylinder** Ø4 ที่ปลายซ้าย → **Difference** (รูห่วง)
6. **Print Preparation** ตรวจ wall thickness ≥ 1.2 แล้ว **Export STL** หน่วย mm

{: .shot }
[SCREENSHOT: พวงกุญแจใน formZ]

{: .shot }
[SCREENSHOT: STL เปิดใน slicer (เช่น Bambu Studio / Cura)]

{: .easy }
ทั้งหมดคือเครื่องมือที่ใช้ใน C1–C2 อยู่แล้ว 6 ขั้นจบ

{: .warning }
ตัวอักษรเส้นบาง (เช่นฟอนต์ serif เล็ก) อาจพิมพ์ไม่ออก ให้ใช้ฟอนต์หนาและสูง ≥ 6 mm

{: .verify }
การแปลง Text เป็นวัตถุที่ extrude ได้ใน 10.1.x (อาจต้อง Convert ก่อน) และ edition ที่มี Print Preparation

{: .shot }
[SCREENSHOT: พวงกุญแจที่พิมพ์ออกมาจริงในมือ]

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำแบบตัวอักษรจมลง (Difference แทน Union) แล้วเทียบว่าอ่านง่ายกว่าไหม
</div>

## ✅ เช็คตัวเอง
<details><summary>1. รูห่วงทำด้วยอะไร?</summary>Cylinder + Difference</details>
<details><summary>2. ก่อน export ควรตรวจอะไร?</summary>Print Preparation (ความหนาผนัง) และหน่วย mm</details>

📚 อ้างอิง: R1 Text, 3D Extrusion, Union, Difference, Print Preparation, STL Export · [C8]({{ '/courses/c8-make-it/' | relative_url }})
