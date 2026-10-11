---
title: "3. เหลาดินสอด้วย Intersection"
parent: "C3 · ผิวโค้งแบบมือโปร"
nav_order: 3
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c3-curves-surfaces/03-sharpen/
---

# 3. เหลาดินสอด้วย Intersection
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Intersection** เก็บเฉพาะส่วนที่ 2 ชิ้นซ้อนทับกัน
- ได้ปลายดินสอที่มี **ขอบหยัก 6 ลอน** เหมือนเหลาจริง
- เรนเดอร์ดินสอ 1 ภาพ (ไม้ + สี + ไส้)

## 💡 ไอเดียสั้น ๆ
ทำไมปลายดินสอที่เหลาแล้วถึงมี "ลอน" 6 ลอน? เพราะกบเหลาตัดเป็น **กรวย** ทะลุ **หกเหลี่ยม** ส่วนที่เหลือคือส่วนที่อยู่ในทั้งสองรูป ซึ่งก็คือ **Intersection** นั่นเอง (เหมือนกบเหลาจริง)

## 👣 ลงมือทำ (4 นาที)
1. เลือก **Intersection** แล้วคลิก `Hex` จากนั้นคลิก `SharpenShape`
2. หมุนดูปลาย จะเห็นลอนที่หน้าแบนทั้ง 6 ไปบรรจบกับกรวย
3. ไส้ดินสอ: **Cone > Preset** R **1.2** H **5** วางที่ปลายกรวย (snap ที่ปลาย) แล้วจัดให้จมลงไปในเนื้อไม้เล็กน้อย
4. Material:
   - ตัวดินสอใช้สีเหลือง
   - ใช้ **Paint** คลิกเฉพาะ **หน้ากรวย** ให้เป็นสีไม้
   - ไส้ใช้สีเทาดำ กึ่งเงา
5. วางนอน (Rotate บนระนาบ ZX 90°) แล้ว **RenderZone** ภาพ `C3_Pencil.png`

{: .shot }
[SCREENSHOT: ปลายดินสอหลัง Intersection เห็นลอน 6 ลอน]
{: .shot }
[SCREENSHOT: ภาพเรนเดอร์ดินสอ (เหลือง + ไม้ + ไส้)]

{: .note }
ผลจาก Boolean ระหว่าง facetted กับ smooth จะได้วัตถุ **smooth** ที่มีหน้าแบนผสมอยู่ ถ้าจะส่งไปพิมพ์ 3D ภายหลังก็ยังเป็น solid ปกติ

{: .verify }
ชนิดของผลลัพธ์ (smooth หรือ facetted) เมื่อ Boolean ระหว่างวัตถุต่างชนิดกันใน v10 ให้ตรวจใน Inspector > Info ของเครื่องจริง

{: .power }
ปลายแบบลอนนี้ใน SketchUp ทำได้ยากมาก เพราะ Intersect Faces ของ SketchUp ทิ้งเศษผิวไว้เต็มไปหมด ส่วน formZ ได้ solid ที่สะอาดในคลิกเดียว

{: .shapr }
Shapr3D: **Intersect** · formZ: **Intersection** (ชื่อต่างกันนิดเดียว)

## ✅ เช็คตัวเอง
<details><summary>1. Intersection เก็บส่วนไหนไว้?</summary>ส่วนที่อยู่ในทั้งสองชิ้น</details>
<details><summary>2. ใส่สีให้หน้าเดียวทำอย่างไร?</summary>ทำ material ให้ active แล้วใช้ Paint คลิกหน้านั้น</details>
<details><summary>3. ทำไมได้ 6 ลอน?</summary>เพราะหน้าแบนทั้ง 6 ของหกเหลี่ยมถูกกรวยตัดเป็นเส้นโค้ง</details>

📚 อ้างอิง: R1 Intersection, Paint
