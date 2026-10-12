---
title: "5. ภาพ hero ใหญ่ 50%: Place Image"
parent: "C6 · บอร์ดขายไอเดีย A3 แผ่นเดียว"
nav_order: 5
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c6-layout-boards/05-images/
hook: "วางภาพเรนเดอร์ด้วย Place Image และ Place Image Fit และcrop ภาพด้วย controls 9 จุด"
---

# 5. ภาพ hero ใหญ่ 50%: Place Image
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- วางภาพเรนเดอร์ด้วย **Place Image** และ **Place Image Fit**
- **crop** ภาพด้วย controls 9 จุด
- รู้ว่าภาพบน layout **ลิงก์กับไฟล์** เรนเดอร์ใหม่แล้วอัปเดตได้

## 💡 ไอเดียสั้น ๆ

| เครื่องมือ | เหมาะกับ |
|---|---|
| **Place Image** | วางตามจุดคลิก ตั้ง **By Dimensions** หรือ **By Scale** และเลือก Cursor Position ได้ 9 จุด |
| **Place Image Fit** | ลากกรอบ 2 คลิก แล้วภาพยืดให้พอดีกรอบ |

หลังวางแล้ว ถ้าเปิด **Show Controls** ภาพจะมีจุดควบคุม 9 จุด: ลากขอบ = **crop** · กด **Cmd/Ctrl** + ลาก = **ยืด** · กด **Shift** = รักษาสัดส่วน (R1: Layout)

## 👣 ลงมือทำ (4 นาที)
1. ทำให้แผ่น `01_Hero` active
2. **Place Image** → ไอคอน Open → `C6_Family_Hero.png` → **By Dimensions** กว้าง **260 mm** → Cursor Position มุมบนซ้าย → คลิกที่มุมบนซ้ายของพื้นที่ที่ออกแบบไว้
3. Pick ภาพ → คลิกขวา **Show Controls** → crop ขอบให้สินค้าอยู่ตำแหน่งตาม thumbnail
4. **Place Image Fit** วาง `C6_Detail.png` ในกรอบด้านขวา

{: .shot }
[SCREENSHOT: Place Image Tool Options (By Dimensions + Cursor Position 9 จุด)]
{: .shot }
[SCREENSHOT: board ที่มีภาพ hero + detail แล้ว]

{: .note }
ไฟล์ภาพลิงก์อยู่ ถ้าเรนเดอร์ใหม่แล้วบันทึกทับชื่อเดิม layout จะโหลดภาพใหม่ จัดการลิงก์ได้ที่ **Help > Project Information** (linked files)

{: .verify }
ตำแหน่ง **Project Information** ใน Help menu ของ v10 ตามที่คู่มือบอก ให้ยืนยัน

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** Crop ภาพ hero ให้เหลือเฉพาะส่วนที่ชอบที่สุด
</div>

## ✅ เช็คตัวเอง
<details><summary>1. crop กับยืดภาพต่างกันอย่างไร?</summary>ลากขอบ = crop · กด Cmd/Ctrl ค้างแล้วลาก = ยืด</details>
<details><summary>2. ถ้าเรนเดอร์ภาพใหม่ต้องวางใหม่ไหม?</summary>ไม่ต้อง ถ้าบันทึกทับชื่อเดิม ภาพบน layout จะอัปเดต</details>
<details><summary>3. อยากให้ภาพพอดีกรอบใช้อะไร?</summary>Place Image Fit</details>

📚 อ้างอิง: R1 Layout (Place Image, Place Image Fit)
