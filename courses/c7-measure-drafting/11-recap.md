---
title: "11. สรุป C7: แบบที่ส่งโรงงานได้"
parent: "C7 · เขียนแบบให้โรงงานอ่านออก: กบเหลา 3 ด้าน"
nav_order: 11
chapter: true
read_time: 4
do_time: 1
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/11-recap/
hook: "ดูภาพรวมของทั้ง course, แกลเลอรีผลงาน และเลือกทางไปต่อ"
---

# 11. สรุป C7: แบบที่ส่งโรงงานได้
{% include meta.html %}

## 🖼 แกลเลอรี
{: .shot }
[SCREENSHOT: เทียบ 3 ภาพ: ภาพร่างด้วยมือ → โมเดลที่มี dimension → แบบ A4]

## 🧭 ทำไมต้องเรียนสิ่งนี้
นักออกแบบที่ **เขียนแบบเป็น** คุยกับวิศวกรและโรงงานรู้เรื่อง งานออกแบบจึงถูกผลิตออกมา "เหมือนที่คิด" ไม่ใช่ "เหมือนที่โรงงานเดา"

| ขั้น | เครื่องมือ formZ |
|---|---|
| วัดและตรวจ | **Measure Distance**, **Measure Between**, Measure Angle |
| ข้อมูลวัสดุ | **Measure Quantities** (ปริมาตร, จุดศูนย์ถ่วง) → น้ำหนัก |
| ขนาด | **Linear / Multi / Angular / Radial-Diameter Dimension**, Leader Line, Text Note, **Dimension Styles** |
| ความเชื่อมโยง | **Associativity** |
| ภายใน | **Clipping Planes**, **Section**, **Hatch** |
| แบบ | Layout: **Multi-Frame** (first-angle, 2:1), Section frame, Hidden Line, title block → PDF |

## ✅ ตอนนี้เราทำได้แล้ว
- [ ] อ่านและเขียนแบบภาพฉายแบบ first-angle ได้
- [ ] ใส่ขนาดที่ผูกกับโมเดล
- [ ] ทำภาพตัดและ hatch
- [ ] ประมาณน้ำหนักและส่งแบบเป็น PDF ได้

{: .power }
แบบทั้งหมด **ลิงก์กับโมเดล 3D** ถ้าแก้ขนาดในโมเดล แบบก็ regenerate ตามได้ ไม่ต้องวาดใหม่ทั้งหมดแบบงาน 2D CAD สมัยก่อน

## 🎁 โจทย์เสริม
- เขียนแบบ **แม็กเย็บ (C2)** 3 ชิ้น แยกแผ่นละชิ้น + แผ่นประกอบ (assembly) ที่มี **balloon** (leader line + เลขชิ้น)
- ทำ **ตารางชิ้นส่วน (BOM)** ด้วย Text Note

## 👉 ต่อไป
**[C8 · เตรียมผลิต: 3D Print, STEP]({{ '/courses/c8-make-it/' | relative_url }})** <span class="tag tag-eng">Engineering</span> ทำ **ขวดน้ำ + ฝาเกลียว** ที่พิมพ์ 3D แล้วขันได้จริง

## 🧭 ไปต่อที่ไหน: 3 ทางเลือก
<div class="next-steps"><a href="{{ '/courses/c8-make-it/' | relative_url }}"><strong>➡️ ไปต่อ</strong><br>C8 พิมพ์ 3D ฝาเกลียว</a><a href="{{ '/courses/c6-layout-boards/' | relative_url }}"><strong>🖼️ แบบ + บอร์ด</strong><br>C6</a><a href="{{ '/courses/c9-capstone/' | relative_url }}"><strong>🎓 แบบของงานตัวเอง</strong><br>C9</a></div>
