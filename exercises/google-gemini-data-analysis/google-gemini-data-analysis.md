
# Part 2-5: Google Gemini การวิเคราะห์ข้อมูลจาก Spreadsheet

## ขั้นตอนที่ 1: เตรียมและอัปโหลดเอกสาร
1. ไปที่ [gemini.google.com](https://gemini.google.com) และเข้าสู่ระบบด้วย Gmail ส่วนตัวของพวกเรา
2. คลิกไอคอนคลิปหนีบกระดาษ (📎) และอัปโหลดไฟล์ [02_sample_product_revenue.xlsx](https://docs.google.com/spreadsheets/d/1NUliLmuv4_xLS42ppdBV_ODOYBat0imh/edit?usp=drive_link&ouid=109881510505807400189&rtpof=true&sd=true)
3. รอให้ Gemini ยืนยันว่าไฟล์ถูกอัปโหลดแล้ว

🧠 เคล็ดลับ: พวกเราสามารถลากและวางไฟล์ลงในพื้นที่แชทได้โดยตรง


## Example 1: Get Instant Data Summaries for a Report (รับสรุปข้อมูลทันทีสำหรับรายงาน)

แทนที่จะสร้าง Pivot Table หรือใช้สูตร `SUMIF` คุณสามารถขอให้ Gemini หาตัวเลขที่คุณต้องการสำหรับอีเมลหรือการประชุมประจำสัปดาห์ได้ทันที

### The Idea (แนวคิด)

สร้างสรุปผลการดำเนินงานระดับภาพรวมอย่างรวดเร็ว

### How to Use It (วิธีใช้)

**Prompt:**

```
provide a quick summary for my weekly sales report. I need:
1. The Total Revenue from all sales.
2. The top 3 best-selling 'Products' by 'Revenue'.
```

**ข้อความที่คุณป้อน (Thai Translation):**

```
สรุปข้อมูลสำหรับรายงานการขายประจำสัปดาห์ ฉันต้องการ:
1. รายได้รวม (Total Revenue) จากการขายทั้งหมด
2. สินค้า (Products) ที่ขายดีที่สุด 3 อันดับแรกตามรายได้ (Revenue)
```

### Why It's Useful (ประโยชน์)

ช่วยให้คุณได้ประเด็นสำคัญสำหรับการพูดคุยในที่ประชุมหรือการอัปเดตทางอีเมลได้ในไม่กี่วินาที ประหยัดเวลาทำงานกับข้อมูลใน Excel ไปได้ 10-15 นาที

-----

## Example 2: Identify and Analyze Performance Issues (ระบุและวิเคราะห์ปัญหาด้านประสิทธิภาพ)

ค้นหา "การทำงานที่อาจจะมีปัญหา" ที่ต้องให้ความสนใจได้อย่างรวดเร็ว โดยไม่ต้องจัดเรียงและกรองข้อมูลด้วยตนเอง

### The Idea (แนวคิด)

ค้นหาสินค้าที่มีผลงานต่ำที่สุดเพื่อดูว่าดำเนินการปรับปรุงได้อย่างไร

### How to Use It (วิธีใช้)

**Your Prompt (ข้อความที่คุณป้อน):**

```
I need to know where to focus my team's improvement efforts.
* Which 'Product' has the lowest sales 'Revenue'?
```

**ข้อความที่คุณป้อน (Thai Translation):**

```
ฉันต้องการรู้ว่าควรปรับปรุงส่วนไหน:
* สินค้า (Product) ใดที่มีรายได้จากการขาย (Revenue) ต่ำที่สุด?
```

### Why It's Useful (ประโยชน์)

สามารถเจาะจงสินค้า, พนักงานขาย, หรือภูมิภาคที่อาจต้องการการสนับสนุน การฝึกอบรม หรือการทบทวนกลยุทธ์เพิ่มเติมได้ทันที

-----

## Example 3: Draft Communications Based on Data (ร่างข้อมูลการสื่อสารโดยอ้างอิงจากข้อมูลที่ให้)

ใช้ Gemini วิเคราะห์ข้อมูลและร่างการสื่อสาร ทำให้เปลี่ยนข้อมูลเชิงลึกเป็นการดำเนินการได้ทันที

### The Idea (แนวคิด)

ร่างอีเมลแสดงประกาศความสำเร็จของสินค้าขายดี ให้กับทีม

### How to Use It (วิธีใช้)

**Your Prompt (ข้อความที่คุณป้อน):**

```
please identify the best-selling product by total 'Revenue'.

After you identify it, please draft a short announcement email to the team celebrating this product's success. Include key metrics like total revenue generated and mention how this achievement contributes to our overall sales goals. Keep the tone positive and motivating.
```

**ข้อความที่คุณป้อน (Thai Translation):**

```
โปรดระบุสินค้าที่ขายดีที่สุดตามรายได้ (Revenue) รวม

เมื่อระบุได้แล้ว โปรดร่างอีเมลประกาศสั้นๆ ให้กับทีมเพื่อเฉลิมฉลองความสำเร็จของสินค้านี้ ระบุตัวเลขสำคัญ เช่น รายได้รวมที่สร้างได้ และกล่าวถึงว่าความสำเร็จนี้มีส่วนช่วยให้เป้าหมายการขายโดยรวมของเราอย่างไร ใช้น้ำเสียงที่เป็นบวกและสร้างแรงบันดาลใจ
```

### Why It's Useful (ประโยชน์)

ประหยัดเวลาโดยไม่เพียงแค่ค้นหาข้อมูล (ใครคืออันดับ 1) แต่ยังช่วยจัดการงาน "ทักษะด้านอารมณ์" (soft skill) ในการเขียนอีเมล ซึ่งช่วยรักษาขวัญและกำลังใจของทีม

-----

## 4\. Create a Summary Table (Text-Based Pivot Table) (สร้างตารางสรุปข้อมูล)

หากข้อมูลดิบมีมากเกินไป ลองขอให้ Gemini รวบรวมข้อมูลให้เป็นตารางที่เรียบง่ายขึ้น ซึ่งคุณสามารถคัดลอก/วางได้

### The Idea (แนวคิด)

สร้างตารางสรุปที่แสดงรายได้รวมของแต่ละสินค้า

### How to Use It (วิธีใช้)

**Your Prompt (ข้อความที่คุณป้อน):**

```
Please create a summary table with all unique 'Products' listed in the left column, existing each quarter's revenues and add a new column on the right showing the total 'Revenue' for each product. Sort the table from highest total revenue to lowest.
```

**ข้อความที่คุณป้อน (Thai Translation):**

```
โปรดสร้างตารางสรุปที่แสดงรายการ 'สินค้า' (Products) ที่ไม่ซ้ำกันทั้งหมดในคอลัมน์ซ้าย, รายได้ (Revenue) เดิมของแต่ละ quarter และเพิ่มคอลัมน์ใหม่ทางด้านขวาที่แสดง 'รายได้รวม' (Total Revenue) ของแต่ละสินค้า จัดเรียงตารางจากรายได้รวมสูงสุดไปต่ำสุด
```

### Why It's Useful (ประโยชน์)

เร็วกว่าการสร้าง Pivot Table ใน Excel มาก โดยเฉพาะอย่างยิ่งหากคุณไม่ใช่ผู้เชี่ยวชาญด้าน Excel คุณจะได้ตารางที่พร้อมคัดลอกและวางสำหรับงานนำเสนอหรือรายงานของคุณ
