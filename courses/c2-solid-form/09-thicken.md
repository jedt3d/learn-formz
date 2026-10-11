---
title: "9. Thicken: ฝาบนแบบพลาสติกฉีด"
parent: "C2 · ฟอร์มสวยด้วย Solid"
nav_order: 9
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c2-solid-form/09-thicken/
---

# 9. Thicken: ฝาบนแบบพลาสติกฉีด
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Thicken** ทำ solid ให้ **กลวง** โดยมีผนังหนาตามที่กำหนด
- เปิดก้นฝาด้วย **Difference** เพื่อให้ได้ **เปลือก (shell)** แบบชิ้นพลาสติกจริง
- เข้าใจว่าทำไมชิ้นพลาสติกต้องหนา **1.5–3 mm**

## 💡 ไอเดียสั้น ๆ
ลองพลิกแม็กเย็บของจริงดู ฝาบนเป็น **เปลือกกลวง** ไม่ใช่ก้อนตัน ชิ้นพลาสติกฉีด (injection molding) ต้อง **หนาเท่า ๆ กันทั้งชิ้น** ไม่อย่างนั้นจะยุบหรือบิด

**Thicken**: ถ้าใช้กับผิว (surface) จะได้ solid ที่มีความหนา แต่ถ้าใช้กับ **solid** จะได้ solid **กลวง** ที่ผนังหนาตามค่าที่ตั้ง มีตัวเลือก **Justification** กำหนดว่าความหนาจะไปทางด้านใน กลาง หรือด้านนอก (R1: Thicken)

## 👣 ลงมือทำ (4 นาที)
1. **Save As** เป็น `C2_Stapler_v2.fmz` (เก็บไฟล์ก่อนกลวงไว้)
2. เลือก **Thicken** ตั้งความหนา **1.5** และ Justification ให้ความหนาอยู่ **ด้านใน** แล้วคลิก `Cover`
3. Cover จะกลวง แต่ยังปิดรอบทิศ ให้สร้าง Cube ตัวตัดที่คลุม **หน้าล่าง** ของ Cover หนาเกิน 1.5 mm เล็กน้อย
4. **Difference**: คลิก Cover แล้วคลิกตัวตัด ก้นฝาจะเปิด
5. หมุนมองจากด้านล่าง หรือใช้ **Wire Frame** จะเห็นผนังหนา 1.5 mm แล้วบันทึกไฟล์

{: .shot }
[SCREENSHOT: Thicken Tool Options (ความหนา 1.5 + Justification)]
{: .shot }
[SCREENSHOT: มุมล่างของ Cover ที่เห็นเปลือกบาง]

{: .verify }
ชื่อค่าของ **Justification** (Inside / Center / Outside หรือชื่ออื่น) ใน v10 ต้องยืนยันบนหน้าจอจริง

{: .power }
SketchUp ทำ shell ของ solid ไม่ได้ในตัว (ต้องลง extension) ส่วน Thicken ของ formZ ทำได้ทั้งกับผิวและ solid ในคลิกเดียว

{: .shapr }
Shapr3D: **Shell** · formZ: **Thicken** (ใช้กับ solid) หรือ **Offset Surface** (ใช้กับผิว)

## ✅ เช็คตัวเอง
<details><summary>1. Thicken กับ solid ได้ผลอย่างไร?</summary>ได้ solid กลวงที่ผนังหนาตามค่าที่ตั้ง</details>
<details><summary>2. ทำไมชิ้นพลาสติกต้องหนาเท่า ๆ กัน?</summary>เพื่อให้เย็นตัวเท่ากัน ไม่ยุบหรือบิดตอนฉีด</details>
<details><summary>3. ทำไมต้อง Save As ก่อน?</summary>เพื่อเก็บเวอร์ชันตันไว้ เผื่อจะแก้ฟอร์มภายหลัง (formZ ไม่มี history tree ให้ย้อน)</details>

📚 อ้างอิง: R1 Thicken, Offset Surface, Difference
