---
title: "2. ฐานแม็กใน 3 คลิก: Rectangle + 3D Extrusion"
parent: "C2 · แม็กเย็บ: 10 ท่า Solid ที่ใช้ทุกวัน"
nav_order: 2
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c2-solid-form/02-base/
hook: "รู้จัก Draw suite และ object type 6 แบบ ใน Tool Options และวาด Rectangle แล้วได้เป็น solid ทันทีด้วย 3D Extrusion"
---

# 2. ฐานแม็กใน 3 คลิก: Rectangle + 3D Extrusion
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- รู้จัก **Draw suite** และ **object type 6 แบบ** ใน Tool Options
- วาด **Rectangle** แล้วได้เป็น solid ทันทีด้วย **3D Extrusion**
- ใช้ช่อง **Length / Width / Height** ใน Input palette และกด **Tab** เพื่อล็อกค่า

## 💡 ไอเดียสั้น ๆ
ใน C1 เราใช้ **Create suite** (primitive) ส่วน **Draw suite** คือการวาดรูป 2D ซึ่งจะเลือกได้ว่าอยากได้ผลเป็นอะไร (R1: Drawing Objects)

| object type (ไอคอนใน Tool Options) | ได้อะไร |
|---|---|
| **2D** (เส้นหรือผิว) | รูป 2D แบน ๆ |
| **3D Extrusion** | solid ที่ดึงขึ้นตามความสูง ⭐ ใช้บ่อยที่สุด |
| **3D Extrusion To Point** | ดึงขึ้นไปบรรจบที่จุดเดียว (แบบพีระมิด) |
| **3D Wall** | ผนังหนาตามเส้นที่วาด |
| อีก 2 แบบ | ดูใน Tool Options |

{: .verify }
คู่มือบอกว่ามี **6 ไอคอน** และระบุชื่อ 2D, 3D Extrusion, 3D Extrusion To Point, 3D Wall ส่วนอีก 2 แบบที่เหลือให้ยืนยันชื่อบนหน้าจอจริง

## 👣 ลงมือทำ (4 นาที)
1. สลับ reference plane กลับเป็น **XY**
2. เลือกเครื่องมือ **Rectangle** (Draw suite) แล้วเลือก object type **3D Extrusion**
3. คลิกจุดแรกที่ (0, 0, 0)
4. ระหว่างลากมุมที่สอง ให้ดู **Input palette** ช่องด้านขวาจะมี **Length** และ **Width** พิมพ์ `130` แล้วกด **Tab** (ค่าจะล็อก) จากนั้นพิมพ์ `35` แล้วกด Enter
5. ช่องจะเปลี่ยนเป็น **Height** ให้พิมพ์ `10` แล้วกด Enter
6. ตั้งชื่อ object เป็น `Base` แล้วบันทึกไฟล์

{: .shot }
[SCREENSHOT: Input palette ตอนวาด Rectangle เห็นช่อง Length 130 (ล็อกแล้ว) และ Width]
{: .shot }
[SCREENSHOT: ฐาน 130 × 35 × 10 ใน Shaded Work]

{: .note }
เมนูด้านขวาของช่อง x, y, z ใน Input palette เลือกได้ 4 โหมด คือ **3D / 3D Delta / Plane / Plane Delta** โหมด *Delta* จะบอกระยะจากจุดที่คลิกล่าสุด ใช้เวลาอยากรู้ว่า "ห่างจากจุดก่อนหน้าเท่าไร" (R1: Prompts and Numeric Input)

{: .easy }
เหมือน **Rectangle + Push/Pull** ของ SketchUp แต่จบได้ในเครื่องมือเดียว และพิมพ์ตัวเลขได้ตลอดทาง

{: .power }
ผลที่ได้เป็น **solid ปิดสนิท** ตั้งแต่แรก ส่วนใน SketchUp ต้อง Make Group หรือ Component และต้องระวังผิวหลุดก่อนถึงจะเป็น solid

{: .shapr }
Shapr3D: วาด rectangle แล้วดึงหน้าขึ้น · formZ: เลือก **3D Extrusion** ก่อนวาด ได้ผลเหมือนกันในจังหวะเดียว

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำฐานแม็กแบบที่ 2 ที่สั้นลง 10 mm แล้ววางเทียบกัน
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ถ้าอยากได้แค่รูป 2D แบน ๆ เลือก type ไหน?</summary>2D</details>
<details><summary>2. กด Tab หลังพิมพ์ค่าแล้วเกิดอะไรขึ้น?</summary>ค่านั้นถูกล็อกไว้ จนกว่าจะกด Return หรือคลิก</details>
<details><summary>3. Plane Delta ใช้ทำอะไร?</summary>ดูระยะจากจุดที่คลิกล่าสุด ตามแกนของ reference plane ที่ใช้อยู่</details>

📚 อ้างอิง: R1 Drawing Objects, Prompts and Numeric Input
