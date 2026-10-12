---
title: "3. กล่องมุมมนใน 60 วินาที"
parent: "C0 · เริ่มตรงนี้! formZ ใน 10 นาที"
nav_order: 3
chapter: true
read_time: 2
do_time: 1
hook: "ทำลูกเต๋ามุมมนใน 60 วินาที แล้วเปลี่ยนความมนได้ทุกเมื่อ"

permalink: /courses/c0-start-here/03-rounded-box/
---

# 3. กล่องมุมมนใน 60 วินาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำลูกเต๋า / กล่องสบู่มุมมนใน **60 วินาที**
- กลับมา **แก้รัศมีมุมมนได้ทีหลัง** (Controlled Round)

## 💡 ทำไมบทนี้ถึงสำคัญ
คลิป "Rounded Cube with Native Tools" ของช่อง SketchUp ทางการมีคนดูเกือบ 3 แสนครั้ง และยาว **7:50 นาที** เพราะ SketchUp ไม่มีเครื่องมือมนขอบในตัว ใน formZ ใช้แค่ **2 คลิก**

## 👣 ลงมือทำ (60 วินาที)
| วินาที | ทำ |
|---|---|
| 0–20 | **Cube** 16 × 16 × 16 (ขนาดลูกเต๋าจริง) |
| 20–40 | **Controlled Round** เลือกทั้ง object → Radius **2** |
| 40–60 | เปิด controls ของ round แล้วเปลี่ยน Radius เป็น **4** ดูความต่าง |

**ทางเลือกแบบปั้นดินน้ำมัน:** **Subdivision / Create** กับ Cube (Iterations 3) จะได้ก้อนกลมแบบสบู่ (ดู [C3 บท 8]({{ '/courses/c3-curves-surfaces/08-subd-intro/' | relative_url }}))

{: .shot }
[SCREENSHOT: ลูกเต๋า Radius 2 vs 4 วางคู่กัน]

{: .power }
**SketchUp ทำได้ไหม?** ได้ แต่ต้องใช้หลายขั้น (Follow Me ตามขอบ) หรือต้องลง extension เช่น RoundCorner และแก้รัศมีทีหลังไม่ได้ ส่วน formZ ใช้ **Controlled Round ในตัว และแก้ค่าได้ภายหลัง**

{: .verify }
วิธีเรียกใช้ controls ของ Controlled Round เพื่อแก้ค่าทีหลังใน 10.1.x (ดู C1 บท 5)

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำจุดลูกเต๋า 6 หน้าด้วย Sphere + **Difference** (ทำหน้า 1 ก่อน)
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ใช้กี่คลิกทำกล่องมุมมน?</summary>2 คลิก: Cube + Controlled Round</details>
<details><summary>2. แก้ความมนทีหลังได้ไหม?</summary>ได้ เพราะเป็น Controlled Round</details>

## 🧭 ไปต่อที่ไหน: 3 ทางเลือก
<div class="next-steps"><a href="{{ '/courses/c1-quick-win/' | relative_url }}"><strong>➡️ เรียนแบบเต็ม</strong><br>C1 ปากกาเมจิกสวยใน 90 นาที</a><a href="{{ '/can-sketchup/' | relative_url }}"><strong>🤔 SketchUp ทำได้ไหม?</strong><br>10 อย่างที่ formZ ทำได้</a><a href="{{ '/tool-map/' | relative_url }}"><strong>🔁 เคยใช้ SketchUp/Shapr3D</strong><br>ตารางเทียบเครื่องมือ</a></div>
