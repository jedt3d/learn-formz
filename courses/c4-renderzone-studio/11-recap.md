---
title: "11. สรุป C4: สูตรถ่ายสินค้าของเรา"
parent: "C4 · ถ่ายสินค้าแบบสตูดิโอ: เครื่องปิ้งขนมปัง 3 มุม"
nav_order: 11
chapter: true
read_time: 4
do_time: 1
permalink: /courses/c4-renderzone-studio/11-recap/
hook: "ดูภาพรวมของทั้ง course, แกลเลอรีผลงาน และเลือกทางไปต่อ"
---

# 11. สรุป C4: สูตรถ่ายสินค้าของเรา
{% include meta.html %}

## 🖼 แกลเลอรี
{: .shot }
[SCREENSHOT: ภาพเรียง: โมเดลเปล่า (Shaded Work) → ใส่วัสดุ → แสง 3 จุด → GI สุดท้าย (4 ขั้น)]

## 🧭 ทำไมต้องเรียนสิ่งนี้
ลูกค้าและอาจารย์ตัดสินงานจาก **ภาพ** ก่อนเสมอ C4 สอนว่าภาพสวยมาจาก 3 ขา

| ขา | สิ่งที่เรียน |
|---|---|
| **วัสดุ** | shader 4 ชั้น · Metal, Accurate · Multilayer Paint · Glossy · Color Map · Bump · **Decal** |
| **แสง** | Area light 3 จุด · Environment light · ความสว่างเป็น lumens |
| **ภาพ** | Environment สำหรับการสะท้อน · AO + Final Gather · ภาพชุด 3 มุม · ไม่ใช้ Postprocess |

## ✅ ตอนนี้เราทำได้แล้ว
- [ ] สร้างวัสดุ RenderZone เองได้ทุกชั้น และทำ colorway ได้
- [ ] ติดโลโก้แบรนด์ด้วย Decal
- [ ] จัดแสงสตูดิโอแบบช่างภาพสินค้า
- [ ] ทำภาพชุดสำหรับ portfolio ได้ในเวลาที่คุมได้

{: .power }
ทั้งหมดนี้ทำได้ **ในโปรแกรมเดียว** ไม่ต้อง export ไปโปรแกรมเรนเดอร์อื่น ในขณะที่ SketchUp ต้องซื้อ renderer เพิ่ม

## 🎁 โจทย์เสริม
- เรนเดอร์ **ดินสอ + กาต้มน้ำ** จาก C3 ใหม่ด้วยแสงสตูดิโอของ C4 แล้วเทียบภาพก่อน/หลัง
- ทำ **กาน้ำแก้ว**: ใช้ Glass, Accurate (ระวังอย่าใส่ Transparency ซ้ำ)

## 👉 ต่อไป
**[C5 · ให้ของขยับได้: Animation]({{ '/courses/c5-animation/' | relative_url }})** พาแม็กเย็บจาก C2 มา **เปิด-ปิด** และทำ **exploded view** กับ **turntable** 360°

## 🧭 ไปต่อที่ไหน: 3 ทางเลือก
<div class="next-steps"><a href="{{ '/courses/c5-animation/' | relative_url }}"><strong>➡️ ไปต่อ</strong><br>C5 วิดีโอสินค้า 15 วินาที</a><a href="{{ '/courses/c6-layout-boards/' | relative_url }}"><strong>🖼️ ใช้ภาพทำบอร์ด</strong><br>C6 บอร์ด A3</a><a href="{{ '/courses/c9-capstone/' | relative_url }}"><strong>🎓 ใช้กับงานตัวเอง</strong><br>C9 Portfolio ชิ้นแรก</a></div>
