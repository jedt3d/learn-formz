---
title: "9. หูกาใน 4 ขั้น: Grow Face + Offset Face"
parent: "C3 · โค้งแบบมือโปร: ดินสอ + กาต้มน้ำ"
nav_order: 9
chapter: true
read_time: 4
do_time: 5
permalink: /courses/c3-curves-surfaces/09-handle/
hook: "'งอก' หน้าใหม่จาก cage ด้วย Subdivision / Grow Face (Distance + Angle) และทำหูจับรูปตัว C ที่จับถนัดมือ"
---

# 9. หูกาใน 4 ขั้น: Grow Face + Offset Face
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- "งอก" หน้าใหม่จาก cage ด้วย **Subdivision / Grow Face** (Distance + Angle)
- ทำหูจับรูปตัว C ที่จับถนัดมือ
- ใช้ **Subdivision / Offset Face** ทำร่องกันลื่น

## 💡 ไอเดียสั้น ๆ
**Grow Face** เหมือนการ "ดึงดินน้ำมันยืดออกมา" จากหน้าที่คลิก ระยะ (**Distance**) และมุม (**Angle**) ล็อกไว้ได้ จะได้ใช้ค่าเดิมซ้ำทุกท่อน และถ้าเปิด **Join Adjacent** หลายหน้าที่ติดกันจะยืดไปด้วยกัน (R1: Subdivision / Grow Face)

**แผนหูจับ** (ด้านหลังกา ฝั่ง −X)

| ท่อน | ทำอะไร | ค่า |
|---|---|---|
| ① | Cube 20 × 24 × 20 ชิดผนังหลังด้านบน (z ≈ 150–170) | cage เริ่มต้น |
| ② | Grow Face หน้าด้าน −X | 30 mm |
| ③ | Grow Face หน้าล่างของปลาย | 35 mm × 3 ครั้ง (Angle เล็กน้อยให้โค้ง) |
| ④ | Grow Face กลับเข้าหาตัวกา (+X) | 30 mm |

## 👣 ลงมือทำ (5 นาที)
1. สร้าง Cube ① ตำแหน่งตามตาราง แล้ว **Subdivision / Create**
2. **Grow Face** คลิกหน้า −X แล้วใส่ Distance **30**
3. **Grow Face** หน้าล่างของท่อนปลาย Distance **35** ทำซ้ำ 3 ครั้ง (ตั้ง Angle ประมาณ 10° ให้หูจับโค้งเข้าตัว)
4. **Grow Face** หน้าด้าน +X ของท่อนล่างสุด ให้กลับเข้าไปชนผนังตัวกา
5. **Offset Face** คลิกหน้าด้านในของหูจับ ตั้ง Distance **3** และ Depth **−1** จะได้ร่องรองนิ้ว
6. ตั้งชื่อ `Handle` แล้วบันทึก

{: .shot }
[SCREENSHOT: ลำดับ Grow Face ① → ④ (4 ภาพเล็ก)]
{: .shot }
[SCREENSHOT: Handle หลัง Offset Face เห็นร่องรองนิ้ว]

{: .note }
ถ้าหูจับเบี้ยว ให้ใส่ **Object Symmetry** (จาก C2) ที่ระนาบ XZ ทุกการแก้จะสมมาตรซ้ายขวา Symmetry รองรับ SubD โดยตรง (R1: Symmetry)

{: .power }
ทำหูจับแบบนี้ใน SketchUp แทบเป็นไปไม่ได้ถ้าไม่มี extension ส่วน formZ ใช้ประมาณ 6 คลิก

{: .shapr }
Shapr3D SubD: เลือกหน้าแล้ว **Extrude** · formZ: **Grow Face** (ล็อก Distance และ Angle ได้)

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำหูจับทรงที่สองที่จับด้วย 2 นิ้ว
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ล็อก Distance ไว้มีประโยชน์อย่างไร?</summary>ใช้ระยะเดิมซ้ำได้ทุกท่อน ทำให้หูจับสม่ำเสมอ</details>
<details><summary>2. Offset Face ทำอะไร?</summary>สร้างหน้าใหม่ขนานกับหน้าเดิม ย่อเข้าตาม Distance และยกขึ้นหรือกดลงตาม Depth</details>
<details><summary>3. ทำไมหูจับต้องโค้งเข้าหาตัวกา?</summary>เพื่อให้นิ้วสอดได้พอดีและถ่วงน้ำหนักได้ดีตอนเท</details>

📚 อ้างอิง: R1 Subdivision / Grow Face, Subdivision / Offset Face, Symmetry
