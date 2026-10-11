---
title: "5. Measure Quantities: ปริมาตรและน้ำหนัก"
parent: "C7 · วัดขนาดและเขียนแบบ"
nav_order: 5
chapter: true
read_time: 4
do_time: 3
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/05-quantities/
---

# 5. Measure Quantities: ปริมาตรและน้ำหนัก
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ดู **ปริมาตร (volume)** และ **พื้นที่ผิว (surface area)** ของ solid ด้วย **Measure Quantities**
- เห็น **จุดศูนย์ถ่วง (center of gravity)**
- คำนวณ **น้ำหนักโดยประมาณ** = ปริมาตร × ความหนาแน่น

## 💡 ไอเดียสั้น ๆ
**Measure Quantities** แสดงข้อมูลของวัตถุในแท็บ **Selection** และ **Quantities** และถ้าเป็น solid จะแสดง **จุดศูนย์ถ่วงรวม** เป็นจุดในหน้าต่าง (R1: Measure Quantities)
ข้อมูลนี้ใช้ประมาณ **ต้นทุนวัสดุ** และ **น้ำหนัก** ก่อนผลิต ซึ่งเป็นงานประจำของ product engineer

| วัสดุ | ความหนาแน่น (ประมาณ) |
|---|---|
| พลาสติก ABS | 1.05 g/cm³ |
| PLA (พิมพ์ 3D) | 1.24 g/cm³ |
| แมกนีเซียม (กบเหล็กเล็ก) | 1.74 g/cm³ |
| เหล็กกล้า | 7.85 g/cm³ |

> หน่วย: ถ้าโปรแกรมรายงานเป็น mm³ ให้ **หาร 1,000** เพื่อเป็น cm³

## 👣 ลงมือทำ (3 นาที)
1. **Measure Quantities** คลิก `Body` ดูแท็บ **Quantities**
2. จดปริมาตร (เช่น 6,500 mm³ = 6.5 cm³)
3. คำนวณ: ABS 6.5 × 1.05 ≈ **6.8 g** · แมกนีเซียม ≈ **11.3 g**
4. ชั่งของจริงด้วยเครื่องชั่งในครัว (ถ้ามี) แล้วเทียบผล
5. ดูจุดศูนย์ถ่วงที่แสดงในหน้าต่าง

{: .shot }
[SCREENSHOT: Measure Quantities > Quantities tab ของ Body]
{: .shot }
[SCREENSHOT: จุด center of gravity ในหน้าต่าง]

{: .verify }
หน่วยที่แสดงในแท็บ Quantities (mm³ หรือ cm³ ตาม Working Units) และรายการค่าที่แสดง ต้องยืนยันบนเครื่องจริง

{: .power }
SketchUp แสดง volume ได้เฉพาะ solid group ที่ปิดสนิท และไม่มีจุดศูนย์ถ่วง ส่วน formZ ให้ข้อมูลครบทันทีเพราะทำงานเป็น solid ตั้งแต่แรก

{: .note }
formZ ยังมีเครื่องมือ **Mass Properties** (กลุ่ม Measuring) ที่แสดง **Weight And Volume** จาก density และ **Moments Of Inertia** ด้วย ซึ่งเราจะใช้ใน [C8 บท 9]({{ '/courses/c8-make-it/09-step/' | relative_url }})

## ✅ เช็คตัวเอง
<details><summary>1. น้ำหนักคำนวณอย่างไร?</summary>ปริมาตร × ความหนาแน่น</details>
<details><summary>2. 6,500 mm³ เท่ากับกี่ cm³?</summary>6.5 cm³</details>
<details><summary>3. จุดศูนย์ถ่วงสำคัญกับสินค้าอย่างไร?</summary>บอกว่าวางแล้วล้มง่ายไหม และถือแล้วรู้สึกสมดุลไหม</details>

📚 อ้างอิง: R1 Measure Quantities
