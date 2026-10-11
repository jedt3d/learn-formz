---
title: "5. ตรวจว่าชนกันไหม"
parent: "C8 · เตรียมผลิต: 3D Print, STEP"
nav_order: 5
chapter: true
read_time: 4
do_time: 3
track: "📐 Engineering"
permalink: /courses/c8-make-it/05-fit-check/
---

# 5. ตรวจว่าชนกันไหม
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- วางฝาบนขวดในตำแหน่ง **ขันสุด**
- ตรวจ **interference** (ชิ้นทับกัน) ด้วย **Intersection** ของสำเนา
- วัดช่องว่างด้วย **Measure Between** + **Clipping Plane**

## 💡 ไอเดียสั้น ๆ
**ก่อนพิมพ์ต้องรู้ว่าชนกันไหม** เทคนิคง่าย: copy ทั้งสองชิ้นแล้วทำ **Intersection** ถ้ามีเนื้อเหลือ = **ชนกัน** (ตำแหน่งของเนื้อที่เหลือจะบอกว่าชนตรงไหน) ถ้าไม่มีอะไรเหลือ = ผ่าน ✅

## 👣 ลงมือทำ (3 นาที)
1. **Move** ฝาไปที่ศูนย์กลางคอ (snap ที่จุดกลาง) แล้วเลื่อนลงจนหลังคาฝาห่างปากขวด 0.4 mm
2. **Rotate** ฝารอบแกน Z จนเกลียวฝาอยู่ระหว่างเกลียวขวด (มองใน clipping plane)
3. copy ขวดและฝา (Move + copy ไปที่ว่าง) แล้วทำ **Intersection** ระหว่างสำเนาทั้งสอง
4. ถ้ามีเนื้อเหลือ ให้ดูว่าอยู่ตรงไหน แล้วแก้ (เพิ่ม clearance หรือหมุนฝา)
5. **Clipping Plane** ผ่าแนวแกน → **Measure Between** วัดช่องว่างระหว่างฟันเกลียว

{: .shot }
[SCREENSHOT: clipping plane ผ่าฝาที่สวมอยู่บนขวด เห็นช่องว่างระหว่างเกลียว]

{: .warning }
ทำ Intersection กับ **สำเนา** เสมอ เพราะ Boolean จะเปลี่ยนชิ้นต้นฉบับ (formZ ไม่มี history tree ให้ย้อน)

{: .verify }
ถ้า Intersection ไม่มีส่วนที่ทับกัน formZ จะแจ้ง error หรือให้ผลว่าง ต้องยืนยันพฤติกรรมใน v10

## ✅ เช็คตัวเอง
<details><summary>1. Intersection แล้วมีเนื้อเหลือแปลว่าอะไร?</summary>ชิ้นงานทับกัน (interference)</details>
<details><summary>2. ทำไมต้องใช้สำเนา?</summary>Boolean เปลี่ยนชิ้นต้นฉบับ</details>
<details><summary>3. ใช้อะไรดูช่องว่างระหว่างเกลียวโดยไม่ตัดโมเดล?</summary>Clipping Plane</details>

📚 อ้างอิง: R1 Intersection, Measure Between, Clipping Planes
