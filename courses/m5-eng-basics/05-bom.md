---
title: "5. รายการชิ้นส่วน (BOM) + น้ำหนัก: Mass Properties"
parent: "M5 · วิศวกรตัวน้อย: 6 เช็กก่อนส่งผลิต"
nav_order: 5
chapter: true
read_time: 2
do_time: 3
hook: "ทำตาราง BOM ของกล่องดินสอ 3 ชิ้น พร้อมวัสดุ จำนวน และน้ำหนักจริงจาก formZ"
track: "📐 Engineering"
permalink: /courses/m5-eng-basics/05-bom/
---

# 5. รายการชิ้นส่วน (BOM) + น้ำหนัก: Mass Properties
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เขียน **BOM (Bill of Materials)**: เลขชิ้น · ชื่อ · จำนวน · วัสดุ · วิธีผลิต · น้ำหนัก
- ใช้ **Mass Properties** (Weight And Volume) หาน้ำหนักจากความหนาแน่น

## 💡 ไอเดียสั้น ๆ
BOM คือ "ใบสั่งซื้อ" ของโรงงาน ทุกชิ้นต้องมีชื่อเดียวกันใน **โมเดล ตาราง และแบบ (C7)**

| # | ชิ้น | จำนวน | วัสดุ | วิธีผลิต | น้ำหนัก (g) |
|---|---|---|---|---|---|
| 01 | box_body | 1 | PP | ฉีดพลาสติก | (Mass Properties) |
| 02 | lid | 1 | PP | ฉีดพลาสติก | … |
| 03 | magnet_6x2 | 2 | แม่เหล็กนีโอดิเมียม | ซื้อสำเร็จ | 0.4 🔍 |

## 👣 ลงมือทำ (3 นาที)
1. ตั้งชื่อ object ทุกชิ้นใน **Objects palette** ตามตาราง (01_box_body, 02_lid…)
2. **Mass Properties** → คลิก box_body → ส่วน **Weight And Volume** ใส่ density PP **0.9 g/cm³** 🔍 → อ่าน Volume/Weight (เลือกหน่วยจาก popup)
3. ทำซ้ำกับ lid
4. ใส่ตัวเลขลงตาราง BOM (Google Sheets / กระดาษ) แล้วแนบในบอร์ด C9

{: .shot }
[SCREENSHOT: Mass Properties › Weight And Volume]

{: .shot }
[SCREENSHOT: ตาราง BOM เสร็จ]

{: .verify }
formZ 10 ไม่มีคำสั่ง "BOM อัตโนมัติ" ในคู่มือ ใช้ Objects palette + ตารางเองไปก่อน (หรือ **Measure Quantities** ดูข้อมูล object)

{: .note }
ชิ้นซื้อสำเร็จ (สกรู แม่เหล็ก) ใส่ใน BOM ด้วยแม้ไม่ได้ปั้นเอง

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ประมาณค่าพลาสติกของกล่อง: น้ำหนัก × ราคา PP ต่อกิโล
</div>

## ✅ เช็คตัวเอง
<details><summary>1. น้ำหนักหาจากเครื่องมือไหน?</summary>Mass Properties (Weight And Volume)</details>
<details><summary>2. ชิ้นที่ซื้อสำเร็จต้องอยู่ใน BOM ไหม?</summary>ต้องอยู่</details>

📚 อ้างอิง: Manual: Mass Properties, Measure Quantities
