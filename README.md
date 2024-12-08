# การตั้งค่า Login และ SignUp ใน Android ด้วย MySQL
## ข้อกำหนดในการตั้งค่า
- ติดตั้ง XAMPP เพื่อใช้งาน Apache และ MySQL
- เริ่มต้นบริการ Apache และ MySQL ผ่าน XAMPP Control Panel
## การสร้างฐานข้อมูล:
```
-- สร้างฐานข้อมูล android
CREATE DATABASE android;

-- ใช้ฐานข้อมูล android
USE android;

-- สร้างตาราง users
CREATE TABLE users (
    id INT(11) AUTO_INCREMENT PRIMARY KEY,
    fullname TEXT COLLATE utf8mb4_general_ci NOT NULL,
    username VARCHAR(100) COLLATE utf8mb4_general_ci NOT NULL UNIQUE,
    password TEXT COLLATE utf8mb4_general_ci NOT NULL,
    email VARCHAR(300) COLLATE utf8mb4_general_ci NOT NULL UNIQUE
);
```
## ดาวน์โหลดไฟล์และสร้างโฟร์เดอร์
- สร้าง
## สร้างโปรเจค android studio ตั้งชื่อ Login-Register
- Name:    Login-Register
