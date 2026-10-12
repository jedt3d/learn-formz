---
title: "4. วาดโค้งสวยด้วย 5 จุด: Spline + Curve Edit"
parent: "C3 · โค้งแบบมือโปร: ดินสอ + กาต้มน้ำ"
nav_order: 4
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c3-curves-surfaces/04-curves/
hook: "เปลี่ยนเส้นหักธรรมดา (Vector Line) ให้เป็นเส้นโค้งเนียนด้วย Curve Create และเลือกได้ว่าจะเป็น NURBS Curve หรือ Spline Curve Through Points"
---

# 4. วาดโค้งสวยด้วย 5 จุด: Spline + Curve Edit
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เปลี่ยนเส้นหักธรรมดา (**Vector Line**) ให้เป็นเส้นโค้งเนียนด้วย **Curve Create**
- เลือกได้ว่าจะเป็น **NURBS Curve** หรือ **Spline Curve Through Points**
- ปรับรูปโค้งด้วย **Curve Edit** (control points / edit points)

## 💡 ไอเดียสั้น ๆ
ฟอร์มสวย ๆ ของกาต้มน้ำมาจาก **เส้นโค้งด้านข้างเพียงเส้นเดียว** ถ้าเส้นนี้สวย ตัวกาก็จะสวย (R1: Curve Create, Curve Edit)

| ชนิด | นิสัย |
|---|---|
| **NURBS Curve** | ถูกดึงด้วย control points ได้เส้นนุ่มมาก แต่ไม่ผ่านจุดที่คลิกเป๊ะ |
| **Spline Curve Through Points** | วิ่งผ่านทุกจุดที่คลิก คุมตำแหน่งได้ง่าย |

**โปรไฟล์ด้านข้างของตัวกา** (ระนาบ ZX ค่า x = รัศมี, z = ความสูง, หน่วย mm) เป็นรูปเปิดที่ **ไม่ปิดกลับแกน**

| จุด | (x, z) | หมายเหตุ |
|---|---|---|
| P0 | (0, 0) | จุดกลางก้น |
| P1 | (72, 0) | ขอบก้น |
| P2 | (78, 25) | ป่องล่าง |
| P3 | (74, 110) | |
| P4 | (60, 175) | ไหล่ |
| P5 | (50, 185) | ขอบปากกา |

## 👣 ลงมือทำ (4 นาที)
1. ไฟล์ใหม่ `C3_Kettle.fmz` ใส่ Underlay ภาพด้านข้างของกาบนระนาบ **ZX** (ทำแบบ C2 บทที่ 1)
2. **Vector Line** (type **2D**) คลิก P0 → P1 แล้วกด **e** เพื่อจบ (ได้เส้นก้น)
3. **Vector Line** อีกเส้นตั้งแต่ P1 → P2 → P3 → P4 → P5 แล้วกด **e**
4. **Curve Create** คลิกเส้นที่สอง เลือก **Spline Curve Through Points** จะได้เส้นโค้งเนียนผ่านทุกจุด
5. **Curve Edit** คลิกเส้นโค้ง แล้วเปิด **Show Edit Points** ลากจุด P3 ออกหรือเข้า 2–3 mm ให้ตรงกับภาพ Underlay

{: .shot }
[SCREENSHOT: Vector Line กับเส้นที่ผ่าน Curve Create แล้ว (Spline Through Points)]
{: .shot }
[SCREENSHOT: Curve Edit Tool Options (Show Control/Edit Points) และจุดที่กำลังลาก]

{: .verify }
บทถัดไปจะ Revolve **2 เส้นแยกกัน** (เส้นก้นกับเส้นข้าง) ถ้า Revolve รับได้ทีละเส้น อาจต้องต่อเส้นเป็นเส้นเดียวด้วย **Curve Attach** หรือ **Stitch** ก่อน ให้ทดสอบบน v10 จริง

{: .power }
SketchUp ไม่มีเส้นโค้งที่แก้ด้วย control point ได้ (ต้องลง extension Bezier) ส่วน formZ มีทั้ง NURBS และ Spline ในตัว แก้ได้จุดต่อจุด

{: .shapr }
Shapr3D: **Spline** (control points / interpolated) · formZ: **Curve Create** (NURBS / Through Points) + **Curve Edit**

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** วาดโปรไฟล์กาต้มน้ำแบบอ้วนเตี้ยด้วยจุดไม่เกิน 6 จุด
</div>

## ✅ เช็คตัวเอง
<details><summary>1. อยากให้เส้นผ่านทุกจุดที่คลิก เลือกชนิดไหน?</summary>Spline Curve Through Points</details>
<details><summary>2. ทำไมโปรไฟล์ไม่ปิดกลับแกน?</summary>เพราะจะ Revolve เป็นผิว แล้วค่อย Thicken ให้มีผนัง (กาต้มน้ำต้องกลวง)</details>
<details><summary>3. Curve Edit แสดงจุดแบบไหนได้บ้าง?</summary>Control Points และ Edit Points (รวมถึง Weights)</details>

📚 อ้างอิง: R1 Curve Create, Curve Edit
