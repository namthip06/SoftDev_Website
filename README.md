# WannaGo! - Modern Travel Planning Platform

WannaGo! คือแพลตฟอร์มวางแผนการท่องเที่ยวแบบครบวงจรที่ช่วยให้ผู้ใช้งานทั่วไปสามารถสร้างแผนการเดินทางได้ในคลิกเดียว และช่วยให้ผู้ประกอบการสามารถจัดการสถานที่และโฆษณาผ่านระบบ Dashboard ที่ชาญฉลาด

## Project Overview

การวางแผนท่องเที่ยวในปัจจุบันมักกระจัดกระจายระหว่างการหาข้อมูล การจอง และการจัดตารางเวลา WannaGo! จึงถูกสร้างขึ้นเพื่อแก้ปัญหาเหล่านี้:

* **User Side:** ลดความยุ่งยากในการจัดตารางเวลาด้วยระบบ Drag-and-Drop Itinerary และการแสดงผลบนแผนที่แบบ Real-time
* **Business Side:** ให้บริการ Dashboard วิเคราะห์ข้อมูลโฆษณา เช่น Views, Clicks และ CTR เพื่อช่วยให้ผู้ประกอบการตัดสินใจทางการตลาดได้แม่นยำขึ้น

## Core Functionality

* **Dynamic Itinerary Builder:** ระบบสร้างแผนการเดินทางที่รองรับการลากวางสถานที่ข้ามวัน พร้อมคำนวณลำดับสถานที่ใหม่โดยอัตโนมัติ
* **Interactive Data Visualization:** Dashboard สำหรับผู้ประกอบการที่ใช้ Recharts แสดงสถิติประสิทธิภาพโฆษณาในรูปแบบ Interactive Area Charts
* **Geolocation Integration:** ระบบระบุตำแหน่งผู้ใช้เพื่อกำหนดจุดเริ่มต้นการเดินทาง และการทำงานร่วมกับ Leaflet Maps เพื่อวาดเส้นทางบนแผนที่
* **Complex Form Handling:** ระบบจัดการข้อมูลสถานที่แบบ CRUD ที่รองรับหมวดหมู่ที่แตกต่างกัน เช่น ที่พัก ร้านอาหาร และสถานที่ท่องเที่ยว พร้อมระบบตรวจสอบความถูกต้องของข้อมูล

## Tech Stack & Tools

### Frontend

* **React 19:** ใช้ฟีเจอร์ล่าสุดของ React ในการจัดการ UI และ Lifecycle
* **Vite:** เครื่องมือ Build tool เพื่อเพิ่มความรวดเร็วในการพัฒนาและประสิทธิภาพของโปรเจกต์
* **Tailwind CSS v4 & shadcn/ui:** ใช้สำหรับการจัดการ Styling และ Accessible component library
* **React Router DOM v7:** จัดการ Client-side routing และ Protected routes

### Libraries & Frameworks

* **@dnd-kit:** จัดการ State การลากวางที่ซับซ้อนในหน้าตารางเวลา
* **Recharts:** สำหรับการสร้างแผนภูมิแสดงข้อมูลในหน้า Dashboard
* **React-Leaflet:** เชื่อมต่อกับ OpenStreetMap เพื่อแสดงพิกัดและเส้นทาง
* **js-cookie:** จัดการ Session และ Authentication tokens

### DevOps & Tools

* **Docker:** รองรับ Containerization โดยมี Dockerfile สำหรับการนำไปใช้งานบน Production
* **ESLint:** ควบคุมคุณภาพและมาตรฐานของซอร์สโค้ด
* **Environment Variables:** แยกการตั้งค่าระบบผ่านไฟล์ .env

## Key Skills Demonstrated

* **RESTful API Integration:** การเชื่อมต่อและจัดการข้อมูลจาก Backend ผ่าน fetch พร้อมระบบ Retry และ Timeout handling
* **Authentication & Security:** จัดการระบบ Login และ Signup โดยใช้ JWT และจัดเก็บผ่าน Cookies อย่างปลอดภัย
* **State Management & Normalization:** การจัดการ Object แผนการเดินทางที่มีความซ้อนและพยากรณ์ข้อมูลใหม่ก่อนส่งไปยัง API
* **Component Composition:** การออกแบบ Reusable UI components เพื่อลดความซ้ำซ้อนและเพิ่มความง่ายในการบำรุงรักษาโค้ด

## Getting Started

1. **Clone the project**

```bash
git clone https://github.com/yourusername/namthip06-softdev_website.git

```

2. **Install dependencies**

```bash
npm install

```

3. **Set environment variables**
สร้างไฟล์ .env และกำหนดค่า VITE_PUBLIC_API_URL
4. **Run development server**

```bash
npm run dev

```
