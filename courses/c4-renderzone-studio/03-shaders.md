---
title: "3. Material 4 ชั้นของ RenderZone"
parent: "C4 · RenderZone ระดับสตูดิโอ"
nav_order: 3
chapter: true
read_time: 5
do_time: 3
permalink: /courses/c4-renderzone-studio/03-shaders/
---

# 3. Material 4 ชั้นของ RenderZone
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- สลับ **Material Type** เป็น **RenderZone** ใน Material Parameters
- เข้าใจ **4 ชั้นของ shader**: Color · Reflection · Transparency · Bump
- ใช้ปุ่ม **Options...** ของแต่ละชั้น

## 💡 ไอเดียสั้น ๆ
material ของ RenderZone คือ **ขนมชั้น 4 ชั้น** แต่ละชั้นเลือก shader จาก popup menu และกด **Options...** เพื่อปรับค่า (R3: Editing the parameters of a material)

| ชั้น | คำถามที่ตอบ | ตัวอย่าง shader |
|---|---|---|
| **Color** | สีหรือลายอะไร? | Plain color, ลาย procedural (ไม้ หินอ่อน), **Color Map** (ภาพ) |
| **Reflection** | เงาแค่ไหน สะท้อนแบบไหน? | Matte (ไม่สะท้อน), **Glossy**, **Metal, Accurate**, **Mirror**, **Multilayer Paint**, Glass |
| **Transparency** | โปร่งใสไหม? | None, ค่าโปร่งใส, จากภาพ |
| **Bump** | ผิวมีพื้นผิวนูนไหม? | ลาย procedural (เช่น **Cells** = หนัง), จากภาพ |

**วิธีเปิด:** ดับเบิลคลิก material ใน Materials palette → Material Parameters → ที่ **Material Type** เลือก **RenderZone**

## 👣 ลงมือทำ (3 นาที)
1. สร้าง material `TS_Test` แล้วดับเบิลคลิกเพื่อเปิด Material Parameters
2. เปลี่ยน **Material Type** เป็น **RenderZone** จะเห็น popup 4 ชั้น
3. ลองเปลี่ยน Reflection เป็น Glossy แล้ว Mirror ดูพรีวิว จากนั้นลอง Bump เป็น **Cells** แล้วดูพรีวิวอีกครั้ง
4. ลบ `TS_Test` ทิ้ง (บทนี้แค่ให้รู้จัก)

{: .shot }
[SCREENSHOT: Material Parameters (Material Type = RenderZone) ที่มี 4 popup และปุ่ม Options...]

{: .note }
**Keep Synchronized** (10.0.1+) จะพยายามทำให้ Shaded กับ RenderZone ดูเหมือนกัน ถ้าตั้งค่า RenderZone เองแบบละเอียด อาจต้อง **ปิด** ตัวเลือกนี้ เพื่อไม่ให้ค่าถูกเขียนทับ (R7)

{: .verify }
ชื่อ shader ในแต่ละ popup ของ v10 อาจต่างจากคู่มือ RenderZone ซึ่งเหมือน v9 ให้ยืนยันรายการจริงแล้วแก้ตารางนี้

{: .power }
SketchUp material มีแค่ **สี + ภาพ + opacity** ส่วน RenderZone มี **shader 4 ชั้น** ที่มีหลายสิบแบบ เช่น สีรถยนต์ (Multilayer Paint) หรือแก้วแบบ Fresnel

{: .shapr }
Shapr3D: Appearance (preset) · formZ: **สร้าง material เองได้ทุกชั้น** และบันทึกเป็น library ใช้ซ้ำได้

## ✅ เช็คตัวเอง
<details><summary>1. จะเห็น 4 ชั้นต้องตั้งอะไร?</summary>Material Type = RenderZone</details>
<details><summary>2. ผิวหนังลายนูนใช้ชั้นไหน?</summary>Bump (เช่น Cells)</details>
<details><summary>3. เปลี่ยนความเงาที่ชั้นไหน?</summary>Reflection</details>

📚 อ้างอิง: R3 Materials (Editing the parameters, Color/Reflection/Transparency/Bump shaders) · R7 Keep Synchronized
