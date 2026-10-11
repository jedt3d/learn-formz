---
title: "1. แก้วมัค: Revolve + Pipe"
parent: "C6 · Brand & Presentation Boards"
nav_order: 1
chapter: true
read_time: 4
do_time: 5
permalink: /courses/c6-layout-boards/01-mug/
---

# 1. แก้วมัค: Revolve + Pipe
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทวน **Revolve** + **Thicken** (จาก C3) ทำตัวแก้ว
- ทำหูจับด้วย **Pipe** จากเส้นโค้งรูปตัว C
- แก้ขนาดหูจับภายหลังได้ใน **Inspector** (Pipe เป็น parametric)

## 💡 ไอเดียสั้น ๆ
แก้วมัคเป็นของที่ "ง่ายแต่สวย" และเป็นคู่หูที่ดีของกาต้มน้ำในการทำ **product family** วัดแก้วที่บ้าน (ตัวอย่าง: Ø82 สูง 95 ผนังหนา 4)

| ส่วน | วิธี | ค่า |
|---|---|---|
| ตัวแก้ว | โปรไฟล์เปิด (ก้น + ข้าง) → **Revolve** 360° → **Thicken** 4 | Ø82 × 95 |
| ขอบปาก | Controlled Round ขอบบน | R2 |
| หูจับ | Spline รูป C บนระนาบ ZX → **Pipe** | Ø10 |

**Pipe** สร้างท่อตามเส้นโค้ง ตั้ง radius (หรือ diameter) ได้ และแก้ภายหลังได้ที่แท็บ Parameters ใน Inspector (R1: Pipe · Pro)

## 👣 ลงมือทำ (5 นาที)
1. ไฟล์ `C6_Mug.fmz` ระนาบ ZX: Vector Line (0, 0) → (38, 0) แล้วสลับเป็น Spline ขึ้นไป (41, 95) กด **e**
2. **Revolve** รอบแกน Z → **Thicken** 4 (ไปด้านใน) → Controlled Round ขอบปาก R2
3. วาด **Spline** รูปตัว C บนระนาบ ZX จาก (40, 80) ออกไป (68, 60) แล้วกลับมาที่ (40, 25) โดยปลายทั้งสองจมเข้าไปในผนังแก้ว
4. **Pipe** คลิกเส้นแล้วตั้ง diameter **10**
5. **Union** ตัวแก้วกับหูจับ (ถ้า Union ไม่ผ่าน ให้ปรับปลายเส้นให้จมในผนังมากขึ้น)

{: .shot }
[SCREENSHOT: เส้นตัว C บนระนาบ ZX + Pipe Tool Options]
{: .shot }
[SCREENSHOT: แก้วมัคเสร็จ (Shaded Work)]

{: .verify }
ตัวเลือก radius/diameter ของ Pipe และการ Union ระหว่าง Pipe object กับ solid (อาจต้อง convert ก่อน) ต้องยืนยันบน v10

{: .power }
SketchUp ทำหูจับด้วย **Follow Me** ได้ แต่แก้ขนาดภายหลังไม่ได้ ส่วน **Pipe** ของ formZ แก้ diameter ได้ทุกเมื่อ

{: .shapr }
Shapr3D: **Sweep** วงกลมไปตามเส้น · formZ: **Pipe** (หรือ Sweep ถ้าอยากได้หน้าตัดแบบอื่น)

## ✅ เช็คตัวเอง
<details><summary>1. แก้ diameter ของ Pipe ได้ที่ไหน?</summary>Inspector แท็บ Parameters</details>
<details><summary>2. ทำไมปลายเส้นหูจับต้องจมในผนัง?</summary>เพื่อให้ Union ได้ solid ที่ต่อกันจริง</details>
<details><summary>3. อยากได้หูจับหน้าตัดรี ใช้อะไรแทน Pipe?</summary>Sweep ด้วยหน้าตัดวงรี</details>

📚 อ้างอิง: R1 Revolve, Thicken, Pipe, Union
