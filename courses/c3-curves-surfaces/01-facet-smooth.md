---
title: "1. Facetted vs Smooth ใน 5 นาที"
parent: "C3 · โค้งแบบมือโปร: ดินสอ + กาต้มน้ำ"
nav_order: 1
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c3-curves-surfaces/01-facet-smooth/
hook: "อธิบายได้ว่า facetted object กับ smooth object ต่างกันอย่างไร และปรับ Display Resolution ของวัตถุ smooth"
---

# 1. Facetted vs Smooth ใน 5 นาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- อธิบายได้ว่า **facetted object** กับ **smooth object** ต่างกันอย่างไร
- ปรับ **Display Resolution** ของวัตถุ smooth
- แปลงชนิดวัตถุด้วย **Convert Object Type**

## 💡 ไอเดียสั้น ๆ
formZ มีวัตถุ 2 ตระกูล
- **Facetted**: ผิวเป็น **หน้าแบนหลายเหลี่ยม** (polygon) จริง ๆ เหมาะกับของเหลี่ยม เช่น ดินสอหกเหลี่ยม
- **Smooth**: ผิวเป็น **คณิตศาสตร์โค้งจริง** แต่บนจอจะแสดงเป็นเหลี่ยมเล็ก ๆ (faceting) เพื่อให้วาดเร็ว ความละเอียดของการแสดงผลตั้งได้ที่ **Display Resolution** ใน Tool Options และใช้ **Faceting Schemes** สำเร็จรูปได้ (R1: Faceting Schemes)

> ถ้าเห็นเหลี่ยมบนวัตถุ smooth ไม่ได้แปลว่าผิวเป็นเหลี่ยมจริง แค่ **แสดงผล** แบบหยาบ

## 👣 ลงมือทำ (3 นาที)
1. ไฟล์ใหม่ `C3_Warmup.fmz` · **Sphere** (Preset) รัศมี 20 จำนวน 2 ลูก วางห่างกัน 60 mm
2. เลือกลูกที่ 2 แล้วใช้ **Convert Object Type** ในหน้าต่าง Convert Options เปลี่ยนเป็น **Facetted**
3. สลับไป **Wire Frame** แล้วเทียบ: ลูก smooth มีเส้นน้อย ส่วนลูก facetted มีหน้าเหลี่ยมจริง
4. เลือกลูก smooth แล้วเพิ่ม **Display Resolution** ใน Tool Options จะเห็นว่าเนียนขึ้นบนจอ

{: .shot }
[SCREENSHOT: ลูกบอล smooth กับ facetted ใน Wire Frame คู่กัน]
{: .shot }
[SCREENSHOT: Convert Options dialog (Current Object Type → Facetted)]

{: .verify }
ช่อง Display Resolution ของ Sphere ที่สร้างแล้ว แก้ได้ใน Tool Options เลย หรือต้องแก้ผ่าน Inspector ให้ยืนยันใน v10

{: .power }
SketchUp มีแต่วัตถุแบบ **facetted** (ผิวเหลี่ยม) วงกลมใน SketchUp คือรูปหลายเหลี่ยม 24 ด้าน ส่วน formZ มีผิวโค้งจริง และแปลงไปมาระหว่าง 2 แบบได้

{: .shapr }
Shapr3D (Parasolid) เป็นผิวโค้งจริงทั้งหมด จึงเทียบได้กับ **Smooth** ของ formZ · ส่วน Blender mesh คือ **Facetted**

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** เปลี่ยน Display Resolution ของทรงกลมแล้วจับภาพ 3 ระดับ
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมวัตถุ smooth ยังเห็นเป็นเหลี่ยมบนจอ?</summary>เพราะจอแสดงผลด้วย faceting ตาม Display Resolution ส่วนผิวจริงยังโค้งเนียน</details>
<details><summary>2. ดินสอหกเหลี่ยมควรเป็นวัตถุแบบไหน?</summary>Facetted เพราะมีหน้าแบนจริง</details>
<details><summary>3. ใช้เครื่องมืออะไรแปลงชนิด?</summary>Convert Object Type</details>

📚 อ้างอิง: R1 Faceting Schemes, Convert Object Type
