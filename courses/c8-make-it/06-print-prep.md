---
title: "6. Print Preparation"
parent: "C8 · เตรียมผลิต: 3D Print, STEP"
nav_order: 6
chapter: true
read_time: 4
do_time: 3
track: "📐 Engineering"
permalink: /courses/c8-make-it/06-print-prep/
---

# 6. Print Preparation: ตรวจก่อนพิมพ์
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Print Preparation** ตรวจทั้งโปรเจกต์ในคลิกเดียว
- รู้จักเงื่อนไขทั้ง 6: **Non Solids, Inside Out, Duplicate Surfaces, Small Objects, Thin Objects, Large Volume**
- เข้าใจ **World units** กับ **Print units** (หลังคูณ Scale)

## 💡 ไอเดียสั้น ๆ
Print Preparation **ตรวจและไฮไลต์** ปัญหาเท่านั้น **ไม่ซ่อมให้** (ซ่อมด้วย Object Doctor ในบทหน้า หรือแก้เอง) ตรวจ **ทั้งโปรเจกต์** โดยไม่สนว่าเลือกชิ้นไหนไว้ (R1: Print Preparation)

| ส่วนใน palette | ใช้ทำอะไร |
|---|---|
| Device pop-out | เลือกเครื่องพิมพ์ (แต่ละเครื่องมีข้อกำหนดต่างกัน) |
| **Scale**: Scale Factor / Fit Box / Scale To Printer | ขนาดจริงที่จะพิมพ์ (เราใช้ 1 : 1) |
| **Non Solids** | ชิ้นที่ไม่ปิดสนิท |
| **Inside Out** | ผิวกลับด้าน |
| **Duplicate Surfaces** | ผิวซ้อนกัน |
| **Small Objects** | ชิ้นเล็กเกินจะพิมพ์ |
| **Thin Objects** (+ **Create Cross Sections**) | ส่วนที่บางเกิน พร้อมสร้างหน้าตัดให้ดูจุดที่บาง |
| **Large Volume** | ชิ้นตันใหญ่ เปลืองวัสดุ ควรทำให้กลวง |
| **All / None / Execute** | เปิดหรือปิดทุกข้อ และสั่งตรวจ |

## 👣 ลงมือทำ (3 นาที)
1. เลือก **Print Preparation** (กลุ่ม Measuring) → Scale Factor **1**
2. กด **All** แล้วตั้ง Thin Objects = **1.2 mm** (Print units) และเปิด **Create Cross Sections**
3. คลิกในหน้าต่าง (หรือกด **Execute**) แล้วดูว่ามีชิ้นไหนถูกไฮไลต์
4. จดรายการปัญหา เช่น "ปลายเกลียวบาง" หรือ "เส้น 2D ที่ลืมลบเป็น Non Solid"
5. แก้: ลบเส้น 2D และโปรไฟล์ที่เหลือ (หรือย้ายไป Layer ที่ซ่อน) แล้วตรวจซ้ำ

{: .shot }
[SCREENSHOT: Print Prep Tool Options palette ครบทุกช่อง]
{: .shot }
[SCREENSHOT: ปลายเกลียวถูกไฮไลต์ว่า Thin + cross sections]

{: .verify }
ค่าเริ่มต้นของ Small/Thin Objects และรายการ Device ใน 10.1.x ต้องยืนยันจากหน้าจอจริง และควรตรวจว่า layer ที่ซ่อนอยู่ถูกตรวจด้วยหรือไม่

{: .power }
SketchUp ต้องลง extension (เช่น Solid Inspector) ส่วน formZ มีเครื่องมือนี้ **ในตัว**

## ✅ เช็คตัวเอง
<details><summary>1. Print Preparation ซ่อมให้ไหม?</summary>ไม่ซ่อม แค่ตรวจและไฮไลต์</details>
<details><summary>2. Print units ต่างจาก World units อย่างไร?</summary>Print units คือขนาดหลังคูณ Scale ซึ่งเป็นขนาดของชิ้นที่พิมพ์ออกมาจริง</details>
<details><summary>3. Large Volume เตือนเพื่ออะไร?</summary>เตือนว่าชิ้นตันใหญ่เกินไป ควรทำให้กลวงเพื่อประหยัดวัสดุ</details>

📚 อ้างอิง: R1 Print Preparation
