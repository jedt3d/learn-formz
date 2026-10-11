---
title: "2. ตั้งค่าแค่พอดี: mm, Snap, Template"
parent: "C1 · Quick Win"
nav_order: 2
chapter: true
read_time: 5
do_time: 6
permalink: /courses/c1-quick-win/02-setup/
---

# 2. ตั้งค่าแค่พอดี: mm, Snap, Template
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ตั้งหน่วยเป็น **มิลลิเมตร (mm)** ให้เหมาะกับงาน product
- ตั้ง **Grid Snap** และ **Object Snap** ที่จำเป็น
- บันทึกทุกอย่างเป็น **Template** เพื่อให้ไฟล์ใหม่ทุกไฟล์พร้อมใช้ตั้งแต่เปิด

## 💡 ไอเดียสั้น ๆ
งาน product design ส่วนใหญ่วัดเป็น **mm** เช่น ลำโพงกว้าง 70 mm หรือปุ่มกว้าง 10 mm ถ้าตั้งหน่วยถูกตั้งแต่แรก เราจะพิมพ์แค่ `70` ไม่ต้องคิดแปลงหน่วย
และเมื่อบันทึกเป็น template **ทำครั้งเดียวก็ใช้ได้ตลอด** นี่คือเหตุผลที่ formZ ที่ตั้งค่าถูกไม่ได้ยากกว่า SketchUp เลย

## 📍 อยู่ตรงไหน

| ตั้งค่า | ที่อยู่ (ชื่อ official) |
|---|---|
| หน่วยของไฟล์นี้ | **File > Project Settings... > Working Units** |
| กริด | **Reference Plane tool palette** (ล่างซ้าย) ช่อง **Module** และ **Divisions** · เปิดปิดด้วย **Display > Show Grid** |
| Grid snap | ไอคอน **Grid Snap** ด้านล่าง ข้าง ๆ มีช่องระยะและช่องมุม |
| Object snap | ไอคอน **Object Snap** + snap ย่อยต่าง ๆ ด้านล่าง (คลิกขวาที่ไอคอน > **Snap Options**) |
| Template | **Edit > Preferences... > Project > General > Use Template Project > Choose Template File...** |
| Auto save | **Edit > Preferences... > Project > Auto Save** |

## 👣 ลงมือทำ (6 นาที)

### ขั้น A: หน่วย mm
1. **File > Project Settings...** แล้วไปที่แท็บ **Working Units**
2. เลือกระบบ **Metric** และหน่วย **มิลลิเมตร**
3. ตั้งความละเอียด (accuracy) เป็น **0.1 mm** ซึ่งพอสำหรับงานพิมพ์ 3D ทั่วไป

{: .shot }
[SCREENSHOT: Project Settings > Working Units ตั้งค่า Metric / Millimeters / accuracy 0.1]

{: .verify }
ชื่อตัวเลือกในเมนู (เช่น "Millimeters" และชื่อช่อง accuracy) ในคู่มือ v10 ยังเป็นภาพของ v9 ให้ยืนยันจากหน้าจอจริงแล้วแก้ข้อความในบทนี้ให้ตรง ถ้ามีช่อง **Data Scale** ให้ปล่อยเป็นค่าเริ่มต้น (1:1)

### ขั้น B: กริดและ snap
4. ที่ **Reference Plane tool palette** ด้านล่าง ตั้ง **Module = 10 mm** และ **Divisions = 10** จะได้เส้นหนาทุก 1 cm และเส้นบางทุก 1 mm
5. เปิด **Grid Snap** แล้วตั้งระยะ **1 mm** และมุม **15°**
6. เปิด **Object Snap** และเลือก snap ย่อย 4 ตัวนี้พอ: **Snap to Point**, **Snap to Segment**, **Snap to Center**, **Snap to Intersection**

{: .shot }
[SCREENSHOT: แถบด้านล่าง แสดง Reference Plane palette (Module/Divisions) + Grid Snap 1 mm / 15° + Object Snaps ที่เปิดอยู่ 4 ตัว]

{: .note }
ถ้าขยับเมาส์แล้ว snap "ติด" เส้นมากเกินไป ให้ลองเปิดหรือปิดตัวเลือก **Stick To Edges** ใน Snap Options ดู (R1: Snapping)

### ขั้น C: บันทึกเป็น Template
7. **File > Save As...** ตั้งชื่อ `PD_mm_template.fmz` แล้วเก็บไว้ที่ `Documents/formZ/`
8. ปิดไฟล์
9. **Edit > Preferences... > Project > General** เลือก **Use Template Project** แล้วกด **Choose Template File...** เลือกไฟล์ที่เพิ่งบันทึก จากนั้นกด OK
10. (แนะนำ) ที่ **Project > Auto Save** เปิด **Enable Auto Save** และตั้ง **Every 10 Minutes**
11. ทดสอบ: **File > New Project** แล้วเช็คว่าหน่วยเป็น mm เองโดยไม่ต้องตั้งใหม่

{: .shot }
[SCREENSHOT: Preferences > Project: General ที่เลือก Use Template Project และแสดง path ของไฟล์]

{: .easy }
เหมือนการตั้ง **Default Template** ของ SketchUp (Product Design – Millimeters) ทำครั้งเดียว ไฟล์ใหม่ทุกไฟล์ก็พร้อมใช้

{: .power }
template ของ formZ เก็บได้มากกว่าหน่วย คือเก็บได้ทั้ง **layers, materials, lights และ objects** ที่ใช้ประจำ (R12) บทต่อ ๆ ไปเราจะกลับมาเพิ่ม material และพื้นสตูดิโอลงใน template นี้

{: .shapr }
Shapr3D ตั้งหน่วยครั้งเดียวที่ Settings ของแอป แต่ formZ เก็บหน่วยไว้ **ในแต่ละไฟล์** (Project Settings) template จึงเป็นตัวที่ทำให้ไม่ต้องตั้งซ้ำ

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมหน่วยของไฟล์ใหม่ยังเป็นนิ้ว แม้เคยตั้ง mm ไปแล้ว?</summary>เพราะเราตั้งค่าไว้แค่ในไฟล์เก่า ต้องตั้ง Use Template Project ใน Preferences ด้วย</details>
<details><summary>2. Module = 10 และ Divisions = 10 แปลว่าอะไร?</summary>เส้นหนาห่างกัน 10 mm และแบ่งย่อยเป็น 10 ช่อง ช่องละ 1 mm</details>
<details><summary>3. การแก้ template มีผลกับไฟล์เก่าไหม?</summary>ไม่มี template มีผลเฉพาะกับไฟล์ที่สร้างใหม่</details>

{: .warning }
อย่าเก็บ template ไว้ใน Downloads หรือ Desktop เพราะอาจถูกลบทิ้งโดยไม่รู้ตัว แล้วไฟล์ใหม่จะกลับไปใช้ค่าเริ่มต้นของโปรแกรม

📚 อ้างอิง: R1 Project Settings, Preferences – Project, Snapping, Reference planes · R12 [Setting up a Template File](https://support.formz.com/hc/en-us/articles/10364605436179) · [Video: Project Settings](https://support.formz.com/hc/en-us/articles/28597106429331)
