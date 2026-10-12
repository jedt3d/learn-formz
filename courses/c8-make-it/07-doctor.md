---
title: "7. Object Doctor: ซ่อม solid"
parent: "C8 · พิมพ์ 3D ให้ขันได้จริง: ขวด + ฝาเกลียว"
nav_order: 7
chapter: true
read_time: 4
do_time: 3
track: "📐 Engineering"
permalink: /courses/c8-make-it/07-doctor/
hook: "ใช้ Object Doctor แบบ 'ตรวจ' (Add To Selection) และแบบ 'ซ่อม' (Fix If Possible) และรู้จัก 3 แท็บ General / Facetted / Smooth"
---

# 7. Object Doctor: ซ่อม solid
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Object Doctor** แบบ "ตรวจ" (**Add To Selection**) และแบบ "ซ่อม" (**Fix If Possible**)
- รู้จัก 3 แท็บ **General / Facetted / Smooth**
- รู้ทางเลือกเมื่อซ่อมอัตโนมัติไม่สำเร็จ

## 💡 ไอเดียสั้น ๆ

| Print Preparation | Object Doctor |
|---|---|
| ตรวจ "พิมพ์ได้ไหม" ทั้งโปรเจกต์ | ตรวจ "โครงสร้าง solid ถูกต้องไหม" ทีละชิ้น |
| ไม่ซ่อม | **ซ่อมได้** (Fix If Possible) |

ปัญหาที่พบบ่อยหลัง Boolean หลายรอบ: ขอบซ้ำ, หน้าที่ไม่ planar, จุดซ้อน ซึ่ง Object Doctor หาให้ได้ เปิด **Display Results** เพื่อดูรายงาน (R1: Object Doctor)

## 👣 ลงมือทำ (3 นาที)
1. เลือก **Object Doctor** แล้วเปิดทุกหัวข้อในแท็บ General และ Smooth
2. Action: **Add To Selection** + **Display Results** → คลิก `Bottle` แล้วอ่านรายงาน
3. ถ้ามีปัญหา เปลี่ยนเป็น **Fix If Possible** แล้วคลิกซ้ำ
4. ทำแบบเดียวกันกับ `Cap`
5. รัน **Print Preparation** อีกรอบ ควรผ่านหมด ✅

{: .shot }
[SCREENSHOT: Object Doctor palette 3 แท็บ + Action group]
{: .shot }
[SCREENSHOT: Display Results หลังตรวจ Bottle]

{: .note }
**ซ่อมไม่ได้?** ① Undo กลับไปก่อน Boolean ที่มีปัญหาแล้วลองขยับตัวตัด 0.1 mm (ไม่ให้ผิวซ้อนพอดี) ② แปลงเป็น Facetted ด้วย **Convert Object Type** แล้วตรวจใหม่ ③ ทำชิ้นนั้นใหม่

{: .verify }
รายชื่อหัวข้อในแต่ละแท็บของ Object Doctor ใน v10 (manual ไม่ได้ระบุทั้งหมด) ให้ถ่ายภาพหน้าจอ palette ไว้ด้วย

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** จดชื่อปัญหาที่ Object Doctor เจอ แล้วอธิบายเป็นภาษาตัวเอง
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Add To Selection กับ Fix If Possible ต่างกันอย่างไร?</summary>Add To Selection แค่ตรวจและเลือกชิ้นที่มีปัญหา ส่วน Fix If Possible พยายามซ่อมให้</details>
<details><summary>2. ทำไม Boolean แล้วมักมีปัญหา?</summary>ผิวที่ซ้อนกันพอดีหรือขอบที่เฉียดกันทำให้เกิดขอบหรือจุดซ้ำ</details>
<details><summary>3. ซ่อมไม่ได้ ลองอะไรได้บ้าง?</summary>ขยับตัวตัดเล็กน้อยแล้วทำ Boolean ใหม่, Convert Object Type, หรือทำชิ้นนั้นใหม่</details>

📚 อ้างอิง: R1 Object Doctor, Project Doctor, Convert Object Type
