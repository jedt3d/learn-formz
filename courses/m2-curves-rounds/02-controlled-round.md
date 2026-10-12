---
title: "2. วิธีที่ 1 · มนบางขอบ: Controlled Round"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 2
chapter: true
read_time: 3
do_time: 5
hook: "ทำรีโมททีวีที่ขอบบนมนใหญ่ ขอบล่างมนเล็ก และแก้ค่าได้ทีหลัง"
permalink: /courses/m2-curves-rounds/02-controlled-round/
---

# 2. วิธีที่ 1 · มนบางขอบ: Controlled Round
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- มนเฉพาะขอบที่เลือก **คนละรัศมี**
- กลับมาแก้รัศมีได้ทีหลัง (controlled object)

## 💡 ไอเดียสั้น ๆ
Controlled Round เป็น **controlled object** ที่จำค่ารัศมีไว้ จึงกลับมาแก้ได้ เหมาะกับงานที่ยังไม่แน่ใจขนาด (formZ ไม่มี history tree แต่ object แบบนี้แก้ได้เอง)

## 👣 ลงมือทำ (5 นาที)
1. **Cube** 45 × 180 × 20 (รีโมท)
2. **Controlled Round** เลือกขอบบน 4 เส้น → Radius **8**
3. เพิ่มชุดใหม่: ขอบล่าง 4 เส้น → Radius **2**
4. กลับไปแก้ขอบบนเป็น **10** แล้วดูว่าขอบล่างยังเหมือนเดิม
5. **Insert** ปุ่ม 3 ปุ่ม (Cylinder Ø8) ด้านบน

{: .shot }
[SCREENSHOT: รีโมทขอบบน R10 ขอบล่าง R2]

{: .easy }
คลิกขอบ → พิมพ์รัศมี ง่ายเท่ากับ Push/Pull

{: .verify }
วิธีเปิด controls ของ Controlled Round เพื่อแก้ค่า ดู C1 บท 5 / C2 บท 8

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำรีโมทแบบที่ 2 ที่ขอบบนเป็น R2 แล้วเทียบว่าแบบไหนจับถนัดกว่า
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมแก้รัศมีทีหลังได้?</summary>เพราะ Controlled Round เป็น controlled object ที่จำค่าไว้</details>
<details><summary>2. มนคนละขนาดในชิ้นเดียวได้ไหม?</summary>ได้ โดยแยกเป็นหลายชุดขอบ</details>

📚 อ้างอิง: R1 Controlled Round · [C2-8]({{ '/courses/c2-solid-form/08-rounds/' | relative_url }})
