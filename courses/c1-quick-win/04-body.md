---
title: "4. ปั้นตัวลำโพงด้วยตัวเลข"
parent: "C1 · Quick Win"
nav_order: 4
chapter: true
read_time: 5
do_time: 7
permalink: /courses/c1-quick-win/04-body/
---

# 4. ปั้นตัวลำโพงด้วยตัวเลข
{% include meta.html %}

{: .note }
**Build-along เริ่มตรงนี้** บทที่ 4–8 จะต่อยอดไฟล์เดียวกันจนได้ภาพเรนเดอร์ เปิด **File > New Project** (ซึ่งตอนนี้ใช้ template mm แล้ว) แล้วบันทึกเป็น `C1_PebbleSpeaker.fmz`

## 🎯 จบบทนี้แล้วเราจะ...
- สร้าง **Cylinder** ขนาดแม่นยำได้ใน 1 คลิกด้วยวิธี **Preset**
- วางชิ้นที่สองบนหน้าของชิ้นแรกได้ตรงศูนย์กลางพอดีด้วย **Snap to Center**
- แก้ขนาดภายหลังได้ใน **Inspector** และตั้งชื่อ object ได้

## 💡 ไอเดียสั้น ๆ
**Primitive** ของ formZ (Cube, Cylinder, Sphere ...) ไม่ใช่แค่ก้อนรูปทรง แต่เป็น **วัตถุที่จำพารามิเตอร์ได้** (parametric) วาดไปก่อนแล้วค่อยแก้เส้นผ่านศูนย์กลางทีหลังก็ได้ ส่วนวิธี **Preset** สร้างวัตถุตามตัวเลขใน Tool Options ด้วยคลิกเดียว (R1: Cone/Cylinder, Cube)

**แบบของเรา: Pebble Speaker**

| ชิ้น | รูปทรง | ขนาด |
|---|---|---|
| Body | Cylinder | Ø70 × สูง 80 mm (Radius 35) |
| Cap | Cylinder | Ø54 × หนา 2 mm (Radius 27) วางบนหน้าบนของ Body |

{: .shot }
[SCREENSHOT: ภาพ sketch หรือ orthographic ของลำโพงพร้อมขนาด Ø70 × 80 และ Ø54 × 2 (ภาพประกอบโจทย์)]

## 👣 ลงมือทำ (7 นาที)

### Body
1. เลือก **Cylinder** (อยู่ในกลุ่ม Create ของ Modeling tool palette หรือพิมพ์ `cyl` ใน Assistant)
2. ใน **Tool Options** เลือกวิธี **Preset** แล้วพิมพ์ **Radius X = 35**, **Radius Y = 35**, **Height = 80**
3. ขยับเมาส์ไปที่จุดกำเนิดของกริด (ดูช่อง x, y, z ใน **Input palette** ให้เป็น 0, 0, 0) แล้วคลิก 1 ครั้ง
4. ผลลัพธ์จะเป็นสีส้ม หมายความว่ายังแก้ค่าใน Tool Options ได้ทันที

{: .shot }
[SCREENSHOT: Cylinder Tool Options ที่เลือก Preset และกรอก Radius X/Y = 35, Height = 80]

### Cap
5. ยังใช้ **Cylinder** วิธี **Preset** แต่เปลี่ยนค่าเป็น **Radius X/Y = 27**, **Height = 2**
6. เลื่อนเมาส์ไปที่ **หน้าบน** ของ Body formZ จะสร้าง reference plane บนหน้านั้นให้อัตโนมัติ (face reference plane, R1: Reference planes)
7. ให้เคอร์เซอร์ **snap** เข้าจุดศูนย์กลางของหน้าบน (เปิด **Snap to Center** ไว้แล้วจากบทที่ 2) แล้วคลิก

{: .shot }
[SCREENSHOT: ตอนเคอร์เซอร์ snap จุดศูนย์กลางหน้าบนของ Body และเห็นพรีวิว Cap]

### ตั้งชื่อและตรวจขนาด
8. เปิด **Objects** palette แล้วเปลี่ยนชื่อ 2 object เป็น `Body` และ `Cap` (ดับเบิลคลิกที่ชื่อ)
9. เลือก Body ด้วย **Pick** แล้วเปิด **Inspector** (Palettes menu > Inspector หรือปุ่ม Inspector ใน Tool Options) ดูแท็บ **Parameters** ว่า Radius เป็น 35 และ Height เป็น 80
10. ลองแก้ Height เป็น 85 แล้วแก้กลับเป็น 80 จะเห็นว่าแก้ขนาดได้โดยไม่ต้องสร้างใหม่ **บันทึกไฟล์**

{: .shot }
[SCREENSHOT: Inspector > Parameters ของ Body]

{: .verify }
ชื่อช่องใน Tool Options ของ Cylinder (Radius X, Radius Y, Height) มาจากคู่มือ v10 หน้า Cone ซึ่งเขียนว่า Cylinder มี 5 วิธีเหมือน Cone และยังไม่มีภาพจริงของ v10 ส่วนการแก้ขนาดหลังสร้างใน Inspector > Parameters ให้ยืนยันบนเครื่องจริงด้วยว่าค่าที่แก้ได้ชื่ออะไร

{: .easy }
คลิกเดียวได้ทรงกระบอกที่ขนาดตรงเป๊ะ ไม่ต้องวาดวงกลมแล้ว Push/Pull เหมือนใน SketchUp

{: .power }
Cylinder ของ SketchUp เป็นแค่ผิวหลายเหลี่ยมที่เอามาต่อกัน ขนาดเปลี่ยนไม่ได้ และผิวโค้งเป็นเหลี่ยม ๆ ส่วน formZ เป็น **solid ที่จำพารามิเตอร์ได้** และผิวโค้งจริงแบบ smooth (ความละเอียดของการแสดงผลปรับได้ภายหลัง)

{: .shapr }
Shapr3D: วาดวงกลมแล้วดึงขึ้น (extrude) · formZ: ใช้ Cylinder Preset คลิกเดียวจบ หรือถ้าชอบแบบ sketch-extrude ก็ใช้เครื่องมือกลุ่ม Draw ได้ (เรียนใน C2)

## ✅ เช็คตัวเอง
<details><summary>1. วิธีไหนสร้าง Cylinder ด้วยคลิกเดียว?</summary>Preset ซึ่งใช้ค่า Radius X, Radius Y, Height จาก Tool Options</details>
<details><summary>2. ทำไม Cap ถึงไปอยู่บนหน้าของ Body ได้เลย?</summary>formZ สร้าง face reference plane ให้อัตโนมัติเมื่อเมาส์ชี้บนหน้าของวัตถุ และ Snap to Center ทำให้ตรงศูนย์กลางพอดี</details>
<details><summary>3. formZ มี history tree แบบ Shapr3D ไหม?</summary>ไม่มี แต่วัตถุแบบ parametric อย่าง primitive จะจำค่าที่ใช้สร้างไว้ให้แก้ภายหลังได้</details>

{: .warning }
ถ้า Cap ลอยหรือจมอยู่ในตัว Body ให้ตรวจว่าตอนคลิกเคอร์เซอร์อยู่บนหน้าบนจริง (ไม่ใช่กริด XY) ถ้าไม่ใช่ ให้ Undo แล้ววางใหม่

📚 อ้างอิง: R1 Cylinder, Cone, Cube, Reference planes, Snapping · [Video: 3D Parametric Primitives](https://support.formz.com/hc/en-us/articles/28597325504659)
