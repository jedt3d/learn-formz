---
title: "C1 · Quick Win"
nav_order: 10
has_children: true
permalink: /courses/c1-quick-win/
track: "🎨 Designer"
---

# C1 · Quick Win: ปั้น → ใส่วัสดุ → เรนเดอร์
{: .no_toc }

<span class="tag tag-designer">Designer</span><span class="tag tag-ready">พร้อมเรียน</span> ⏱ รวมประมาณ **90 นาที** (อ่าน ~43 + ลงมือ ~53) · 9 บท

**จบ course นี้แล้วเราจะได้ภาพเรนเดอร์แบบนี้หนึ่งภาพ:** **ปากกาเมจิก** ที่วัดจากของจริงในบ้านเรา มีปลอกกลวงพร้อมคลิป ขอบมน วัสดุ 3 แบบ (พลาสติกขาว, ปลอกสี, หัวสักหลาด) วางบนพื้นสตูดิโอสีขาวที่มีเงานุ่ม ๆ

{: .shot }
[SCREENSHOT: ภาพ hero shot ของปากกาเมจิก + ปลอก ที่เรนเดอร์ด้วย RenderZone เสร็จแล้ว ขนาด 1600×1000 px ใช้เป็นภาพปกของ course]

## เส้นทางของ course

| # | บท | อ่าน | ลงมือ | ได้อะไร |
|---|---|---|---|---|
| 1 | [เริ่มต้น 5 นาที: หน้าจอ + Assistant]({{ '/courses/c1-quick-win/01-start/' | relative_url }}) | 5 | 5 | รู้ว่าอะไรอยู่ตรงไหน หาเครื่องมือด้วยการพิมพ์ |
| 2 | [ตั้งค่าแค่พอดี: mm, Snap, Template]({{ '/courses/c1-quick-win/02-setup/' | relative_url }}) | 5 | 6 | ไฟล์ `PD_mm_template.fmz` |
| 3 | [มองรอบชิ้นงานและโหมดการแสดงผล]({{ '/courses/c1-quick-win/03-view/' | relative_url }}) | 4 | 3 | หมุน ซูม และสลับ Shaded/Wire ได้คล่อง |
| 4 | [วัดปากกาจริง แล้วปั้นด้าม]({{ '/courses/c1-quick-win/04-body/' | relative_url }}) | 5 | 7 | ด้าม + คอ + หัว ขนาดตรงของจริง |
| 5 | [ปลอกปากกา: ขอบมน + เจาะ + คลิป]({{ '/courses/c1-quick-win/05-details/' | relative_url }}) | 5 | 8 | ปลอกกลวงที่มีคลิป |
| 6 | [ใส่วัสดุ 3 แบบ]({{ '/courses/c1-quick-win/06-materials/' | relative_url }}) | 5 | 6 | ปากกาที่มีสีและผิวสัมผัส |
| 7 | [แสงและฉากสตูดิโอ]({{ '/courses/c1-quick-win/07-light-scene/' | relative_url }}) | 5 | 7 | วางปากกานอน + พื้นรับเงา + มุมกล้อง "Hero" |
| 8 | [RenderZone ครั้งแรก + ส่งการบ้าน]({{ '/courses/c1-quick-win/08-render/' | relative_url }}) | 5 | 8 | ภาพเรนเดอร์ 1 ภาพลง portfolio |
| 9 | [สรุป: ภาพรวม C1]({{ '/courses/c1-quick-win/09-recap/' | relative_url }}) | 4 | 3 | ภาพรวม + โจทย์เสริม (Pebble Speaker) |

**Workshop:** บทที่ 4–8 เป็น **build-along** ทำต่อเนื่องเป็นชิ้นเดียวกัน ใช้เวลาลงมือรวมประมาณ 35 นาที

## ต้องเตรียมอะไร
- formZ 10 **Pro** (หรือ Core) + **RenderZone** เวอร์ชัน 10.1.x
- **ปากกาเมจิกทรงกลม 1 ด้าม + ไม้บรรทัด** (จากบ้านเรา)
- เมาส์ 3 ปุ่ม (มี scroll wheel) จะสบายกว่า trackpad มาก
- โฟลเดอร์ `Documents/formZ/` สำหรับเก็บ template และโฟลเดอร์ `portfolio/` สำหรับเก็บภาพการบ้าน

{: .note }
course นี้ตั้งใจ **ไม่สอนทุกอย่าง** เราตั้งค่าเท่าที่จำเป็นเพื่อให้ได้ผลงานเร็วที่สุด เรื่อง solid เชิงลึก NURBS และงานพิมพ์ 3D อยู่ใน C2, C3 และ C8

{: .warning }
**ไม่ต้องใช้ RenderZone Postprocess ใน course นี้** มีรายงานในฟอรัม official ว่า formZ 10.1.5 บน Mac อาจ crash เมื่อเปิดหน้าต่าง Postprocessing (ดู [แหล่งอ้างอิง]({{ '/references/' | relative_url }}))
