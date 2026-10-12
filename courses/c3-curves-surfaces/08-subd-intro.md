---
title: "8. Subdivision 101: ก้อนดินน้ำมันดิจิทัล"
parent: "C3 · โค้งแบบมือโปร: ดินสอ + กาต้มน้ำ"
nav_order: 8
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c3-curves-surfaces/08-subd-intro/
hook: "เข้าใจ cage (กรงเหลี่ยม) กับ subdivision surface (ผิวนุ่มที่ได้) และใช้ Subdivision / Create และตั้ง Iterations"
---

# 8. Subdivision 101: ก้อนดินน้ำมันดิจิทัล
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เข้าใจ **cage** (กรงเหลี่ยม) กับ **subdivision surface** (ผิวนุ่มที่ได้)
- ใช้ **Subdivision / Create** และตั้ง **Iterations**
- ใช้ **Sharpness** ทำขอบให้คมขึ้นเฉพาะจุด

## 💡 ไอเดียสั้น ๆ
Subdivision (SubD) คือการปั้นผิวนุ่มจาก **กล่องเหลี่ยมหยาบ ๆ** formZ จะเกลี่ยผิวให้นุ่มเองทุกครั้งที่เราขยับ cage เหมาะกับฟอร์ม "ออร์แกนิก" ที่จับถนัดมือ เช่น หูจับ เมาส์ หรือด้ามจับ (R1: Subdivision Surfaces)

| ค่า | ผล |
|---|---|
| **Iterations** (ค่าเริ่มต้น 3) | ยิ่งมากยิ่งเนียน แต่โปรแกรมช้าลง |
| **Sharpness** (0 = นุ่มสุด) | ทำให้จุด ขอบ หรือหน้าที่เลือก (prepick) คมขึ้น |

## 👣 ลงมือทำ (3 นาที)
1. ในไฟล์ `C3_Warmup.fmz` สร้าง **Cube** 40 × 40 × 40 (Preset)
2. **Subdivision / Create** คลิก cube จะกลายเป็นก้อนเกือบกลม
3. ลอง Iterations = **1** และ **4** แล้วดูความต่าง จากนั้นตั้งกลับ **3**
4. แสดง controls ของวัตถุ เลือกขอบบน 4 เส้น (prepick) แล้วเลื่อน **Sharpness** ขึ้น ขอบบนจะคมขึ้น ได้ทรง "หมอนอิง"
5. **Subdivision / Soften** ลองกับ cube อีกลูก ขอบทุกเส้นจะถูกลบมุมแล้วเปลี่ยนเป็น SubD ในคลิกเดียว (ปรับ **Distance**)

{: .shot }
[SCREENSHOT: Cube → Subdivision / Create (Iterations 1 / 3 / 4) เรียง 3 ลูก]
{: .shot }
[SCREENSHOT: Subdivision / Soften ที่ Distance ต่างกัน 2 ค่า]

{: .verify }
วิธี "แสดง controls" ของวัตถุ SubD (ปุ่มใน Tool Options หรือ context menu) ต้องยืนยันบน v10 ดูได้จาก R1: Right-Click Context Menu for Subdivision Surfaces

{: .power }
SketchUp ไม่มี SubD ในตัว (ต้องลง extension เสียเงิน) ส่วน formZ มี **SubD + Symmetry + แปลงเป็น NURBS** อยู่ในโปรแกรมเดียว

{: .shapr }
Shapr3D (ตั้งแต่ 2023) มี **SubD** แบบ cage เหมือนกัน · ถ้าเคยใช้ Blender ก็คือ **Subdivision Surface modifier** นั่นเอง

{% include can-sketchup.html id=5 %}

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ปั้นก้อนสบู่จาก Cube ด้วย Iterations 2 กับ 4 แล้วเทียบกัน
</div>

## ✅ เช็คตัวเอง
<details><summary>1. cage คืออะไร?</summary>วัตถุเหลี่ยมหยาบ ๆ ที่ควบคุมผิว subdivision ที่นุ่มอยู่ด้านใน</details>
<details><summary>2. ถ้าโปรแกรมช้า ควรลดค่าอะไร?</summary>Iterations</details>
<details><summary>3. Soften ต่างจาก Create อย่างไร?</summary>Soften ลบมุมขอบทุกเส้นก่อนแล้วค่อยแปลงเป็น SubD ทำให้ทรงยังใกล้กล่องเดิม</details>

📚 อ้างอิง: R1 Subdivision / Create, Subdivision / Soften, Subdivision Surfaces
