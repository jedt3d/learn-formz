---
title: "2. ตัวขวด: Tangent Loft + Caps"
parent: "C8 · เตรียมผลิต: 3D Print, STEP"
nav_order: 2
chapter: true
read_time: 4
do_time: 5
track: "📐 Engineering"
permalink: /courses/c8-make-it/02-body/
---

# 2. ตัวขวด: Tangent Loft + Caps
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำตัวขวดจากหน้าตัด 4 อันด้วย **Tangent Loft** แบบเปิด **Caps** (ได้ solid ทันที)
- ต่อคอขวดด้วย Cylinder + Union
- ทำให้ขวด **กลวง** ด้วย **Thicken** แล้วเปิดปากขวดด้วย **Difference**

## 💡 ไอเดียสั้น ๆ
ใน C3 เราใช้ **NURBS by Lofting** ได้ "ผิว" ส่วนตระกูล **Loft tools** (Ruled / Tangent / Guided ...) มีตัวเลือก **Caps**: เปิด = ได้ **solid** · ปิด = ได้ผิว (R1: Tangent Loft) ซึ่งเหมาะกับงานพิมพ์มากกว่า

| หน้าตัด | z (mm) | Ø |
|---|---|---|
| S0 ก้น | 0 | 44 |
| S1 เอว | 30 | 38 |
| S2 ไหล่ | 52 | 44 |
| S3 ฐานคอ | 66 | 22 |
| Neck (Cylinder) | 66 → 82 | 22 |

## 👣 ลงมือทำ (5 นาที)
1. ไฟล์ `C8_Bottle.fmz` วาด **Circle** 4 วงตามตาราง (ศูนย์กลางที่ x = 0, y = 0)
2. **Tangent Loft**: Shift-คลิก S0 → S1 → S2 → S3 แล้วคลิกที่ว่าง จากนั้นเปิด **Caps**
3. **Cylinder** R **11** H **16** บน S3 → **Union** ตั้งชื่อ `Bottle`
4. **Thicken** **1.6** (ไปด้านใน) → ได้ขวดกลวงที่ยังปิดสนิท
5. **Difference** ด้วย Cylinder R **9.4** สูง 10 ที่ปลายคอ เพื่อเปิดปากขวด
6. ตรวจไหล่ (S2 → S3): ถ้าเอียงเกิน 45° จากแนวตั้ง ให้ยก S3 ขึ้นไป z = 70

{: .shot }
[SCREENSHOT: วงกลม 4 วง + ผล Tangent Loft (Caps on)]
{: .shot }
[SCREENSHOT: ขวดผ่าครึ่งด้วย clipping plane เห็นผนัง 1.6]

{: .verify }
Tangent Loft กับวงกลมที่วาดด้วย type 2D (ไม่ใช่หน้าของวัตถุ) ใช้ได้ทันทีหรือไม่ และความเนียนระหว่างหน้าตัด (ถ้าไม่เนียน ให้ลอง **NURBS by Lofting** แล้วปิดก้นด้วย Cover/Cap) ต้องยืนยันใน v10

{: .shapr }
Shapr3D: Loft → Shell · formZ: **Tangent Loft (Caps)** → **Thicken**

## ✅ เช็คตัวเอง
<details><summary>1. Caps เปิดกับปิดต่างกันอย่างไร?</summary>เปิด = ได้ solid · ปิด = ได้ผิว</details>
<details><summary>2. ทำไม Thicken ก่อนเจาะปาก?</summary>Thicken solid จะได้ผนังรอบทิศ แล้วค่อยเจาะปากออก ทำให้ผนังหนาเท่ากันทั้งขวด</details>
<details><summary>3. ไหล่ขวดเอียงเกิน 45° ทำให้เกิดอะไร?</summary>overhang ที่พิมพ์แล้วอาจย้อยหรือต้องใช้ support</details>

📚 อ้างอิง: R1 Tangent Loft, Ruled Loft, Thicken, Difference
