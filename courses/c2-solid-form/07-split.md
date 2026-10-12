---
title: "7. ผ่าครึ่งได้ 2 ชิ้น: Split"
parent: "C2 · แม็กเย็บ: 10 ท่า Solid ที่ใช้ทุกวัน"
nav_order: 7
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c2-solid-form/07-split/
hook: "ใช้ Split (Boolean Split) แบ่ง solid หนึ่งชิ้นเป็นสองชิ้นด้วยตัวตัด และรู้ว่า One Way ต่างจาก Two Way อย่างไร"
---

# 7. ผ่าครึ่งได้ 2 ชิ้น: Split
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Split** (Boolean Split) แบ่ง solid หนึ่งชิ้นเป็นสองชิ้นด้วยตัวตัด
- รู้ว่า **One Way** ต่างจาก **Two Way** อย่างไร
- รู้จัก **Slice** ซึ่งเป็นการตัดด้วยเส้น

## 💡 ไอเดียสั้น ๆ
นักออกแบบมักปั้น **ก้อนรวม** ก่อนให้ฟอร์มสวย แล้วค่อย **แบ่งเป็นชิ้นส่วน** ที่ผลิตได้ วิธีนี้ทำให้ทุกชิ้นต่อกันพอดีเสมอ
**Split** = Difference + Intersection ในครั้งเดียว (R1: Boolean Split)

| ตัวเลือก | ผล |
|---|---|
| **One Way** | ชิ้นแรกถูกแบ่งด้วยชิ้นที่สอง |
| **Two Way** | ทั้งสองชิ้นแบ่งกันและกัน |
| **Slice** (อีกเครื่องมือ) | ตัดด้วย **เส้น** ที่ดึงตั้งฉากกับ reference plane เปิด **Heal** เพื่อปิดรอยตัด |

## 👣 ลงมือทำ (4 นาที)
1. สร้าง **ตัวตัด** ด้วย **Cube** (Diagonal) จากมุม (0, −10, 30) ถึง (140, 50, 30) แล้วตั้ง Height **30** (กล่องจะคลุมส่วนบนตั้งแต่ z = 30 ขึ้นไป)
2. เลือก **Split** ใน Tool Options ตั้ง **One Way**
3. คลิก `Upper` ก่อน แล้วคลิกตัวตัด
4. ตัวบนจะแบ่งเป็น 2 ชิ้น: ส่วนบน (z > 30) ตั้งชื่อ `Cover` และส่วนล่างตั้งชื่อ `Magazine` (รางลวด)
5. ลบตัวตัดทิ้ง (ถ้ายังเหลือ) แล้วลอง Move `Cover` ขึ้น 10 mm ดูรอยแยก จากนั้น Undo และบันทึกไฟล์

{: .shot }
[SCREENSHOT: ตัวตัดคลุมส่วนบนของ Upper ก่อนทำ Split]
{: .shot }
[SCREENSHOT: Cover ยกขึ้น 10 mm ให้เห็นว่าแยกจาก Magazine]

{: .verify }
ผลของ One Way ใน v10 (ได้ 2 ชิ้นแยกกันทันที หรือได้ 1 object ที่มี 2 volume แล้วต้องใช้ **Separate** แยกอีกที) ต้องยืนยันบนเครื่องจริง ถ้าได้ 1 object ให้ใช้เครื่องมือ **Separate**

{: .easy }
ทำแค่ 2 คลิก แล้วชิ้นส่วนจะต่อกันพอดี 100%

{: .power }
SketchUp ต้องใช้ **Solid Tools > Split** ซึ่งทำงานได้กับ solid group ที่ปิดสนิทเท่านั้น (และอยู่ในรุ่นเสียเงิน) ส่วน formZ ทำได้กับ solid ทุกชิ้น และยังมี Slice กับ Trim/Split ให้เลือกอีก

{: .shapr }
Shapr3D: **Split body** ด้วย plane หรือ body · formZ: **Split** (ใช้ body) หรือ **Slice** (ใช้เส้น)

{% include can-sketchup.html id=3 %}

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** Split ฐานออกเป็น 2 สีแล้วใส่วัสดุคนละสี
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Split ต่างจาก Difference อย่างไร?</summary>Difference ทิ้งส่วนที่ตัดออก ส่วน Split เก็บไว้ทั้งสองส่วน</details>
<details><summary>2. ทำไมต้องปั้นเป็นก้อนรวมก่อนแล้วค่อยแบ่ง?</summary>เพื่อให้ผิวต่อกันพอดีและฟอร์มรวมไหลต่อเนื่อง</details>
<details><summary>3. Heal ใน Slice ทำอะไร?</summary>ปิดรอยตัดให้ชิ้นที่ได้ยังเป็น solid</details>

📚 อ้างอิง: R1 Boolean Split, Slice, Separating Grouping and Ungrouping
