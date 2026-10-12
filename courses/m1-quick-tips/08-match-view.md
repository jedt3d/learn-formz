---
title: "8. วางโมเดลลงในรูปถ่ายจริง: Match View"
parent: "M1 · 8 ทริกทำงานไวขึ้น 2 เท่า"
nav_order: 8
chapter: true
read_time: 3
do_time: 5
hook: "วางแก้วที่ปั้นลงบนรูปถ่ายโต๊ะจริงให้มุมกล้องตรงกัน"
renderzone: true
permalink: /courses/m1-quick-tips/08-match-view/
---

# 8. วางโมเดลลงในรูปถ่ายจริง: Match View
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใส่รูปถ่ายเป็น background (**Display Options › Background › Flat Image**)
- ใช้ **Match View** จับคู่จุด 3D กับ 2D อย่างน้อย 4 คู่

## 💡 ไอเดียสั้น ๆ
Matching Views To Pictures ทำให้ภาพ "เหมือนถ่ายจริง" โดยไม่ต้องตัดต่อ เหมาะทำภาพ mockup ใน portfolio

## 👣 ลงมือทำ (5 นาที)
1. ถ่ายรูปโต๊ะที่มี **กล่องหรือสมุดรูปสี่เหลี่ยม** วางอยู่ (ใช้เป็นจุดอ้างอิง) แล้ววัดขนาดกล่องจริง
2. ปั้น **Cube** ขนาดเท่ากล่องจริงในไฟล์
3. **Display › Display Options...** → Background **Flat Image** → **Options... › Load...** เลือกรูป
4. **View › 3 Point Perspective**
5. **Match View** (Navigation palette มุมขวาบน): คลิกมุม Cube (3D bullet) แล้วคลิกมุมกล่องในรูป (2D cross mark) 4 คู่ขึ้นไป ใช้หน้าต่างขยายช่วยเล็ง
6. วางแก้วข้าง Cube แล้วซ่อน Cube → render

{: .shot }
[SCREENSHOT: จับคู่จุด 4 คู่ (เส้นประ)]

{: .shot }
[SCREENSHOT: แก้ว formZ อยู่บนโต๊ะจริง]

{: .warning }
ห้ามใช้ **Move** ขยับโมเดลระหว่างจับคู่ ให้เปลี่ยนแค่ view เท่านั้น (manual)

{: .power }
SketchUp มี Match Photo ใกล้เคียงกัน แต่ formZ render ด้วย RenderZone ต่อได้ทันที

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ถ่ายรูปห้องตัวเองแล้ววางเครื่องปิ้งขนมปังจาก C4 ลงไป
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ต้องจับคู่อย่างน้อยกี่คู่?</summary>อย่างน้อย 3 คู่ ควรเป็น 4 คู่ขึ้นไป</details>
<details><summary>2. ต้องใช้มุมมองแบบไหน?</summary>3 Point Perspective</details>

📚 อ้างอิง: Manual: Matching Views To Pictures
