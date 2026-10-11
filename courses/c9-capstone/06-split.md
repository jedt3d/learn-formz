---
title: "6. แยกชิ้น: ปุ่ม + Split"
parent: "C9 · Capstone: ของจากบ้านตั้งแต่ต้นจนจบ"
nav_order: 6
chapter: true
read_time: 3
do_time: 5
track: "🎨 Designer + 📐 Engineering"
permalink: /courses/c9-capstone/06-split/
---

# 6. แยกชิ้น: ปุ่ม + Split
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- แปลง SubD เป็น solid ด้วย **Subdivision / Convert** (เป็น NURBS)
- ใช้ **Split** (Boolean) แยกเป็นฝาบน ฐาน ปุ่มซ้าย และปุ่มขวา
- ทำ **ร่อง (parting line)** กว้าง 0.8 mm ระหว่างชิ้น

## 💡 ไอเดียสั้น ๆ
ของจริงไม่ได้เป็นก้อนเดียว ตรงที่ชิ้นต่อกันมี **ร่อง** ที่เรียกว่า parting line ซึ่งทำให้ดูเป็นของที่ผลิตได้จริง วิธีทำ: ใช้แผ่นตัดหนา 0.8 แล้ว **Difference** ก่อน จากนั้นจึง **Split**

## 👣 ลงมือทำ (5 นาที)
1. **Subdivision / Convert** → ได้ NURBS solid (Save As `v03_split`)
2. **ฐาน/ฝา:** แผ่น Cube หนา **0.8** ที่ z = 8 → **Difference** ได้ร่องรอบตัว จากนั้นใช้แผ่นบาง ๆ ตรงกลางร่อง **Split** แยกฐานกับฝา
3. **ปุ่ม:** วาดเส้นแบ่งปุ่มบนภาพด้านบน (Vector Line) แล้ว **3D Extrusion** เป็นแผ่น 0.8 → **Difference** กับฝา
4. **Split** แยกปุ่มซ้าย ขวา และฝาหลัง ตั้งชื่อ `Btn_L`, `Btn_R`, `Shell`, `Base`
5. ซ่อนทีละชิ้นเพื่อตรวจว่าแยกได้ครบ

{: .shot }
[SCREENSHOT: เมาส์มีร่องปุ่มและร่องฐาน]
{: .shot }
[SCREENSHOT: Exploded แยก 4 ชิ้น]

{: .note }
🔀 **ถ้าเลือกของอื่น:** ไฟฉาย → แยกหัว/ตัว/ฝาท้าย · แปรงสีฟัน → แยกด้าม/ยางจับ (ใช้วัสดุต่างกันใน CMF)

## ✅ เช็คตัวเอง
<details><summary>1. Parting line คืออะไร?</summary>ร่องตรงที่ชิ้นส่วนต่อกัน</details>
<details><summary>2. ทำไมต้อง Convert ก่อน Split?</summary>Boolean ทำงานบน solid หรือ NURBS ได้แม่นยำกว่า SubD</details>
<details><summary>3. ร่องกว้างเท่าไร?</summary>0.8 mm</details>

📚 อ้างอิง: R1 Subdivision / Convert, Split, Difference · [C2 บท 7]({{ '/courses/c2-solid-form/07-split/' | relative_url }})
