---
title: "2. วัด + ถ่ายรูป + Underlay"
parent: "C9 · Portfolio ชิ้นแรก: ของจากบ้านใน 90 นาที"
nav_order: 2
chapter: true
read_time: 3
do_time: 5
track: "🎨 Designer + 📐 Engineering"
permalink: /courses/c9-capstone/02-reference/
hook: "ทำ dimension sheet ของของจริง และถ่ายภาพ ด้านบน + ด้านข้าง ที่ใช้เป็นแบบอ้างอิงได้"
---

# 2. วัด + ถ่ายรูป + Underlay
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **dimension sheet** ของของจริง
- ถ่ายภาพ **ด้านบน + ด้านข้าง** ที่ใช้เป็นแบบอ้างอิงได้
- วาง **Underlay** 2 ระนาบ (XY และ ZX) ที่ scale ตรงกัน

## 💡 ไอเดียสั้น ๆ
ทำซ้ำสิ่งที่เคยทำใน C2 แต่ใช้ **2 ภาพ** เพื่อให้เห็นฟอร์ม 3D ได้ครบ

| ค่าที่วัด (เมาส์ตัวอย่าง) | mm |
|---|---|
| ยาว × กว้าง × สูง | 115 × 62 × 38 |
| จุดสูงสุด (ห่างจากท้าย) | 40 |
| ล้อ Ø × กว้าง | 18 × 7 |
| ร่องปุ่ม | กว้าง ~1 |

เป้าหมายใน brief คือ **เล็กลง 10%** → **104 × 56 × 35**

## 👣 ลงมือทำ (5 นาที)
1. วัดตามตาราง แล้วจดใน [dimension sheet]({{ '/home-reference/' | relative_url }})
2. ถ่ายภาพด้านบนและด้านข้าง โดยวางไม้บรรทัดข้างของ ถือกล้องตั้งฉากและอยู่ห่าง ~1 m แล้วซูมเข้า (ลดการบิดเบี้ยวของมุมมอง)
3. ไฟล์ `C9_Capstone.fmz` เปิด **Underlay** บน **XY** (ภาพด้านบน) แล้วปรับให้ไม้บรรทัดตรงกับกริด
4. เปลี่ยน reference plane เป็น **ZX** แล้ววางภาพด้านข้าง ให้ท้ายเมาส์ตรงกันทั้งสองภาพ
5. ใช้ **Measure Distance** ตรวจความยาวบนภาพ ควรได้ใกล้ 115

{: .shot }
[SCREENSHOT: Underlay ภาพบน (XY) + ภาพข้าง (ZX) ในมุม Axonometric]

{: .verify }
formZ เก็บ Underlay แยกต่อ reference plane (XY/ZX/YZ) และแสดงพร้อมกันได้ไหม ต้องยืนยันใน v10 (ถ้าไม่ได้ ให้ใช้ภาพทีละระนาบ หรือ map ภาพลงแผ่นบาง ๆ แทน)

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ถ่ายภาพมุมที่ 3 (ด้านหน้า) เพิ่ม
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมถ่ายจากไกลแล้วซูม?</summary>ลดการบิดเบี้ยวจาก perspective ทำให้ภาพใกล้เคียงมุมมองตรงมากขึ้น</details>
<details><summary>2. ใช้อะไรตรวจ scale ของ underlay?</summary>Measure Distance วัดเทียบกับขนาดจริง</details>
<details><summary>3. ย่อลง 10% ความยาว 115 จะเหลือเท่าไร?</summary>~104 mm</details>

📚 อ้างอิง: R1 Reference Plane Parameters (Underlay), Measure Distance · [C2 บท 1]({{ '/courses/c2-solid-form/01-measure/' | relative_url }})
