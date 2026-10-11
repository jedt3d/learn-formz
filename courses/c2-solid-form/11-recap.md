---
title: "11. สรุป: ภาพรวม C2"
parent: "C2 · ฟอร์มสวยด้วย Solid"
nav_order: 11
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c2-solid-form/11-recap/
---

# 11. สรุป: ภาพรวม C2 🎉
{% include meta.html %}

## 🖼 แกลเลอรี
{: .shot }
[SCREENSHOT: ภาพเรียง 4 ช่อง: ① ภาพถ่ายแม็กเย็บจริง + Underlay ② โปรไฟล์บนระนาบ ZX ③ ชิ้นส่วนที่ Split แล้ว (ยกฝาขึ้น) ④ ภาพเรนเดอร์สุดท้าย]

## 🧭 ทำไมต้องเรียนสิ่งนี้
ผลิตภัณฑ์จริงไม่ได้เป็นก้อนเดียว มี **หลายชิ้นส่วน** ที่ต้องผลิตได้และประกอบได้ C2 สอนวิธีคิดแบบนักออกแบบผลิตภัณฑ์:

> **มองโปรไฟล์ → ขึ้นรูปก้อนรวม → แบ่งเป็นชิ้น → ใส่ขอบมน → ทำให้บางแบบผลิตได้ → จัดระเบียบ**

| เรื่อง | เครื่องมือ formZ |
|---|---|
| อ้างอิงของจริง | Underlay, Plane / Plane Delta |
| ขึ้นรูป | Draw suite + **3D Extrusion**, Vector Line + Arc, Reshape |
| แก้บนหน้า | **Insert** (Cut / Fill) |
| ประกอบ | Move, **Align / Distribute**, Transform |
| แบ่งชิ้น | **Split**, Slice, Separate |
| ความงาม | Controlled Round หลาย set, Round to Holdline |
| ผลิตได้ | **Thicken** (shell 1.5 mm) |
| ระเบียบ | Object Symmetry, Layers, Group |

## ✅ ตอนนี้เราทำได้แล้ว
- [ ] เปลี่ยนภาพถ่ายของจริงให้เป็นโมเดลที่ขนาดถูก
- [ ] วาดโปรไฟล์ผสมเส้นตรงกับโค้งแล้วดึงเป็น solid
- [ ] แบ่ง ประกอบ และจัดชิ้นส่วนอย่างแม่นยำ
- [ ] ทำชิ้นแบบพลาสติกฉีดที่ผนังบางเท่ากัน

{: .easy }
เกือบทุกอย่างใน C2 คือ **วาด 2D แล้วดึงเป็น 3D** เหมือน SketchUp ต่างกันแค่ formZ ให้ผลเป็น solid ที่ผลิตได้จริง

## 🎁 โจทย์เสริม
- **ที่ตัดเทป (tape dispenser)**: ใช้ workflow เดียวกัน วาดโปรไฟล์ด้านข้าง → 3D Extrusion → Insert ร่องใบมีด → ทำม้วนเทปด้วย Cylinder 2 ชิ้นแล้ว Difference
- ปรับแม็กเย็บให้เป็น **colorway 3 สี** แล้วเรนเดอร์เทียบกัน

## 👉 ต่อไป
**[C3 · ผิวโค้งแบบมือโปร]({{ '/courses/c3-curves-surfaces/' | relative_url }})** จะเลิกใช้แค่กล่องกับกระบอก ไปทำ **ดินสอ** (Facetted vs Smooth) และ **กาต้มน้ำไฟฟ้า** ด้วย Revolve, NURBS, Loft และ Subdivision
