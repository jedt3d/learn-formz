---
title: "7. รัศมี มุม ลูกศร + ขนาดที่ตามโมเดล"
parent: "C7 · เขียนแบบให้โรงงานอ่านออก: กบเหลา 3 ด้าน"
nav_order: 7
chapter: true
read_time: 4
do_time: 4
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/07-radial/
hook: "ใส่ Radial/Diameter Dimension (สลับ R ↔ Ø ได้) และใส่ Angular Dimension (มุมของรูกรวย)"
---

# 7. รัศมี มุม ลูกศร + ขนาดที่ตามโมเดล
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใส่ **Radial/Diameter Dimension** (สลับ R ↔ Ø ได้)
- ใส่ **Angular Dimension** (มุมของรูกรวย)
- เขียนหมายเหตุด้วย **Leader Line** และ **Text Note**
- ทดสอบ **Associativity**: แก้โมเดลแล้วขนาดตามเอง

## 💡 ไอเดียสั้น ๆ

| เครื่องมือ | วิธี |
|---|---|
| **Radial/Diameter Dimension** | คลิกส่วนโค้ง/วงกลม 1 ครั้ง แล้วคลิกวาง · เลือก **Diameter** ใน Tool Options จะแสดง "Ø" |
| **Angular Dimension** | คลิก 3 จุด: **จุดศูนย์กลาง → จุดเริ่ม → จุดจบ** (หรือคลิกเส้นโค้ง) |
| **Leader Line** | ลูกศรชี้ + ข้อความ เช่น "ใบมีดเหล็ก t = 0.6" |
| **Text Note** | ข้อความลอย เช่น "ทุกขอบ R1.5 ยกเว้นระบุ" |

**Associativity:** ถ้าตอนสร้าง dimension เรา snap กับจุดของวัตถุ เมื่อแก้วัตถุ (เช่น ใช้ Reshape) dimension จะขยับตาม ถ้าหลุด ให้ Show Controls (กด **F6**) แล้วลากจุดของ dimension กลับไป snap ใหม่ (R1: Associativity)

## 👣 ลงมือทำ (4 นาที)
1. **Radial/Diameter** คลิกขอบรูทางเข้า → เลือก Diameter → ได้ **Ø8.2**
2. มุมมอง Top: **Angular Dimension** วัดมุมกรวย (ศูนย์กลาง = ปลายกรวย)
3. **Leader Line** ชี้ที่ใบมีด → "Blade: steel t0.6" · **Text Note**: "ขอบทั้งหมด R1.5"
4. **ทดสอบ Associativity**: **Reshape** หน้าขวาของ Body ออก 4 mm → dimension 26 ควรเปลี่ยนเป็น 30 → Undo

{: .shot }
[SCREENSHOT: Ø8.2 + มุมกรวย + leader line บนโมเดล]
{: .shot }
[SCREENSHOT: ก่อน/หลัง Reshape ที่ dimension ตามเอง]

{: .warning }
ขอบที่ลบมุมแล้วจะไม่มีมุมแหลมให้ snap ให้วัดจาก **หน้า** หรือใช้ **Measure Between** แทน

{: .power }
**Associative dimensions** (ขนาดที่ตามโมเดล) เป็นฟีเจอร์ระดับ CAD ที่ SketchUp ทำได้แค่บางกรณี

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ลองแก้ขนาดโมเดลแล้วดูว่า dimension เปลี่ยนตามไหม
</div>

## ✅ เช็คตัวเอง
<details><summary>1. สลับ R เป็น Ø ทำที่ไหน?</summary>Tool Options ของ Radial/Diameter Dimension</details>
<details><summary>2. Angular Dimension คลิกจุดไหนก่อน?</summary>จุดศูนย์กลางของมุม</details>
<details><summary>3. ถ้า dimension ไม่ตามโมเดล แก้อย่างไร?</summary>Show Controls (F6) แล้วลากจุดกลับไป snap กับวัตถุใหม่</details>

📚 อ้างอิง: R1 Radial/Diameter Dimension, Angular Dimension, Leader Line, Text Note, Associativity
