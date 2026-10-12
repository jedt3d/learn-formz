---
title: "11. สรุป C8: จากจอสู่ของจริง"
parent: "C8 · พิมพ์ 3D ให้ขันได้จริง: ขวด + ฝาเกลียว"
nav_order: 11
chapter: true
read_time: 4
do_time: 1
track: "📐 Engineering"
permalink: /courses/c8-make-it/11-recap/
hook: "ดูภาพรวมของทั้ง course, แกลเลอรีผลงาน และเลือกทางไปต่อ"
---

# 11. สรุป C8: จากจอสู่ของจริง
{% include meta.html %}

## 🖼️ แกลเลอรี
{: .shot }
[SCREENSHOT: ขวด + ฝา เรนเดอร์ / ผ่าครึ่ง / STL facetted / ชิ้นพิมพ์จริง เรียง 4 ภาพ]

## 🗺️ ภาพรวม: workflow เตรียมผลิต
```
ออกแบบตามกฎ DfAM → โมเดล solid (Loft · Helix · Boolean)
   → ตรวจชน (Intersection · Clipping)
   → Print Preparation → Object Doctor
   → Facetted / Simplify → STL ──→ Slicer → พิมพ์ทดสอบ → ปรับ clearance
   └→ STEP (AP214) ───────────→ CAD / โรงงาน
```

## 🤔 ทำไมเราต้องเรียนเรื่องนี้?
Product designer ไม่ได้หยุดที่ภาพสวย **ของต้องผลิตได้** การรู้กฎของการผลิต (ผนัง, overhang, clearance) ทำให้เราออกแบบได้ถูกต้องตั้งแต่ต้น และคุยกับวิศวกรหรือโรงงานได้รู้เรื่อง

## ✅ ตอนนี้เราทำได้แล้ว
- [x] ใช้กฎ 5 ข้อของ FDM printing
- [x] ทำ solid ด้วย **Tangent Loft + Caps** แล้วทำให้กลวงด้วย **Thicken**
- [x] สร้างเกลียวนอกและในด้วย **Helix** พร้อม **clearance**
- [x] ตรวจชนด้วย Intersection ของสำเนา
- [x] ตรวจและซ่อมด้วย **Print Preparation** และ **Object Doctor**
- [x] Export **STL** และ **STEP** อย่างถูกวิธี
- [x] ประมาณน้ำหนักด้วย **Mass Properties**

## 🏆 ภารกิจโบนัส
1. **ที่ตัดเทปจิ๋ว:** ทำแกนเทปที่สวมกับฐานด้วย clearance 0.3 mm
2. **สกรูจริง:** ใช้ **Screw/Bolt** สร้างสกรู M6 แล้วทำน็อตด้วย Helix เกลียวใน
3. **ประหยัดวัสดุ:** ทำของตันใหญ่ให้ Print Preparation เตือน **Large Volume** แล้วแก้ด้วย Thicken

{: .power }
**ทั้ง course นี้ใช้โปรแกรมเดียว** ตั้งแต่ออกแบบ เกลียว ตรวจ ซ่อม จนถึง STL/STEP ซึ่ง SketchUp ต้องใช้ extension หลายตัว

## ➡️ ต่อไป
[C9 · Capstone: ของจากบ้านตั้งแต่ต้นจนจบ]({{ '/courses/c9-capstone/' | relative_url }}) ใช้ทุกอย่างที่เรียนมากับของ 1 ชิ้นที่เราเลือกเอง

{% include homework.html id="c8-recap" title="C8 · Recap" what="ภาพรวม 4 ภาพ: เรนเดอร์, ผ่าครึ่ง, STL, ชิ้นพิมพ์/slicer" %}

## 🧭 ไปต่อที่ไหน: 3 ทางเลือก
<div class="next-steps"><a href="{{ '/courses/m5-eng-basics/' | relative_url }}"><strong>✏️ เช็กก่อนผลิต</strong><br>M5 DFM 6 ข้อ</a><a href="{{ '/courses/c9-capstone/' | relative_url }}"><strong>➡️ ไปต่อ</strong><br>C9 Portfolio ชิ้นแรก</a><a href="{{ '/courses/c7-measure-drafting/' | relative_url }}"><strong>📐 ส่งแบบคู่ไฟล์</strong><br>C7</a><a href="{{ '/courses/m1-quick-tips/' | relative_url }}"><strong>⚡ ทำงานไวขึ้น</strong><br>M1</a></div>
