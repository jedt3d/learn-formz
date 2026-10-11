---
title: "9. Environment light + ฉากหลัง"
parent: "C4 · RenderZone ระดับสตูดิโอ"
nav_order: 9
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c4-renderzone-studio/09-environment/
---

# 9. Environment light + ฉากหลัง
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Environment light** (แสงจากภาพรอบฉาก) เพิ่มแสงนุ่มทั่วทั้งฉาก
- ตั้ง **Environment** ในแท็บ **Scene** ให้โลหะมีภาพให้สะท้อน
- เลือก **Background** ให้กลืนกับพื้น Catcher

## 💡 ไอเดียสั้น ๆ
**Environment light** ล้อมฉากด้วย cube หรือ sphere ที่มีภาพ พิกเซลที่สว่างจะปล่อยแสงมากกว่า ได้แสงนุ่มสมจริงโดยเรนเดอร์ไม่นาน (R3: Environment Lights)
ส่วน **Environment** ใน Scene tab คือ "ภาพที่โลหะสะท้อน" ซึ่ง **ไม่แสดงเป็นฉากหลัง** ยกเว้นเลือก Environment ใน Background (R3: Setting The Environment)

## 👣 ลงมือทำ (3 นาที)
1. เตรียมภาพสตูดิโอโทนขาวเทา (ภาพพาโนรามาที่อนุญาตให้ใช้ หรือภาพไล่สีที่ทำเอง)
2. **Lights** palette → ไฟใหม่ Type **Environment** → โหลดภาพ ตั้ง intensity ต่ำ ๆ (ให้ area light ยังเป็นแสงหลัก)
3. **Display > RenderZone Options... > Scene tab** → Environment: ใช้ภาพเดียวกันแบบ **mapped** (spherical)
4. ตรวจว่าเปิด **Reflections** อยู่ใน Shading tab
5. Background: ให้กลืนกับพื้น Catcher (ทวน C1) แล้วทดสอบเรนเดอร์ลูกบิดโครเมียม ตอนนี้ควรเห็นแถบสะท้อนสวยแล้ว

{: .shot }
[SCREENSHOT: RenderZone Options > Scene tab ส่วน Environment (mapped, spherical)]
{: .shot }
[SCREENSHOT: ก่อน/หลังใส่ Environment บนลูกบิดโครเมียม]

{: .verify }
ประเภทภาพที่ v10 รองรับสำหรับ Environment (HDR หรือแค่ JPG/PNG/TIFF) ต้องยืนยัน

## ✅ เช็คตัวเอง
<details><summary>1. Environment ใน Scene tab จะแสดงเป็นฉากหลังไหม?</summary>ไม่แสดง ยกเว้นเลือก Environment ใน Background</details>
<details><summary>2. ทำไม environment light ถึงตั้งให้อ่อน?</summary>เพื่อให้ area light ยังเป็นแสงหลักที่กำหนดทิศเงา</details>
<details><summary>3. ถ้าโลหะไม่สะท้อนเลย ตรวจอะไรก่อน?</summary>ดูว่าเปิด Reflections ใน Shading tab อยู่หรือไม่</details>

📚 อ้างอิง: R3 Environment Lights, Setting The Environment, Background · R22 Environment Lights
