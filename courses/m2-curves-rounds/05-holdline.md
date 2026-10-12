---
title: "5. วิธีที่ 4 · มนตามเส้น: Round to Holdline"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 5
chapter: true
read_time: 3
do_time: 5
hook: "ทำตลับเทปวัดที่ขอบมนไม่เท่ากันตามเส้นที่วาดเอง"
permalink: /courses/m2-curves-rounds/05-holdline/
---

# 5. วิธีที่ 4 · มนตามเส้น: Round to Holdline
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Round to Holdline** ทำมนที่ขนาดเปลี่ยนไปตามเส้น holdline
- รู้ว่าเมื่อไรใช้แทน Controlled Round

## 💡 ไอเดียสั้น ๆ
บางชิ้นต้องการขอบที่ **กว้างไม่เท่ากัน** (ด้านหน้ามนกว้าง ด้านหลังมนแคบ) Round to Holdline ให้วาดเส้นบนหน้าเพื่อกำหนดว่าความมนจะไปสิ้นสุดตรงไหน

## 👣 ลงมือทำ (5 นาที)
1. **Cube** 65 × 65 × 35 (ตลับเทป)
2. วาดเส้น holdline บนหน้าบน: เริ่มห่างขอบหน้า 12 mm ค่อย ๆ แคบลงเหลือ 4 mm ที่ขอบหลัง
3. **Round to Holdline** → เลือกขอบ → คลิกเส้น holdline
4. เทียบกับ Controlled Round รัศมีเท่ากันทั้งเส้น

{: .shot }
[SCREENSHOT: ขอบตลับเทปแบบ holdline (กว้างไม่เท่ากัน)]

{: .verify }
ขั้นตอนการเลือกขอบและเส้น holdline ใน 10.1.x (ดู C2 บท 8 ประกอบ)

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** วาด holdline เป็นคลื่น แล้วดูว่าขอบเป็นอย่างไร
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ข้อดีของ holdline?</summary>ขอบมนที่ขนาดเปลี่ยนไปตามเส้นที่เราวาด</details>
<details><summary>2. ต่างจาก Controlled Round อย่างไร?</summary>Controlled Round ใช้รัศมีเท่ากันทั้งขอบ</details>

📚 อ้างอิง: R1 Round to Holdline · [C2-8]({{ '/courses/c2-solid-form/08-rounds/' | relative_url }})
