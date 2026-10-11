---
title: "6. Linear + Multi Dimension"
parent: "C7 · วัดขนาดและเขียนแบบ"
nav_order: 6
chapter: true
read_time: 5
do_time: 4
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/06-linear/
---

# 6. Linear + Multi Dimension
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใส่ขนาดด้วย **Linear Dimension** (คลิก 2 จุด หรือคลิกเส้น)
- ใส่ขนาดต่อเนื่องด้วย **Multi Dimension** แบบ **Chain / Stack / Ordinate**
- ตั้ง **Dimension Styles** (ขนาดตัวหนังสือ, Screen vs World)

## 💡 ไอเดียสั้น ๆ
formZ ใส่ dimension บน **โมเดล 3D** ได้โดยตรง (อยู่ในกลุ่ม Text) และถ้า snap กับจุดของวัตถุ dimension จะ **ผูกกับวัตถุ** (บทถัดไป) (R1: Dimensions)

| เครื่องมือ | ใช้เมื่อ |
|---|---|
| **Linear Dimension** | ขนาดเดี่ยว: คลิก 2 จุด → คลิกที่ 3 เพื่อวาง (หรือคลิกเส้นตรง 1 เส้น) |
| **Multi Dimension: Chain** | ระยะต่อกันเป็นช่วง ๆ |
| **Stack** | ทุกระยะวัดจากจุดเริ่มเดียวกัน (ซ้อนชั้น) |
| **Ordinate** | บอกเป็นพิกัดจากจุดศูนย์ (นิยมในงาน CNC) |

**Dimension Styles:** **Type = World** ตัวหนังสือจะมีขนาดจริงในโลก 3D (ย่อขยายตามการซูม) ส่วน **Screen** มีขนาดคงที่บนจอ และสร้าง style ใหม่ได้ด้วย **Edit Styles...** (R1: Dimension Styles)

## 👣 ลงมือทำ (4 นาที)
1. เปิด **Snap to Point** · สลับเป็นระนาบ **XY** · มุมมอง **Top**
2. **Linear Dimension** ใส่ความยาว 26 และความกว้าง 14 (คลิกเส้นขอบ)
3. ระนาบ **ZX** มุมมอง **Front** ใส่ความสูง 20
4. **Multi Dimension (Chain)**: คลิกขอบซ้าย → ขอบช่องเศษไม้ด้านซ้าย → ขอบด้านขวา → ขอบ Body ด้านขวา แล้ว double-click เพื่อวาง
5. **Edit Styles...** สร้าง style `PD_mm_3.5` ตัวหนังสือ 3.5 · Type **World** · ทศนิยม 1 ตำแหน่ง

{: .shot }
[SCREENSHOT: Dimensions dialog (Edit Styles) ที่มี style PD_mm_3.5]
{: .shot }
[SCREENSHOT: Body ที่มี linear + chain dimensions]

{: .verify }
ช่องตั้ง **ทศนิยม/หน่วย** ของ dimension อยู่ใน Dimension Styles หรือใน Working Units ของโปรเจกต์ ต้องยืนยันใน v10

{: .power }
Dimension ของ SketchUp เป็นแค่ข้อความ ส่วน formZ มี Multi Dimension 3 แบบ (Chain/Stack/Ordinate) และ style ที่ใช้กับงานผลิตได้

## ✅ เช็คตัวเอง
<details><summary>1. Chain กับ Stack ต่างกันอย่างไร?</summary>Chain วัดต่อกันทีละช่วง ส่วน Stack วัดจากจุดเริ่มเดียวกันทุกเส้น</details>
<details><summary>2. Ordinate เหมาะกับงานแบบไหน?</summary>งาน CNC หรือเจาะรูที่บอกพิกัดจากจุดอ้างอิง</details>
<details><summary>3. World กับ Screen ต่างกันอย่างไร?</summary>World = ขนาดจริงในโมเดล · Screen = ขนาดคงที่บนจอ</details>

📚 อ้างอิง: R1 Dimensions, Linear Dimension, Multi Dimension, Dimension Styles
