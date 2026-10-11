---
title: "10. ฝา + ปุ่ม: Subdivision / Soften + Convert"
parent: "C3 · ผิวโค้งแบบมือโปร"
nav_order: 10
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c3-curves-surfaces/10-lid/
---

# 10. ฝา + ปุ่ม: Subdivision / Soften + Convert
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำฝาด้วย **Revolve** (ทวนบทที่ 5) และปุ่มจับด้วย **Subdivision / Soften**
- แปลง SubD เป็น **NURBS** ด้วย **Subdivision / Convert** ก่อนรวมกับชิ้นอื่น
- รู้ว่าเมื่อไรควรใช้ Convert to **Quad Mesh** (เรียนต่อใน C8)

## 💡 ไอเดียสั้น ๆ
SubD เหมาะกับ **ช่วงปั้น** เพราะ cage ปรับง่าย พอฟอร์มลงตัวแล้ว **Subdivision / Convert** จะเปลี่ยนเป็นวัตถุ **NURBS (smooth)** ไว้ใช้ในงานผลิต หรือเป็น **quad mesh (facetted)** ก็ได้ (R1: Subdivision / Convert)

| ชิ้น | วิธี | ค่า |
|---|---|---|
| Lid | โปรไฟล์โดมเตี้ย → Revolve → Thicken 2 | Ø100, สูง 12 |
| Knob | Cube 30 × 14 × 12 → **Subdivision / Soften** | Distance 4 |

## 👣 ลงมือทำ (4 นาที)
1. วาดโปรไฟล์ฝา (ระนาบ ZX): (0, 197) → Spline ผ่าน (35, 194) ไป (50, 185) แล้ว **Revolve** 360° และ **Thicken** 2 ตั้งชื่อ `Lid`
2. **Cube** 30 × 14 × 12 วางกลางฝา แล้ว **Subdivision / Soften** Distance **4** ตั้งชื่อ `Knob`
3. **Subdivision / Convert** คลิก Knob เลือก **NURBS** แล้ว Union Knob กับ Lid
4. ทำแบบเดียวกันกับ `Handle` (Convert เป็น NURBS) แล้ว **Union** เข้ากับ Body

{: .shot }
[SCREENSHOT: Subdivision / Convert options (NURBS / Convert to Quad Mesh)]
{: .shot }
[SCREENSHOT: ฝา + ปุ่มจับบนตัวกา]

{: .verify }
Boolean ระหว่างวัตถุ SubD กับ smooth ใน v10 อาจทำได้เลยโดยไม่ต้อง Convert ก่อน ให้ทดสอบบนเครื่องจริง ถ้าทำได้ ให้ทำขั้น Convert เป็นทางเลือก

{: .power }
formZ แปลงไปมาได้ครบ 3 ตระกูล **Facetted ↔ Smooth/NURBS ↔ SubD** ในโปรแกรมเดียว ซึ่ง SketchUp, Blender และ Shapr3D แต่ละตัวทำได้ไม่ครบ

{: .shapr }
Shapr3D: SubD → **Convert to solid** · formZ: **Subdivision / Convert** → NURBS

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมต้อง Convert SubD เป็น NURBS?</summary>เพื่อให้ใช้กับเครื่องมือ solid หรือ NURBS ได้ และส่งต่องานผลิตได้</details>
<details><summary>2. Quad Mesh เป็นวัตถุชนิดไหน?</summary>Facetted (หน้าเหลี่ยมสี่ด้านเรียงกันสม่ำเสมอ)</details>
<details><summary>3. Soften เหมาะกับชิ้นแบบไหน?</summary>ชิ้นที่ทรงยังเป็นกล่องแต่ขอบนุ่ม เช่น ปุ่มจับ หรือรีโมต</details>

📚 อ้างอิง: R1 Subdivision / Soften, Subdivision / Convert, Revolve
