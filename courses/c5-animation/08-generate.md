---
title: "8. กด Generate ได้ MP4 15 วินาที"
parent: "C5 · วิดีโอสินค้า 15 วินาที: แม็กเย็บขยับได้"
nav_order: 8
chapter: true
read_time: 5
do_time: 8
permalink: /courses/c5-animation/08-generate/
hook: "ใช้ Display > Generate Animation... เรนเดอร์ทุกเฟรม และเลือก Display Type ให้เหมาะกับเวลาที่มี"
---

# 8. กด Generate ได้ MP4 15 วินาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ **Display > Generate Animation...** เรนเดอร์ทุกเฟรม
- เลือก **Display Type** ให้เหมาะกับเวลาที่มี
- เลือก **Store Frames In**: เป็นไฟล์วิดีโอ หรือเป็นภาพทีละเฟรม

## 💡 ไอเดียสั้น ๆ
**คำนวณเวลาก่อนกดปุ่มเสมอ** ถ้าเรนเดอร์ภาพละ 20 วินาที × 300 เฟรม = **100 นาที** แต่ถ้าใช้ Shaded Full อาจใช้แค่ไม่กี่นาที

| Display Type | เวลา/เฟรม | เหมาะกับ |
|---|---|---|
| **Shaded Full** | เร็วมาก (ใช้การ์ดจอ) | ตรวจจังหวะ, ส่งงานด่วน |
| **RenderZone** (ไม่มี GI) | ปานกลาง | วิดีโอลง portfolio |
| RenderZone + GI | ช้ามาก | งานจริงที่มีเวลาเรนเดอร์ข้ามคืน |

| Store Frames In | ผล |
|---|---|
| **Animation File** | ไฟล์เดียว · Format: form•Z Animation (.fan), **QuickTime Movie** (และ AVI บน Windows) |
| ภาพแยกเฟรม | ไฟล์ภาพทีละเฟรม เอาไปต่อในโปรแกรมตัดต่อ ถ้าเรนเดอร์ค้างกลางทาง ก็ไม่เสียภาพที่เสร็จแล้ว |

## 👣 ลงมือทำ (8 นาที รวมเวลารอ)
1. ตั้งขนาดภาพ **1280 × 720** (HD) ให้ไฟล์เล็กและเรนเดอร์เร็ว
2. **Display > Generate Animation...** → Display Type **Shaded Full** ก่อน (ทดสอบ)
3. Store Frames In = **Animation File** → Format **QuickTime Movie** (ใส่ชื่อ `C5_Stapler.mov`)
4. กด Generate แล้วอย่าเอาหน้าต่างหรือ palette อื่นมาบังหน้าต่าง formZ (Shaded ต้องจับภาพจากการ์ดจอ)
5. ถ้าเวลาเหลือ: ทำซ้ำด้วย **RenderZone** แบบ Store เป็นภาพแยกเฟรม

{: .shot }
[SCREENSHOT: Animation Generation dialog (Display Type / Store Frames In / Format)]

{: .warning }
อย่าเปิด **Postprocess** ในวิดีโอ (ทำให้ crash ใน 10.1.5 และเพิ่มเวลาทุกเฟรม)

{: .verify }
ชื่อตัวเลือก "ภาพแยกเฟรม" ใน Store Frames In และรูปแบบวิดีโอที่ v10 รองรับ (เช่น ยังมี QuickTime บน macOS รุ่นใหม่หรือไม่) ต้องยืนยัน

{% include homework.html id="c5-workshop" title="C5 · Stapler Animation" what="ไฟล์วิดีโอ (หรือ GIF) ยาว ~10 วินาที + ภาพหน้าจอ Animation Time Line ที่เห็น key ทั้งหมด" %}

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** export วิดีโอแนวตั้ง 9:16 สำหรับโพสต์ลงโซเชียล
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ภาพละ 20 วินาที 300 เฟรม ใช้เวลาเท่าไร?</summary>6,000 วินาที = 100 นาที</details>
<details><summary>2. ทำไมการเก็บเป็นภาพแยกเฟรมจึงปลอดภัยกว่า?</summary>ถ้าค้างกลางทาง ภาพที่เสร็จแล้วยังอยู่ เรนเดอร์ต่อได้</details>
<details><summary>3. ทำไมห้ามบังหน้าต่างตอนใช้ Shaded?</summary>เพราะ formZ จับภาพจากการ์ดจอ ถ้ามีอะไรบังจะติดไปในภาพ</details>

📚 อ้างอิง: R5 Generating and Saving Animations
