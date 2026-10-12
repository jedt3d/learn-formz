---
title: "3. 4 แบบโมเดล เลือกให้ถูกงาน"
parent: "C9 · Portfolio ชิ้นแรก: ของจากบ้านใน 90 นาที"
nav_order: 3
chapter: true
read_time: 4
do_time: 3
track: "🎨 Designer + 📐 Engineering"
permalink: /courses/c9-capstone/03-strategy/
hook: "ใช้ ตารางตัดสินใจ เลือกระหว่าง Solid / NURBS / Subdivision / Facetted และแบ่งชิ้นงานเป็น ชิ้นส่วนและลำดับการทำ"
---

# 3. 4 แบบโมเดล เลือกให้ถูกงาน
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **ตารางตัดสินใจ** เลือกระหว่าง Solid / NURBS / Subdivision / Facetted
- แบ่งชิ้นงานเป็น **ชิ้นส่วนและลำดับการทำ**
- รู้ว่าขั้นไหน **ย้อนแก้ยาก** (formZ ไม่มี history tree) จึงต้องบันทึกเป็นเวอร์ชันด้วย **File › Save Incremental**

## 💡 ไอเดียสั้น ๆ

| ถ้ารูปทรงเป็น... | ใช้ | เรียนใน |
|---|---|---|
| กล่อง มุมมน รูเจาะ (ที่ตัดเทป) | **Solid** + Controlled Round + Boolean | C1, C2 |
| สมมาตรรอบแกน (ไฟฉาย กระปุก) | **Revolve** / **Helix** | C3, C8 |
| เปลี่ยนหน้าตัดตามความยาว (แปรงสีฟัน) | **Loft** / Sweep | C3, C8 |
| ฟอร์มอิสระ จับถนัดมือ (**เมาส์**) | **Subdivision** → Convert to NURBS | C3 |
| ไฟล์พิมพ์/ส่งเรนเดอร์ | **Facetted** (Convert / Simplify) | C8 |

**แผนเมาส์:**
1. Body: Subdivision cage + Object Symmetry
2. Convert → NURBS/solid
3. Split → ปุ่มซ้าย ขวา และฝา
4. Wheel: Cylinder + Controlled Round
5. ตรวจ → Render → บอร์ด → export

## 👣 ลงมือทำ (3 นาที)
1. เขียนแผน 5 ขั้นของของที่เราเลือกเอง โดยใช้ตาราง
2. ตั้ง Layer: `Body`, `Parts`, `Ref` (underlay, เส้นช่วย), `Render`
3. บันทึกไฟล์แรกเป็น `C9_mouse_01.fmz` แล้วกด **File › Save Incremental** ทุกครั้งที่จบขั้นใหญ่ (blockout → shape → split ...) จะได้ `_02`, `_03` ... อัตโนมัติ และจดใน text note ว่าแต่ละเวอร์ชันคือขั้นไหน [🔍 รูปแบบชื่อไฟล์จริง]

{: .shot }
[SCREENSHOT: Layers palette 4 layer + ชื่อไฟล์เวอร์ชันใน Finder/Explorer]

{: .note }
🔀 **ถ้าเลือกของอื่น:** ที่ตัดเทป → C2 · แปรงสีฟัน → Loft + Bend/Taper · ไฟฉาย → Revolve + Helix (ฝาเกลียวจาก C8)

{: .power }
SketchUp มีแค่ mesh แบบเดียว ส่วน formZ ให้เลือก **4 แบบตามรูปทรง** และแปลงไปมาระหว่างกันได้ในไฟล์เดียว

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** เขียนแผนของสำรองอีก 1 ชิ้นด้วยเทคนิคที่ต่างกัน
</div>

## ✅ เช็คตัวเอง
<details><summary>1. เมาส์ควรใช้เทคนิคอะไร ทำไม?</summary>Subdivision เพราะเป็นฟอร์มอิสระที่ปั้นง่าย</details>
<details><summary>2. ทำไมต้องกด Save Incremental?</summary>formZ ไม่มี history tree ไฟล์เวอร์ชันที่ Save Incremental สร้างจึงเป็นจุดย้อนกลับ</details>
<details><summary>3. ไฟฉายใช้อะไร?</summary>Revolve + Helix สำหรับฝาเกลียว</details>
