---
title: "12. สรุป: ภาพรวม C3"
parent: "C3 · ผิวโค้งแบบมือโปร"
nav_order: 12
chapter: true
read_time: 4
do_time: 1
permalink: /courses/c3-curves-surfaces/12-recap/
---

# 12. สรุป: ภาพรวม C3 🎉
{% include meta.html %}

## 🖼 แกลเลอรี
{: .shot }
[SCREENSHOT: ภาพเรียง 6 ช่อง: ลูกบอล facetted/smooth · ดินสอหลัง Intersection · โปรไฟล์ Spline · Revolve ผ่าครึ่ง · หูจับ SubD · ภาพเรนเดอร์สุดท้าย]

## 🧭 ทำไมต้องเรียนสิ่งนี้
ผลิตภัณฑ์ส่วนใหญ่ในบ้าน **ไม่ใช่กล่อง** C3 พาไปรู้จัก **3 ตระกูลผิว** ที่นักออกแบบมืออาชีพใช้ และวิธีเลือกให้เหมาะกับงาน

| ตระกูล | เหมาะกับ | เครื่องมือที่ใช้ใน C3 |
|---|---|---|
| **Facetted** | ของเหลี่ยม เช่น ดินสอ หรือ mesh สำหรับพิมพ์ 3D | Polygon + 3D Extrusion, Convert Object Type |
| **Smooth / NURBS** | ผิวโค้งแม่นยำ ที่วัดขนาดได้ | Curve Create, Curve Edit, **Revolve**, **NURBS by Lofting**, Zebra |
| **Subdivision** | ฟอร์มอิสระ จับถนัดมือ | **Subdivision / Create, Grow Face, Offset Face, Soften, Convert** |

## ✅ ตอนนี้เราทำได้แล้ว
- [ ] เลือกชนิดวัตถุให้เหมาะ และแปลงไปมาได้
- [ ] วาดเส้นโค้งที่คุมได้ แล้ว **Revolve** หรือ **Loft** เป็นผิว
- [ ] ตรวจผิวด้วย **Zebra** แบบนักออกแบบรถยนต์
- [ ] ปั้นฟอร์มออร์แกนิกด้วย **SubD** แล้วแปลงเป็น NURBS ไปใช้งานต่อได้

{: .power }
C3 ทั้ง course แทบไม่มีอะไรที่ SketchUp ทำได้ในตัวเลย: ผิวโค้งจริง, loft, การวิเคราะห์ผิว, SubD และการแปลงชนิดวัตถุ

## 🎁 โจทย์เสริม
- **แก้วมัค**: Revolve โปรไฟล์ + หูจับด้วย **Pipe** (วาดเส้นโค้งรูป C แล้วใช้ Pipe ตั้ง radius) ซึ่งจะได้ใช้จริงใน C6
- **ทัพพี**: Revolve ตัวถ้วยแบบครึ่งทรงกลม + ด้ามด้วย NURBS by Lofting

## 👉 ต่อไป
**[C4 · RenderZone ระดับสตูดิโอ]({{ '/courses/c4-renderzone-studio/' | relative_url }})** ปั้น **เครื่องปิ้งขนมปัง** แบบเร็ว แล้วใช้เวลาส่วนใหญ่ไปกับ **วัสดุ แสง และภาพ** ระดับโฆษณา
