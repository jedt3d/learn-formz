---
title: "2. Waffle: ซี่ U/V + Notch"
parent: "M4 · ขาตั้งมือถือ Waffle: ตัดเลเซอร์ใน 30 นาที"
nav_order: 2
chapter: true
read_time: 3
do_time: 6
hook: "เปลี่ยนผิวโค้งเป็นโครงซี่ไขว้กันที่มีร่องสวมพอดีความหนาไม้"
edition: pro
track: "📐 Engineering"
permalink: /courses/m4-waffle/02-waffle/
---

# 2. Waffle: ซี่ U/V + Notch
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ตั้ง **Number in U / Number in V**, **Height**, **Justification**
- ตั้ง **Object Type = Surfaces** + **Notch** ให้ Width = ความหนาวัสดุ

## 💡 ไอเดียสั้น ๆ
| ค่า | ตั้ง | เพราะ |
|---|---|---|
| Number in U / V | 6 / 3 | ซี่ตามยาว 6 ชิ้น ตามขวาง 3 ชิ้น พอแข็งแรง |
| Height | 25 | ความลึกของซี่ |
| Justification | Below | ซี่อยู่ใต้ผิว ด้านบนเรียบสำหรับวางมือถือ |
| Derive From | (orthogonal) 🔍 | ระยะห่างเท่ากัน ตัดง่าย |
| Object Type | **Surfaces** + **Notch** | manual แนะนำสำหรับเลเซอร์/CNC |
| Width | **3** (= ไม้อัด 3 mm) | ร่องลึกครึ่งหนึ่งของ Height อัตโนมัติ |

## 👣 ลงมือทำ (6 นาที)
1. เลือก **Waffle** (Pro 10.1) → คลิก surface จากบท 1
2. ตั้งค่าตามตาราง
3. ดูผล: ทุกจุดที่ซี่ตัดกันต้องมีร่อง (notch)
4. ถ้าซี่ปลายสั้นเกิน (< 10 mm) ลด Number in U ลง 1

{: .shot }
[SCREENSHOT: Waffle Tool Options + โครงซี่ที่ได้]

{: .shot }
[SCREENSHOT: ซูมดู notch ที่ซี่ตัดกัน]

{: .warning }
ไม้จริงหนาไม่ตรง 3.00 เสมอ ให้วัดด้วยเวอร์เนียร์ก่อน แล้วลองตัดชิ้นทดสอบ 2 ชิ้น (manual: ความกว้างอาจต้องปรับตามเครื่องตัดและวัสดุ)

{: .note }
ถ้าจะ **พิมพ์ 3D** แทน ให้ใช้ **Solids** + Notch + **Notch Tolerance** (เช่น 0.3) แล้ว export STL

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ใส่ Number in V = 0 แล้วดูว่าเกิดอะไร (จะเหลือซี่ทิศเดียว)
</div>

## ✅ เช็คตัวเอง
<details><summary>1. notch ลึกเท่าไร?</summary>ครึ่งหนึ่งของ Height</details>
<details><summary>2. ตัดเลเซอร์ควรใช้ Object Type อะไร?</summary>Surfaces + Notch โดยตั้ง Width เท่ากับความหนาวัสดุ</details>

📚 อ้างอิง: Manual: Waffle (Ribs, Object Type, Notch, Fabrication Guide)
