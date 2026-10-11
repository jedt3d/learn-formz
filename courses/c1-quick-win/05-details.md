---
title: "5. ปลอกปากกา: ขอบมน + เจาะ + คลิป"
parent: "C1 · Quick Win"
nav_order: 5
chapter: true
read_time: 5
do_time: 8
permalink: /courses/c1-quick-win/05-details/
---

# 5. ปลอกปากกา: ขอบมน + เจาะ + คลิป
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำขอบมนที่กลับมาแก้ได้ด้วย **Controlled Round**
- รวมชิ้นด้วย **Union** และเจาะรูด้วย **Difference** (Boolean)
- ได้ปลอกปากกาที่ **กลวงจริง** เสียบด้ามได้

## 💡 ไอเดียสั้น ๆ
ของที่ดู "เป็นสินค้าจริง" มี 2 อย่างที่ต้องมีคือ **ขอบมน** และ **ความหนาจริง** ปลอกปากกาเป็นตัวอย่างที่ดี มีทั้งขอบมน คลิป และรูด้านใน

| ส่วน | ค่า (ตัวอย่าง) |
|---|---|
| Cap (ปลอก) | Ø18 × 55 mm วางที่ X = 40 (ข้าง ๆ ปากกา) |
| ขอบบนของปลอก | R3 |
| Clip | กล่อง 4 × 3 × 38 mm ติดข้างปลอก |
| รูด้านใน | Ø16.4 ลึก 50 mm (เผื่อหลวม 0.2 mm ต่อด้าน) |

**ลำดับที่ดี:** ทำขอบมนก่อน แล้วค่อย Union และ Difference

## 👣 ลงมือทำ (8 นาที)

### A. ปลอก + ขอบมน
1. **Cylinder > Preset** ตั้ง Radius X/Y = **9**, Height = **55** แล้วคลิกที่ (40, 0, 0) โดยดูค่าใน Input palette
2. เลือก **Controlled Round** คลิกที่ปลอก แล้วคลิก **ขอบวงกลมด้านบน** ตั้งรัศมี **3**
3. ลองแก้เป็น 5 แล้วแก้กลับเป็น 3 จะเห็นว่าแก้ได้ตลอด

{: .shot }
[SCREENSHOT: Controlled Rounding Tool Options ที่ set แรกมีค่า R3 และขอบบนของปลอกมน]

### B. คลิป (Union)
4. เลือก **Cube** วิธี **Diagonal** แล้วพิมพ์มุมแรก (38, 8, 15) และมุมที่สอง (42, 11, 15) ใน **Input palette** จากนั้นตั้งความสูง **38** (คลิปจะซ้อนเข้าไปในผนังปลอก 1 mm)
5. เลือก **Union** แล้วคลิกปลอกกับคลิป จะได้เป็น object เดียว

### C. รูด้านใน (Difference)
6. **Cylinder > Preset** ตั้ง Radius X/Y = **8.2**, Height = **50** แล้วคลิกที่ (40, 0, 0) ซึ่งเป็นตัวตัดจากด้านล่าง
7. เลือก **Difference** แล้วคลิก **ปลอกก่อน** จากนั้นคลิกตัวตัด ชิ้นที่สองจะถูกลบออกจากชิ้นแรก (R1: Difference)
8. สลับไป **Wire Frame** เพื่อดูว่ารูอยู่ข้างในจริง ตั้งชื่อ `Cap` แล้ว **บันทึกไฟล์**

{: .shot }
[SCREENSHOT: ปลอกใน Wire Frame ให้เห็นรูด้านในและคลิป]

{: .verify }
- ค่าเริ่มต้นของ **Edit menu > Ghost / Delete / Keep** (สิ่งที่จะเกิดกับตัวตัดหลังทำ Boolean) ยังไม่ได้ยืนยันใน v10 ถ้าตัวตัดเหลือเป็นเงาจาง ให้ใช้ **Edit > Clear Ghosted Operands**
- การพิมพ์มุมของ Cube Diagonal ใน Input palette ต้องยืนยันว่าพิมพ์ x, y, z ได้ครบหรือต้องกด Tab สลับช่อง

{: .easy }
ลบมุมแค่คลิกขอบแล้วพิมพ์รัศมี ไม่ต้องลง extension เพิ่มเหมือน SketchUp

{: .power }
SketchUp ไม่มี fillet แบบ solid ในตัว และ Boolean ของ SketchUp ใช้ได้เฉพาะ solid group ที่ปิดสนิท (Solid Tools มีครบเฉพาะรุ่นเสียเงิน) ส่วน formZ ทำได้ทันที และผลลัพธ์เป็น solid ที่พร้อมพิมพ์ 3D

{: .shapr }
Shapr3D Fillet ≈ **Controlled Round** · Union ≈ **Union** · Subtract ≈ **Difference** (formZ คลิกชิ้นหลักก่อน แล้วค่อยคลิกตัวตัด)

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมรูด้านในกว้าง 16.4 ไม่ใช่ 16?</summary>เผื่อให้หลวมด้านละ 0.2 mm ถ้าพิมพ์ 3D จริงจะได้สวมเข้าไปได้ (เรียนเรื่อง clearance ใน C8)</details>
<details><summary>2. ใน Difference ต้องคลิกชิ้นไหนก่อน?</summary>ชิ้นที่ต้องการเก็บไว้ (ปลอก) ก่อน แล้วค่อยคลิกตัวตัด</details>
<details><summary>3. ทำไมต้องทำขอบมนก่อน Boolean?</summary>เพราะขอบหลัง Boolean มักซับซ้อนกว่า ลบมุมยากกว่าและพังง่ายกว่า</details>

📚 อ้างอิง: R1 Controlled Round, Cube, Union, Difference · R17 [Controlled Rounding](https://support.formz.com/hc/en-us/articles/28220737857683) · [Video: Booleans Part 1](https://support.formz.com/hc/en-us/articles/28597341000851)
