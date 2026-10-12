---
title: "8. วิธีที่ 7 · ลากหน้าตัดตามเส้น: Sweep + Pipe"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 8
chapter: true
read_time: 3
do_time: 6
hook: "ทำหูหิ้วถุงด้วย Axial Sweep และสายชาร์จด้วย Pipe"
permalink: /courses/m2-curves-rounds/08-sweep-pipe/
---

# 8. วิธีที่ 7 · ลากหน้าตัดตามเส้น: Sweep + Pipe
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Axial Sweep** ลาก source ไปตาม path (ตั้ง **Alignment**)
- ใช้ **Pipe** ทำท่อกลมจากเส้นเดียว แล้ว **แก้ diameter ทีหลังได้**
- รู้จัก **Two Source Sweep** (หน้าตัดเปลี่ยนระหว่างทาง)

## 💡 ไอเดียสั้น ๆ

| เครื่องมือ | ใช้เมื่อ |
|---|---|
| **Axial Sweep** | หน้าตัดรูปไหนก็ได้ ลากตามเส้นทาง (หูหิ้วหน้าตัดแบน) |
| **Two Source Sweep** | หน้าตัดต้นทางกับปลายทางไม่เหมือนกัน |
| **Pipe** | หน้าตัดกลม (สายไฟ, ท่อ, ขอบเบาะ) เป็น parametric แก้ diameter ใน **Inspector** ได้ |

## 👣 ลงมือทำ (6 นาที)
1. วาด path หูหิ้วเป็น **Spline** รูปตัว U กว้าง 100 สูง 60
2. วาด source เป็น Rectangle 12 × 3 (Fit Fillet R1)
3. **Axial Sweep** → Model Type **Smooth** → Alignment **Centroid** → คลิก source แล้วคลิก path
4. สายชาร์จ: วาด Spline คดเคี้ยวยาว ~300 → **Pipe** Diameter **3**
5. แก้ diameter ของ Pipe เป็น **4** ใน Inspector

{: .shot }
[SCREENSHOT: หูหิ้วจาก Axial Sweep + สายชาร์จจาก Pipe]

{: .power }
SketchUp มี Follow Me แต่ทำ Pipe ที่แก้ขนาดทีหลังไม่ได้

{: .verify }
ชื่อแท็บ parameter ของ Pipe ใน Inspector ใน 10.1.x

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำหัวชาร์จที่ปลายสายด้วย Cube + Controlled Round
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Pipe แก้ขนาดทีหลังได้ไหม?</summary>ได้ ผ่าน Inspector</details>
<details><summary>2. หน้าตัดเปลี่ยนระหว่างทางใช้อะไร?</summary>Two Source Sweep</details>

📚 อ้างอิง: R1 Axial Sweep, Two Source Sweep, Pipe
