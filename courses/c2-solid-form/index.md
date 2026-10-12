---
title: "C2 · แม็กเย็บ: 10 ท่า Solid ที่ใช้ทุกวัน"
nav_order: 20
has_children: true
permalink: /courses/c2-solid-form/
n_chapters: 11
minutes: 90
outcome: "แม็กเย็บ solid ครบชิ้น ฝาเปิดได้ พร้อมไปทำ animation"
---

# C2 · แม็กเย็บ: 10 ท่า Solid ที่ใช้ทุกวัน
{: .no_toc }
<p class="course-sub">ฐาน · ฝาโค้ง · ร่อง · ขอบมน · บานพับ เหมือนของจริง</p>

{% include course_header.html %}

<span class="tag tag-designer">Designer</span><span class="tag tag-ready">พร้อมเรียน</span> ⏱ รวมประมาณ **90 นาที** (อ่าน ~46 + ลงมือ ~44) · 11 บท

**จบ course นี้แล้วเราจะได้:** แม็กเย็บกระดาษแบบตั้งโต๊ะ **3 ชิ้น** (ฐาน, ตัวรางลวด, ฝาบน) + แกนหมุน ที่มีขนาดตามของจริงในบ้านเรา มีร่องรองลวด ฝาบนเป็นเปลือกบางแบบพลาสติกฉีดจริง และขอบมนสวยงาม พร้อมเอาไปทำ animation ต่อใน C5

{: .shot }
[SCREENSHOT: ภาพเรนเดอร์ปกของแม็กเย็บ 3 ชิ้น (ประกอบแล้ว + exploded เล็กน้อย)]

{: .note }
ต้องมี: **แม็กเย็บกระดาษ 1 ตัว + ไม้บรรทัด** · ไฟล์ `PD_mm_template.fmz` จาก C1 · ใช้เครื่องมือจาก C1 (Preset primitives, Controlled Round, Union/Difference)

| # | บท | อ่าน | ลงมือ | ได้อะไร |
|---|---|---|---|---|
| 1 | [วัด 5 ค่า + วางรูปเป็นแบบ (Underlay)]({{ '/courses/c2-solid-form/01-measure/' | relative_url }}) | 4 | 4 | ภาพด้านข้างอยู่บนระนาบในโปรแกรม |
| 2 | [ฐานแม็กใน 3 คลิก: Rectangle + 3D Extrusion]({{ '/courses/c2-solid-form/02-base/' | relative_url }}) | 4 | 4 | ฐาน 130 × 35 × 10 |
| 3 | [ดึงหน้าเหมือน Push/Pull: Pick + Reshape]({{ '/courses/c2-solid-form/03-pick-reshape/' | relative_url }}) | 5 | 3 | แก้ฐานด้วยการดึงหน้า |
| 4 | [ฝาโค้งจากเส้นเดียว: Vector Line + Arc]({{ '/courses/c2-solid-form/04-profile/' | relative_url }}) | 5 | 5 | ตัวบนจากโปรไฟล์ด้านข้าง |
| 5 | [เจาะร่องลวดในคลิกเดียว: Insert]({{ '/courses/c2-solid-form/05-insert/' | relative_url }}) | 4 | 3 | ร่องบนฐานแบบ push/pull |
| 6 | [วางตรงเป๊ะ 0.1 mm: Move + Align / Distribute]({{ '/courses/c2-solid-form/06-align/' | relative_url }}) | 4 | 3 | ตัวบนอยู่กึ่งกลางฐาน |
| 7 | [ผ่าครึ่งได้ 2 ชิ้น: Split]({{ '/courses/c2-solid-form/07-split/' | relative_url }}) | 4 | 4 | 1 ชิ้นแยกเป็น 2 |
| 8 | [ขอบมน 4 ชุดในครั้งเดียว + Round to Holdline]({{ '/courses/c2-solid-form/08-rounds/' | relative_url }}) | 4 | 5 | ขอบมนทุกชิ้น |
| 9 | [ผนังพลาสติก 2 mm ในคลิกเดียว: Thicken]({{ '/courses/c2-solid-form/09-thicken/' | relative_url }}) | 4 | 4 | เปลือกหนา 1.5 mm |
| 10 | [แก้ข้างเดียวได้ 2 ข้าง: Symmetry + จัดระเบียบ]({{ '/courses/c2-solid-form/10-organize/' | relative_url }}) | 4 | 6 | Layers, Group, hinge pin + ภาพเรนเดอร์ |
| 11 | [สรุป C2: 10 ท่า Solid ในแม็กเย็บตัวเดียว]({{ '/courses/c2-solid-form/11-recap/' | relative_url }}) | 4 | 3 | ภาพรวม + โจทย์เสริม |
