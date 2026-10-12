---
title: "7. Decal: โลโก้แบรนด์ของเรา"
parent: "C4 · ถ่ายสินค้าแบบสตูดิโอ: เครื่องปิ้งขนมปัง 3 มุม"
nav_order: 7
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c4-renderzone-studio/07-decal/
hook: "ออกแบบ โลโก้แบรนด์สมมติ ของเราเอง (ภาพ PNG) และติดโลโก้บนวัตถุด้วยเครื่องมือ Decal"
---

# 7. Decal: โลโก้แบรนด์ของเรา
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ออกแบบ **โลโก้แบรนด์สมมติ** ของเราเอง (ภาพ PNG)
- ติดโลโก้บนวัตถุด้วยเครื่องมือ **Decal**
- จัดลำดับ decal หลายชิ้นในรายการ (สูงสุด 32 ต่อวัตถุ)

## 💡 ไอเดียสั้น ๆ
**Decal** คือ "สติกเกอร์" ที่แปะ **ทับ** material เดิม เหมาะกับโลโก้ ตัวหนังสือ หรือสเกลบนลูกบิด decal อยู่บนสุดของรายการจะแปะทับ decal ด้านล่าง (R3: Decals)

## 👣 ลงมือทำ (4 นาที)
1. ออกแบบโลโก้ง่าย ๆ (ชื่อแบรนด์ + สัญลักษณ์) ในโปรแกรมกราฟิกที่ถนัด บันทึกเป็น PNG **พื้นหลังโปร่งใส**
2. สร้าง material `TS_Logo` · Color = **Color Map** ใช้ภาพโลโก้ และตั้ง transparency ให้มาจากภาพเดียวกัน (Transparencies from images)
3. เลือกเครื่องมือ **Decal** แล้วคลิก `Body` หน้าต่าง **Decals** จะเปิดขึ้น
4. กด **+** เพื่อสร้าง decal ใหม่ เลือก `TS_Logo` แล้วตั้ง **Origin / Rotation / Mapping Type** และขนาด (กว้างประมาณ 60 mm) ให้อยู่ด้านหน้าตัวเครื่อง
5. ดูพรีวิวในหน้าต่าง แล้วกด OK จากนั้นทดสอบด้วย Render Area Rectangle

{: .shot }
[SCREENSHOT: Decals dialog (Origin / Rotation / Mapping Type + รายการ decal + ปุ่ม +)]
{: .shot }
[SCREENSHOT: โลโก้บนหน้าเครื่องปิ้ง]

{: .verify }
การตั้งให้ส่วนโปร่งใสของ PNG ไม่ถูกแปะใน decal ของ v10 (ใช้ alpha ของ PNG ได้เลย หรือต้องตั้ง Transparency shader) ต้องทดสอบบนเครื่องจริง

{: .power }
SketchUp ไม่มีระบบ decal แยกชั้น ต้องใส่ภาพเป็น material ของหน้าทั้งหน้า ส่วน formZ แปะทับได้ 32 ชั้นโดยไม่ทำลาย material เดิม

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำโลโก้แบรนด์ของตัวเอง (ชื่อเล่น) แล้วติดเป็น Decal
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Decal ต่างจาก material ปกติอย่างไร?</summary>แปะทับ material เดิมได้โดยไม่แทนที่</details>
<details><summary>2. Decal ไหนอยู่บนสุดเมื่อซ้อนกัน?</summary>อันที่อยู่บนสุดของรายการ</details>
<details><summary>3. วัตถุหนึ่งชิ้นมี decal ได้สูงสุดกี่อัน?</summary>32</details>

📚 อ้างอิง: R3 The Decal Tool, Creating Decals, Transparencies from images
