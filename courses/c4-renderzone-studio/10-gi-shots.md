---
title: "10. GI + ภาพชุด 3 มุม"
parent: "C4 · RenderZone ระดับสตูดิโอ"
nav_order: 10
chapter: true
read_time: 5
do_time: 6
permalink: /courses/c4-renderzone-studio/10-gi-shots/
---

# 10. GI + ภาพชุด 3 มุม
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เปิด **Ambient Occlusion** + **Final Gather** ให้แสงสะท้อนในฉากสมจริง
- คุมเวลาเรนเดอร์ด้วยการทดสอบเป็นขั้น
- ได้ **ภาพชุด 3 มุม** (Hero · Side · Detail) ลง portfolio

## 💡 ไอเดียสั้น ๆ
**Ambient Occlusion** ทำเงามืดตามซอกมุม (เร็ว) ส่วน **Final Gather** คำนวณ **แสงสะท้อนต่อ** (indirect light) ภาพรวมจะดูมีมิติ คู่มือแนะนำให้ใช้ทั้งสองอย่างคู่กันในภาพจริง เพราะคำนวณข้อมูลที่เสริมกัน (R3: When To Use Final Gather)

| ขั้นทดสอบ | ตั้งค่า | ใช้เมื่อ |
|---|---|---|
| ① ร่าง | ภาพเล็ก 800 px · ไม่มี GI | จัดกล้องและแสง |
| ② ตรวจ | Render Area Rectangle + GI | ดูวัสดุใกล้ ๆ |
| ③ จริง | 1920 px + AO + Final Gather | ภาพสุดท้าย |

## 👣 ลงมือทำ (6 นาที)
1. **RenderZone Options > Global Illumination tab** เปิด **Ambient Occlusion** และ **Final Gather** โดยใช้ค่า quality เริ่มต้นก่อน
2. บันทึก 3 views ใน **Views** palette:
   - `Hero`: เฉียงหน้า กล้องต่ำ
   - `Side`: ด้านข้าง เห็นคันโยกและลูกบิด
   - `Detail`: ซูมเข้าไปที่ลูกบิดกับโลโก้
3. เรนเดอร์ขั้น ① ทั้ง 3 มุม แล้วปรับแสง จากนั้นทำขั้น ③
4. บันทึก `C4_Toaster_Hero.png`, `_Side.png`, `_Detail.png`

{: .shot }
[SCREENSHOT: Global Illumination tab ที่เปิด Ambient Occlusion + Final Gather]
{: .shot }
[SCREENSHOT: ภาพชุด 3 มุม (Hero / Side / Detail)]

{: .warning }
**อย่าใช้ Postprocess** (เช่น Depth Blurring หรือ Lens Flares) ใน 10.1.5 มีรายงานว่าทำโปรแกรม crash ถ้าอยากได้ฉากหลังเบลอ ให้ไปทำในโปรแกรมแต่งภาพภายหลัง

{: .verify }
ชื่อแท็บและค่า quality ของ Final Gather ใน v10 ต้องยืนยัน (ในคู่มือ RZ แยกเป็น Ambient Occlusion tab และ Final Gather tab)

{% include homework.html id="c4-workshop" title="C4 · Toaster 3 Shots" what="ภาพเรนเดอร์ 3 มุม (Hero / Side / Detail) + ภาพหน้าจอ Materials palette ที่เห็น material ทั้งหมด" %}

📚 อ้างอิง: R3 Ambient Occlusion, Final Gather, Postprocessed Rendering Effects · R22
