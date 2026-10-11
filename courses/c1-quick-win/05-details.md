---
title: "5. ใส่รายละเอียด: ขอบมน + ปุ่ม"
parent: "C1 · Quick Win"
nav_order: 5
chapter: true
read_time: 5
do_time: 8
permalink: /courses/c1-quick-win/05-details/
---

# 5. ใส่รายละเอียด: ขอบมน + ปุ่ม
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำขอบมนด้วย **Controlled Round** ซึ่งกลับมาแก้รัศมีได้ตลอด
- เจาะร่องด้วย **Difference** (Boolean)
- ใส่ปุ่มลงในร่องได้ตรงศูนย์กลาง

## 💡 ไอเดียสั้น ๆ
ของที่ดู "แพง" ส่วนใหญ่ **ไม่มีขอบคม** แค่ลบมุม 3–6 mm ลำโพงก็ดูเป็นสินค้าจริงทันที
**Controlled Round** ต่างจาก Round ธรรมดาตรงที่วัตถุ **จำค่าการลบมุมไว้** จึงกลับมาแก้ได้ทุกเมื่อ (R1: Controlled Round, R17)

| รายละเอียด | ค่า |
|---|---|
| ขอบบนของ Body | R6 |
| ขอบล่างของ Body | R3 |
| ร่องปุ่มบน Cap | Ø12 ลึก 1 mm |
| ปุ่ม | Ø10 สูง 2 mm (โผล่พ้นผิว Cap 1 mm) |

## 👣 ลงมือทำ (8 นาที)

### A. ขอบมน (Controlled Round)
1. เลือกเครื่องมือ **Controlled Round** (Assistant: พิมพ์ `round`)
2. คลิกที่ **Body** 1 ครั้ง palette จะขยายตัวเลือกเพิ่มขึ้น
3. คลิก **ขอบวงกลมด้านบน** แล้วตั้งรัศมี **6**
4. กดปุ่ม **+** ที่รายการ set ด้านล่างของ palette เพื่อสร้าง set ใหม่ แล้วคลิก **ขอบวงกลมด้านล่าง** และตั้งรัศมี **3**
5. หมุนมุมมองดูให้ทั่ว แล้วลองกลับไปแก้ set แรกเป็น 8 แล้วแก้กลับเป็น 6

{: .shot }
[SCREENSHOT: Controlled Rounding Tool Options ที่มี 2 sets (R6, R3) และเห็นขอบมนบนตัวลำโพง]

{: .note }
ถ้า Cap ซ้อนอยู่บนขอบที่ลบมุมแล้วดูแปลก ให้เช็คว่า Cap กว้าง Ø54 ซึ่งเล็กกว่าหน้าแบนที่เหลือของ Body (70 − 2×6 = 58 mm)

### B. เจาะร่องปุ่ม (Difference)
6. **Cylinder > Preset** ตั้ง Radius X/Y = **6**, Height = **2** แล้ววางบนหน้าบนของ **Cap** ที่ **Snap to Center**
7. เลื่อนชิ้นนี้ (ตัวตัด) ลงไป **1 mm** ด้วย **Move** หรือ **Transform** โดยพิมพ์ค่า Z = −1 (R19)
8. เลือก **Difference** แล้วคลิก **Cap ก่อน** จากนั้นคลิกตัวตัด เพราะลำดับสำคัญ ชิ้นที่สองจะถูกลบออกจากชิ้นแรก (R1: Difference)

{: .shot }
[SCREENSHOT: ก่อนและหลัง Difference ให้เห็นร่อง Ø12 บน Cap]

### C. ปุ่ม
9. **Cylinder > Preset** ตั้ง Radius X/Y = **5**, Height = **2** แล้ววางที่ **ศูนย์กลางของพื้นร่อง**
10. ตั้งชื่อใน Objects palette ว่า `Button` แล้ว **บันทึกไฟล์**

{: .verify }
ค่าเริ่มต้นของ **Edit menu > Ghost / Delete / Keep** (สิ่งที่จะเกิดกับตัวตัดหลังทำ Boolean) ยังไม่ได้ยืนยันใน v10 ถ้าตัวตัดยังเหลือเป็นเงาจาง ๆ (ghosted) ให้ใช้ **Edit > Clear Ghosted Operands** ส่วนวิธีพิมพ์ค่าเลื่อนใน Move หรือ Transform ให้ยืนยันกับหน้าจอจริงแล้วจับภาพมาใส่

{: .easy }
ลบมุมแค่คลิกขอบแล้วพิมพ์รัศมี ไม่ต้องลง extension เพิ่มเหมือน SketchUp

{: .power }
SketchUp ไม่มีการลบมุม (fillet) แบบ solid ในตัว และแก้ย้อนหลังไม่ได้ ส่วน **Controlled Round ของ formZ แก้ย้อนหลังได้** และ Difference ก็ให้ผลเป็น solid ที่ปิดสนิทพร้อมพิมพ์ 3D

{: .shapr }
Shapr3D Fillet ≈ **Controlled Round** · Shapr3D Subtract ≈ **Difference** (formZ คลิกชิ้นหลักก่อน แล้วค่อยคลิกตัวตัด)

## ✅ เช็คตัวเอง
<details><summary>1. ต่างกันอย่างไรระหว่าง Round กับ Controlled Round?</summary>Controlled Round เก็บค่าการลบมุมไว้ จึงแก้ภายหลังได้</details>
<details><summary>2. ใน Difference ต้องคลิกชิ้นไหนก่อน?</summary>ชิ้นที่ต้องการเก็บไว้ (Cap) ก่อน แล้วค่อยคลิกตัวตัด</details>
<details><summary>3. ทำไมปุ่มสูง 2 mm แต่ร่องลึก 1 mm?</summary>ให้ปุ่มโผล่พ้นผิว 1 mm กดได้จริงและเห็นเงาชัดตอนเรนเดอร์</details>

{: .warning }
ทำ Controlled Round **ก่อน** Boolean ทุกครั้งที่ทำได้ เพราะการทำ Boolean กับขอบที่ลบมุมแล้วบางครั้งจะได้ผลที่แก้ยากกว่า

📚 อ้างอิง: R1 Controlled Round, Round, Difference · R17 [Controlled Rounding](https://support.formz.com/hc/en-us/articles/28220737857683) · R19 [Transform tool](https://support.formz.com/hc/en-us/articles/28223037374995) · [Video: Booleans Part 1](https://support.formz.com/hc/en-us/articles/28597341000851)
