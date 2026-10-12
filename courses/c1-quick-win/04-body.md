---
title: "4. วัดปากกาจริง → ด้ามเสร็จใน 5 นาที"
parent: "C1 · ปากกาเมจิกสวยใน 90 นาที"
nav_order: 4
chapter: true
read_time: 5
do_time: 7
permalink: /courses/c1-quick-win/04-body/
hook: "วัด ปากกาเมจิกของจริง แล้วจดขนาดเป็น mm และสร้าง Cylinder และ Cone แบบ Truncated ด้วยวิธี Preset ให้ขนาดตรงเป๊ะ"
---

# 4. วัดปากกาจริง → ด้ามเสร็จใน 5 นาที
{% include meta.html %}

{: .note }
**Build-along เริ่มตรงนี้** บทที่ 4–8 จะต่อยอดไฟล์เดียวกันจนได้ภาพเรนเดอร์ เปิด **File > New Project** (ใช้ template mm แล้ว) แล้วบันทึกเป็น `C1_Marker.fmz`

## 🎯 จบบทนี้แล้วเราจะ...
- วัด **ปากกาเมจิกของจริง** แล้วจดขนาดเป็น mm
- สร้าง **Cylinder** และ **Cone** แบบ **Truncated** ด้วยวิธี **Preset** ให้ขนาดตรงเป๊ะ
- วางชิ้นที่สองต่อจากชิ้นแรกได้ตรงศูนย์กลางพอดีด้วย **Snap to Center**

## 💡 ไอเดียสั้น ๆ
นักออกแบบผลิตภัณฑ์เริ่มงานจาก **การวัดของจริง** หยิบปากกาเมจิกทรงกลม (ปากกาไวท์บอร์ดก็ได้) กับไม้บรรทัดมาวางบนโต๊ะ (ดูขั้นตอนเต็มที่ [อ้างอิงจากของในบ้าน]({{ '/home-reference/' | relative_url }}))

**ขนาดตัวอย่าง** (ถ้าวัดของเราได้ค่าอื่น ให้ใช้ค่าของเรา)

| ชิ้น | รูปทรง formZ | ขนาด |
|---|---|---|
| Barrel (ด้าม) | Cylinder | Ø16 × ยาว 110 mm → Radius 8 |
| Neck (คอเรียว) | Cone + Truncated | ฐาน Ø16 → ปลาย Ø8 สูง 10 mm |
| Tip (หัวปากกา) | Cylinder | Ø5 × 6 mm → Radius 2.5 |

{: .shot }
[SCREENSHOT: ภาพถ่ายปากกาเมจิกจริงวางคู่ไม้บรรทัด พร้อมเส้นบอกขนาด Ø16 / 110 / 10 / 6]

**Primitive** ของ formZ จำพารามิเตอร์ได้ (parametric) วาดผิดก็แก้ตัวเลขทีหลังได้ ส่วนวิธี **Preset** สร้างวัตถุจากตัวเลขใน Tool Options ด้วยคลิกเดียว (R1: Cylinder, Cone)

## 👣 ลงมือทำ (7 นาที)
เราจะปั้นปากกา **ตั้งตรง** ไปตามแกน Z ก่อน แล้วค่อยวางนอนในบทที่ 7

### Barrel
1. เลือก **Cylinder** (Assistant: พิมพ์ `cyl`) แล้วใน **Tool Options** เลือกวิธี **Preset**
2. พิมพ์ **Radius X = 8**, **Radius Y = 8**, **Height = 110**
3. เลื่อนเมาส์ไปที่จุดกำเนิด (ดูใน **Input palette** ให้เป็น 0, 0, 0) แล้วคลิก ผลลัพธ์สีส้มยังแก้ค่าได้ทันที

### Neck
4. เลือก **Cone** วิธี **Preset** ตั้ง Radius X/Y = **8**, Height = **10** แล้วเปิด **Truncated Cone**
5. วางบน **หน้าบน** ของ Barrel ที่ **Snap to Center** (formZ สร้าง face reference plane บนหน้านั้นให้อัตโนมัติ)
6. ตอนที่ยังเป็นสีส้ม ให้ตั้ง **Top Is = 50%** (ปลายจะเหลือ Ø8)

### Tip
7. **Cylinder > Preset** ตั้ง Radius X/Y = **2.5**, Height = **6** แล้ววางบนหน้าบนของ Neck ที่ Snap to Center

### ตั้งชื่อ
8. เปิด **Objects** palette ตั้งชื่อ `Barrel`, `Neck`, `Tip` (ดับเบิลคลิกที่ชื่อ)
9. เลือก Barrel แล้วเปิด **Inspector** ไปที่แท็บ **Parameters** ลองแก้ Height เป็น 120 ดูแล้วแก้กลับเป็น 110 จากนั้น **บันทึกไฟล์**

{: .shot }
[SCREENSHOT: Cone Tool Options ที่เลือก Preset + Truncated Cone และ Top Is 50%]
{: .shot }
[SCREENSHOT: ปากกา 3 ชิ้นตั้งตรงใน Shaded Work + Objects palette ที่มีชื่อครบ]

{: .verify }
ชื่อช่อง **Radius X / Radius Y / Height**, ตัวเลือก **Truncated Cone** และ **Top Is** มาจากคู่มือ v10 (หน้า Cone ซึ่งบอกว่า Cylinder ใช้ 5 วิธีเดียวกัน) แต่ยังไม่มีภาพของ v10 จริง ส่วนการแก้ค่าใน Inspector > Parameters ให้ยืนยันบนเครื่องจริง

{: .easy }
คลิกเดียวได้ทรงกระบอกที่ขนาดตรงเป๊ะ ไม่ต้องวาดวงกลมแล้ว Push/Pull เหมือนใน SketchUp

{: .power }
ใน SketchUp การทำกรวยปลายตัด (truncated cone) ต้องวาดวงกลมแล้ว Push/Pull แล้ว Scale หน้าบน ซึ่งขนาดคลาดง่าย ส่วน formZ พิมพ์ **Top Is 50%** ได้เลย และยังกลับมาแก้ได้ภายหลัง

{: .shapr }
Shapr3D: วาดวงกลมแล้ว extrude แล้วใช้ draft ส่วน formZ ใช้ **Cone Preset + Truncated** ได้ในคลิกเดียว

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ปั้นปากกาอีกด้ามที่ยาวขึ้น 20 mm ภายใน 2 นาที
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมต้องวัดของจริงก่อนปั้น?</summary>เพราะได้สัดส่วนที่ถูกต้องและจับได้จริงในมือ ไม่ต้องเดา</details>
<details><summary>2. Top Is = 50% หมายถึงอะไร?</summary>หน้าบนของกรวยมีขนาด 50% ของฐาน คือ Ø16 → Ø8</details>
<details><summary>3. formZ มี history tree ไหม?</summary>ไม่มี แต่ primitive จำค่าที่ใช้สร้างไว้ให้แก้ภายหลังได้</details>

{: .warning }
ถ้าชิ้นที่วางต่อลอยหรือจมอยู่ในตัวด้าม ให้ตรวจว่าตอนคลิกเคอร์เซอร์อยู่บน **หน้าบน** จริง ไม่ใช่กริด XY ถ้าไม่ใช่ ให้ Undo แล้ววางใหม่

📚 อ้างอิง: R1 Cylinder, Cone, Reference planes, Snapping · [Video: 3D Parametric Primitives](https://support.formz.com/hc/en-us/articles/28597325504659)
