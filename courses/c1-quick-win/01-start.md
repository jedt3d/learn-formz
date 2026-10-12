---
title: "1. เริ่มต้น 5 นาที: หน้าจอ + Assistant"
parent: "C1 · ปากกาเมจิกสวยใน 90 นาที"
nav_order: 1
chapter: true
read_time: 5
do_time: 5
permalink: /courses/c1-quick-win/01-start/
hook: "เปิดโปรเจกต์ใหม่และรู้ว่า เวอร์ชัน formZ บนเครื่องเราคือเวอร์ชันไหน และชี้ได้ว่า 6 ส่วนหลักของหน้าจออยู่ตรงไหน"
---

# 1. เริ่มต้น 5 นาที: หน้าจอ + Assistant
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เปิดโปรเจกต์ใหม่และรู้ว่า **เวอร์ชัน formZ** บนเครื่องเราคือเวอร์ชันไหน
- ชี้ได้ว่า 6 ส่วนหลักของหน้าจออยู่ตรงไหน
- ใช้ **Assistant** หาเครื่องมือได้ด้วยการพิมพ์ ไม่ต้องจำไอคอน

## 💡 ไอเดียสั้น ๆ
หน้าจอแรกของ formZ อาจดูมีปุ่มเยอะกว่า SketchUp แต่ทุกอย่างทำงานตาม **จังหวะเดียวกันเสมอ**:

> **เลือกเครื่องมือ → ตั้งค่าใน Tool Options → คลิกในหน้าต่าง → ดูผล (สีส้ม = ยังแก้ได้)**

เมื่อจำจังหวะนี้ได้ ไอคอนจะเยอะแค่ไหนก็ไม่น่ากลัวแล้ว ผลลัพธ์ที่เป็น **สีส้ม** คือช่วงที่ formZ เรียกว่า result ซึ่งยังเปลี่ยนตัวเลือกได้ทันทีโดยไม่ต้องทำใหม่ (อ้างอิง R1: Layout and Interface)

## 📍 6 ส่วนของหน้าจอ

| # | ส่วน (ชื่อ official) | อยู่ตรงไหน | เอาไว้ทำอะไร |
|---|---|---|---|
| 1 | **Modeling tool palette** | ซ้าย | เครื่องมือปั้นทั้งหมด จัดเป็นแถว (suite) ชี้ที่ไอคอนแล้วเครื่องมืออื่นในกลุ่มเดียวกันจะเด้งออกมา |
| 2 | **Tool Options palette** | ขวา | ตัวเลือกของเครื่องมือที่กำลังใช้ |
| 3 | **Action palette** + **Input palette** | ซ้ายบน | บอกว่าคลิกถัดไปจะเกิดอะไร และใช้พิมพ์ตัวเลขพิกัดหรือขนาด |
| 4 | **Display Tools** / **Navigation tool palette** | ด้านบน | โหมดการแสดงผล และการหมุน/ซูมมุมมอง |
| 5 | **Reference Plane tool palette** + **Snap tool palette** | ด้านล่าง | ระนาบที่ใช้วาด, กริด, snap |
| 6 | **Palette dock** (Materials, Objects, Layers, Lights, Views ...) + **Inspector** | ขวา | จัดการข้อมูลในโปรเจกต์ และดู/แก้ค่าของสิ่งที่เลือก |

{: .shot }
[SCREENSHOT: หน้าจอ formZ 10.1.x ทั้งจอ ตอนเปิด New Project พร้อมป้ายตัวเลข 1–6 ตามตารางด้านบน (ใช้ workspace "Modeling")]

## 👣 ลงมือทำ (5 นาที)
1. เปิด formZ แล้วเลือก **File > New Project** (ถ้าโปรแกรมยังไม่เปิดหน้าใหม่ให้เอง)
2. เช็คเวอร์ชัน: **Help > Check for Update** แล้วจดเลขเวอร์ชันไว้ (เช่น 10.1.5)
3. ตรวจว่าใช้ workspace มาตรฐาน: **Workspace > Modeling**
4. กด **spacebar** จะมี **Favorites palette** โผล่ขึ้นมา ให้พิมพ์ `cyl` เพื่อหา **Cylinder** แล้วกด Enter
5. ลองพิมพ์ `round` และ `union` ดูว่าเจอเครื่องมืออะไรบ้าง
6. ทางลัด: กด **Option + spacebar** (Mac) เพื่อเปิด **Assistant** ได้ทันที

