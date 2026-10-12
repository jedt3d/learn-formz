---
title: "6. สรุป: DFM checklist 10 ข้อ"
parent: "M5 · วิศวกรตัวน้อย: 6 เช็กก่อนส่งผลิต"
nav_order: 6
chapter: true
read_time: 3
do_time: 2
track: "📐 Engineering"
hook: "ดูภาพรวมของทั้ง course, แกลเลอรีผลงาน และเลือกทางไปต่อ"
permalink: /courses/m5-eng-basics/06-recap/
---

# 6. สรุป: DFM checklist 10 ข้อ
{% include meta.html %}

**DFM (Design for Manufacturing)** = ออกแบบให้ผลิตได้ง่าย ถูก และพังน้อย พิมพ์ checklist นี้แปะไว้ แล้วติ๊กก่อนส่งงานทุกครั้ง

## ✅ DFM checklist
- [ ] 1. ขนาดมาจาก **การวัดจริง** 3 ครั้ง (บท 1)
- [ ] 2. หน่วย **mm** ตรวจด้วย Measure Distance แล้ว
- [ ] 3. ทุกจุดที่สวมกันเลือก **fit** แล้ว และเขียนว่าเผื่อต่อข้าง (บท 2)
- [ ] 4. พิมพ์ **ชิ้นทดสอบ fit** ก่อนพิมพ์ชิ้นจริง
- [ ] 5. **ผนังหนาเท่ากัน** (ฉีด: ~2 mm 🔍 / พิมพ์: ≥ 0.8 mm) (บท 3)
- [ ] 6. ผนังที่ถอดแม่พิมพ์มี **draft** ≥ 1° 🔍 (เฉพาะงานฉีด)
- [ ] 7. **Intersection** ทุกคู่ชิ้นที่ประกอบ = ว่าง (บท 4)
- [ ] 8. มุมด้านในมี **Round** (ลดจุดแตกร้าว) ([M2]({{ '/courses/m2-curves-rounds/' | relative_url }}))
- [ ] 9. **Print Preparation** ผ่าน (Non Solids, Thin Objects) ถ้าพิมพ์ 3D
- [ ] 10. **BOM** ครบ ชื่อชิ้นตรงกับโมเดลและแบบ (บท 5)

{: .shot }
[SCREENSHOT: กล่องดินสอที่ผ่าน checklist ครบ render + ตาราง BOM]

{% include homework.html id="m5-dfm" title="M5 · DFM" what="ภาพ checklist ที่ติ๊กครบ + ตาราง BOM + ภาพ Intersection ที่ว่าง" %}

## 🧭 ไปต่อที่ไหน: 3 ทางเลือก
<div class="next-steps"><a href="{{ '/courses/c9-capstone/' | relative_url }}"><strong>🎓 ไปต่อ</strong><br>C9 Portfolio (ใช้ checklist นี้ด้วย)</a><a href="{{ '/courses/c7-measure-drafting/' | relative_url }}"><strong>📐 ทำแบบ</strong><br>C7 เขียนแบบใส่ BOM</a><a href="{{ '/courses/m4-waffle/' | relative_url }}"><strong>🪵 ตัดเลเซอร์</strong><br>M4 Waffle</a></div>
