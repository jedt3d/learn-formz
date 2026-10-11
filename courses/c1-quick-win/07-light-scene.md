---
title: "7. แสงและฉากสตูดิโอ"
parent: "C1 · Quick Win"
nav_order: 7
chapter: true
read_time: 5
do_time: 6
permalink: /courses/c1-quick-win/07-light-scene/
---

# 7. แสงและฉากสตูดิโอ
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **พื้นสตูดิโอ** ที่รับเงาแต่ไม่เห็นเป็นแผ่น ด้วย **Catcher** shader
- ปรับ **แสงหลัก** และ **ambient light** ให้ภาพนุ่ม
- ตั้งมุมกล้อง **Hero** แล้วบันทึกไว้ใน Views palette

## 💡 ไอเดียสั้น ๆ
ภาพสินค้าสวย ๆ ส่วนใหญ่ใช้สูตรเดียวกัน: **พื้นหลังสีเรียบ + เงานุ่มใต้ชิ้นงาน + มุมกล้องต่ำนิดหน่อย**
formZ เริ่มโปรเจกต์มาพร้อม **distant light 1 ดวง (แทนดวงอาทิตย์)** และ **ambient light** อยู่แล้ว (R1: Lights and Shadows) เราจึงแค่ปรับค่านิดหน่อย ไม่ต้องสร้างแสงเองทั้งหมด

## 👣 ลงมือทำ (6 นาที)

### A. พื้นรับเงา
1. วาดสี่เหลี่ยมพื้น **600 × 600 mm** บนระนาบ XY ที่ Z = 0 โดยให้ลำโพงอยู่ตรงกลาง: ใช้เครื่องมือ **Rectangle** (กลุ่ม Draw) แล้วเลือก object type ที่เป็น **ผิว (surface)** ใน Tool Options จากนั้นพิมพ์มุมแรก (−300, −300, 0) และมุมที่สอง (300, 300, 0) ใน **Input palette**
2. ตั้งชื่อ object ว่า `Floor`
3. สร้าง material ใหม่ชื่อ `PS_Floor_Catcher` แล้วใน Material Parameters ตั้ง **Color = Background** และ **Reflection = Catcher** จากนั้นกด **Options** เพื่อปรับ **Shadow Intensity** และ **Reflectivity** (เริ่มที่สะท้อนน้อย ๆ ก่อน) (R22: Catcher Shader)
4. ลาก material นี้ไปวางบน `Floor`

{: .shot }
[SCREENSHOT: Material Parameters ของ PS_Floor_Catcher ที่ Color = Background และ Reflection = Catcher พร้อมหน้าต่าง Options]

### B. แสง
5. เปิด **Lights** palette จะเห็นแสงที่มากับโปรเจกต์ ดับเบิลคลิกชื่อแสงเพื่อเปิด **Light Parameters**
6. ตั้ง **ambient light** ไว้ราว **50–70%** ซึ่งเป็นช่วงที่คู่มือ RenderZone แนะนำเมื่อจะใช้ Ambient Occlusion (R3: How to use ambient occlusion)
7. หมุนแสงหลักให้ส่องเฉียงจากหน้าซ้ายบน ใช้เครื่องมือ **Orbit Light** (Lights palette, เพิ่มมาใน 10.1) หรือแก้ทิศใน Light Parameters
8. สลับไปโหมด **Shaded Full** แล้วเปิด **Shadows** ใน Display Options เพื่อพรีวิวเงา

{: .shot }
[SCREENSHOT: Lights palette + Light Parameters ของ distant light]

{: .shot }
[SCREENSHOT: Shaded Full ที่เห็นเงาของลำโพงบนพื้น]

### C. มุมกล้อง Hero
9. หมุนมุมมองให้กล้องอยู่ต่ำ มองเฉียงลงเล็กน้อย ประมาณ 15–25° และให้ลำโพงกินพื้นที่ราว 60% ของจอ
10. บันทึก view ใน **Views** palette ชื่อ `Hero` แล้ว **บันทึกไฟล์**

{: .verify }
ไอคอน object type แบบ "surface" ของเครื่องมือ Draw (คู่มือบอกว่ามี 6 ไอคอน), ตำแหน่งช่องปรับความสว่างของ ambient light ใน Lights palette และชื่อ tab ใน Light Parameters ยังไม่ได้ยืนยันกับหน้าจอ v10 จริง ถ้าวาดผิวไม่ได้ ใช้วิธีสำรองได้: **Cube > Preset** ขนาด 600 × 600 × 1 mm แล้วเลื่อนลง 1 mm

{: .easy }
ภาพพรีวิวที่มีเงาได้ทันทีด้วย Shaded Full เหมือนการเปิด Shadows ใน SketchUp

{: .power }
**Catcher** shader ทำให้พื้นที่มองไม่เห็นรับเงาและเงาสะท้อนได้ เทคนิคแบบนี้ปกติต้องใช้ renderer ราคาแพง แต่ใน formZ มีอยู่แล้วใน RenderZone

{: .shapr }
Shapr3D Visualization ตั้งพื้นและแสงแบบ preset ให้ ส่วน formZ เราตั้งเองได้ทุกส่วน ช่วงแรกจะใช้เวลามากกว่านิดหน่อย แต่บันทึกพื้นและแสงชุดนี้ลง **template** ไว้ใช้ซ้ำได้ (ทำในบทที่ 8)

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมตั้ง Color ของพื้นเป็น Background?</summary>ให้พื้นกลืนไปกับฉากหลัง จะได้เห็นแค่เงา เป็นลุคสตูดิโอที่ไม่มีขอบพื้น</details>
<details><summary>2. ใน formZ แสงเริ่มต้นมีอะไรบ้าง?</summary>distant light 1 ดวง (แทนดวงอาทิตย์) และ ambient light</details>
<details><summary>3. บันทึกมุมกล้องไว้ทำไม?</summary>เพื่อให้กลับมาเรนเดอร์ที่มุมเดิมได้ทุกครั้ง</details>

📚 อ้างอิง: R1 Lights and Shadows, Shaded Full, Drawing Objects · R22 [Catcher Shader](https://support.formz.com/hc/en-us/articles/28221227477395) · R3 Ambient Occlusion · R7 (10.1 Orbit Light)