{: .verify }
คู่มือระบุคีย์ลัดของ Assistant เป็น Option+spacebar (Mac) แต่ยังไม่พบคีย์ที่ใช้บน Windows (คาดว่าเป็น Alt+spacebar) ให้ยืนยันบนเครื่องจริง ตำแหน่งของคำสั่ง **Check for Update** อ้างจากโพสต์ของ moderator ในฟอรัม official ส่วนเมนู About ยังไม่ได้ยืนยัน

{: .shot }
[SCREENSHOT: Assistant ตอนพิมพ์ "cyl" และมี Cylinder อยู่บนสุดของรายการ]

## Assistant: ผู้ช่วยสำหรับคนที่ยังจำชื่อเครื่องมือไม่ได้
Assistant ค้นหาได้ทั้ง **เครื่องมือ, คำสั่งในเมนู, layer, material, view** และค้นได้แม้พิมพ์ไม่ตรงชื่อ เช่น พิมพ์ `pipe` ก็จะเจอเครื่องมือกลุ่ม Sweep (R8: New Features)

| พิมพ์ | ได้อะไร |
|---|---|
| `m ` ตามด้วยชื่อ | หา material แล้วคลิกเพื่อตั้งเป็น material ที่ active |
| `l ` ตามด้วยชื่อ | หา layer |
| `o ` ตามด้วยชื่อ | หา object |
| `v ` ตามด้วยชื่อ | หา view ที่บันทึกไว้ |
| Shift + คลิกผลลัพธ์ | เปิดหน้าคู่มือของเครื่องมือนั้น |

{: .easy }
Assistant ทำงานคล้ายช่อง **Search** ของ SketchUp ไม่ต้องรู้ว่าเครื่องมืออยู่ในแถวไหน แค่พิมพ์ชื่อ และ Assistant ยังจำได้ว่าเราเลือกอะไรบ่อย ครั้งต่อไปจะขึ้นมาเป็นอันดับแรก

{: .shapr }
Shapr3D แทบไม่มีแผงตัวเลือก เพราะตัวเลือกจะโผล่ใกล้ ๆ เคอร์เซอร์ ส่วนใน formZ ตัวเลือกจะอยู่ใน **Tool Options palette** ด้านขวาเสมอ ให้ฝึก **มองขวาก่อนคลิก** ทุกครั้ง

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** เปิด formZ แล้วหาเครื่องมือ Cylinder ให้เจอภายใน 10 วินาทีโดยใช้ Assistant แข่งกับเพื่อน
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ผลลัพธ์ที่เป็นสีส้มหมายถึงอะไร?</summary>ผลลัพธ์ที่ยังแก้ตัวเลือกใน Tool Options ได้ทันที โดยไม่ต้องสั่งเครื่องมือใหม่</details>
<details><summary>2. ถ้าจำไม่ได้ว่าเครื่องมืออยู่แถวไหน ทำอย่างไร?</summary>กด spacebar หรือ Option+spacebar แล้วพิมพ์ชื่อหรือคำใกล้เคียงใน Assistant</details>
<details><summary>3. ตัวเลือกของเครื่องมืออยู่ที่ไหน?</summary>Tool Options palette ด้านขวาของหน้าต่าง</details>

{: .warning }
ถ้าไอคอนบางตัวหายไปหลังอัปเดต (มีรายงานใน 10.1) ให้ใช้ **Workspace > Reset Workspace**

📚 อ้างอิง: R1 Layout and Interface · R8 New Features (Assistant) · [Fundamentals Video: Interface Tour](https://support.formz.com/hc/en-us/articles/28596825311763)
