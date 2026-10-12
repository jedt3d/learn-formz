---
title: "8. 4 มุมมองในคลิกเดียว: Multi-Frame"
parent: "C6 · บอร์ดขายไอเดีย A3 แผ่นเดียว"
nav_order: 8
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c6-layout-boards/08-multiframe/
hook: "วางหลาย frame พร้อมกันด้วย Place Multi-Frame และเลือก Layout ของตาราง (เช่น 2 × 2) และ Margin ระหว่างกรอบ"
---

# 8. 4 มุมมองในคลิกเดียว: Multi-Frame
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- วางหลาย frame พร้อมกันด้วย **Place Multi-Frame**
- เลือก **Layout** ของตาราง (เช่น 2 × 2) และ **Margin** ระหว่างกรอบ
- ใช้ **Apply To All Frames** ให้ทุกกรอบใช้มาตราส่วนเดียวกัน

## 💡 ไอเดียสั้น ๆ
**views board** แสดงสินค้า 4 ด้านที่ **มาตราส่วนเท่ากัน** ทำให้คนดูเปรียบเทียบสัดส่วนได้ เป็นสะพานไปสู่ **แบบ drawing** ใน C7

| กรอบ | View |
|---|---|
| ซ้ายบน | Front |
| ขวาบน | Right |
| ซ้ายล่าง | Top |
| ขวาล่าง | view `Hero` (3D ที่บันทึกไว้) |

## 👣 ลงมือทำ (4 นาที)
1. ทำให้แผ่น `02_Views` active
2. **Place Multi-Frame** ลากกรอบใหญ่เกือบเต็มหน้า
3. **Multiple Frame Parameters**: Layout = **2 × 2**, Margin 10 mm, File = ไฟล์กาต้มน้ำ
4. คลิกแต่ละกรอบในพรีวิวด้านซ้าย แล้วตั้ง View ตามตาราง และตั้ง Scale = **1:2** (Drawing Scale หรือ Ratio) โดยเปิด **Apply To All Frames**
5. OK แล้วใส่หัวกระดาษ "VIEWS · scale 1:2" ด้วย Place Text

{: .shot }
[SCREENSHOT: Multiple Frame Parameters dialog (2×2 preview)]
{: .shot }
[SCREENSHOT: views board 4 มุม]

{: .note }
Layers และ Clipping Planes ของแต่ละกรอบ ตั้งเพิ่มได้ **หลัง** สร้างแล้ว (แก้ frame ทีละกรอบ) เช่น ซ่อน layer ดินสอในกรอบ Top

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** เปลี่ยนจาก 2×2 เป็น 1×3 แล้วดูว่าแบบไหนสวยกว่า
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไม views ต้องมาตราส่วนเท่ากัน?</summary>เพื่อให้เทียบสัดส่วนระหว่างด้านได้ถูกต้อง</details>
<details><summary>2. 1:2 หมายถึงอะไร?</summary>บนกระดาษ 1 mm = ของจริง 2 mm (ย่อลงครึ่งหนึ่ง)</details>
<details><summary>3. กรอบที่ 4 ใช้ view อะไรได้?</summary>view ที่บันทึกไว้ในโปรเจกต์ เช่น Hero</details>

📚 อ้างอิง: R1 Layout (Place Multi-Frame)
