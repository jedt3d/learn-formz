---
title: "4. ประกอบแล้วชนไหม: Intersection + Measure Between"
parent: "M5 · วิศวกรตัวน้อย: 6 เช็กก่อนส่งผลิต"
nav_order: 4
chapter: true
read_time: 2
do_time: 3
hook: "สวมฝาเข้ากล่องในจอ แล้วพิสูจน์ว่าไม่ชนกันและมีช่องว่างตามที่ตั้ง"
track: "📐 Engineering"
permalink: /courses/m5-eng-basics/04-clearance/
---

# 4. ประกอบแล้วชนไหม: Intersection + Measure Between
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Intersection** หาส่วนที่ชนกัน (ถ้าไม่ชนจะได้ผลว่าง)
- ใช้ **Measure Between** วัดช่องว่างระหว่าง 2 หน้าขนาน

## 💡 ไอเดียสั้น ๆ
Intersection คืนค่า **ปริมาตรที่ซ้อนกัน** ของ 2 object ถ้าไม่ซ้อนกันเลยจะได้ object ว่าง (manual) ดังนั้นเป็นการ "ตรวจการชน" ที่ง่ายที่สุด

## 👣 ลงมือทำ (3 นาที)
1. วางฝาครอบกล่องในตำแหน่งที่ประกอบจริง
2. **Save Incremental** ก่อน
3. **Intersection** คลิกกล่อง แล้วคลิกฝา → ไม่มีผลลัพธ์ = ✅ ไม่ชน / มีชิ้นเล็กโผล่ = ❌ ชนตรงนั้น
4. **Undo** กลับ แล้ว **Measure Between** คลิกผนังนอกกล่องกับผนังในฝา (ต้องขนานกัน) → ควรได้ 0.2

{: .shot }
[SCREENSHOT: Intersection ที่ชนกัน (ชิ้นแดงเล็ก ๆ)]

{: .shot }
[SCREENSHOT: Measure Between ได้ 0.2 mm]

{: .warning }
Intersection ทำให้ object เดิมเป็น ghost ให้ Undo หรือเปิดไฟล์ Save Incremental กลับมา

{: .easy }
Measure Between บอก error ถ้า 2 หน้าไม่ขนาน แปลว่าเลือกหน้าผิด ให้ลองเลือกใหม่

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** เพิ่มสลักกันฝาหลุดแล้วตรวจการชนอีกรอบ
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Intersection แล้วว่าง แปลว่าอะไร?</summary>ไม่มีส่วนที่ชนกัน</details>
<details><summary>2. Measure Between ใช้กับอะไรได้?</summary>จุด เส้น และหน้า ที่ขนานกัน</details>

📚 อ้างอิง: Manual: Intersection, Measure Between
