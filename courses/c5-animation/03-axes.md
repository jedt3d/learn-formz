---
title: "3. Edit Axes: ย้ายจุดหมุนไปที่ hinge"
parent: "C5 · Animation จากโมเดล"
nav_order: 3
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c5-animation/03-axes/
---

# 3. Edit Axes: ย้ายจุดหมุนไปที่ hinge
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- รู้ว่าทุก object มี **แกนของตัวเอง (axes)** ซึ่งเป็นจุดหมุนตอนทำ animation
- ย้ายแกนด้วย **Edit Axes** ไปไว้ที่ **แกนหมุน (hinge pin)**
- รวม Cover + Magazine เป็น **Group** ให้หมุนไปด้วยกัน

## 💡 ไอเดียสั้น ๆ
ถ้าหมุนฝาแม็กโดยไม่ย้ายแกน ฝาจะหมุนรอบ **มุมของกล่องที่ล้อมมันไว้** และดูผิดธรรมชาติ ในงานจริงเราย้ายแกนไปไว้ที่ **บานพับ** ก่อน ซึ่งเป็นวิธีเดียวกับ tutorial ประตูหมุนในคู่มือ formZ (R5: Swinging door tutorial)

## 👣 ลงมือทำ (4 นาที)
1. **Group** `Cover` + `Magazine` ตั้งชื่อ `UpperArm`
2. เลือกเครื่องมือ **Edit Axes** (Modeling workspace) แล้วคลิก `UpperArm` จะเห็น transform widget ที่ตำแหน่งแกนปัจจุบัน
3. เปิด **Snap to Point** แล้วลากจุดกลาง widget ไปวางที่ **ศูนย์กลางของ HingePin** (ใช้ snap ที่จุดกึ่งกลางหน้าวงกลมของ pin)
4. ทดสอบ: ใช้ **Transform** หมุน `UpperArm` −30° รอบแกน Y ฝาควรยกขึ้นที่ด้านหน้าและหมุนรอบ pin จากนั้น **Undo**

{: .shot }
[SCREENSHOT: Edit Axes widget ก่อนและหลังย้ายไปที่ HingePin]

{: .note }
ทิศของมุมบวก (ตามเข็มหรือทวนเข็มนาฬิกา) ตั้งได้ใน **Project Settings: Working Units** (แท็บ Angle Options) ค่าเริ่มต้น **ทวนเข็ม = บวก** (R5)

{: .verify }
ถ้าใช้ Edit Axes กับ Group ไม่ได้ ให้ใช้กับแต่ละชิ้นแล้วรวมด้วย **Animation Group** tool แทน ต้องยืนยันใน v10

{: .shapr }
Shapr3D ไม่มีการตั้ง pivot สำหรับ animation · ส่วน Blender คือการตั้ง **Origin** ซึ่งคล้ายกับ Edit Axes

## ✅ เช็คตัวเอง
<details><summary>1. แกนของ object ใช้ทำอะไรใน animation?</summary>เป็นจุดอ้างอิงของการหมุนและการเลื่อน</details>
<details><summary>2. ทำไมต้อง group ฝากับราง?</summary>เพื่อให้หมุนไปพร้อมกันรอบ pin เดียว</details>
<details><summary>3. ค่าเริ่มต้นของมุมบวกคือทิศไหน?</summary>ทวนเข็มนาฬิกา</details>

📚 อ้างอิง: R5 Swinging door tutorial, Animation Group Tool · R1 Transform
