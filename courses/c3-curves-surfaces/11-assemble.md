---
title: "11. ประกอบร่าง + render กาต้มน้ำ"
parent: "C3 · โค้งแบบมือโปร: ดินสอ + กาต้มน้ำ"
nav_order: 11
chapter: true
read_time: 4
do_time: 5
permalink: /courses/c3-curves-surfaces/11-assemble/
renderzone: true
hook: "ทำ ฐานไฟฟ้า (power base) เร็ว ๆ ด้วยเครื่องมือจาก C1 และใส่วัสดุ สแตนเลส / พลาสติก / ยาง"
---

# 11. ประกอบร่าง + render กาต้มน้ำ
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **ฐานไฟฟ้า** (power base) เร็ว ๆ ด้วยเครื่องมือจาก C1
- ใส่วัสดุ **สแตนเลส / พลาสติก / ยาง**
- เรนเดอร์ภาพ **ดินสอ + กาต้มน้ำ** ภาพเดียว

## 👣 ลงมือทำ (5 นาที)
1. **ฐาน:** Cylinder Preset R **80** H **12** ใต้ตัวกา + **Controlled Round** ขอบบน R4 ตั้งชื่อ `PowerBase`
2. **Layers:** สร้าง `Kettle` และ `Pencil` แล้วย้ายชิ้นเข้า layer ให้ถูก
3. **Materials:**

| ชิ้น | material |
|---|---|
| Body + Spout | `KT_Steel` โลหะเงา (จาก Library หมวดโลหะ) |
| Handle + Lid + Knob | `KT_Plastic_Black` พลาสติกดำกึ่งเงา |
| PowerBase | `KT_Plastic_White` |
| ยางรองฐาน (ถ้าทำ) | `KT_Rubber` |

4. **Merge:** เปิดไฟล์ดินสอ แล้ว copy ดินสอมาวางข้างฐานกา (File menu > Import หรือ copy/paste ระหว่างไฟล์)
5. **ฉาก:** ใช้พื้น Catcher จาก template ถ้ามีแสงสะท้อนบนโลหะแรงเกินไป ให้ลด Reflectivity ของพื้น
6. **RenderZone** (Raytrace + Shadows + Ambient Occlusion) แล้วบันทึกภาพ `C3_Kettle_Pencil.png`

{: .shot }
[SCREENSHOT: ภาพเรนเดอร์กาต้มน้ำ (สแตนเลส + ดำ) กับดินสอวางข้าง ๆ]

{: .note }
โลหะเงาจะสวยเมื่อมี **สิ่งให้สะท้อน** ถ้าโลหะดูดำ ๆ ให้ลองวาง **ผนังสีขาว** 2 แผ่นไว้นอกกล้องเพื่อให้มีอะไรสะท้อน (เรียนแสงสตูดิโอจริงจังใน C4)

{: .verify }
วิธีรวมวัตถุจากไฟล์อื่น (File > Import หรือ copy/paste ข้ามหน้าต่างโปรเจกต์) ใน formZ 10 ต้องยืนยันบนเครื่องจริง

{% include homework.html id="c3-workshop" title="C3 · Kettle + Pencil" what="ภาพถ่ายกาต้มน้ำและดินสอจริง + ภาพเรนเดอร์ + ภาพหน้าจอ Zebra ของตัวกา" %}

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** render กาต้มน้ำ 2 สีวางคู่กันเป็นภาพ family
</div>

📚 อ้างอิง: R1 Layers, Creating and Editing Materials · R3 RenderZone
