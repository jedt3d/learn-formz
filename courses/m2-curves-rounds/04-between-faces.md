---
title: "4. วิธีที่ 3 · มนระหว่าง 2 ผิว: Round Between Faces"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 4
chapter: true
read_time: 3
do_time: 5
hook: "ทำที่จับลิ้นชักที่ขาต่อกับแผ่นแบบโค้งเนียน"
permalink: /courses/m2-curves-rounds/04-between-faces/
---

# 4. วิธีที่ 3 · มนระหว่าง 2 ผิว: Round Between Faces
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- สร้าง **fillet** ระหว่าง 2 หน้า (ชิ้นเดียวกันหรือคนละชิ้นก็ได้)
- รู้ว่าถ้าเป็นคนละชิ้น formZ จะ **รวมเป็นชิ้นเดียว** ให้

## 💡 ไอเดียสั้น ๆ
Round Between Faces สร้างผิวมนเชื่อมระหว่าง 2 หน้า ตั้งขนาดที่ **Fillet Radius** ถ้ารัศมีเล็กหรือใหญ่เกินจะมี error (R1)

## 👣 ลงมือทำ (5 นาที)
1. **Cube** 120 × 12 × 6 (คานที่จับ) ลอยสูง 25
2. **Cylinder** Ø10 สูง 25 ใต้ปลายคาน 2 ต้น (ขา)
3. **Round Between Faces** Fillet Radius **4** → คลิกหน้าข้างขา แล้วคลิกหน้าล่างคาน
4. ทำซ้ำที่ขาอีกต้น

{: .shot }
[SCREENSHOT: รอยต่อขากับคานก่อน/หลัง fillet]

{: .verify }
การใช้ Round Between Faces กับหน้าโค้ง (ผิวข้างของ Cylinder) กับหน้าเรียบ ใน 10.1.x

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ลอง Fillet Radius 1 กับ 8 แล้วดูว่าอันไหน error
</div>

## ✅ เช็คตัวเอง
<details><summary>1. 2 ชิ้นแยกกัน ใช้ได้ไหม?</summary>ได้ และ formZ จะรวมเป็นชิ้นเดียว</details>
<details><summary>2. ตั้งขนาดตรงไหน?</summary>Fillet Radius</details>

📚 อ้างอิง: R1 Round Between Faces
