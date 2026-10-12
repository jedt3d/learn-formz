---
title: "4. วัด 2 แบบที่ใช้ทุกวัน: Distance + Between"
parent: "C7 · เขียนแบบให้โรงงานอ่านออก: กบเหลา 3 ด้าน"
nav_order: 4
chapter: true
read_time: 4
do_time: 3
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/04-measure/
hook: "วัดระยะระหว่างจุดด้วย Measure Distance (+ Also Measure Perpendicular) และวัดระยะระหว่าง หน้า/เส้นที่ขนานกัน ด้วย Measure Between"
---

# 4. วัด 2 แบบที่ใช้ทุกวัน: Distance + Between
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- วัดระยะระหว่างจุดด้วย **Measure Distance** (+ **Also Measure Perpendicular**)
- วัดระยะระหว่าง **หน้า/เส้นที่ขนานกัน** ด้วย **Measure Between**
- ใช้ Measure Distance **ปรับขนาด** underlay ให้ตรง (ปุ่ม **Update**)

## 💡 ไอเดียสั้น ๆ
| เครื่องมือ | วัดอะไร |
|---|---|
| **Measure Distance** | จุด → จุด (มี hint บอกระยะ) และตั้งฉากกับหน้าได้ |
| **Measure Between** | ระหว่างคู่ของจุด เส้น หรือหน้า (ต้อง **ขนานกัน** ไม่อย่างนั้นจะขึ้น error) |
| **Measure Angle** | มุม |

**ทริกเด็ด:** หลังวัดด้วย Measure Distance ถ้าพิมพ์ค่าใหม่ในช่อง **Distance** แล้วกด **Update** วัตถุ underlay หรือ billboard ที่วัดจะถูก **scale ทั้งชิ้น** ให้ระยะนั้นเท่ากับค่าที่พิมพ์ เหมาะกับการปรับภาพถ่ายให้ตรงขนาดจริง (R1: Measure Distance)

## 👣 ลงมือทำ (3 นาที)
1. **Measure Distance** (เปิด Snap to Point) วัดความยาว Body จากมุมถึงมุม → ควรได้ 26
2. **Measure Between** คลิกหน้าซ้ายกับหน้าขวา → 26 · ลองคลิกหน้าบนกับหน้าข้าง (ไม่ขนาน) → จะเห็นข้อความแจ้งว่าวัดไม่ได้
3. วัดความหนาผนังระหว่างรูกรวยกับหน้าล่าง เทียบกับของจริง แล้วบันทึกตัวเลขลงภาพร่าง

{: .shot }
[SCREENSHOT: Measure Distance hint + ช่อง Distance / Update ใน Tool Options]

{: .easy }
เหมือน **Tape Measure** ของ SketchUp แต่วัดระหว่างหน้าที่ขนานกันได้โดยตรง

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** วัดระยะระหว่างรูกับขอบให้ได้ 3 ค่า
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไม Measure Between บางคู่ถึงวัดไม่ได้?</summary>เพราะหน้าหรือเส้นคู่นั้นไม่ขนานกัน ระยะจึงไม่นิยาม</details>
<details><summary>2. ปุ่ม Update ใช้ทำอะไร?</summary>scale วัตถุให้ระยะที่วัดได้เท่ากับค่าที่พิมพ์</details>
<details><summary>3. Also Measure Perpendicular ทำอะไร?</summary>วัดเพิ่มจากจุดแรกในแนวตั้งฉากกับเส้น ระนาบ หรือหน้า</details>

📚 อ้างอิง: R1 Measure Distance, Measure Between, Measure Angle
