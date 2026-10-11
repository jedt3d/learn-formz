---
title: "4. Blockout: cage ด้วย Subdivision"
parent: "C9 · Capstone: ของจากบ้านตั้งแต่ต้นจนจบ"
nav_order: 4
chapter: true
read_time: 4
do_time: 6
track: "🎨 Designer + 📐 Engineering"
permalink: /courses/c9-capstone/04-blockout/
---

# 4. Blockout: cage ด้วย Subdivision
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **cage** (กล่องหยาบ) ให้มีขนาดตามเป้า 104 × 56 × 35
- ใช้ **Subdivision / Create** (Iterations 3) แล้วเปิด/ปิด controls ด้วย **F6**
- เพิ่มเส้น edge ด้วย **Insert Sequence** (คลิกขวา)

## 💡 ไอเดียสั้น ๆ
**Blockout = ปั้นก้อนให้สัดส่วนถูกก่อน แล้วค่อยใส่รายละเอียด** ถ้าสัดส่วนผิด รายละเอียดสวยแค่ไหนก็ไม่ช่วย

cage ที่ดี: **ใช้ face น้อยที่สุดที่ได้ฟอร์ม** เริ่มที่กล่อง 4 × 3 × 2 ช่อง

## 👣 ลงมือทำ (6 นาที)
1. **Cube** 104 × 56 × 35 (Facetted) วางท้ายที่ x = 0 บน layer `Body`
2. **Subdivision / Create** → Iterations **3** → คลิกกล่อง จะได้ก้อนกลมแบบสบู่
3. กด **F6** เพื่อแสดง cage แล้ว **คลิกขวาที่ edge → Insert Sequence** เพิ่มเส้นตามยาว 3 เส้น และตามขวาง 1 เส้น
4. เลือกจุดบนสุดของ cage แล้ว **Move** ให้สูงสุดที่ ~38% จากท้าย (ดู underlay ด้านข้าง)
5. ลากจุดด้านหน้าลงเพื่อให้หัวเมาส์ลาด เทียบกับภาพด้านข้าง

{: .shot }
[SCREENSHOT: cage (F6) ทับบน underlay ด้านข้าง]
{: .shot }
[SCREENSHOT: blockout เมาส์ใน Shaded]

{: .shapr }
Shapr3D (บน iPad) มี SubD ด้วย แต่ formZ มีชุด edit tools ที่ละเอียดกว่า (Grow, Stretch, Squeeze, Bridge, Close ...)

{: .note }
🔀 **ถ้าเลือกของอื่น:** ของทรงกล่องให้ blockout ด้วย **Cube** + **Controlled Round** ได้เลย ไม่ต้องใช้ SubD

## ✅ เช็คตัวเอง
<details><summary>1. ปุ่มลัดแสดง cage คืออะไร?</summary>F6 (Show Controls)</details>
<details><summary>2. Insert Sequence อยู่ที่ไหน?</summary>คลิกขวาบน subdivision object ขณะที่แสดง controls อยู่</details>
<details><summary>3. ทำไมต้องใช้ face น้อย?</summary>แก้ฟอร์มง่ายกว่าและผิวเรียบกว่า</details>

📚 อ้างอิง: R1 Subdivision / Create, Right-Click Context Menu for Subdivision Surfaces
