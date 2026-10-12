---
title: "1. ผิวโค้งของขาตั้ง: 1 surface ก่อน"
parent: "M4 · ขาตั้งมือถือ Waffle: ตัดเลเซอร์ใน 30 นาที"
nav_order: 1
chapter: true
read_time: 3
do_time: 5
hook: "สร้างผิวโค้งรูปคลื่นที่จะกลายเป็นขาตั้งมือถือ"
edition: pro
track: "📐 Engineering"
permalink: /courses/m4-waffle/01-surface/
---

# 1. ผิวโค้งของขาตั้ง: 1 surface ก่อน
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- สร้าง **surface** (ไม่ใช่ solid) จากโปรไฟล์ Spline
- รู้ว่า Waffle ทำงานกับ **planar หรือ curved surface**

## 💡 ไอเดียสั้น ๆ
Waffle "ผ่า" ผิวเป็นซี่ในแนว U และ V คล้ายโครงกล่องไข่ ดังนั้นเริ่มจาก **ผิวเดียว** ที่มีรูปทรงตามที่ต้องการ (manual: Waffle)

## 👣 ลงมือทำ (5 นาที)
1. ระนาบ ZX: วาดโปรไฟล์ด้านข้างด้วย **Spline**: ฐานยาว 110, โค้งขึ้นเป็นพนักเอียง ~65° สูง 120, ปลายล่างงอขึ้นเป็นขอบกันลื่น 15
2. **3D Extrusion** แบบ surface กว้าง **80** 🔍 (ตั้ง output เป็น surface)
3. ตรวจด้วย **Measure Distance** ว่าขนาดรวมไม่เกินแผ่นไม้ของ FabLab (เช่น 300 × 200)

{: .shot }
[SCREENSHOT: โปรไฟล์ Spline + surface ที่ได้]

{: .verify }
ตัวเลือกให้ 3D Extrusion สร้าง surface แทน solid ใน 10.1.x (หรือใช้ Ruled Surface ระหว่าง 2 เส้นแทน)

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำผิวแบบที่ 2 ที่พนักโค้งเข้าหามือถือมากขึ้น
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Waffle ใช้กับ object แบบไหน?</summary>planar หรือ curved surface</details>
<details><summary>2. ทำไมต้องวัดก่อน?</summary>ให้ชิ้นไม่เกินขนาดแผ่นวัสดุ</details>

📚 อ้างอิง: Manual: Waffle
