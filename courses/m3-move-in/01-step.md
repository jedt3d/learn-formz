---
title: "1. ขั้น 1 · พางานจาก Shapr3D มาด้วย STEP"
parent: "M3 · ย้ายบ้านมา formZ ใน 4 ขั้น"
nav_order: 1
chapter: true
read_time: 3
do_time: 4
hook: "เอางาน Shapr3D ชิ้นเก่ามาเปิดใน formZ เป็น solid ที่แก้ต่อได้"
edition: core
permalink: /courses/m3-move-in/01-step/
---

# 1. ขั้น 1 · พางานจาก Shapr3D มาด้วย STEP
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- Export **STEP** จาก Shapr3D แล้ว **File › Import** ใน formZ
- เปิดตัวเลือก **Heal Corrupt Geometry** และ **Preserve Assembly Hierarchy**

## 💡 ไอเดียสั้น ๆ
STEP เก็บ solid แบบ B-rep เหมือนกันทั้ง 2 โปรแกรม (Shapr3D ใช้ Parasolid ส่วน formZ ใช้ ACIS) จึงย้ายได้แทบไม่เสียรายละเอียด แต่ **ประวัติการสร้างจะไม่ตามมา**

## 👣 ลงมือทำ (4 นาที)
1. Shapr3D: **Export › STEP**
2. formZ: **File › Import** เลือกไฟล์ .step
3. ในหน้าต่าง **Modeling Import Options: STEP** ตรวจว่าติ๊ก **Heal Corrupt Geometry** และ **Preserve Assembly Hierarchy**
4. ตรวจ **Objects palette**: ชิ้นส่วนยังแยกเป็นกลุ่มเหมือนเดิม
5. ลอง **Controlled Round** ขอบหนึ่งเพื่อดูว่าเป็น solid จริง

{: .shot }
[SCREENSHOT: Import options ของ STEP]

{: .shot }
[SCREENSHOT: Objects palette หลัง import]

{: .shapr }
ใน Shapr3D Free export STEP ไม่ได้ 🔍 ถ้าไม่มีให้ใช้ STL แทน (แต่จะได้ mesh)

{: .verify }
edition ที่ import STEP ได้ (Free อาจไม่ได้) · ✅ ชื่อ option ตรวจกับคู่มือแล้ว: ทั้ง 2 ตัว **เปิดอยู่แล้วโดยค่าเริ่มต้น** และถ้าปิด Preserve Assembly Hierarchy, assembly จะถูกรวมแบนเป็นชั้นเดียว

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** Import ไฟล์เดิมแบบไม่ติ๊ก Preserve Assembly Hierarchy แล้วเทียบ Objects palette
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ประวัติจาก Shapr3D ตามมาไหม?</summary>ไม่ ได้แค่รูปทรง solid</details>
<details><summary>2. ทำให้ชิ้นยังแยกกลุ่มต้องติ๊กอะไร?</summary>Preserve Assembly Hierarchy</details>

📚 อ้างอิง: R1 File Formats: STEP Import
