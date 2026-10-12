---
title: "9. วิธีที่ 8 · ผิวจากหลายหน้าตัด: Skin + NURBS by Lofting"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 9
chapter: true
read_time: 3
do_time: 6
hook: "ทำช้อนจากหน้าตัด 4 อัน ด้วย NURBS by Lofting และรู้ว่าเมื่อไรใช้ Skin"
permalink: /courses/m2-curves-rounds/09-skin-loft/
---

# 9. วิธีที่ 8 · ผิวจากหลายหน้าตัด: Skin + NURBS by Lofting
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำผิวจาก **หน้าตัดหลายอันเรียงกัน** (NURBS by Lofting)
- รู้ว่า **Skin** ใช้ **sources + paths** (หน้าตัด + เส้นนำ) เมื่อต้องการคุมขอบด้วยเส้น

## 💡 ไอเดียสั้น ๆ
Loft = หน้าตัดเรียงกันแล้วขึงผิว ส่วน **Skin** = หน้าตัด + เส้นทางนำ โดยเลือกด้วย pick sets: กด Shift เลือก sources ตามลำดับ → ปล่อย → คลิกที่ว่าง → แล้วทำแบบเดียวกันกับ paths (R1: Skin)

## 👣 ลงมือทำ (6 นาที)
1. วาดหน้าตัดช้อน 4 อันบนระนาบ YZ ตามความยาว: ปลายด้าม (วงรี 8×3), คอ (6×3), โคนแอ่ง (30×8 ทรงโค้ง), ปลายแอ่ง (20×4)
2. **NURBS by Lofting** คลิกตามลำดับ
3. ถ้าแอ่งไม่สวย: เพิ่มเส้นนำขอบซ้าย/ขวา แล้วลอง **Skin**
4. **Thicken** 1.5

{: .shot }
[SCREENSHOT: หน้าตัด 4 อัน + ช้อนที่ได้]

{: .power }
SketchUp ต้องใช้ extension Curviloft

{: .verify }
ลำดับการเลือก pick sets ของ Skin ใน 10.1.x

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำช้อนส้อม (spork) โดยตัดปลายเป็นซี่ด้วย Difference
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Loft ต่างจาก Skin อย่างไร?</summary>Loft ใช้หน้าตัดอย่างเดียว ส่วน Skin ใช้หน้าตัดกับเส้นนำ</details>
<details><summary>2. ผิวช้อนบางให้หนาด้วยอะไร?</summary>Thicken</details>

📚 อ้างอิง: R1 Skin, NURBS by Lofting · [C3-6]({{ '/courses/c3-curves-surfaces/06-loft/' | relative_url }})
