---
title: "3. ผนังหนาเท่ากัน + มุมถอดแม่พิมพ์: Thicken · Draft Angle"
parent: "M5 · วิศวกรตัวน้อย: 6 เช็กก่อนส่งผลิต"
nav_order: 3
chapter: true
read_time: 3
do_time: 3
hook: "ทำกล่องดินสอให้ผนังหนาเท่ากันทั้งชิ้น และใส่มุม draft 1° แบบของที่ฉีดพลาสติกจริง"
track: "📐 Engineering"
permalink: /courses/m5-eng-basics/03-wall-draft/
---

# 3. ผนังหนาเท่ากัน + มุมถอดแม่พิมพ์: Thicken · Draft Angle
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Thicken** กับ solid เพื่อทำให้กลวง ผนังหนาเท่ากัน
- ใส่ **Draft Angle** (Inclination Angle) และตรวจด้วย Surface analysis แบบ **Draft Angle**

## 💡 ไอเดียสั้น ๆ
ของพลาสติกในบ้านส่วนใหญ่ผลิตด้วย **การฉีดพลาสติก (injection molding)** มี 2 กฎพื้นฐาน:
1. **ผนังหนาเท่ากัน** (เช่น 1.5–2.5 mm 🔍) ถ้าหนาไม่เท่ากัน เวลาเย็นตัวจะยุบหรือบิด
2. **มุม draft** ผนังเอียงเล็กน้อย (~1–2° 🔍) เพื่อให้ถอดออกจากแม่พิมพ์ได้ (manual: Draft Angle) ลองดูกล่องพลาสติกในบ้าน จะเห็นว่าปากกว้างกว่าก้นเล็กน้อย

## 👣 ลงมือทำ (3 นาที)
1. **Cube** ขนาดนอก 210 × 60 × 30
2. **Draft Angle** → Inclination Angle **1** → ใช้ค่า **Faces Within n° Of Plane Normal** (ผนังข้าง) → คลิก object
3. **Thicken** ความหนา **2** (ใช้กับ solid = กลวงด้วยผนังเท่ากัน) แล้วลบหน้าบนให้เป็นกล่องเปิด 🔍 วิธีเปิดหน้าบน
4. **Surface analysis** แบบ **Draft Angle**: ตั้ง Minimum/Maximum Angle แล้วดูสี (น้ำเงิน = draft น้อยเกิน)

{: .shot }
[SCREENSHOT: Draft Angle tool options + กล่องก่อน/หลัง]

{: .shot }
[SCREENSHOT: Surface analysis แบบ Draft Angle (สีน้ำเงิน→แดง)]

{: .note }
ถ้าจะ **พิมพ์ 3D** ไม่จำเป็นต้องมี draft แต่ต้องผนัง ≥ 2 เท่าของหัวฉีด (0.4 → 0.8 mm) ตรวจด้วย **Print Preparation › Thin Objects**

{: .verify }
ลำดับ Draft Angle → Thicken ให้ผลดีกว่าสลับกันไหม และเมนูที่เปิด Surface analysis ใน 10.1.x

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ใส่ draft 3° แล้วเทียบว่ามองออกไหมด้วยตาเปล่า
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Thicken กับ solid ได้อะไร?</summary>solid กลวงที่ผนังหนาตามค่าที่ตั้ง</details>
<details><summary>2. draft มีไว้ทำไม?</summary>ให้ถอดชิ้นงานออกจากแม่พิมพ์ได้</details>

📚 อ้างอิง: Manual: Thicken, Draft Angle, Surface analysis (Draft Angle)
