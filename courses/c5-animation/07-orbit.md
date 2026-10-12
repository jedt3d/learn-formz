---
title: "7. กล้องบินรอบ + ไฟหมุนตาม"
parent: "C5 · วิดีโอสินค้า 15 วินาที: แม็กเย็บขยับได้"
nav_order: 7
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c5-animation/07-orbit/
hook: "ใช้ Create Orbit View ให้กล้องโคจรทั้งแนวนอน (Azimuth) และแนวตั้ง (Altitude) และใช้ Orbit Light (ใน Lights palette) ให้แสงเคลื่อนรอบสินค้า"
---

# 7. กล้องบินรอบ + ไฟหมุนตาม
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Create Orbit View** ให้กล้องโคจรทั้งแนวนอน (**Azimuth**) และแนวตั้ง (**Altitude**)
- ใช้ **Orbit Light** (ใน Lights palette) ให้แสงเคลื่อนรอบสินค้า
- ได้ช็อตจบแบบ "hero reveal"

## 💡 ไอเดียสั้น ๆ
Turntable หมุนในแนวนอนอย่างเดียว ส่วน **Orbit View** ยกกล้องขึ้นหรือลงไปพร้อมกันได้ ช็อตจบแบบโฆษณาที่นิยมคือ **กล้องเริ่มต่ำแล้วค่อย ๆ ยกขึ้น** ในขณะที่ **แสงเคลื่อน** ทำให้ไฮไลต์วิ่งบนผิว (R7: formZ 10.1)

| ค่า (Create Orbit View) | ตัวอย่าง |
|---|---|
| **Azimuth Start / End** | 0 → 45 (องศา สัมพัทธ์กับมุมเริ่มต้น) |
| **Altitude Start / End** | −10 → 15 |
| Start / Duration | 8.5 / 1.5 |
| Ease In/Out | เปิด (ช็อตจบไม่ต้องวนลูป) |

## 👣 ลงมือทำ (4 นาที)
1. สร้าง view ใหม่ `Reveal_Cam` (มุมต่ำด้านหน้า)
2. เลือก view นั้นแล้วเรียก **Create Orbit View** ตั้งค่าตามตาราง
3. **Lights** palette: เลือกไฟ Key แล้วใช้ **Orbit Light** ให้หมุนรอบสินค้าในช่วงเวลาเดียวกัน
4. Preview ใน **Shaded Work** (เร็วกว่า RenderZone มาก)

{: .shot }
[SCREENSHOT: Create Orbit View dialog (Azimuth / Altitude)]
{: .shot }
[SCREENSHOT: Lights palette ที่เห็นคำสั่ง Orbit Light]

{: .verify }
ค่าของ **Orbit Light** และวิธีสลับ "กล้องที่ใช้" ระหว่าง Turntable_Cam กับ Reveal_Cam ภายในวิดีโอเดียว ยังไม่มีเอกสารละเอียด ต้องทดสอบบน 10.1.x · ถ้าสลับกล้องไม่ได้ ให้ generate เป็น 2 คลิปแล้วไปตัดต่อรวมกันทีหลัง

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำกล้องบินรอบต่ำกว่าเดิม (Altitude ต่ำ) ให้ดูยิ่งใหญ่
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Azimuth กับ Altitude ต่างกันอย่างไร?</summary>Azimuth = หมุนแนวนอน · Altitude = ยกขึ้นหรือลงแนวตั้ง</details>
<details><summary>2. ทำไมช็อตจบควรเปิด Ease In/Out?</summary>ให้กล้องค่อย ๆ หยุด ดูนุ่มแบบโฆษณา</details>
<details><summary>3. ทำไม preview ด้วย Shaded Work?</summary>เพราะเร็ว ช่วยตรวจจังหวะก่อนเรนเดอร์จริง</details>

📚 อ้างอิง: R7 formZ 10.1 Release Notes (Create Orbit View, Orbit Light)
