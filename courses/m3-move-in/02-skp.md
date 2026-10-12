---
title: "2. ขั้น 2 · พางานจาก SketchUp มาด้วย SKP + Object Doctor"
parent: "M3 · ย้ายบ้านมา formZ ใน 4 ขั้น"
nav_order: 2
chapter: true
read_time: 3
do_time: 4
hook: "เปิดไฟล์ SketchUp ใน formZ แล้วซ่อมให้เป็น solid ที่พิมพ์ 3D ได้"
permalink: /courses/m3-move-in/02-skp/
---

# 2. ขั้น 2 · พางานจาก SketchUp มาด้วย SKP + Object Doctor
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- Import ไฟล์ **.skp** โดยตรง
- ใช้ **Object Doctor** ตรวจ/ซ่อม และ **Convert Object Type** เปลี่ยนเป็น solid

## 💡 ไอเดียสั้น ๆ
โมเดล SketchUp เป็น **mesh/facetted** ที่มักมีหน้าหายหรือเส้นซ้อน formZ อ่าน .skp ได้ตรง ๆ (import อย่างเดียว) และ **พยายามแปลงเป็น solid ให้** แต่ทำไม่สำเร็จเสมอถ้าโมเดลปิดไม่สนิท (manual: Trimble SketchUp)

## 👣 ลงมือทำ (4 นาที)
1. **File › Import** → เลือก .skp → ในหน้าต่าง **Modeling Import Options: SketchUp** (ไม่มี option เฉพาะ SketchUp) ปล่อย **Import Textures** ไว้ตามค่าเริ่มต้น (เปิด)
2. **Object Doctor** → ในแท็บ General / Facetted เลือกปัญหาที่จะตรวจ → Action **Fix If Possible** → คลิก object
3. **Convert Object Type** → คลิก object → ใน **Convert Options** ดู Current Object Type แล้วเลือกเป็น solid (ทำได้ถ้าปิดสนิท)
4. ทดลอง **Difference** เจาะรูเพื่อยืนยัน

{: .shot }
[SCREENSHOT: ผล Object Doctor ก่อน/หลังซ่อม]

{: .warning }
ถ้า Group / Component ใน SketchUp ไม่ได้เป็น "Solid" มาตั้งแต่แรก อาจต้องปิดรูเองก่อน

{: .verify }
เวอร์ชัน .skp ที่ formZ 10 รองรับ (คู่มือไม่ระบุ) · ✅ Object Doctor, Fix If Possible, Convert Options ตรวจกับคู่มือแล้ว

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** Import โมเดลจาก 3D Warehouse 1 ชิ้นแล้วลองซ่อม
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ตรวจรูรั่วใช้อะไร?</summary>Object Doctor</details>
<details><summary>2. ทำไม SKP ต้องตรวจก่อน?</summary>เพราะเป็น mesh ที่มักมีหน้าหาย</details>

📚 อ้างอิง: R1 Object Doctor, Convert Object Type, SKP Import
