---
title: "4. ขั้น 4 · เซฟแบบไม่มีวันหาย: Save Incremental"
parent: "M3 · ย้ายบ้านมา formZ ใน 4 ขั้น"
nav_order: 4
chapter: true
read_time: 2
do_time: 3
hook: "ตั้งนิสัยเซฟเป็นเวอร์ชัน v01, v02… ย้อนกลับได้เสมอ"
edition: free
permalink: /courses/m3-move-in/04-save-incremental/
---

# 4. ขั้น 4 · เซฟแบบไม่มีวันหาย: Save Incremental
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **File › Save Incremental** (ใหม่ใน formZ 10)
- รู้ว่าใช้ต่างจาก **Save A Copy As** อย่างไร

## 💡 ไอเดียสั้น ๆ
formZ **ไม่มี history tree** แบบ Shapr3D ดังนั้นวิธีย้อนกลับไปหาแบบเก่าที่ดีที่สุดคือ **เซฟเป็นเวอร์ชัน** ก่อนทำขั้นที่เสี่ยง (Boolean, Round)

## 👣 ลงมือทำ (3 นาที)
1. เซฟครั้งแรก: `remote.fmz`
2. ก่อน Boolean → **File › Save Incremental**
3. สังเกตชื่อไฟล์ใหม่ในโฟลเดอร์ 🔍
4. อยากส่งเพื่อนโดยไม่เปลี่ยนไฟล์ที่เปิดอยู่ → **Save A Copy As**

{: .shot }
[SCREENSHOT: โฟลเดอร์ที่มีไฟล์หลายเวอร์ชัน]

{: .verify }
รูปแบบชื่อไฟล์ที่ Save Incremental สร้าง (เช่น `_001` หรือ `-2`) ใน 10.1.x

{: .shapr }
Shapr3D มี history ใน Parametric mode แต่ formZ ใช้การเซฟเวอร์ชันแทน

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำงานชิ้นเดียวให้ได้ 5 เวอร์ชัน แล้วเปิดเวอร์ชัน 2 กลับมา
</div>

## ✅ เช็คตัวเอง
<details><summary>1. formZ มี history tree ไหม?</summary>ไม่มี ให้ใช้ Save Incremental</details>
<details><summary>2. Save A Copy As ต่างอย่างไร?</summary>เซฟสำเนาโดยไฟล์ที่เปิดอยู่ยังเป็นไฟล์เดิม</details>

📚 อ้างอิง: R1 File menu: Save Incremental, Save A Copy As
