---
title: "7. รายละเอียด: ล้อ + ร่อง + โลโก้"
parent: "C9 · Portfolio ชิ้นแรก: ของจากบ้านใน 90 นาที"
nav_order: 7
chapter: true
read_time: 3
do_time: 5
track: "🎨 Designer + 📐 Engineering"
permalink: /courses/c9-capstone/07-details/
hook: "ทำ ล้อ scroll (Cylinder + Controlled Round) พร้อมช่องรอบล้อ (clearance 0.5) และทำ ลายกันลื่น ของล้อด้วย Difference แบบกระจายรอบวง (ทวนจาก C8)"
---

# 7. รายละเอียด: ล้อ + ร่อง + โลโก้
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **ล้อ scroll** (Cylinder + Controlled Round) พร้อมช่องรอบล้อ (clearance 0.5)
- ทำ **ลายกันลื่น** ของล้อด้วย Difference แบบกระจายรอบวง (ทวนจาก C8)
- ใส่ **โลโก้** ด้วย Decal ตอนเรนเดอร์ หรือทำเป็นร่องนูน/จม

## 👣 ลงมือทำ (5 นาที)
1. **Cylinder** Ø **18** กว้าง **7** วางแนวแกน Y ระหว่างปุ่ม → **Controlled Round** 1 mm ตั้งชื่อ `Wheel`
2. **ช่องล้อ:** copy ล้อแล้วขยาย (Scale) ให้ใหญ่ขึ้น 0.5 mm รอบตัว → **Difference** ออกจากปุ่ม
3. **ลายล้อ:** กล่องเล็ก 0.6 × 7 × 0.6 หมุน copy 24 ชุด → **Difference**
4. **โลโก้:** ใช้ **Decal** ในเรนเดอร์ (C4 บท 7) หรือ **Text** + **3D Extrusion** 0.3 แล้ว **Difference** จากฐาน
5. **Controlled Round** ขอบร่องทุกขอบ 0.2 mm (ของจริงไม่มีขอบคมกริบ)

{: .shot }
[SCREENSHOT: ซูมล้อ scroll + ช่องล้อ]
{: .shot }
[SCREENSHOT: โลโก้จมที่ฐานเมาส์]

{: .warning }
Controlled Round ขอบเล็ก ๆ หลังทำ Boolean หลายรอบอาจไม่ผ่าน ให้ทำทีละกลุ่มขอบ และกด **Save Incremental** ก่อนทุกครั้ง

{: .verify }
การทำ Text เป็น solid เพื่อทำ Boolean ใน v10 (Text tool → 3D Extrusion) และฟอนต์ไทยทำงานได้ไหม ต้องยืนยัน

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำลายล้อแบบเฉียงแทนแบบตรง
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ช่องล้อเว้นเท่าไร?</summary>0.5 mm รอบตัว</details>
<details><summary>2. ทำไมต้องลบมุมขอบร่อง 0.2 mm?</summary>ดูสมจริง และเรนเดอร์แล้วมีไฮไลต์ที่ขอบ</details>
<details><summary>3. โลโก้ทำได้กี่วิธี?</summary>2 วิธี: Decal ในเรนเดอร์ หรือ Text เป็นร่องนูน/จมจริง</details>

📚 อ้างอิง: R1 Cylinder, Controlled Round, Difference, Text · R2 Decal
