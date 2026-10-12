---
title: "6. ชิ้นส่วนกระจายออกเอง: Object Staging"
parent: "C5 · วิดีโอสินค้า 15 วินาที: แม็กเย็บขยับได้"
nav_order: 6
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c5-animation/06-staging/
hook: "ทำ exploded view แบบเคลื่อนไหวด้วย Animate Object Staging (10.1+) และเลือก Disperse (แยกออก) หรือ Collect (รวมเข้า)"
---

# 6. ชิ้นส่วนกระจายออกเอง: Object Staging
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **exploded view** แบบเคลื่อนไหวด้วย **Animate Object Staging** (10.1+)
- เลือก **Disperse** (แยกออก) หรือ **Collect** (รวมเข้า)
- ตั้ง **Offset / Direction / Object Order / Speed**

## 💡 ไอเดียสั้น ๆ
**Exploded view** คือภาพที่ชิ้นส่วน "ลอย" แยกออกจากกันตามแนวประกอบ ใช้บอกว่าสินค้าประกอบจากอะไรบ้าง เป็นภาพที่ใช้กันมากในงาน product design ทั้ง portfolio และคู่มือ (R7: formZ 10.1)

| ค่า | ใช้ทำอะไร |
|---|---|
| **Disperse / Collect** | เริ่มจากตำแหน่งปกติแล้วแยกออก / เริ่มจากแยกอยู่แล้วรวมเข้าที่ปกติ |
| **Offset** | ระยะที่แต่ละชิ้นเคลื่อน |
| **Direction** | X±, Y±, Z± (แนวเส้นตรง) · **XY / XYZ** (กระจายออกจากจุดกลาง) |
| **Object Order** | ลำดับที่ชิ้นเริ่มขยับ (**Automatic** มักดีที่สุด) |
| **Speed / Accelerate / Decelerate** | ความเร็วและการเร่ง/ผ่อนของแต่ละชิ้น |
| **Delete Existing Tracks** | ลบ animation เดิมของชิ้นที่เลือก ⚠ |

## 👣 ลงมือทำ (4 นาที)
1. **Ungroup** UpperArm ชั่วคราว **หรือ** ทำงานในไฟล์สำเนา `C5_Stapler_Explode.fmz` (เพื่อไม่ให้ track เปิดฝาหาย)
2. เลือกทุกชิ้น (Base, Magazine, Cover, HingePin)
3. **Animate Object Staging**: Start **6.5**, Duration **2**, **Disperse**, Offset **40**, Direction **Z+**, Object Order Automatic และ **ปิด Delete Existing Tracks**
4. Play: ชิ้นส่วนจะลอยขึ้นทีละชิ้น
5. ทำอีกครั้งด้วย **Collect** ที่ Start **8.5** Duration **1.5** เพื่อประกอบกลับ

{: .shot }
[SCREENSHOT: Animate Object Staging dialog]
{: .shot }
[SCREENSHOT: เฟรมที่ชิ้นส่วนแยกเต็มที่ (exploded)]

{: .verify }
ถ้าใช้ Staging ครั้งที่ 2 บนชิ้นเดิม (ช่วงเวลาใหม่ + ปิด Delete Existing Tracks) แล้ว key เดิมถูกเขียนทับหรือไม่ ต้องยืนยันบนเครื่องจริง · ส่วน Group ที่มี track อยู่แล้วจะถูก staging อย่างไร ต้องทดสอบ

{: .power }
ใน SketchUp การทำ exploded แบบเคลื่อนไหวต้องใช้ extension หรือทำเป็นหลาย scene ส่วน formZ 10.1 ทำได้ในคำสั่งเดียว

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำ exploded view ที่กระจายขึ้นด้านบนแทนด้านข้าง
</div>

## ✅ เช็คตัวเอง
<details><summary>1. Disperse กับ Collect ต่างกันอย่างไร?</summary>Disperse เริ่มที่ตำแหน่งปกติแล้วแยกออก ส่วน Collect จบที่ตำแหน่งปกติ</details>
<details><summary>2. แม็กเย็บควรแยกตามแนวไหน?</summary>Z+ (ตามแนวที่ประกอบจากบนลงล่าง)</details>
<details><summary>3. ทำไมต้องระวัง Delete Existing Tracks?</summary>เพราะจะลบ animation เดิม เช่น การเปิดฝา</details>

📚 อ้างอิง: R7 formZ 10.1 Release Notes (Animate Object Staging)
