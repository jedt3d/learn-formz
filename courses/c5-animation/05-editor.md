---
title: "5. Animation Editor: ทำให้นุ่ม"
parent: "C5 · Animation จากโมเดล"
nav_order: 5
chapter: true
read_time: 4
do_time: 5
permalink: /courses/c5-animation/05-editor/
---

# 5. Animation Editor: ทำให้นุ่ม
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- อ่าน **กราฟ track** (เช่น Rotation Y) ใน **Animation Editor** palette
- ปรับ **lead in / lead out** ของ key ให้เป็น **flat** (ค่อย ๆ หยุด) หรือ **Linear** (กระชาก)
- ทำให้ฝาเปิดเร็ว แต่ปิดนุ่มแบบสปริง

## 💡 ไอเดียสั้น ๆ
กราฟใน Animation Editor มี **แกนนอน = เวลา** และ **แกนตั้ง = ค่า** (เช่น มุม) ช่วงที่กราฟ **ชัน** = เร็ว ส่วนช่วงที่ **แบน** = ช้า แต่ละ key มี "หนวด" 2 ข้าง คือ **lead in** (ซ้าย) และ **lead out** (ขวา) ซึ่งกำหนดการเร่ง/ผ่อนความเร็ว (R5: Swinging door tutorial)

| ต้องการ | ทำที่ key |
|---|---|
| ค่อย ๆ หยุดนุ่ม (ease) | ทำ lead ให้ **flat** |
| เริ่มทันทีแบบกระชาก | Lead Out = **Linear** |

## 👣 ลงมือทำ (5 นาที)
1. เปิด **Animation Editor** palette แล้วเลือก `UpperArm`
2. คลิก track **Rotation Y** (ซ่อน track อื่นด้วยรูปตา)
3. คลิก key ที่ 4.0 → ส่วน **Key** ด้านล่าง ตั้ง **Lead Out = Linear** (ฝาเริ่มเปิดทันที)
4. คลิก key ที่ 6.0 → ทำ lead in ให้ flat (ฝาปิดลงนุ่ม)
5. Play แล้วเทียบกับก่อนแก้ ถ้ากราฟอยู่นอกจอ ให้ใช้ปุ่ม **Zoom out** ของ palette

{: .shot }
[SCREENSHOT: Animation Editor: กราฟ Rotation Y พร้อม lead in/out ที่ key 6.0]

{: .easy }
เหมือนการตั้ง easing ใน Keynote หรือ PowerPoint แต่เราวาดกราฟเองได้

{: .shapr }
คนที่เคยใช้ Blender จะคุ้นกับ **Graph Editor** ซึ่งมีหลักการเดียวกัน

## ✅ เช็คตัวเอง
<details><summary>1. กราฟชันหมายถึงอะไร?</summary>ค่าเปลี่ยนเร็ว (ของขยับเร็ว)</details>
<details><summary>2. อยากให้หยุดนุ่มต้องทำอะไร?</summary>ทำ lead ของ key ที่จุดหยุดให้ flat</details>
<details><summary>3. lead out อยู่ด้านไหนของ key?</summary>ด้านขวา (ไปทางเวลาข้างหน้า)</details>

📚 อ้างอิง: R5 The Animation Editor Palette, Animation Controller Functions, Swinging door tutorial
