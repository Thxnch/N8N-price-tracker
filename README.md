🛒 E-commerce Price Monitoring & Multi-Channel Deal Alert System
ระบบเฝ้าระวังราคาสินค้าอัจฉริยะแบบอัตโนมัติ 24/7 ที่เชื่อมต่อการทำงานระหว่าง n8n, Airtable, OpenAI, และ LINE Messaging API เพื่อช่วยให้คุณไม่พลาดดีลที่ดีที่สุดในทุกวัน

🌟 Key Features
Automated Daily Tracking: ระบบตรวจสอบราคาสินค้าตามเวลาที่กำหนดโดยอัตโนมัติ (Cron Job)

Smart Data Extraction: ดึงข้อมูลราคาจากหน้าเว็บ (Web Scraping) พร้อมระบบจำลอง User-Agent เพื่อความเสถียร

AI-Powered Analysis: ใช้ GPT-4o-mini ในการวิเคราะห์ความคุ้มค่าของดีลและให้คำแนะนำในการตัดสินใจซื้อ

Multi-Channel Notification: แจ้งเตือนทันทีผ่าน LINE เมื่อราคาสินค้าลดลงถึงเป้าหมาย (Target Price)

Robust Error Handling: มีระบบแจ้งเตือนข้อผิดพลาดเมื่อการดึงข้อมูลจากเว็บมีปัญหา (Scraping Error Notification)

Historical Data Logging: บันทึกประวัติราคาสินค้าลงใน Airtable เพื่อวิเคราะห์แนวโน้มราคาย้อนหลัง

🛠 Tech Stack
Automation Hub: n8n

Database: Airtable (Products & Price History Tables)

Intelligence: OpenAI API (GPT-4o-mini)

Communication: LINE Messaging API

Languages: JavaScript (for Data Cleaning & Processing)

📐 Workflow Architecture
Schedule: เริ่มทำงานทุกวันเวลา 07:00 น.

Fetch: ดึงรายการสินค้าที่ต้องเฝ้าดูจาก Airtable

Process: วนลูปตรวจสอบสินค้าทีละรายการ (Split in Batches)

Scrape & Clean: ดึง HTML จากหน้าเว็บและใช้ Regex/JavaScript แปลงข้อมูลราคาให้เป็นตัวเลข

Evaluate: เปรียบเทียบกับราคาเป้าหมายในฐานข้อมูล

AI Insight: ส่งข้อมูลราคาให้ AI สรุปความคุ้มค่า

Alert: หากราคาตรงเงื่อนไข ส่งการแจ้งเตือนเข้า LINE พร้อมบทวิเคราะห์

Record: อัปเดตข้อมูลและบันทึกประวัติลงฐานข้อมูล

🚀 Getting Started
นำไฟล์ .json ของ Workflow ไป Import ลงใน n8n ของคุณ

ตั้งค่า Credentials สำหรับ:

Airtable Personal Access Token

OpenAI API Key

LINE Channel Access Token / Secret

เตรียมตารางใน Airtable ให้มีฟิลด์ตามที่กำหนด (Product Name, URL, Target Price, Current Price)

เปิดการทำงาน (Active) และรอรับดีลเด็ดได้เลย!

Developed by: ธนชัย เอี่ยมสอาด (Thanachai Iamsa-ard)
นักศึกษามหาวิทยาลัยศรีปทุม (SPU)
