---
title: "8. กด Render! ภาพแรกของเรา"
parent: "C1 · ปากกาเมจิกสวยใน 90 นาที"
nav_order: 8
chapter: true
read_time: 5
do_time: 8
permalink: /courses/c1-quick-win/08-render/
renderzone: true
hook: "เปิด RenderZone Options และตั้งค่าที่จำเป็นแค่ 4 อย่าง และเรนเดอร์ส่วนเล็ก ๆ เพื่อทดสอบก่อน ด้วย Render Area Rectangle"
---

# 8. กด Render! ภาพแรกของเรา
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เปิด **RenderZone Options** และตั้งค่าที่จำเป็นแค่ 4 อย่าง
- เรนเดอร์ส่วนเล็ก ๆ เพื่อทดสอบก่อน ด้วย **Render Area Rectangle**
- เรนเดอร์ภาพจริง เก็บไฟล์ และส่งการบ้าน 🎉

## 💡 ไอเดียสั้น ๆ
RenderZone อยู่ใน **Display** menu ข้าง ๆ โหมดการแสดงผลอื่น ชื่อในเมนูมีเครื่องหมาย * ต่อท้าย ถ้ากด **Option** (Mac) หรือ **Alt** (Windows) ค้างไว้ตอนคลิก จะเปิดหน้าต่าง **RenderZone Options** ซึ่งมี 5 แท็บ: **Shading, Global Illumination, Geometry, Scene, Postprocess** (R3)

**สูตรเรนเดอร์ของเรา (4 ค่า)**

| ที่ไหน | ตั้งค่า | ทำไม |
|---|---|---|
| ด้านบนของหน้าต่าง | **Rendering Type = Raytrace** | ได้เงาและเงาสะท้อนที่สมจริงที่สุด และใช้ CPU หลาย core |
| Shading tab | เปิด **Shadows** | ให้มีเงาใต้ปากกา |
| Global Illumination tab | เปิด **Use Ambient Occlusion** | เงานุ่มตามซอกตามมุม ทำให้ชิ้นงานดูมีน้ำหนัก |
| Scene tab | **Background** = สีเรียบ (ขาวหรือเทาอ่อน) | ฉากหลังสตูดิโอ (พื้น Catcher จะกลืนไปกับสีนี้) |

{: .warning }
**ไม่ต้องแตะแท็บ Postprocess** และเมนู RenderZone Postprocess ใน course นี้ มีรายงานในฟอรัม official ว่า formZ 10.1.5 บน Mac crash เมื่อเปิดหน้าต่าง Postprocessing

## 👣 ลงมือทำ (8 นาที)
1. เลือก view **Hero** ใน Views palette
2. **Option/Alt + คลิก Display > RenderZone** เพื่อเปิด **RenderZone Options**
3. ตั้ง 4 ค่าตามตารางด้านบน แล้วกด OK
4. **ทดสอบก่อน:** ใช้ **Display > Render Area Rectangle** ลากกรอบเล็ก ๆ รอบหัวปากกากับคลิป จะได้ภาพทดสอบภายในไม่กี่วินาที
5. ถ้าเงาเข้มเกินไป ให้เพิ่ม ambient light (บทที่ 7) หรือลด Shadow Intensity ของพื้น Catcher
6. ถ้าพลาสติกดูไม่เงา ให้กลับไปที่ `MK_Cap_Color` แล้วเพิ่มค่าการสะท้อน (reflection) เล็กน้อย
7. **เรนเดอร์จริง:** คลิก **Display > RenderZone** (ไม่ต้องกด Option/Alt)
8. เก็บภาพไว้ในโฟลเดอร์ `portfolio/` ตั้งชื่อ `C1_Marker_Hero.png`

{: .shot }
[SCREENSHOT: RenderZone Options > Shading tab ที่ Rendering Type = Raytrace และเปิด Shadows]

{: .shot }
[SCREENSHOT: Global Illumination tab ที่เลือก Use Ambient Occlusion]

{: .shot }
[SCREENSHOT: Scene tab > Background popup ที่เลือกสีเรียบ]

{: .shot }
[SCREENSHOT: ภาพเรนเดอร์สุดท้ายของปากกาเมจิก + ปลอก (ใช้เป็นตัวอย่างการบ้าน)]

