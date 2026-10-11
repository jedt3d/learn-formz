---
title: "C2 · ฟอร์มสวยด้วย Solid"
nav_order: 20
has_children: true
permalink: /courses/c2-solid-form/
---

# C2 · ฟอร์มสวยด้วย Solid: แม็กเย็บกระดาษ
{: .no_toc }

<span class="tag tag-designer">Designer</span><span class="tag tag-ready">พร้อมเรียน</span> ⏱ รวมประมาณ **90 นาที** (อ่าน ~46 + ลงมือ ~44) · 11 บท

**จบ course นี้แล้วเราจะได้:** แม็กเย็บกระดาษแบบตั้งโต๊ะ **3 ชิ้น** (ฐาน, ตัวรางลวด, ฝาบน) + แกนหมุน ที่มีขนาดตามของจริงในบ้านเรา มีร่องรองลวด ฝาบนเป็นเปลือกบางแบบพลาสติกฉีดจริง และขอบมนสวยงาม พร้อมเอาไปทำ animation ต่อใน C5

{: .shot }
[SCREENSHOT: ภาพเรนเดอร์ปกของแม็กเย็บ 3 ชิ้น (ประกอบแล้ว + exploded เล็กน้อย)]

{: .note }
ต้องมี: **แม็กเย็บกระดาษ 1 ตัว + ไม้บรรทัด** · ไฟล์ `PD_mm_template.fmz` จาก C1 · ใช้เครื่องมือจาก C1 (Preset primitives, Controlled Round, Union/Difference)

| # | บท | อ่าน | ลงมือ | ได้อะไร |
|---|---|---|---|---|
| 1 | [วัดแม็กเย็บ + Underlay]({{ '/courses/c2-solid-form/01-measure/' | relative_url }}) | 4 | 4 | ภาพด้านข้างอยู่บนระนาบในโปรแกรม |
| 2 | [Draw + 3D Extrusion: ฐาน]({{ '/courses/c2-solid-form/02-base/' | relative_url }}) | 4 | 4 | ฐาน 130 × 35 × 10 |
| 3 | [เลือกให้เป็น: Pick + Reshape]({{ '/courses/c2-solid-form/03-pick-reshape/' | relative_url }}) | 5 | 3 | แก้ฐานด้วยการดึงหน้า |
| 4 | [โปรไฟล์โค้ง: Vector Line + Arc]({{ '/courses/c2-solid-form/04-profile/' | relative_url }}) | 5 | 5 | ตัวบนจากโปรไฟล์ด้านข้าง |
| 5 | [Insert: ร่องรองลวด]({{ '/courses/c2-solid-form/05-insert/' | relative_url }}) | 4 | 3 | ร่องบนฐานแบบ push/pull |
| 6 | [วางให้ตรง: Move, Align / Distribute]({{ '/courses/c2-solid-form/06-align/' | relative_url }}) | 4 | 3 | ตัวบนอยู่กึ่งกลางฐาน |
| 7 | [Boolean Split: แยกฝากับราง]({{ '/courses/c2-solid-form/07-split/' | relative_url }}) | 4 | 4 | 1 ชิ้นแยกเป็น 2 |
| 8 | [ขอบมนหลายชุด + Round to Holdline]({{ '/courses/c2-solid-form/08-rounds/' | relative_url }}) | 4 | 5 | ขอบมนทุกชิ้น |
| 9 | [Thicken: ฝาบนแบบพลาสติกฉีด]({{ '/courses/c2-solid-form/09-thicken/' | relative_url }}) | 4 | 4 | เปลือกหนา 1.5 mm |
| 10 | [Symmetry + จัดระเบียบ + แกนหมุน]({{ '/courses/c2-solid-form/10-organize/' | relative_url }}) | 4 | 6 | Layers, Group, hinge pin + ภาพเรนเดอร์ |
| 11 | [สรุป: ภาพรวม C2]({{ '/courses/c2-solid-form/11-recap/' | relative_url }}) | 4 | 3 | ภาพรวม + โจทย์เสริม |
