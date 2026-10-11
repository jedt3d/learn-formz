---
title: "5. ปั้นฟอร์ม: Symmetry + Edit tools"
parent: "C9 · Capstone: ของจากบ้านตั้งแต่ต้นจนจบ"
nav_order: 5
chapter: true
read_time: 4
do_time: 6
track: "🎨 Designer + 📐 Engineering"
permalink: /courses/c9-capstone/05-shape/
---

# 5. ปั้นฟอร์ม: Symmetry + Edit tools
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ใส่ **Object Symmetry** ให้แก้ข้างเดียวแล้วอีกข้างตามด้วย
- ใช้ **Subdivision / Squeeze**, **Stretch**, **Offset Face** ปั้นรายละเอียดของฟอร์ม
- ใช้ **Sharpness** ทำขอบล่างให้คม

## 💡 ไอเดียสั้น ๆ
| Tool | ทำอะไร | ใช้กับเมาส์ |
|---|---|---|
| **Object Symmetry** | หลังจากใส่แล้ว การแก้ไขต่อจากนั้นจะคงความสมมาตร (Sub-D ถูกจัดการเป็นพิเศษ) | แกนกลางเมาส์ |
| **Squeeze** | ขยาย/หด edge หรือ sequence | คอดเอวให้นิ้วโป้งจับ |
| **Stretch** | ดัน face ออกตั้งฉาก (ไม่เพิ่ม face) | ป่องท้ายรับอุ้งมือ |
| **Offset Face** | สร้าง face ซ้อนเข้าด้านใน | ขอบฐานเรียบ |
| **Sharpness** | ขอบคมขึ้นโดยไม่เพิ่ม face | ขอบล่างแบน |

## 👣 ลงมือทำ (6 นาที)
1. **Object Symmetry** → คลิกเมาส์ แล้ววาง plane ที่แกนกลาง (y = 0)
2. **Squeeze**: เลือก sequence ด้านข้างตรงกลาง → Distance **−2** (คอดเอว)
3. **Stretch**: เลือก face ท้ายบน → Distance **3** (ป่อง)
4. เลือก edge รอบฐาน → **Sharpness** ~70% ให้ฐานแบนคม
5. หมุนดูทุกมุม แล้ว **ลองจับจริง**: พิมพ์ภาพด้านข้าง 1:1 แล้ววางมือเทียบ
6. **Save As** `C9_v02_shape`

{: .shot }
[SCREENSHOT: Object Symmetry plane บนเมาส์]
{: .shot }
[SCREENSHOT: ก่อน/หลัง Squeeze + Stretch]

{: .verify }
Object Symmetry กับ Subdivision edit tools (Squeeze/Stretch) ยังคงความสมมาตรระหว่างแก้ไขจริงไหม และ Sharpness ใช้กับ edge ที่เลือกหรือทั้ง object ต้องยืนยันใน v10

## ✅ เช็คตัวเอง
<details><summary>1. Squeeze ใช้ทำอะไร?</summary>ขยายหรือหด edge หรือ sequence ของ edge</details>
<details><summary>2. Stretch เพิ่ม face ไหม?</summary>ไม่เพิ่ม</details>
<details><summary>3. ทำไมต้องลองจับจริง?</summary>ergonomics ดูจากหน้าจออย่างเดียวไม่ได้</details>

📚 อ้างอิง: R1 Symmetry, Subdivision / Squeeze, Stretch, Offset Face, Subdivision / Create (Sharpness)
