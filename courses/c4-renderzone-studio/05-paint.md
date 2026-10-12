---
title: "5. 3 ผิวที่ใช้บ่อยที่สุด: สีรถ · พลาสติก · ยาง"
parent: "C4 · ถ่ายสินค้าแบบสตูดิโอ: เครื่องปิ้งขนมปัง 3 มุม"
nav_order: 5
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c4-renderzone-studio/05-paint/
hook: "ทำสีตัวเครื่องแบบ สีรถยนต์ ด้วย Multilayer Paint และทำ พลาสติกเงา ด้วย Glossy และ ยางด้าน แบบไม่สะท้อน"
---

# 5. 3 ผิวที่ใช้บ่อยที่สุด: สีรถ · พลาสติก · ยาง
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำสีตัวเครื่องแบบ **สีรถยนต์** ด้วย **Multilayer Paint**
- ทำ **พลาสติกเงา** ด้วย **Glossy** และ **ยางด้าน** แบบไม่สะท้อน
- ทำ **colorway 3 สี** จาก material เดียว

## 💡 ไอเดียสั้น ๆ
เครื่องใช้ในครัวรุ่นใหม่นิยม **สีพาสเทลเคลือบเงา** shader **Multilayer Paint** จำลองสีรถที่มี **ชั้นสี + ชั้นเคลือบใส** จึงดูลึกกว่า Glossy ธรรมดา (R3: Ray-Traced Reflections)

| วัสดุ | Color | Reflection |
|---|---|---|
| `TS_Body_Paint` | พาสเทล (เช่น มิ้นต์ ครีม ชมพูอ่อน) | **Multilayer Paint** |
| `TS_Plastic_Gloss` (ขอบช่อง) | ขาวหรือดำ | **Glossy** |
| `TS_Rubber` (ขา) | เทาเข้ม | ไม่สะท้อน (Matte) |

## 👣 ลงมือทำ (4 นาที)
1. สร้าง `TS_Body_Paint` แล้วตั้ง Reflection = **Multilayer Paint** (กด Options... ปรับความเงาของชั้นเคลือบ) ลากไปวางที่ `Body`
2. สร้าง `TS_Rubber` ไปใส่ที่ `Feet` และ `TS_Plastic_Gloss` สำหรับขอบปากช่อง (ใช้ **Paint** คลิกหน้าขอบช่อง)
3. **Duplicate** `TS_Body_Paint` เป็น 3 สี: `_Mint`, `_Cream`, `_Coral`
4. ทดสอบด้วย Render Area Rectangle ทีละสี แล้วเลือกสีหลัก

{: .shot }
[SCREENSHOT: Multilayer Paint Options dialog]
{: .shot }
[SCREENSHOT: ภาพทดสอบ 3 colorway เรียงกัน]

{: .verify }
คำสั่ง Duplicate material (ในเมนู ⋯ ของ Materials palette หรือคลิกขวา) และค่าใน Multilayer Paint Options ของ v10 ต้องยืนยันบนเครื่องจริง

{: .power }
**Multilayer Paint** ไม่มีใน SketchUp และเป็น shader ที่ใช้กันใน renderer ราคาแพง

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำเครื่องปิ้งสีพาสเทล 3 สีแล้ว render เทียบกัน
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Multilayer Paint ต่างจาก Glossy อย่างไร?</summary>จำลองชั้นสีกับชั้นเคลือบใส สีจึงดูลึกเหมือนสีรถ</details>
<details><summary>2. ยางควรสะท้อนไหม?</summary>แทบไม่สะท้อน (Matte)</details>
<details><summary>3. Colorway คืออะไร?</summary>ชุดสีหลายแบบของสินค้ารุ่นเดียวกัน</details>

📚 อ้างอิง: R3 Ray-Traced Reflections (Multilayer Paint, Glossy), Non-reflective shaders
