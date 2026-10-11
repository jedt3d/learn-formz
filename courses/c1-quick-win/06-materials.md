---
title: "6. ใส่วัสดุ 3 แบบ"
parent: "C1 · Quick Win"
nav_order: 6
chapter: true
read_time: 5
do_time: 6
permalink: /courses/c1-quick-win/06-materials/
---

# 6. ใส่วัสดุ 3 แบบ
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- สร้าง material ใหม่ และเลือกค่าตั้งต้นจาก **Material Library**
- ใส่ material ให้วัตถุด้วยการ **ลากไปวาง (drag-and-drop)** หรือใช้เครื่องมือ **Paint**
- เข้าใจว่าทำไมภาพใน Shaded Work กับใน RenderZone ถึงไม่เหมือนกันเป๊ะ

## 💡 ไอเดียสั้น ๆ
ลำโพงที่ใช้ material ครบ 3 แบบ คือ **ด้าน, ยาง, โลหะ** จะดูเป็นสินค้าจริงทันที เพราะสายตาคนแยกวัตถุจาก **ความเงา** ก่อนจะสังเกตสี

| ชิ้น | ชื่อ material | ไอเดีย |
|---|---|---|
| Body | `PS_Body_Matte` | พลาสติกหรือผ้าสีเข้ม (เช่น teal หรือ navy) เงาน้อย |
| Cap | `PS_Cap_Rubber` | ยางเทาเข้ม ด้านมาก |
| Button | `PS_Button_Metal` | อะลูมิเนียมหรือโลหะที่สะท้อนแสง |

Material ทั้งหมดของโปรเจกต์อยู่ใน **Materials palette** ใน dock ด้านขวา material ที่ active (มีจุดแดงหรือกรอบแดง) จะถูกใส่ให้วัตถุที่สร้างใหม่โดยอัตโนมัติ (R1: Creating and Editing Materials)

## 👣 ลงมือทำ (6 นาที)
1. ที่ **Materials** palette กดไอคอน **New Material** จะได้ material ใหม่ต่อท้ายรายการ
2. ดับเบิลคลิก material ใหม่เพื่อเปิด **Material Parameters** palette แล้วตั้งชื่อเป็น `PS_Body_Matte`
3. ขยาย Material Parameters palette (ปุ่มขยายที่มุมขวาล่าง) จะเจอ popup **Library** ให้เลือกหมวด material สำเร็จรูป แล้วเลือกตัวที่ใกล้เคียงพลาสติกด้าน จากนั้นปรับสีตามใจ
4. ทำแบบเดียวกันอีก 2 รอบสำหรับ `PS_Cap_Rubber` และ `PS_Button_Metal` (หมวดโลหะ)
5. **ลาก** material จาก palette ไป **วาง** บนแต่ละชิ้น
6. ถ้าต้องการให้ material ลงแค่ **หน้าเดียว** ให้ทำ material นั้นเป็น active แล้วใช้เครื่องมือ **Paint** คลิกที่หน้านั้น (R1: Paint)
7. ดูผลใน **Shaded Work** แล้ว **บันทึกไฟล์**

{: .shot }
[SCREENSHOT: Materials palette ที่มี 3 materials ใหม่ (Large Icon view)]

{: .shot }
[SCREENSHOT: Material Parameters palette แบบขยาย ที่เปิด Library popup และเลือกหมวดโลหะ]

{: .shot }
[SCREENSHOT: ลำโพงใน Shaded Work หลังใส่ material ครบ 3 ชิ้น]

{: .note }
**Keep Synchronized** (เพิ่มมาใน 10.0.1): formZ จะพยายามทำให้ material ดูเหมือนกันในทุก renderer (Shaded, RenderZone, V-Ray) ปล่อยเปิดไว้ก่อนใน course นี้ ถ้าวันหนึ่งอยากให้ RenderZone มีค่าเฉพาะของตัวเองค่อยปิด (R7)

{: .verify }
ชื่อหมวดใน Library และหน้าตาของ Material Parameters palette ใน v10 ยังไม่ได้ยืนยัน (คู่มือยังใช้ภาพเก่า) ให้จับภาพหน้าจอจริงแล้วใส่ชื่อ material สำเร็จรูปที่แนะนำ 3 ตัวลงในบทนี้

{: .easy }
ลากไปวางเหมือน Paint Bucket ของ SketchUp และ formZ 10 ยังมี **Edit > Paste Attributes** ไว้คัดลอกวัสดุและคุณสมบัติจากชิ้นหนึ่งไปอีกชิ้นได้ด้วย (R8)

{: .power }
material ของ formZ ตั้งค่าแยกได้เป็น **color / reflection / transparency / bump** ตามแบบของ RenderZone (R3) ส่วน SketchUp มีแค่สีกับภาพ texture และต้องใช้ renderer ภายนอกถึงจะได้ผิวโลหะจริง

{: .shapr }
Shapr3D: แท็บ Appearance ใน Visualization · formZ: **Materials palette + Material Parameters** หลักการเหมือนกัน คือเลือกวัสดุแล้ววางบนชิ้นงาน

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมวัตถุที่สร้างใหม่ถึงได้ material แปลก ๆ?</summary>เพราะวัตถุใหม่จะได้ material ที่ active อยู่ในขณะนั้นเสมอ</details>
<details><summary>2. ถ้าจะใส่ material ให้หน้าเดียวต้องทำอย่างไร?</summary>ทำ material นั้นเป็น active แล้วใช้ Paint คลิกที่หน้านั้น</details>
<details><summary>3. ภาพใน Shaded Work เหมือนภาพเรนเดอร์ 100% ไหม?</summary>ไม่ Shaded เป็นแค่การประมาณ ภาพจริงจะเห็นใน RenderZone</details>

{: .warning }
ตั้งชื่อ material ขึ้นต้นด้วยชื่อโปรเจกต์ (`PS_...`) เสมอ เพราะพอโปรเจกต์ใหญ่ขึ้น material จะเยอะมากจนหาไม่เจอ

📚 อ้างอิง: R1 Creating and Editing Materials, Paint · R7 (10.0.1 Keep Synchronized, 10.1.3 แก้เรื่อง drag-drop บน macOS 15.3) · R8 Paste Attributes
