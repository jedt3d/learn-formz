---
title: "3. เกลียวนอกด้วย Helix"
parent: "C8 · เตรียมผลิต: 3D Print, STEP"
nav_order: 3
chapter: true
read_time: 4
do_time: 5
track: "📐 Engineering"
permalink: /courses/c8-make-it/03-thread/
---

# 3. เกลียวนอกด้วย Helix
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- วาด **โปรไฟล์ฟันเกลียว** รูปสามเหลี่ยม
- ใช้ **Helix** หมุนพร้อมเลื่อนขึ้น (# Of Cycles, Length Each Cycle, Caps)
- รวมเกลียวเข้ากับคอขวด

## 💡 ไอเดียสั้น ๆ
**Helix** ทำงานเหมือน **Revolve** แต่ทุกขั้นของการหมุนจะ **เลื่อนขึ้น** ทีละนิด จึงได้รูปสปริงหรือเกลียว ถ้าโปรไฟล์เป็นรูปปิดและเปิด **Caps** จะได้ **solid** (R1: Helix)

| ค่า | ตั้งเป็น |
|---|---|
| โปรไฟล์ | สามเหลี่ยม: ฐาน 2.4 (ตามแกน Z) ยื่นออก 1.2 จากผิวคอ (x = 11 → 12.2) ที่ z = 70 |
| Model Type | **Smooth** |
| **# Of Cycles** | 3 |
| **Length** | **Each Cycle = 3** (= pitch) |
| Direction | ตามเข็ม (เกลียวขวา หมุนตามเข็มเพื่อปิด) |
| **Caps** | ✅ |

## 👣 ลงมือทำ (5 นาที)
1. ระนาบ **ZX** วาดสามเหลี่ยมด้วย **Vector Line** (type 2D): (11, 70) → (12.2, 71.2) → (11, 72.4) แล้วกด **c**
2. เลือก **Helix** แล้วตั้งค่าตามตาราง คลิกสามเหลี่ยม แล้วเลือกแกน **Z** เป็นแกน (ทำแบบเดียวกับ Revolve)
3. ตรวจด้วย **Wire Frame** ว่ามี 3 รอบ ช่วงสูงประมาณ z = 70–81
4. **Union** เกลียวกับ `Bottle` (ให้ฐานสามเหลี่ยมจมในคอ 0.1 mm ถ้า Union ไม่ผ่าน)
5. (สวย + พิมพ์ง่าย) ลบปลายเกลียวให้เรียวด้วยการตัดปลายเกลียวด้วย Difference กล่องเล็ก ๆ

{: .shot }
[SCREENSHOT: Helix Tool Options (# Of Cycles, Length Each Cycle, Caps)]
{: .shot }
[SCREENSHOT: คอขวดที่มีเกลียว 3 รอบ]

{: .note }
ทางลัด: เครื่องมือ **Screw/Bolt** ทำเกลียวให้ทั้งตัว (เหมาะกับสกรู) แต่ใช้กับคอขวดที่กลวงไม่ได้ จึงใช้ Helix ที่ควบคุมได้มากกว่า

{: .verify }
ทิศ Direction ที่ได้ "เกลียวขวา" (right-hand) ใน formZ ต้องยืนยันด้วยการดูในมุมมองด้านข้าง (เกลียวขวาจะเอียงขึ้นไปทางขวาเมื่อมองจากด้านหน้า)

{: .power }
SketchUp ทำเกลียวที่ใช้งานได้จริงแทบไม่ได้ ส่วน formZ มีทั้ง **Helix**, **Wire Helix** และ **Screw/Bolt**

## ✅ เช็คตัวเอง
<details><summary>1. Helix ต่างจาก Revolve อย่างไร?</summary>หมุนพร้อมเลื่อนขึ้นทุกขั้น ได้รูปเกลียว และหมุนเกิน 360° ได้</details>
<details><summary>2. Length Each Cycle คือค่าอะไรของเกลียว?</summary>pitch</details>
<details><summary>3. ทำไมฐานสามเหลี่ยมต้องจมในคอนิดหนึ่ง?</summary>เพื่อให้ Union ได้ solid ที่ต่อกันสนิท</details>

📚 อ้างอิง: R1 Helix, Wire Helix, Screw/Bolt, Union
