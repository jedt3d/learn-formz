---
title: "2. ปั้นกบเหลาใน 10 นาที"
parent: "C7 · เขียนแบบให้โรงงานอ่านออก: กบเหลา 3 ด้าน"
nav_order: 2
chapter: true
read_time: 3
do_time: 6
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/02-model/
hook: "ปั้นตัวกบด้วยเครื่องมือที่รู้แล้ว (Cube, Controlled Round, Difference, Insert) และเจาะ รูกรวย ตามแนวแกน X ด้วย Cone + Difference"
---

# 2. ปั้นกบเหลาใน 10 นาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ปั้นตัวกบด้วยเครื่องมือที่รู้แล้ว (Cube, Controlled Round, Difference, Insert)
- เจาะ **รูกรวย** ตามแนวแกน X ด้วย Cone + Difference
- ได้โมเดลที่ขนาดตรงกับภาพร่าง

## 💡 ไอเดียสั้น ๆ

| ส่วน | วิธี | ค่า (ตัวอย่าง) |
|---|---|---|
| Body | Cube (Diagonal) (0,0,0)→(26,14,0) สูง 20 | 26 × 14 × 20 |
| ขอบ | Controlled Round ขอบแนวตั้ง | R1.5 |
| รูกรวย | **Cone** R4.1 สูง 24 (ไม่ตัดปลาย) วาดบนระนาบ **YZ** ให้แกนวิ่งตาม X | Ø8.2 |
| ช่องเศษไม้ | Insert: Cut บนหน้าบน | 16 × 3 ทะลุถึงรู |

## 👣 ลงมือทำ (6 นาที)
1. ไฟล์ `C7_Sharpener.fmz` (template mm) สร้าง Body และลบมุม R1.5
2. สลับเป็นระนาบ **YZ** แล้วใช้ **Cone > Preset** R **4.1**, H **24** คลิกที่ (0, 7, 10) ปลายแหลมจะชี้ไปทาง +X (ถ้าชี้ผิดทาง ให้ Mirror หรือ Rotate 180°)
3. **Difference**: Body ก่อน แล้วค่อย Cone
4. **Insert: Cut** วาดช่อง 16 × 3 บนหน้าบน ห่างจากด้านหน้า 5 mm แล้วตั้งความลึกให้ทะลุถึงรูกรวย (ประมาณ 10 mm)
5. หมุนดูใน **Wire Frame** แล้วตั้งชื่อ `Body`

{: .shot }
[SCREENSHOT: Cone บนระนาบ YZ ก่อนทำ Difference]
{: .shot }
[SCREENSHOT: Body ใน Wire Frame เห็นรูกรวยและช่อง]

{: .verify }
ทิศของ Height เมื่อวาด Cone บนระนาบ YZ (+X หรือ −X) ต้องยืนยันบนเครื่องจริง

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำกบเหลาแบบ 2 รูภายใน 3 นาที
</div>

📚 อ้างอิง: R1 Cube, Cone, Difference, Drawing Objects (Insert), Reference planes
