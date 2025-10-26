
# Part 2-4: Google Gemini กับการสร้าง presentation

## ขั้นตอนที่ 1: เตรียมและอัปโหลดเอกสาร
1. ไปที่ [gemini.google.com](https://gemini.google.com) และเข้าสู่ระบบด้วย Gmail ส่วนตัวของพวกเรา
2. คลิกไอคอนคลิปหนีบกระดาษ (📎) และอัปโหลดไฟล์ [01_Feature-3-Expenses_Policy.pdf](https://drive.google.com/drive/folders/1TwnQlfWuv8y2Cvmz-TsCAxakHTgpbHnk?usp=drive_link)
3. รอให้ Gemini ยืนยันว่าไฟล์ถูกอัปโหลดแล้ว

🧠 เคล็ดลับ: พวกเราสามารถลากและวางไฟล์ลงในพื้นที่แชทได้โดยตรง

## ขั้นตอนที่ 2: ขอให้ Gemini สรุปเอกสาร

### ตัวอย่าง Prompt:

```
Summarise this document into key sections suitable for a presentation slide deck. Include a brief description for each section.
```

```
สรุปเอกสารนี้เป็นหัวข้อหลักที่เหมาะสมสำหรับการนำเสนอ พร้อมคำอธิบายสั้นๆ สำหรับแต่ละหัวข้อ
```

Gemini น่าจะแสดงผลรายการแบบนี้:
- Travel Expenses: Policy, limits, and booking guidelines
- Accommodation: Hotel standards and restrictions
- Meals: Daily limit and approved conditions
- Entertainment: Approval requirements
- Office Supplies: Usage and reimbursement policy

## ขั้นตอนที่ 3: สร้าง outline สำหรับ slide

### ตัวอย่าง Prompt:

```
Create a 7-slide outline for a presentation explaining the Expense Policy to new employees. Include slide titles and short summaries.
```

```
สร้าง outline สำหรับการนำเสนอ 7 สไลด์ เพื่ออธิบายนโยบายค่าใช้จ่ายให้กับพนักงานใหม่ พร้อมหัวข้อสไลด์และสรุปสั้นๆ
```

ตัวอย่าง outline ที่คาดว่าจะได้:
1. Introduction to Expense Policy
2. Travel Guidelines
3. Accommodation Rules
4. Meal Allowances
5. Entertainment Policy
6. Office Supplies and Reimbursement
7. Summary and Q&A

> ในขั้นตอนนี้ ตัว Gemini อาจจะสร้าง Canvas ขึ้นมาให้เราด้วย ซึ่งเราสามารถใช้เป็นแนวทางในการสร้าง presentation ได้

## ขั้นตอนที่ 4: สร้างเนื้อหา slide

### ตัวอย่าง Prompt:

```
Using the outline above, write slide titles, 3 bullet points per slide, and one short speaker note per slide.
```
```
ใช้โครงร่างข้างต้น เขียนหัวข้อสไลด์ 3 จุดย่อยต่อสไลด์ และโน้ตสั้นๆ สำหรับผู้พูดต่อสไลด์
```

Gemini อาจสร้างเนื้อหาแบบนี้:
- Slide 2 – Travel Guidelines:
    - Book economy transport via approved tools.
    - Avoid upgrades and personal add-ons.
    - Keep receipts for all transport claims.
Speaker Note: Emphasize the need for cost-efficient travel and compliance with policy.


## ขั้นตอนที่ 5: นำโครงสร้างไปใช้ใน Google Slides หรือ Presentation อื่นๆ ตามความเหมาะสม