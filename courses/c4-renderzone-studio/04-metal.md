---
title: "4. โลหะ 2 แบบ: โครเมียมเงา vs สแตนเลสขัดลาย"
parent: "C4 · ถ่ายสินค้าแบบสตูดิโอ: เครื่องปิ้งขนมปัง 3 มุม"
nav_order: 4
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c4-renderzone-studio/04-metal/
hook: "ทำ โครเมียม (เงาเหมือนกระจก) และ สแตนเลสขัดด้าน และใช้ shader Metal, Accurate (มี Fresnel) และ Mirror"
---

# 4. โลหะ 2 แบบ: โครเมียมเงา vs สแตนเลสขัดลาย
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **โครเมียม** (เงาเหมือนกระจก) และ **สแตนเลสขัดด้าน**
- ใช้ shader **Metal, Accurate** (มี Fresnel) และ **Mirror**
- เข้าใจว่า **โลหะสวยเพราะมีสิ่งให้สะท้อน**

## 💡 ไอเดียสั้น ๆ
โลหะ **ไม่มีสีของตัวเอง** มากนัก สิ่งที่เราเห็นคือ **ภาพสะท้อนรอบตัว** ถ้าฉากว่าง โลหะจะดูดำ บทที่ 8–9 จะเติมแสงและสิ่งแวดล้อมให้สะท้อน

| วัสดุ | Reflection | ไอเดีย |
|---|---|---|
| `TS_Chrome` (ลูกบิด, คันโยก) | **Metal, Accurate** (หรือ Mirror) | เงาสูงสุด สีเทาอ่อน |
| `TS_Steel_Brushed` (แผ่นข้าง) | Metal, Accurate + เบลอ (ถ้ามีค่าให้ปรับ) + **Bump** ลายเส้นละเอียด | ขัดด้านเป็นเส้น |

shader **Metal, Accurate** และ **Glass, Accurate** ใช้การคำนวณแบบ **Fresnel** คือมุมยิ่งเฉียง ยิ่งสะท้อนมาก ได้ผลสมจริงแต่ใช้เวลาคำนวณมากขึ้น (R3: Ray-Traced Reflections)

## 👣 ลงมือทำ (4 นาที)
1. สร้าง `TS_Chrome`: Material Type = RenderZone · Reflection = **Metal, Accurate** · Color เป็นเทาอ่อน
2. ลากไปวางที่ `Knob` และ `Lever`
3. สร้าง `TS_Steel_Brushed`: Reflection = Metal, Accurate · Bump เลือก shader ลายเส้นหรือ noise ละเอียด แล้วปรับ amplitude ให้ต่ำ
4. **Render Area Rectangle** รอบลูกบิด เพื่อทดสอบ (ยังดูดำ ๆ ได้ เพราะยังไม่มีฉาก)

{: .shot }
[SCREENSHOT: Metal, Accurate Options dialog]
{: .shot }
[SCREENSHOT: ภาพทดสอบลูกบิดโครเมียม (ก่อนจัดแสง)]

{: .verify }
ชื่อ bump shader ที่เหมาะกับ "brushed" ในรายการของ v10 ยังไม่ได้ยืนยัน ให้ลองดูในหมวด wrapped/solid procedural แล้วบันทึกชื่อที่ใช้ได้

{: .warning }
อย่าใส่ **Transparency** ให้วัสดุที่ใช้ Glass shader ซ้ำ เพราะความโปร่งใสถูกควบคุมใน Glass แล้ว ถ้าใส่ซ้ำจะเรนเดอร์ช้ามาก (R22: RenderZone Efficiency)

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำโลหะสีทองจาก material โครเมียม
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมโลหะในฉากว่างดูดำ?</summary>เพราะไม่มีอะไรให้สะท้อน</details>
<details><summary>2. Fresnel คืออะไร?</summary>การสะท้อนที่เพิ่มขึ้นเมื่อมองผิวในมุมเฉียง</details>
<details><summary>3. สแตนเลสขัดด้านต่างจากโครเมียมที่ชั้นไหน?</summary>Bump (ลายเส้นละเอียด) และความเบลอของการสะท้อน</details>

📚 อ้างอิง: R3 Ray-Traced Reflections, Bump shaders · R22 RenderZone Efficiency
