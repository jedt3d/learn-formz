---
title: "C8 · เตรียมผลิต: 3D Print, STEP, Laser"
nav_order: 26
permalink: /courses/c8-make-it/
---

# C8 · เตรียมผลิต: 3D Print, STEP, Laser
{: .no_toc }

<span class="tag tag-eng">Engineering</span><span class="tag tag-soon">เร็ว ๆ นี้</span> ⏱ เป้าหมายประมาณ 80 นาที

{: .verify }
course นี้ **อยู่ระหว่างวางแผน** โครงด้านล่างคือร่างบทเรียนที่จะเขียนต่อ

**ชิ้นงานหลัก:** ขวดน้ำ + ฝาเกลียว (พิมพ์ทดสอบได้จริง)
**เทคนิค:** NURBS, Screw/Bolt, Facetted mesh, Export

{: .note }
ใช้กิจกรรม [อ้างอิงจากของในบ้าน]({{ '/home-reference/' | relative_url }}) วัดและถ่ายรูปของจริงก่อนเริ่ม

## ร่างบทเรียน
1. ขวด: NURBS by Lofting + Thicken
2. เกลียว: Screw/Bolt หรือ Helix + Difference, ระยะเผื่อ (clearance)
3. Solid หรือไม่? (Inspector Info, Object Doctor)
4. Print Preparation (Non Solids, Scale To Printer) + Mass Properties
5. Polygon Mesh / Simplify Mesh* (Smooth → Facetted) แล้ว export STL และ import กลับมาตรวจ
6. STEP / 3DM สำหรับ CAD อื่น · (เสริม) Waffle* สำหรับ laser
7. Workshop: ไฟล์ STL ฝา + คอขวด (~50 นาที)

<small>* = formZ Pro เท่านั้น · อ้างอิง R1 Screw/Bolt, Helix, NURBS by Lofting, Polygon Mesh, STL/STEP · R14, R15, R7 (Waffle)</small>
