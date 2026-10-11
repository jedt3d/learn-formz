---
title: "6. Texture: ขนมปังกับเขียงไม้"
parent: "C4 · RenderZone ระดับสตูดิโอ"
nav_order: 6
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c4-renderzone-studio/06-texture/
---

# 6. Texture: ขนมปังกับเขียงไม้
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใช้ภาพถ่ายเป็นสีของวัสดุด้วย **Color Map**
- เลือกวิธีห่อภาพด้วย **Map Texture** (Mapping Type)
- เลื่อน หมุน และย่อขยายลายด้วย **Edit Texture**

## 💡 ไอเดียสั้น ๆ
**ขนมปังที่โผล่ขึ้นมาจากช่อง** กับ **เขียงไม้** ช่วยเล่าเรื่องว่าเป็นเครื่องปิ้งขนมปังในครัวจริง (product storytelling) ซึ่งต้องใช้ **ภาพ texture**

| เครื่องมือ | ทำอะไร |
|---|---|
| Color shader = **Color Map** | ใช้ภาพเป็นสี (ตั้ง Repetitions และ Infinite ได้) |
| **Map Texture** | เลือก Mapping Type (เช่น flat, cylindrical, spherical ฯลฯ) ให้วัตถุหรือหน้า |
| **Edit Texture** | ลากตำแหน่ง ขนาด และมุมของลายบนจอ (Edit On Face) |

ก่อนเริ่ม ให้เปิด **Textures** ใน Display Options ของ Shaded Work/Full จะเห็นลายบนจอ (R1: Map Texture)

## 👣 ลงมือทำ (4 นาที)
1. **ขนมปัง:** Cube 110 × 20 × 110 → **Subdivision / Soften** Distance 8 → วางในช่องแรก โผล่ขึ้นมาประมาณ 40 mm
2. ถ่ายภาพผิวขนมปังจริง (หรือหาภาพที่ใช้ได้ฟรี) แล้วทำ material `TS_Bread` · Color = **Color Map** · Bump = **Bumps from images** (ภาพเดียวกัน, ค่าต่ำ)
3. **เขียง:** Cube 400 × 260 × 18 + Controlled Round R6 วางใต้เครื่อง material `TS_Wood` (Color Map ภาพลายไม้ หรือ procedural wood)
4. **Map Texture** คลิกเขียง แล้วเลือก Mapping Type แบบ flat/planar
5. **Edit Texture** คลิกหน้าบนของเขียง แล้วหมุนลายไม้ให้วิ่ง **ตามแนวยาว**

{: .shot }
[SCREENSHOT: Color Map Options (Repetitions / Infinite)]
{: .shot }
[SCREENSHOT: Edit Texture controls บนหน้าเขียง]

{: .verify }
ชื่อ Mapping Type ในเมนูของ Map Texture v10 ต้องยืนยัน (คู่มือมีเมนูนี้ แต่ไม่ได้ระบุรายการไว้ในข้อความ)

{: .warning }
ภาพจากอินเทอร์เน็ตต้องเป็นภาพที่ **อนุญาตให้ใช้ฟรี** (เช่น CC0) ถ้าไม่แน่ใจ ให้ถ่ายเอง ซึ่งเป็นนิสัยที่ดีของนักออกแบบ

{: .easy }
การหมุนลายด้วย Edit Texture ทำงานเหมือน Position Texture ใน SketchUp

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมลายไม่ขึ้นบนจอ?</summary>ยังไม่ได้เปิด Textures ใน Display Options</details>
<details><summary>2. อยากหมุนลายไม้ใช้เครื่องมืออะไร?</summary>Edit Texture</details>
<details><summary>3. ใช้ภาพเดียวกันทำ bump ได้ไหม?</summary>ได้ ด้วย Bumps from images (ตั้งค่าต่ำ)</details>

📚 อ้างอิง: R1 Map Texture, Edit Texture · R3 Color Image Maps, Bumps from images
