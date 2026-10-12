---
title: "2. 3 ชิ้นเล็กใน 10 นาที: คันโยก · ลูกบิด · ขา"
parent: "C4 · ถ่ายสินค้าแบบสตูดิโอ: เครื่องปิ้งขนมปัง 3 มุม"
nav_order: 2
chapter: true
read_time: 3
do_time: 4
permalink: /courses/c4-renderzone-studio/02-parts/
hook: "เพิ่ม รายละเอียดเล็ก ที่ทำให้ภาพดูเป็นสินค้าจริง และใช้ Subdivision / Soften ทำคันโยกให้ขอบนุ่มในคลิกเดียว"
---

# 2. 3 ชิ้นเล็กใน 10 นาที: คันโยก · ลูกบิด · ขา
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เพิ่ม **รายละเอียดเล็ก** ที่ทำให้ภาพดูเป็นสินค้าจริง
- ใช้ **Subdivision / Soften** ทำคันโยกให้ขอบนุ่มในคลิกเดียว
- แยกชิ้นตาม **วัสดุ** ตั้งแต่ตอนปั้น (จะใส่ material ง่าย)

## 💡 ไอเดียสั้น ๆ
กฎของภาพสินค้า: **1 วัสดุ = 1 object (หรือ 1 กลุ่มหน้า)** ปุ่มโลหะต้องเป็นชิ้นแยกจากตัวเครื่องพลาสติก

| ชิ้น | วิธี | ค่า |
|---|---|---|
| Side plate (แผ่นข้าง) | Insert: Fill บนหน้าข้าง แบบรางตั้ง 14 × 110 ลึก 3 → แยกเป็นชิ้น | ร่องสำหรับคันโยก |
| Lever (คันโยก) | Cube 40 × 16 × 12 → **Subdivision / Soften** Distance 3 | |
| Knob (ลูกบิด) | Cylinder R12 H10 + Controlled Round R2 | วางบนหน้าข้าง (face plane) |
| Feet (ขา 4 ข้าง) | Cylinder R8 H6 + Copy (Move + Copy) | |

## 👣 ลงมือทำ (4 นาที)
1. วาดร่องคันโยกที่หน้าข้าง +X ด้วย **Insert: Cut** ลึก 3
2. **Cube** คันโยก ยื่นออกจากร่อง แล้วใช้ **Subdivision / Soften** ตั้งชื่อ `Lever`
3. **Cylinder** ลูกบิด วางบนหน้าข้างใต้ร่อง (face reference plane + Snap) ตั้งชื่อ `Knob`
4. ขา: วาง Cylinder ใต้มุมหนึ่ง แล้วใช้ **Move** ที่เปิดตัวเลือกสร้างสำเนาใน Tool Options ทำซ้ำให้ครบ 4 มุม ตั้งชื่อ `Feet`
5. บันทึก

{: .shot }
[SCREENSHOT: ด้านข้างของเครื่องปิ้ง เห็นร่อง คันโยก และลูกบิด]

{: .verify }
ชื่อตัวเลือก "สร้างสำเนา" ใน Move Tool Options (คู่มือบอกว่าเครื่องมือ transform ทุกตัวมีตัวเลือก transform แบบ with/without copying) ต้องยืนยันชื่อบนหน้าจอจริง

{: .shapr }
Shapr3D: Move + **Copy** toggle · formZ: Move + ตัวเลือก **copy** ใน Tool Options

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ออกแบบลูกบิดใหม่ 1 แบบที่มีร่องกันลื่น
</div>

📚 อ้างอิง: R1 Transforming Objects, Subdivision / Soften, Drawing Objects (Insert)
