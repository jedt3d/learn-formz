---
title: "3. เลือกให้เป็น: Pick + Reshape"
parent: "C2 · ฟอร์มสวยด้วย Solid"
nav_order: 3
chapter: true
read_time: 5
do_time: 3
permalink: /courses/c2-solid-form/03-pick-reshape/
---

# 3. เลือกให้เป็น: Pick + Reshape
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เลือกได้ทั้ง **ทั้งชิ้น / หน้า / เส้น / จุด** ด้วย **topological level**
- เข้าใจความต่างของ **prepick** กับ **postpick**
- แก้ฐานด้วยการดึงหน้าด้วย **Reshape**

## 💡 ไอเดียสั้น ๆ
ทุก solid ประกอบด้วย **จุด (point) → เส้น (segment) → หน้า (face) → วัตถุ (object)** formZ ให้เราเลือกได้ทุกระดับ ใน Tool Options ของ **Pick** มีไอคอนระดับให้เลือก (R1: Picking)

| ไอคอน | เลือกอะไร |
|---|---|
| **Auto Pick** (ซ้ายสุด) | ทั้งชิ้น ถ้ากด **Cmd** (Mac) / **Ctrl** (Win) ค้างไว้จะเลือกส่วนย่อยที่เมาส์ชี้อยู่ |
| Point / Segment / Segment Sequence / Outline / Face / Hole / Object | ล็อกให้เลือกเฉพาะระดับนั้น |

- **Prepick**: เลือกด้วย Pick ก่อน แล้วค่อยเลือกเครื่องมือ (ใช้กับหลายชิ้นพร้อมกัน)
- **Postpick**: เลือกเครื่องมือก่อน แล้วคลิกที่ชิ้นงาน (เร็วกว่าเมื่อทำทีละชิ้น)
- เมาส์ชี้ที่ไหน จะมีไฮไลต์สีแดงจาง ๆ ให้ดูก่อนว่าคลิกแล้วจะได้อะไร (**preview picking**)

## 👣 ลงมือทำ (3 นาที)
1. เลือก **Pick** แล้ววางเมาส์บนฐาน จะเห็นทั้งชิ้นเป็นสีแดงจาง
2. กด **Cmd/Ctrl ค้าง** แล้วชี้ที่หน้าด้านหน้าของฐาน ไฮไลต์จะเปลี่ยนเป็นหน้าเดียว คลิกเพื่อเลือก
3. ดู **Inspector** จะแสดงข้อมูลของหน้านั้น (Selection / Info)
4. เลือกเครื่องมือ **Reshape** แล้วคลิกหน้าเดิม ลากออกไป จากนั้นพิมพ์ **5** ใน Input palette ฐานจะยาวขึ้นเป็น 135 mm
5. **Undo** กลับเป็น 130 (ฐานเราใช้ 130 ตามของจริง)

{: .shot }
[SCREENSHOT: Pick Tool Options ที่ไอคอน topological level ทั้ง 8 ตัว พร้อมป้ายชื่อ]
{: .shot }
[SCREENSHOT: Reshape ระหว่างดึงหน้าด้านหน้าของฐาน]

{: .note }
ระหว่างใช้ Reshape ให้ดู **Action palette** ซึ่งจะบอกคีย์ลัดตามจังหวะ เช่น *Tap Shift* = สลับ Keep Edges, *Tap Command* = สลับ Perpendicular (R1: Prompts and Numeric Input)

{: .easy }
เหมือนการ Push/Pull หน้าใน SketchUp และ formZ ยังมีไฮไลต์ให้ดูก่อนคลิกว่าจะเลือกอะไร

{: .power }
SketchUp ต้องดับเบิลคลิกเข้าไปใน group ก่อนถึงจะแก้หน้าได้ ส่วน formZ เลือกได้ **ทุกระดับจากด้านนอก** และ Reshape ยังรักษาความเป็น solid ไว้ได้เสมอ

{: .shapr }
Shapr3D: แตะหน้าแล้วลาก arrow · formZ: **Reshape** (หน้าเรียบ) หรือเลือกหน้าแล้วใช้ Move

## ✅ เช็คตัวเอง
<details><summary>1. จะเลือกหน้าเดียวตอนใช้ Auto Pick ทำอย่างไร?</summary>กด Cmd/Ctrl ค้างไว้ขณะชี้และคลิก</details>
<details><summary>2. Prepick ต่างจาก postpick อย่างไร?</summary>prepick เลือกก่อนแล้วค่อยใช้เครื่องมือ ส่วน postpick ใช้เครื่องมือคลิกเลือกเอง</details>
<details><summary>3. Reshape ใช้กับหน้าแบบไหน?</summary>หน้าเรียบ (planar) เท่านั้น</details>

📚 อ้างอิง: R1 Picking, Prompts and Numeric Input (Reshape)