{: .verify }
คู่มือ RenderZone ที่มีในโฟลเดอร์ v10 **เป็นเนื้อหาเดียวกับ v9 ทุกหัวข้อ** ให้ยืนยันชื่อแท็บและช่องต่าง ๆ บนหน้าจอจริง เช่น ช่องขนาดภาพ (image size) และวิธีบันทึกภาพ (คู่มือเขียนว่า RenderZone บันทึกภาพล่าสุดลงโฟลเดอร์ "RenderZone Images" ให้อัตโนมัติ และมีเอกสารเก่าที่อ้างถึง **File > Save Image**) ตรวจทั้งสองทางใน 10.1.x

## 🎁 เก็บฉากนี้ไว้ใช้ครั้งหน้า (ไม่บังคับ, 1 นาที)
เปิด `PD_mm_template.fmz` แล้ว **คัดลอก** `Floor` และ material `MK_Floor_Catcher` (เปลี่ยนชื่อเป็น `Studio_Floor_Catcher`) ไปวางในไฟล์นั้น ตั้งค่าแสงให้เหมือนบทที่ 7 แล้วบันทึก ครั้งหน้าที่เปิด New Project จะได้ **ฉากสตูดิโอพร้อมใช้** ทันที

{: .easy }
ไม่ต้องเปิดโปรแกรมอื่น ไม่ต้อง export ไฟล์ไปไหน เรนเดอร์ได้ในโปรแกรมเลย เหมือนกด Shaded แต่สวยกว่ามาก

{: .power }
SketchUp **ไม่มี renderer ในตัว** ต้องติดตั้งและเรียน V-Ray หรือ Enscape แยก ส่วน formZ มี RenderZone พร้อมทั้ง raytrace, ambient occlusion, Catcher shadow และ global illumination อยู่ในโปรแกรม

{: .shapr }
Shapr3D Visualization เน้นความง่ายแบบ preset ส่วน RenderZone ปรับได้ลึกกว่า แต่ใน course นี้เราใช้ **4 ค่าก็พอ**

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** render ปากกา 3 สีวางเรียงกันเป็นภาพ family shot
</div>

## ✅ เช็คตัวเอง
<details><summary>1. เปิด RenderZone Options อย่างไร?</summary>กด Option (Mac) หรือ Alt (Windows) ค้างไว้แล้วคลิก Display > RenderZone หรือใช้ปุ่ม RenderZone Options ใน Display Options</details>
<details><summary>2. ทำไมต้องเรนเดอร์ส่วนเล็กก่อน?</summary>เพื่อประหยัดเวลา ปรับแสงและวัสดุให้ลงตัวก่อนเรนเดอร์ภาพเต็ม</details>
<details><summary>3. แท็บไหนที่ไม่ควรใช้ใน course นี้?</summary>Postprocess</details>

## 🏁 ส่งการบ้าน C1
{% include homework.html id="c1-workshop" title="C1 · Marker Hero Shot" what="ภาพถ่ายปากกาจริงของเรา 1 ภาพ + ภาพเรนเดอร์ RenderZone 1 ภาพ + ภาพหน้าจอ formZ ที่เห็น Materials palette และ Objects palette" %}

**เกณฑ์ "เสร็จ" (เช็คเอง):**
- [ ] ขนาดตรงกับปากกาจริงที่วัดได้ (คลาดไม่เกิน 1 mm)
- [ ] ปลอกกลวงจริง มีคลิป และขอบมน
- [ ] มี material 3 แบบที่ดูต่างกันชัดเจน
- [ ] มีเงานุ่มใต้ปากกา และพื้นกลืนไปกับฉากหลัง
- [ ] ไฟล์ตั้งชื่อเป็นระเบียบ (`C1_...`)

🎉 **ยินดีด้วย!** ภาพนี้คือผลงานชิ้นแรกใน portfolio ของเรา ไปบทสรุปเพื่อดูภาพรวมทั้ง course กันเลย

📚 อ้างอิง: R3 RenderZone: Producing a rendered image, Selecting rendering type, Shading tab, Ambient Occlusion, Background · R1 Display Menu (Render Area Rectangle) · R22 [RenderZone tips](https://support.formz.com/hc/en-us/sections/28221057173395) · forum [10.1.5 Postprocess crash](https://forums.formz.com/topic/10534-formz-pro-1015-mac-m1-pro-max-%E2%80%93-crashes-at-once-when-try-to-change-renderzone-postprocessed-rendering-effects/)
