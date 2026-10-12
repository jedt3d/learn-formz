---
title: "6. วางตรงเป๊ะ 0.1 mm: Move + Align / Distribute"
parent: "C2 · แม็กเย็บ: 10 ท่า Solid ที่ใช้ทุกวัน"
nav_order: 6
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c2-solid-form/06-align/
hook: "จัดตัวบนให้อยู่ กึ่งกลางฐาน ในคลิกเดียวด้วย Align / Distribute และใช้ Move แบบ snap จากจุดไปจุด"
---

# 6. วางตรงเป๊ะ 0.1 mm: Move + Align / Distribute
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- จัดตัวบนให้อยู่ **กึ่งกลางฐาน** ในคลิกเดียวด้วย **Align / Distribute**
- ใช้ **Move** แบบ snap จากจุดไปจุด
- รู้จัก **Transform** tool ที่รวมการย้าย หมุน และย่อขยายไว้ในตัวเดียว

## 💡 ไอเดียสั้น ๆ
งานประกอบหลายชิ้นต้อง **วางให้ตรงกัน** อย่าใช้สายตาลาก ให้ใช้เครื่องมือจัดตำแหน่งแทน
**Align / Distribute** จัดวัตถุได้ทั้งแนว X, Y, Z ทีละแกน แต่ละแกนเลือกได้ว่าจะชิด **min / center / max** หรือจะกระจายระยะเท่ากัน (R1: Align / Distribute)

| เครื่องมือ | เหมาะกับ |
|---|---|
| **Move** | ย้ายจากจุด snap ไปอีกจุด (กด Cmd/Ctrl เพื่อเลื่อนตั้งฉากกับระนาบ) |
| **Align / Distribute** | จัดให้ตรงแนวหรือกระจายระยะเท่ากัน |
| **Transform** | ใช้ controller ที่มีแกน วงหมุน และลูกศร scale |

## 👣 ลงมือทำ (3 นาที)
1. เลือก **Pick** แล้ว **Shift-คลิก** `Base` ก่อน จากนั้น `Upper`
2. เลือก **Align / Distribute** ใน Tool Options ตั้ง **Y = Align Center** ส่วน X และ Z ตั้งเป็น "no action" (ตัวเลือกบนสุด)
3. ตัวบนจะเลื่อนมาอยู่กึ่งกลางความกว้างของฐาน
4. ตรวจด้านล่าง: ตัวบนต้องลอยเหนือฐาน 4 mm (z = 14 เทียบกับฐานสูง 10) ซึ่งเป็นช่องว่างที่เอาไว้สอดกระดาษ ถ้าไม่ใช่ ให้ใช้ **Move** + Cmd/Ctrl ปรับ
5. บันทึกไฟล์

{: .shot }
[SCREENSHOT: Align / Distribute Tool Options ที่ Y = Align Center]
{: .shot }
[SCREENSHOT: มุมมองด้านหน้า (front) เห็นตัวบนอยู่กึ่งกลางฐาน]

{: .verify }
คู่มือไม่ได้บอกชัดว่า Align จะยึดชิ้นไหนเป็นหลัก (ชิ้นแรกที่เลือก หรือกรอบรวมของทุกชิ้น) ให้ทดสอบบนเครื่องจริงแล้วบันทึกผล ถ้าฐานขยับไปด้วย ให้ Undo แล้วล็อก layer ของฐานก่อน

{: .easy }
เหมือนการใช้ Align ในโปรแกรมกราฟิก (Illustrator หรือ Keynote) แต่ใช้กับ 3D

{: .power }
SketchUp ไม่มี Align/Distribute ในตัว ต้องลง extension เพิ่ม

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** วางลวดเย็บ 5 ชิ้นให้ห่างเท่ากันด้วย Distribute
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมต้อง Shift-คลิก?</summary>เพื่อเลือกหลายชิ้นเป็นชุด (set) ซึ่ง Align ต้องใช้อย่างน้อย 2 ชิ้น</details>
<details><summary>2. ช่องว่าง 4 mm ระหว่างฐานกับตัวบนมีไว้ทำไม?</summary>สำหรับสอดกระดาษ (ดีไซน์ต้องใช้งานได้จริง)</details>
<details><summary>3. เครื่องมือไหนทำได้ทั้งย้าย หมุน และ scale?</summary>Transform</details>

📚 อ้างอิง: R1 Align / Distribute, Transforming Objects, Transform · R19 [Transform tool](https://support.formz.com/hc/en-us/articles/28223037374995)
