---
title: "6. วิธีที่ 5 · มุมมนตั้งแต่ 2D: Fit Fillet / Bevel"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 6
chapter: true
read_time: 2
do_time: 4
hook: "ทำไม้บรรทัดมุมมนตั้งแต่ตอนวาดเส้น 2D แล้วค่อย extrude"
permalink: /courses/m2-curves-rounds/06-fit-fillet/
---

# 6. วิธีที่ 5 · มุมมนตั้งแต่ 2D: Fit Fillet / Bevel
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Fit Fillet / Bevel** กับมุมของเส้น 2D (ทั้งรูปหรือทีละจุด)
- รู้ว่าทำมุมมนตั้งแต่ 2D **เร็วกว่าและไม่ค่อย error**

## 💡 ไอเดียสั้น ๆ
Fit Fillet / Bevel ทำ fillet วงกลม (**Radius** หรือ **Distance**) หรือ bevel (**Offset** หรือ **Length**) ที่มุมของ shape ทั้งรูปปิดและเปิด ถ้าจะเลือกทีละจุดหรือทีละเส้นให้กด **Ctrl/Cmd** ค้างแล้วคลิก (R1)

## 👣 ลงมือทำ (4 นาที)
1. **Rectangle** 2D ขนาด 300 × 30 (ไม้บรรทัด)
2. **Fit Fillet / Bevel** → Circular Radius **4** → คลิกทั้งรูป
3. **3D Extrusion** สูง **3**
4. เจาะรูแขวน Ø6 ที่ปลายด้วย Difference

{: .shot }
[SCREENSHOT: ไม้บรรทัดจาก rectangle 2D มุมมน]

{: .easy }
เหมือนวาด Rectangle แล้วตั้งมุมมนใน SketchUp แต่ทำได้กับทุกรูป 2D

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำไม้บรรทัดแบบมุมตัด (Bevel) แล้วเทียบกัน
</div>

## ✅ เช็คตัวเอง
<details><summary>1. เลือกทีละมุมทำอย่างไร?</summary>กด Ctrl/Cmd ค้างแล้วคลิกจุด</details>
<details><summary>2. ทำไมทำตั้งแต่ 2D ดีกว่า?</summary>เร็วกว่าและไม่ค่อย error</details>

📚 อ้างอิง: R1 Fit Fillet / Bevel
