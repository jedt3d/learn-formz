---
title: "3. วิธีที่ 2 · มนทั้งชิ้นในคลิกเดียว: Round"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 3
chapter: true
read_time: 3
do_time: 5
hook: "ทำยางลบที่มนทุกขอบในคลิกเดียว และลองแบบ Bevel"
permalink: /courses/m2-curves-rounds/03-round/
---

# 3. วิธีที่ 2 · มนทั้งชิ้นในคลิกเดียว: Round
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Round** กับทั้ง object
- เลือก **Cross Section** แบบ **Circular** หรือ **Bevel**
- เลือกวัดเป็น **Distance** หรือ **Radius**

## 💡 ไอเดียสั้น ๆ
Round มนหรือลบมุม (bevel) ทั้งชิ้นหรือบางส่วนก็ได้ ถ้าใช้กับ facetted object จะ **ถูกแปลงเป็น smooth อัตโนมัติ** (R1: Round) แต่ต่างจาก Controlled Round ตรงที่ **แก้ค่าทีหลังไม่ได้**

## 👣 ลงมือทำ (5 นาที)
1. **Cube** 40 × 20 × 10 (ยางลบ)
2. **Round** → Cross Section **Circular** → Radius **2** → คลิกทั้ง object
3. copy ยางลบอีกก้อน → **Round** แบบ **Bevel** Distance **1.5**
4. วางคู่กันแล้วใส่วัสดุ (ขาว + น้ำเงิน)

{: .shot }
[SCREENSHOT: ยางลบ Circular vs Bevel]

{: .warning }
Round **แก้ค่าทีหลังไม่ได้** ให้กด **Save Incremental** ก่อน หรือใช้ Controlled Round แทนถ้ายังไม่แน่ใจ

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำยางลบรูปทรงไข่ด้วย Sphere + Scale แล้วดูว่า Round ยังจำเป็นไหม
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Round กับ Controlled Round ต่างกันอย่างไร?</summary>Round แก้ค่าทีหลังไม่ได้ ส่วน Controlled Round แก้ได้</details>
<details><summary>2. Bevel คืออะไร?</summary>ลบมุมเป็นเส้นตรง</details>

📚 อ้างอิง: R1 Round
