---
title: "7. แก้ 1 ที่ เปลี่ยนทั้ง 12 ชิ้น: Components"
parent: "M1 · 8 ทริกทำงานไวขึ้น 2 เท่า"
nav_order: 7
chapter: true
read_time: 2
do_time: 5
hook: "ทำปุ่มรีโมท 12 ปุ่มเป็น Component แก้ปุ่มเดียวแล้วเปลี่ยนตามกันหมด"
permalink: /courses/m1-quick-tips/07-components/
---

# 7. แก้ 1 ที่ เปลี่ยนทั้ง 12 ชิ้น: Components
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เปลี่ยน object เป็น component ด้วย **Create Component**
- วางซ้ำด้วย **Place Component** และแก้ด้วย **Edit Group/Component**

## 💡 ไอเดียสั้น ๆ
Component คือ **ต้นแบบ 1 ชิ้น + instances หลายชิ้น** (SketchUp เรียก Component เหมือนกัน) ข้อมูลจะฝังในไฟล์โปรเจกต์ ถ้าแก้ต้นแบบ instance ทุกชิ้นก็เปลี่ยนตาม (manual: Creating and Placing Components)

## 👣 ลงมือทำ (5 นาที)
1. ทำปุ่ม **Cylinder** Ø8 H2 + **Controlled Round** R0.8
2. **Create Component** → เปิด **Replace With Component** → คลิกจุด origin → ตั้ง Component Name `btn` → **Embed In Project Only**
3. **Place Component** → เลือก `btn` ใน **Component Manager** (หรือกด Space ใช้ตัวที่ active อยู่) → คลิกวาง 12 ครั้ง
4. **Edit › Edit Group/Component** ที่ปุ่มใดปุ่มหนึ่ง → แก้ความสูงเป็น 3 → จบการแก้ แล้วดูว่าทุกปุ่มเปลี่ยนตาม
5. ปุ่มใดอยากให้ต่าง → **Make Individual Component**

{: .shot }
[SCREENSHOT: Component Manager palette]

{: .shot }
[SCREENSHOT: ปุ่ม 12 ปุ่มก่อน/หลังแก้ต้นแบบ]

{: .easy }
เหมือน Component ของ SketchUp ทุกอย่าง

{: .shapr }
Shapr3D ไม่มี component แบบ instance ใน Free 🔍 ส่วน formZ มีทุก edition 🔍

{: .note }
ถ้าเปิด Fixed ใน Tool Options ของ Place Component จะกำหนดขนาดด้วย Scale / Dimension ได้ และมี Keep Proportional

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำขาโต๊ะ 4 ขาเป็น component แล้วเปลี่ยนเป็นขาเรียวด้วย Taper ครั้งเดียว
</div>

## ✅ เช็คตัวเอง
<details><summary>1. สร้าง component จาก object เดิมให้แทนที่ชิ้นเดิมต้องเปิดอะไร?</summary>Replace With Component</details>
<details><summary>2. แยก instance ให้ไม่เปลี่ยนตามทำอย่างไร?</summary>Make Individual Component</details>

📚 อ้างอิง: Manual: Creating and Placing Components, Create Component, Place Component
