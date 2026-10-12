---
title: "1. 24 เฟรม = 1 วินาที: Animation 101"
parent: "C5 · วิดีโอสินค้า 15 วินาที: แม็กเย็บขยับได้"
nav_order: 1
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c5-animation/01-basics/
hook: "สลับไป workspace Rendering/Animation และตั้ง Start Time / End Time / Frames Per Second ใน Animation Options"
---

# 1. 24 เฟรม = 1 วินาที: Animation 101
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- สลับไป workspace **Rendering/Animation**
- ตั้ง **Start Time / End Time / Frames Per Second** ใน **Animation Options**
- ใช้ **Animation Time Line** palette เลื่อนเวลา (scrub) ได้

## 💡 ไอเดียสั้น ๆ
วิดีโอคือ **ภาพนิ่งหลายภาพเรียงกัน** 30 ภาพต่อวินาที (30 fps) ก็พอให้ตาเห็นว่าลื่น ถ้ายาว 10 วินาทีจะเท่ากับ **300 เฟรม** ค่าทั้งหมดนี้ผูกกัน: แก้ค่าใดค่าหนึ่ง ค่าอื่นจะคำนวณตามเอง (R5: Animation Options)

| ค่า (Timing tab) | ค่าเริ่มต้น | ที่เราใช้ |
|---|---|---|
| Start Time | 0 | 0 |
| End Time | 10 วินาที | **10** |
| Frames Per Second | 30 | **30** |
| Frames | (คำนวณ) | 300 |

## 👣 ลงมือทำ (3 นาที)
1. เปิด `C2_Stapler.fmz` แล้ว **Save As** `C5_Stapler_Anim.fmz`
2. **Workspace** menu → **Rendering/Animation**
3. **Palettes > Animation Options** → แท็บ **Timing** ตั้งตามตาราง
4. หา **Animation Time Line** palette แล้วลองลาก **current time marquee** ไปมา (ยังไม่มีอะไรขยับ เพราะยังไม่มี animated entity)

{: .shot }
[SCREENSHOT: Animation Options > Timing tab]
{: .shot }
[SCREENSHOT: Animation Time Line palette พร้อมป้ายชื่อส่วนต่าง ๆ (ruler, marquee, ปุ่ม play, Auto Keyframe)]

{: .power }
SketchUp ทำได้แค่ **ภาพเคลื่อนไหวจาก Scenes** (กล้องเปลี่ยนมุม) ไม่สามารถทำให้ **ชิ้นส่วนขยับ** ได้ถ้าไม่มี extension ส่วน formZ Pro มี animation แบบ keyframe เต็มรูปแบบในตัว

{: .shapr }
Shapr3D Visualization มี turntable แบบพื้นฐาน · formZ มีทั้ง turntable, keyframe, path และ exploded view

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** คำนวณว่าวิดีโอ 15 วินาทีที่ 30 fps มีกี่เฟรม
</div>

## ✅ เช็คตัวเอง
<details><summary>1. 10 วินาทีที่ 30 fps มีกี่เฟรม?</summary>300</details>
<details><summary>2. Animation Options เปิดจากเมนูไหน?</summary>Palettes</details>
<details><summary>3. animated entity จะแสดงอยู่ที่ไหน?</summary>Animation Editor palette</details>

📚 อ้างอิง: R5 Animation Options, The Animation Time Line Palette, The Animation Process
