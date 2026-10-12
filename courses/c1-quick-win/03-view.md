---
title: "3. หมุนดูรอบทิศ + มุมกล้อง hero 3 แบบ"
parent: "C1 · ปากกาเมจิกสวยใน 90 นาที"
nav_order: 3
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c1-quick-win/03-view/
hook: "หมุน แพน และซูมรอบชิ้นงานได้คล่อง และสลับโหมด Wire Frame / Shaded Work / Shaded Full ได้ตามงาน"
---

# 3. หมุนดูรอบทิศ + มุมกล้อง hero 3 แบบ
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- หมุน แพน และซูมรอบชิ้นงานได้คล่อง
- สลับโหมด **Wire Frame / Shaded Work / Shaded Full** ได้ตามงาน
- บันทึกมุมมองที่ชอบไว้ใน **Views** palette

## 💡 ไอเดียสั้น ๆ
formZ มีโหมดการแสดงผลแบบ real-time 3 โหมด และแบบภาพนิ่ง 2 โหมด (R1: Display Methods)

| โหมด | ใช้ตอนไหน |
|---|---|
| **Wire Frame** | ดูเส้นขอบและโครงด้านใน เร็วที่สุด |
| **Shaded Work** | โหมดหลักตอนปั้น |
| **Shaded Full** | เห็นแสงจาก Lights palette และเงา ใช้พรีวิวก่อนเรนเดอร์ |
| Hidden Line / Doodle | ภาพลายเส้นและภาพสเก็ตช์ (ภาพนิ่ง) |

เลือกได้จาก **Display** menu หรือจาก **Display Tools** palette ด้านบน ถ้า option-click (Mac) หรือ ctrl+shift-click (Windows) ที่ชื่อโหมด จะเปิด **Display Options** palette ของโหมดนั้น

## 👣 ลงมือทำ (3 นาที)
1. วาง **Cube** ขนาดไหนก็ได้ 1 ก้อนไว้ทดลอง (ใช้ Assistant: พิมพ์ `cube`)
2. ลองหมุน แพน และซูมด้วยเมาส์ แล้วลองใช้ไอคอนใน **Navigation tool palette** ด้านบน
3. สลับ **Shaded Work → Wire Frame → Shaded Full** แล้วสังเกตความต่าง
4. บันทึกมุมมอง: เปิด **Views** palette (อยู่ใน combo palette ด้านล่างขวา) แล้วเพิ่ม view ใหม่ ตั้งชื่อว่า `Test`
5. ลบ cube ทิ้ง

{: .shot }
[SCREENSHOT: ภาพเปรียบเทียบ 3 ช่อง: Wire Frame / Shaded Work / Shaded Full ของ cube เดียวกัน]

{: .shot }
[SCREENSHOT: Navigation tool palette ด้านบนขวา พร้อมป้ายชื่อไอคอนหลัก]

{: .verify }
การตั้งปุ่มเมาส์ (เช่น ปุ่มกลางเพื่อหมุนหรือแพน) และชื่อ standard views (Top/Front/...) ในคู่มือ v10 ยังไม่ชัดเจน ให้ดูจากวิดีโอ official **Interface Tour Part 1** ช่วง 03:55 *Basic Mouse Navigation*, 04:11 *Resetting the Home View* และ 08:34 *Main Model Views* แล้วบันทึกคีย์ที่ถูกต้องลงในบทนี้

{: .easy }
หมุน ซูม และแพนด้วยเมาส์เหมือน SketchUp และยังมี **Multi View** สำหรับดูหลายมุมพร้อมกันได้ด้วย

{: .shapr }
Shapr3D ใช้ท่าทางนิ้วสองนิ้ว ส่วน formZ เหมาะกับ **เมาส์ 3 ปุ่ม** มากกว่า ถ้าเคยใช้ Blender จะคุ้นกับการใช้ปุ่มกลางหมุนมุมมอง

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** บันทึกมุมกล้อง 3 มุม (hero, ด้านข้าง, มุมบน) แล้วสลับไปมาใน 3 วินาที
</div>

## ✅ เช็คตัวเอง
<details><summary>1. โหมดไหนเห็นเงาจากแสงในฉาก?</summary>Shaded Full (และ RenderZone)</details>
<details><summary>2. เปิดตัวเลือกของโหมดการแสดงผลอย่างไร?</summary>Display > Display Options หรือ option/ctrl+shift-click ที่ชื่อโหมด</details>
<details><summary>3. บันทึกมุมกล้องไว้ที่ไหน?</summary>Views palette</details>

📚 อ้างอิง: R1 Display Methods, View navigation and control · [Video: Interface Tour Part 1](https://support.formz.com/hc/en-us/articles/28596825311763)
