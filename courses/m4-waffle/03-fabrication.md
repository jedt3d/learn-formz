---
title: "3. วางแผ่นลง XY + ส่งไฟล์ตัด"
parent: "M4 · ขาตั้งมือถือ Waffle: ตัดเลเซอร์ใน 30 นาที"
nav_order: 3
chapter: true
read_time: 3
do_time: 7
hook: "วางซี่ทุกชิ้นลงพื้นอัตโนมัติ แล้ว export DXF ไปเครื่องเลเซอร์"
edition: pro
track: "📐 Engineering"
permalink: /courses/m4-waffle/03-fabrication/
---

# 3. วางแผ่นลง XY + ส่งไฟล์ตัด
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เปิด **Create Objects for Fabrication** + **Distance Between Objects**
- Export เส้นขอบเป็น **DXF** (หรือรูปแบบที่เครื่องตัดรับ)

## 💡 ไอเดียสั้น ๆ
Create Objects for Fabrication วาง **สำเนาซี่ลงบน XY Plane** เรียงตามแกน X และวางซี่ V เยื้องในแกน Y ทำให้เป็นไฟล์ตัดได้เลย (manual)

## 👣 ลงมือทำ (7 นาที)
1. แก้ Waffle เดิม: เปิด **Create Objects for Fabrication** · Distance Between Objects **5**
2. ใช้มุมมอง Top: ตรวจว่าทุกชิ้นอยู่ในกรอบแผ่นไม้ (ใช้ Rectangle 300 × 200 เป็นกรอบ)
3. ใส่ **Text** เลขชิ้น U1–U6, V1–V3 (ใช้เป็นเส้นแกะ ไม่ตัดทะลุ)
4. **File › Export** → **DXF** เฉพาะชิ้นที่วางบน XY 🔍 ตัวเลือก export
5. ส่งให้ครู FabLab / ตัดชิ้นทดสอบก่อน → ประกอบ

{: .shot }
[SCREENSHOT: ซี่ทุกชิ้นเรียงบน XY ในกรอบ 300 × 200]

{: .shot }
[SCREENSHOT: DXF เปิดในโปรแกรมของเครื่องเลเซอร์]

{: .verify }
ตัวเลือกใน DXF export ของ 10.1.x (เวอร์ชัน DXF, หน่วย mm) และการแยกเส้นตัด/เส้นแกะตามสี ขึ้นกับเครื่องตัดของโรงเรียน

{: .warning }
ห้ามเปิดเครื่องตัดเลเซอร์เองโดยไม่มีครูหรือเจ้าหน้าที่ดูแล

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** จัดวางชิ้นใหม่ให้ใช้แผ่นไม้น้อยลง 20%
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ชิ้นสำหรับตัดถูกวางที่ไหน?</summary>บน XY Plane เรียงตามแกน X ส่วนซี่ V เยื้องในแกน Y</details>
<details><summary>2. ไฟล์ตัดเลเซอร์ใช้อะไร?</summary>DXF หรือรูปแบบที่เครื่องรับ</details>

📚 อ้างอิง: Manual: Waffle › Fabrication Guide, DXF Export
