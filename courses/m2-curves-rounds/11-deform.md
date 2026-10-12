---
title: "11. วิธีที่ 10 · ดัด บิด เรียว: Radial Bend · Twist · Taper"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 11
chapter: true
read_time: 3
do_time: 5
hook: "ดัดหลอดดูดให้งอ บิดปากกาเป็นเกลียว และทำแก้วทรงเรียว"
permalink: /courses/m2-curves-rounds/11-deform/
---

# 11. วิธีที่ 10 · ดัด บิด เรียว: Radial Bend · Twist · Taper
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Radial Bend** ดัดตามแกน
- ใช้ **Twist** บิดด้วย **Twist Angle**
- ใช้ **Taper** ทำให้ปลายหนึ่งเล็กลง

## 💡 ไอเดียสั้น ๆ
Deform tools มี **deformation axis** ตั้งฉากกับ base reference plane ปลายที่เลือกจะขยับ อีกปลายอยู่กับที่ ทำได้ทั้งลากเมาส์และพิมพ์ตัวเลข (R1)

## 👣 ลงมือทำ (5 นาที)
1. หลอดดูด: **Cylinder** Ø6 H200 (Display Resolution สูง) → **Radial Bend** ที่ปลายบน 60°
2. ปากกาเกลียว: **Polygon** 6 เหลี่ยม Ø10 extrude 140 → **Twist** Twist Angle **180**
3. แก้ว: **Cylinder** Ø70 H100 → **Taper** ให้ก้นเล็กลงเหลือ 80%

{: .shot }
[SCREENSHOT: 3 ชิ้น: หลอดงอ, ปากกาบิด, แก้วเรียว]

{: .power }
SketchUp ต้องใช้ extension (เช่น Shape Bender, FredoScale)

{: .warning }
ชิ้นที่จะ deform ต้องมี **เส้นแบ่งพอ** (facetted ความละเอียดสูง) ไม่อย่างนั้นจะงอเป็นเหลี่ยม

{: .verify }
ตำแหน่ง Base Reference Plane และการพิมพ์ค่าองศาของ Radial Bend ใน 10.1.x

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** Twist ปากกา 720° แล้วดูว่ายังจับได้ไหม
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมหลอดงอเป็นเหลี่ยม?</summary>เส้นแบ่งไม่พอ</details>
<details><summary>2. บิดใช้ค่าอะไร?</summary>Twist Angle</details>

📚 อ้างอิง: R1 Radial Bend, Twist, Taper
