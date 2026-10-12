---
title: "8. ผ่าดูข้างใน: Clipping Plane vs Section"
parent: "C7 · เขียนแบบให้โรงงานอ่านออก: กบเหลา 3 ด้าน"
nav_order: 8
chapter: true
read_time: 4
do_time: 4
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/08-section/
hook: "ผ่าดูด้านในด้วย Clipping Planes (ผ่าแค่การแสดงผล ไม่ทำลายโมเดล) และผ่าจริงด้วย Section (2D / 3D Both / 3D Front / 3D Back)"
---

# 8. ผ่าดูข้างใน: Clipping Plane vs Section
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ผ่าดูด้านในด้วย **Clipping Planes** (ผ่าแค่การแสดงผล ไม่ทำลายโมเดล)
- ผ่าจริงด้วย **Section** (2D / 3D Both / 3D Front / 3D Back)
- ใส่ **Hatch** ที่หน้าตัด

## 💡 ไอเดียสั้น ๆ
| | Clipping Plane | Section tool |
|---|---|---|
| ผล | ผ่าเฉพาะการแสดงผล | **ตัดวัตถุจริง** |
| โมเดลเดิม | ไม่เปลี่ยน | เปลี่ยน (ทำในไฟล์สำเนา) |
| ใช้ทำ | ดูด้านใน, ใช้เป็นภาพตัดใน Layout | ชิ้นผ่าครึ่งสำหรับภาพ cutaway |

**Hatch** เป็น attribute ของ object หรือ face เลือกลายจาก **Hatch** palette (หรือโหลด .pat มาตรฐาน) แล้วใช้เครื่องมือ **Hatch** หรือลากจาก palette ไปวาง (R1: Hatches)

## 👣 ลงมือทำ (4 นาที)
1. **Clipping Planes** palette (ล่างสุดของ palette dock) → กด **New** ระนาบจะถูกสร้างกลางวัตถุ
2. ปรับให้ระนาบผ่า **กลางรูกรวย** ตามแนวยาว (ขนานระนาบ ZX ที่ y = 7) ตั้งชื่อ `SEC_A`
3. เปิด/ปิด clipping plane เพื่อดูด้านใน
4. (สำเนาไฟล์) **Section** เลือก **3D Front** แล้วคลิกตามระนาบเดียวกัน จะได้ชิ้นผ่าครึ่ง
5. **Hatch** palette เลือกลายเส้นเฉียง 45° แล้วลากไปวางบน **หน้าตัด**

{: .shot }
[SCREENSHOT: Clipping Planes palette ที่มี SEC_A]
{: .shot }
[SCREENSHOT: ชิ้นผ่าครึ่งที่หน้าตัดมี hatch เส้นเฉียง]

{: .verify }
การแสดง hatch บนหน้าตัดของ **clipping plane** (แทนที่จะต้องตัดจริง) ใน frame ของ Layout ทำได้หรือไม่ ต้องยืนยันใน v10

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำ section ตัดขวางอีก 1 แนว
</div>

## ✅ เช็คตัวเอง
<details><summary>1. อยากดูด้านในโดยไม่ทำลายโมเดล ใช้อะไร?</summary>Clipping Plane</details>
<details><summary>2. 3D Both ได้ผลอะไร?</summary>ได้ทั้งชิ้นหน้าและชิ้นหลัง</details>
<details><summary>3. ทำไมหน้าตัดต้องมี hatch?</summary>เพื่อแยกให้เห็นว่าส่วนไหนเป็นเนื้อวัสดุที่ถูกตัด</details>

📚 อ้างอิง: R1 Clipping Planes, Section, Hatches
