---
title: "4. Guides: เส้นช่วยด้วย Shift+Space"
parent: "M1 · 8 ทริกทำงานไวขึ้น 2 เท่า"
nav_order: 4
chapter: true
read_time: 3
do_time: 4
permalink: /courses/m1-quick-tips/04-guides/
edition: free
hook: "ดูภาพรวมของทั้ง course"
---

# 4. Guides: เส้นช่วยด้วย Shift+Space
{% include meta.html %}

## 🎯 ทริกนี้
สร้าง **เส้นช่วยชั่วคราว** จากจุดหรือขอบใด ๆ เพื่อวาดให้ตรงแนวโดยไม่ต้องคำนวณ เช่น วางปุ่มให้ตรงกับขอบฝาพอดี

## 💡 Snap 3 แบบ (R1: Snapping)
- **Grid snaps** · **Guide snaps** · **Object snaps** (เปิด/ปิดแยกกันได้)

**Guides** = เส้นช่วยยาวไม่สิ้นสุด
- **ชั่วคราว (Temporary):** ตอนที่ cursor snap กับจุดหรือขอบอยู่ ให้กด **Shift+Space**
  - ที่ **จุด** → ได้เส้นตามแกน X, Y, Z ของ reference plane
  - ที่ **ขอบ** → ได้เส้นสัมผัสและเส้นตั้งฉากกับขอบ + แกน X, Y, Z
- **ถาวร (Permanent):** ใช้เครื่องมือ **Draw Guide** (กลุ่ม Manage) ได้เส้นประสีดำ อยู่บน layer ที่ active ตอนวาด และถูกบันทึกในไฟล์

## 👣 ลองเลย (4 นาที)
1. เปิดโมเดลแม็กเย็บ (C2) เลือก **Circle** แล้ววางเมาส์ที่มุมฐาน (snap) กด **Shift+Space**
2. ลากตามเส้นช่วยแกน X ไป 20 mm แล้วคลิกวาดวงกลม จะได้รูยึดที่ตรงแนวมุมพอดี
3. ใช้ **Draw Guide** วาดเส้นกึ่งกลางของฐานเป็นเส้นถาวรบน layer `Ref`
4. ปิด layer `Ref` เส้นช่วยจะหายไปด้วย

{: .shot }
[SCREENSHOT: เส้นช่วยชั่วคราวจาก Shift+Space ที่มุมฐาน]

{: .easy }
เหมือน **inference** ของ SketchUp แต่เราควบคุมเองได้ว่าจะให้เส้นช่วยขึ้นเมื่อไร

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** วาดวงกลมให้ตรงกลางหน้าพอดีโดยใช้แค่ guides
</div>

📚 อ้างอิง: R1 Snapping, Draw Guide
