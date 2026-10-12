---
title: "6. วาง 36 ชิ้นในคลิกเดียว: Place On"
parent: "M1 · 8 ทริกทำงานไวขึ้น 2 เท่า"
nav_order: 6
chapter: true
read_time: 3
do_time: 4
permalink: /courses/m1-quick-tips/06-place-on/
hook: "ดูภาพรวมของทั้ง course"
---

# 6. วาง 36 ชิ้นในคลิกเดียว: Place On
{% include meta.html %}

## 🎯 ทริกนี้
วาง **สำเนา** ของชิ้นเล็กลงบนทุกหน้า ทุกขอบ หรือทุกจุดของอีกชิ้นใน **คลิกเดียว** เช่น ปุ่มยางกันลื่นใต้เครื่องปิ้งขนมปัง หรือรูลำโพง

## 💡 ตัวเลือก (R1: Place On)
| กลุ่ม | ตัวเลือก |
|---|---|
| **Place On** | **Faces' Centers** (กลางทุกหน้า) · **Segment Midpoint** (กลางทุกขอบ) · **Points** (ทุกจุด) |
| **Alignment** | **None** (คงทิศเดิม) · **Along Normal / Tangent** (แกน Z ตั้งฉากกับผิว) |
| **Make Component** | สำเนาทั้งหมดเป็น component (แก้ตัวเดียว ตัวอื่นเปลี่ยนตาม) |

ใช้งาน: คลิก **ชิ้นต้นฉบับ (source)** แล้วคลิก **ชิ้นเป้าหมาย (target)**

## 👣 ลองเลย (4 นาที): รูลำโพง Pebble
1. **Cylinder** R 1 H 3 (ตัวเจาะรู) วางที่จุดกำเนิด
2. ทำแผ่นช่วย: **Polygon Mesh** หรือ Rectangle ที่แบ่งเป็นกริด 6 × 6 วางบนหน้าลำโพง
3. **Place On** → **Points** + **Along Normal** → คลิก Cylinder แล้วคลิกแผ่นช่วย
4. **Difference** ตัว Cylinder ทั้งหมดออกจากหน้าลำโพง ได้รูลำโพงครบ 🎉
5. ทางเลือก: วางปุ่มยาง 4 ตัวด้วย **Points** บนสี่เหลี่ยมเล็กใต้ฐานเครื่องปิ้ง

{: .shot }
[SCREENSHOT: Place On วาง cylinder บนจุดของกริด]
{: .shot }
[SCREENSHOT: หน้าลำโพงมีรูหลังทำ Difference]

{: .verify }
Polygon Mesh สร้างแผ่นกริดที่มีจุดตามต้องการได้ไหม (หรือใช้ Rectangle ที่ Insert เส้นแบ่ง) และ Difference กับ component ต้อง explode ก่อนหรือไม่ ต้องยืนยัน

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** วางปุ่มยาง 4 มุมใต้เครื่องปิ้งในคลิกเดียว
</div>

📚 อ้างอิง: R1 Place On, Polygon Mesh, Components
