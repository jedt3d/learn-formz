---
title: "10. วิธีที่ 9 · ปั้นแบบดินน้ำมัน: Subdivision"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 10
chapter: true
read_time: 3
do_time: 6
hook: "ปั้นสบู่ก้อนแบบมีร่องจับนิ้วด้วย Subdivision"
permalink: /courses/m2-curves-rounds/10-subd/
---

# 10. วิธีที่ 9 · ปั้นแบบดินน้ำมัน: Subdivision
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- สร้าง cage แล้ว **Subdivision / Create**
- ดัน face ด้วย **Subdivision / Stretch** และทำร่องด้วย **Offset Face**

## 💡 ไอเดียสั้น ๆ
Subdivision เหมาะกับฟอร์มอิสระที่ "ปั้นด้วยมือ" กด **F6** เพื่อสลับดู cage (ทวน C3 บท 8)

## 👣 ลงมือทำ (6 นาที)
1. **Cube** 90 × 60 × 30 → **Subdivision / Create** Iterations **3**
2. F6 → คลิกขวา **Insert Sequence** ตามยาว 2 เส้น
3. เลือก face กลางหน้าบน → **Offset Face** แล้วดันลง 3 mm (ร่องนิ้ว)
4. **Stretch** face ด้านข้างออก 2 mm ให้ป่อง

{: .shot }
[SCREENSHOT: สบู่ก้อน cage (F6) vs ผล]

{: .power }
SketchUp ต้องลง extension SubD

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำสบู่ทรงหัวใจด้วยการลากจุดของ cage
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ดู cage กดปุ่มอะไร?</summary>F6</details>
<details><summary>2. เพิ่มเส้นรอบวัตถุทำอย่างไร?</summary>คลิกขวา Insert Sequence</details>

📚 อ้างอิง: R1 Subdivision / Create, Offset Face, Stretch
