---
title: "2. Turntable ในคลิกเดียว"
parent: "C5 · Animation จากโมเดล"
nav_order: 2
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c5-animation/02-turntable/
---

# 2. Turntable ในคลิกเดียว
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Create Turntable View** ให้กล้องหมุนรอบสินค้า 360°
- เข้าใจ **center of interest (COI)** ของกล้อง
- รู้ว่าเมื่อไรควรเปิดหรือปิด **Ease In/Out**

## 💡 ไอเดียสั้น ๆ
**Turntable** คือวิดีโอที่ใช้บ่อยที่สุดในงานนำเสนอสินค้า กล้องจะหมุนรอบ **COI** (จุดที่กล้องมอง) formZ 10.1 ทำให้ได้ในคำสั่งเดียว (R7: formZ 10.1)

| ค่า | ความหมาย |
|---|---|
| **Start Time / End Time** | ช่วงเวลาบนไทม์ไลน์ที่จะใส่ animation นี้ |
| **Duration** | ความยาวรวม (วินาที) |
| **Ease In/Out** | ค่อย ๆ เร่งแล้วค่อย ๆ ช้าลง · **ปิด** ไว้ถ้าจะเล่นวนลูป |

## 👣 ลงมือทำ (3 นาที)
1. ตั้งมุมกล้อง Hero ให้ COI อยู่ **กลางแม็กเย็บ** แล้วบันทึก view ใหม่ชื่อ `Turntable_Cam` ใน **Views** palette
2. เลือก `Turntable_Cam` ใน Views palette
3. เรียก **Create Turntable View** (ใน Animation palette) ตั้ง Start **0**, Duration **4**, ปิด Ease In/Out
4. ทำให้ view นั้น active แล้วกด **Play** ใน Time Line palette กล้องจะหมุนรอบสินค้าในเวลา 4 วินาที

{: .shot }
[SCREENSHOT: Create Turntable View dialog]
{: .shot }
[SCREENSHOT: Views palette ที่เลือก Turntable_Cam]

{: .verify }
ตำแหน่งของคำสั่ง **Create Turntable View** (Animation palette หรือเมนู) และวิธีทำให้ view ที่ animate แล้วเป็นมุมมองหลักขณะ preview ต้องยืนยันบน 10.1.x · KB มีบทความ "Create Turntable Animation" (support.formz.com/hc/en-us/articles/28218290231955)

{: .warning }
ถ้า COI ไม่อยู่กลางสินค้า กล้องจะหมุน **เหวี่ยง** ออกนอกจอ ให้ตั้ง COI ใหม่ก่อน

## ✅ เช็คตัวเอง
<details><summary>1. Turntable หมุนรอบจุดไหน?</summary>center of interest (COI) ของกล้อง</details>
<details><summary>2. จะเล่นวนลูปให้ลื่นต้องตั้ง Ease In/Out อย่างไร?</summary>ปิด</details>
<details><summary>3. ต้องเลือกอะไรก่อนเรียกคำสั่ง?</summary>กล้อง (view) ในหน้าต่างหรือใน Views palette</details>

📚 อ้างอิง: R7 formZ 10.1 Release Notes (Create Turntable View) · KB Create Turntable Animation
