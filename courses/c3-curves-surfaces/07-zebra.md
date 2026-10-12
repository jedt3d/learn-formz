---
title: "7. ลายม้าลายบอกความเนียน: Zebra"
parent: "C3 · โค้งแบบมือโปร: ดินสอ + กาต้มน้ำ"
nav_order: 7
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c3-curves-surfaces/07-zebra/
hook: "เปิด Surface Analysis แบบ Zebra Stripes บนวัตถุ และอ่านลายม้าลายให้เป็น (เส้นต่อเนื่อง = เนียน, เส้นหัก = รอยต่อ)"
---

# 7. ลายม้าลายบอกความเนียน: Zebra
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เปิด **Surface Analysis** แบบ **Zebra Stripes** บนวัตถุ
- อ่านลายม้าลายให้เป็น (เส้นต่อเนื่อง = เนียน, เส้นหัก = รอยต่อ)
- **Union** พวยกับตัวกา แล้วตรวจรอยต่อ

## 💡 ไอเดียสั้น ๆ
นักออกแบบรถยนต์ตรวจผิวรถต้นแบบด้วยการส่องไฟเป็นแถบยาวสะท้อนบนผิว ถ้าแถบสะท้อน **ต่อเนื่องไม่หัก** แปลว่าผิวเนียน formZ จำลองวิธีนี้ด้วย **Zebra Stripes** (R1: Surface Analysis)
Surface analysis เป็น **attribute ที่ติดไปกับวัตถุ** แสดงใน **Shaded Work** ได้ระหว่างทำงาน

## 👣 ลงมือทำ (3 นาที)
1. **Union** `Body` กับ `Spout`
2. สลับเป็น **Shaded Work** แล้วเลือกตัวกาด้วย **Pick**
3. ใน Pick Tool Options เปิดแท็บ **Attributes** เลือก **Analysis** จาก popup ด้านบน แล้วติ๊ก **Analyze Object**
4. **Analysis Type** เลือก **Zebra Stripes** แล้วปรับจำนวนแถบ
5. หมุนดู: ตัวกาควรมีแถบต่อเนื่องดี ส่วนรอยต่อพวยจะเห็นแถบ **หักมุม** ซึ่งเป็นเรื่องปกติของ Union
6. (เสริม) ถ้าอยากได้รอยต่อนุ่ม ให้ลอง **Controlled Round** ที่ขอบรอยต่อ R3 แล้วดู Zebra อีกครั้ง

{: .shot }
[SCREENSHOT: Pick Tool Options > Attributes > Analysis > Zebra Stripes]
{: .shot }
[SCREENSHOT: ตัวกาที่มีลาย Zebra (เห็นรอยหักที่ฐานพวย)]

{: .power }
SketchUp **ไม่มีเครื่องมือวิเคราะห์ผิว** เลย ส่วน formZ มี Zebra และวิธีอื่น ๆ ใน Analysis Type ให้เลือกแบบเดียวกับ CAD สายรถยนต์

{: .shapr }
Shapr3D: Visualization > **Zebra** · formZ: Pick > Attributes > **Analysis > Zebra Stripes**

{% include can-sketchup.html id=4 %}

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** หาจุดที่ลาย Zebra หักบนกาของเรา แล้วแก้ให้ลายต่อกัน
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Zebra แสดงในโหมดไหน?</summary>Shaded Work</details>
<details><summary>2. แถบหักมุมบอกอะไร?</summary>ผิวไม่ต่อเนื่อง มีรอยหัก (ความโค้งเปลี่ยนแบบกระโดด)</details>
<details><summary>3. ทำให้รอยต่อนุ่มขึ้นได้อย่างไร?</summary>ลบมุมที่ขอบรอยต่อ หรือใช้เครื่องมือ blend ของ NURBS (NURBS Surface Blend)</details>

📚 อ้างอิง: R1 Surface Analysis
