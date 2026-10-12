---
title: "1. ปากกาเมจิก 0 → render ใน 10 นาที"
parent: "C0 · เริ่มตรงนี้! formZ ใน 10 นาที"
nav_order: 1
chapter: true
read_time: 3
do_time: 7
hook: "ปั้นปากกาเมจิก 2 ชิ้น ใส่สี 2 แบบ แล้วกด render ภาพแรกของชีวิตใน formZ"
renderzone: true
permalink: /courses/c0-start-here/01-ten-minutes/
---

# 1. ปากกาเมจิก 0 → render ใน 10 นาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ปั้นปากกาเมจิกด้วย **Cylinder** 2 ชิ้น + ขอบมนด้วย **Controlled Round**
- ใส่วัสดุด้วยการลากจาก **Materials palette**
- กด **RenderZone** แล้วได้ภาพแรก 🎉

## ⏱ 10 นาที 6 ขั้น

| นาที | ทำ |
|---|---|
| 0–1 | เปิด `C0_start.fmz` (หน่วย mm, พื้น, ไฟ, กล้อง hero ตั้งไว้แล้ว) |
| 1–3 | **Cylinder** ด้าม: Radius **8** · Height **110** ที่จุด (0,0,0) |
| 3–4 | **Cylinder** ปลอก: Radius **9** · Height **45** วางต่อด้านบน (Snap to Center) |
| 4–6 | **Controlled Round** ขอบบนของปลอก **2 mm** และขอบล่างของด้าม **1 mm** |
| 6–8 | ลาก material `Matte White` ไปใส่ด้าม และ `Glossy Red` ไปใส่ปลอก |
| 8–10 | เลือก view **Hero** ใน Views palette → render ด้วย **RenderZone** (ไม่ต้องเปิด Postprocess) |

{: .shot }
[SCREENSHOT: ปากกา 2 ชิ้นใน Shaded ก่อนใส่วัสดุ]
{: .shot }
[SCREENSHOT: ภาพ render สุดท้ายของปากกาสีแดง-ขาว]

{: .easy }
6 ขั้นนี้ **ไม่ยากกว่า SketchUp เลย** และต่างกันตรงที่เราได้ render สวย ๆ โดยไม่ต้องลง plugin render เพิ่ม (RenderZone เป็น plugin ของ formZ เอง)

{: .warning }
อย่าเปิด **Postprocess** ของ RenderZone เพราะมีรายงานว่าทำให้ 10.1.5 ค้าง

{: .verify }
- ชื่อ material ในไฟล์ start (Matte White, Glossy Red) จะตั้งตอนทำไฟล์ `C0_start.fmz`
- ปุ่ม/คำสั่ง render ที่เร็วที่สุดใน 10.1.x (ดูภาพหน้าจอ C1 บท 8)

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำปากกาสีที่ 2 โดย copy ทั้งด้ามแล้วเปลี่ยนสีปลอก จากนั้น render คู่กัน
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ใช้เครื่องมืออะไรทำขอบมน?</summary>Controlled Round</details>
<details><summary>2. ใส่วัสดุอย่างไร?</summary>ลากจาก Materials palette ไปวางบน object</details>
<details><summary>3. ตอน render ห้ามเปิดอะไร?</summary>Postprocess</details>

➡️ อยากรู้ว่าแต่ละขั้นทำอะไร? ไปต่อที่ [C1 บท 4]({{ '/courses/c1-quick-win/04-body/' | relative_url }}) ซึ่งสอนแบบละเอียดพร้อมวัดปากกาจริง

📚 อ้างอิง: R1 Cylinder, Controlled Round · R2 RenderZone
