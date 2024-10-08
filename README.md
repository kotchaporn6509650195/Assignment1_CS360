# 🚀Assignment1🚀

## 📚Strapi

### วัตถุประสงค์ของ Strapi

Strapi คือ โปรแกรม headless CMS ที่เป็นโอเพนซอร์ส ซึ่งสามารถนำไปใช้สร้าง API ด้วย Javascript ได้อย่างรวดเร็ว ใช้งานได้ฟรี ยืดหยุ่น บริหารจัดการได้ง่าย ปลอดภัย รวมถึงสามารถปรับขนาดให้เหมาะกับธุรกิจได้ และทำงานร่วมกับ framework รุ่นใหม่ส่วนใหญ่ เช่น React และ Node ได้เป็นอย่างดีอีกด้วย

- Usecases
  
  - **แอปพลิเคชันมือถือ** Strapi สามารถสร้าง API ที่ให้ข้อมูลสำหรับแอปพลิเคชันมือถือ ซึ่งช่วยในการจัดการข้อมูลที่แสดงในแอป
  - **โซเชียลมีเดียและเครือข่ายสังคม** Strapi สามารถใช้ในการจัดการข้อมูลของผู้ใช้, โพสต์, และการโต้ตอบในเครือข่ายสังคม
  - **บล็อกและแพลตฟอร์มการเผยแพร่** ใช้ Strapi เพื่อจัดการบล็อกโพสต์, หมวดหมู่, และแท็ก
    
- Component
  
  **1. Content Types:** 
    - สร้างและจัดการประเภทของข้อมูล (เช่น บทความ, สินค้า)
    - Dynamic Zones สำหรับเนื้อหาแบบยืดหยุ่น

  **2. API:**
   - REST และ GraphQL API อัตโนมัติ
   - Custom API สำหรับการปรับแต่งเพิ่มเติม

  **3. Admin Panel:**
   - แดชบอร์ดสำหรับการจัดการเนื้อหา
   - Content Manager สำหรับการแก้ไขเนื้อหา

  **4. Plugins:**
   - Authentication, Media Library, Internationalization (i18n), Email
   - สร้าง Custom Plugins ได้

  **5. Roles & Permissions:**
   - กำหนดบทบาทและสิทธิ์การเข้าถึงเนื้อหา

  **6. Authentication & Security:**
   - ใช้ JWT สำหรับการรักษาความปลอดภัย
   - รองรับ OAuth Providers (Google, Facebook, ฯลฯ)

  **7. Database:**
   - รองรับหลายฐานข้อมูล (MongoDB, PostgreSQL, MySQL)
   - มีการจัดการการเปลี่ยนแปลงฐานข้อมูล

  **8. Webhooks:**
   - สร้าง Webhooks เพื่อเชื่อมต่อกับระบบภายนอก

  **9. Customization:**
   - ปรับแต่ง Middlewares, Routes, Controllers ตามความต้องการ

  **10. Deployment & Scaling:**
    - Self-host บนเซิร์ฟเวอร์ต่างๆ และรองรับการขยายระบบ
      
 - Refer
   
    - https://morphos.is/th/blog/what-is-strapi-and-how-it-will-dominate-the-world-of-headless-cms
    - https://chatgpt.com
      
### .gitignore
.gitignore มีหน้าที่บอก Git ว่าไฟล์ไหนบ้างที่เราไม่ต้องการให้ Git สนใจและเก็บไว้ใน Version Control

  - Contents in .gitignore file
    
    #### 1. **OS X:**
     - **`.DS_Store`:** ไฟล์ที่ macOS สร้างขึ้นเพื่อเก็บข้อมูลเมตาเกี่ยวกับโฟลเดอร์ (เช่น ตำแหน่งไอคอน)
     - **`.AppleDouble`:** ไฟล์นี้ถูกสร้างขึ้นเมื่อ macOS เก็บข้อมูลไฟล์สองส่วน (data fork และ resource fork) ในระบบไฟล์ที่ไม่รองรับระบบสองส่วนนี้
     - **`.LSOverride`:** ไฟล์ที่ถูกใช้โดยระบบ macOS เพื่อจัดการการเปิดไฟล์ด้วยแอปพลิเคชันเริ่มต้นที่กำหนดเอง
     - **`Icon\r`:** ไฟล์ที่ใช้ในการจัดเก็บไอคอนของโฟลเดอร์ (hidden icon file)
     - **`.Spotlight-V100`:** โฟลเดอร์ที่ Spotlight (ระบบค้นหาของ macOS) สร้างขึ้นเพื่อจัดเก็บดัชนีการค้นหา
     - **`.Trashes`:** โฟลเดอร์ที่ใช้เก็บไฟล์ที่ถูกลบโดยผู้ใช้ (Recycle Bin ของ macOS)
     - **`._*`:** ไฟล์ที่ macOS สร้างขึ้นเมื่อมีการคัดลอกไฟล์ไปยังระบบไฟล์ที่ไม่รองรับข้อมูลเมตาแบบ HFS+ ของ macOS

    #### 2. **Linux:**
     - **`*~`:** ไฟล์สำรองที่สร้างโดยเครื่องมือแก้ไขข้อความใน Linux เช่น `vim` หรือ `emacs` (เช่น `file.txt~`)

    #### 3. **Windows:**
     - **`Thumbs.db`:** ไฟล์แคชภาพขนาดย่อที่ Windows Explorer สร้างขึ้นเมื่อเปิดดูภาพในโฟลเดอร์
     - **`ehthumbs.db`:** ไฟล์แคชภาพขนาดย่อที่สร้างโดย Windows Media Center
     - **`Desktop.ini`:** ไฟล์การตั้งค่าในโฟลเดอร์ของ Windows ซึ่งเก็บข้อมูลการปรับแต่งโฟลเดอร์
     - **`$RECYCLE.BIN/`:** โฟลเดอร์รีไซเคิลของ Windows ที่ใช้เก็บไฟล์ที่ถูกลบ
     - **`*.cab`:** ไฟล์การบีบอัดแบบ Cabinet ที่ใช้สำหรับการติดตั้งซอฟต์แวร์บน Windows
     - **`*.msi`:** ไฟล์แพ็คเกจติดตั้งสำหรับซอฟต์แวร์ที่ใช้โดย Windows Installer
     - **`*.msm`:** ไฟล์ Module ของ Windows Installer ที่ใช้ในการติดตั้งซอฟต์แวร์
     - **`*.msp`:** ไฟล์แพ็คเกจการอัปเดตสำหรับ Windows Installer

    #### 4. **Packages:**
     - **`*.7z`:** ไฟล์บีบอัดแบบ 7-Zip
     - **`*.csv`:** ไฟล์ข้อมูลที่แยกด้วยเครื่องหมายจุลภาค (Comma-Separated Values)
     - **`*.dat`:** ไฟล์ข้อมูล (generic data file)
     - **`*.dmg`:** ไฟล์ภาพดิสก์ที่ใช้บน macOS
     - **`*.gz`:** ไฟล์บีบอัดแบบ Gzip
     - **`*.iso`:** ไฟล์ภาพดิสก์ (ISO image)
     - **`*.jar`:** ไฟล์แพ็กเกจ Java Archive
     - **`*.rar`:** ไฟล์บีบอัดแบบ RAR
     - **`*.tar`:** ไฟล์บีบอัดแบบ TAR
     - **`*.zip`:** ไฟล์บีบอัดแบบ ZIP
     - **`*.com`:** ไฟล์ที่ทำงานได้โดยตรง (command file) บนระบบ DOS
     - **`*.class`:** ไฟล์คลาสของ Java
     - **`*.dll`:** ไฟล์ Dynamic Link Library บน Windows
     - **`*.exe`:** ไฟล์ปฏิบัติการ (executable file) บน Windows
     - **`*.o`:** ไฟล์ object code ที่ได้จากการคอมไพล์
     - **`*.seed`:** ไฟล์ที่ใช้เก็บข้อมูลเมล็ดพันธุ์ (seed data) ที่ใช้ในการทดสอบ
     - **`*.so`:** ไฟล์ shared object library บน Linux/UNIX
     - **`*.swo`, `*.swp`, `*.swn`:** ไฟล์ชั่วคราวที่สร้างโดย `vim` เมื่อเปิดแก้ไขไฟล์
     - **`*.swm`:** ไฟล์ที่แบ่งส่วนจากการสร้างภาพดิสก์โดย Windows Imaging Format (WIM)
     - **`*.out`:** ไฟล์ output จากการคอมไพล์หรือการประมวลผล
     - **`*.pid`:** ไฟล์ที่เก็บ Process ID ที่กำลังทำงานอยู่

    #### 5. **Logs and Databases:**
     - **`.tmp`:** ไฟล์ชั่วคราวที่สร้างขึ้นขณะทำงาน
     - **`*.log`:** ไฟล์บันทึกที่เก็บรายละเอียดการทำงานของแอปพลิเคชัน
     - **`*.sql`:** ไฟล์สคริปต์ SQL ที่ใช้จัดการฐานข้อมูล
     - **`*.sqlite`, `*.sqlite3`:** ไฟล์ฐานข้อมูล SQLite

    #### 6. **Miscellaneous:**
     - **`*#`:** ไฟล์สำรองที่ลงท้ายด้วย `#` ซึ่งมักจะสร้างโดยเครื่องมือแก้ไขข้อความ
     - **`ssl`:** โฟลเดอร์ที่เก็บข้อมูล SSL เช่น ใบรับรองดิจิทัล
     - **`.idea`:** โฟลเดอร์ที่สร้างโดย IDE อย่าง IntelliJ IDEA เพื่อเก็บการตั้งค่าโปรเจกต์
     - **`nbproject`:** โฟลเดอร์ที่สร้างโดย NetBeans IDE เพื่อเก็บการตั้งค่าโปรเจกต์
     - **`public/uploads/*`:** ละเว้นไฟล์ทั้งหมดในโฟลเดอร์นี้ ยกเว้นไฟล์ `.gitkeep` ที่ใช้เพื่อรักษาโครงสร้างของโฟลเดอร์ใน Git

    #### 7. **Node.js:**
     - **`lib-cov`:** โฟลเดอร์ที่เก็บการครอบคลุมโค้ด (code coverage)
     - **`lcov.info`:** ไฟล์ข้อมูลการครอบคลุมโค้ดในรูปแบบ `lcov`
     - **`pids`:** โฟลเดอร์ที่เก็บไฟล์ PID (Process ID)
     - **`logs`:** โฟลเดอร์ที่เก็บไฟล์บันทึก (log files)
     - **`results`:** โฟลเดอร์ที่เก็บผลลัพธ์จากการทดสอบหรือการประมวลผล
     - **`node_modules`:** โฟลเดอร์ที่เก็บแพ็กเกจของ Node.js (ไม่ควรติดตามใน Git เพราะสามารถติดตั้งใหม่ได้ด้วย `npm install`)
     - **`.node_history`:** ไฟล์ที่เก็บประวัติการทำงานของ Node.js REPL

    #### 8. **Tests:**
     - **`coverage`:** โฟลเดอร์ที่เก็บข้อมูลการครอบคลุมการทดสอบ (code coverage reports)

    #### 9. **Strapi:**
     - **`.env`:** ไฟล์ที่เก็บค่าตัวแปรสภาพแวดล้อม (environment variables)
     - **`license.txt`:** ไฟล์ที่เก็บข้อมูลสิทธิ์การใช้งาน
     - **`exports`:** ไฟล์หรือโฟลเดอร์ที่เกี่ยวข้องกับการส่งออกข้อมูล
     - **`.strapi`:** โฟลเดอร์ที่ Strapi ใช้เก็บข้อมูลการตั้งค่าและข้อมูลภายใน
     - **`dist`:** โฟลเดอร์ที่ใช้เก็บไฟล์ที่ถูกสร้างขึ้นจากการคอมไพล์
     - **`build`:** โฟลเดอร์ที่เก็บผลลัพธ์จากการ build โปรเจกต์
     - **`.strapi-updater.json`:** ไฟล์ที่เก็บข้อมูลการอัปเดตของ Strapi
     - **`.strapi-cloud.json`:** ไฟล์ที่เก็บข้อมูลการเชื่อมต่อกับ Strapi Cloud

  - Refer
    
    - https://www.facebook.com/photo.php?fbid=951249207003076&id=100063540163933&set=a.683592353768764
    - https://chatgpt.com
   
## 🤫Steps to Install Strapi

#### 1. Downlode npm and node.js

ดาวน์โหลด npm and node.js ที่ [https://git-scm.com/download/win](https://nodejs.org/en/download/prebuilt-installer)

#### 2. Check version

```
node -v # check version Node.js
npm -v # check version Node Package Manager
```

#### 3. Install Yarn for install Strapi

```
npm install -g yarn # install yarn
yarn -v # check version yarn
```

#### 4. Create Strapi project

```
yarn create strapi-app <Name project>
-> choose quickstart
-> choose skip
```

#### 5. Run

```
cd <Name project> # change directory project
yarn develop # Run project 
```

## ⚙️Steps Push Code to GitHub

#### 1. Create repository

สร้าง repository ที่ https://github.com

#### 2. Downlode Git Bash

ดาวน์โหลด Git Bash ที่ https://git-scm.com/download/win

#### 3. Push code in GitHub

```
git -v # check version Git

cd <Name project> # change project
git init # create new Git repository in current directory
git config --global user.name <Name> # name the username
git config --global user.email <Email> # name the email
git remote add <Name remote> <remote repository URL> # setting repository for connect repository in GitHub
git branch -M main # create branch for keep code

git add . # add all directory
git commit -m "Message" # Save local repository
git push -u <Name remote> main # record remote repository
```

## ✨Steps to Deploy

#### 1. Launch an EC2 Instance

   - ตั้งชื่อ Instance
   - เลือก AMI Ubuntu Server 24.04 LTS (HVM), SSD Volume Type 64-bit
   - เลือก Instance type t2.small
   - เลือก Key pair
   - Network settings เลือก Edit สร้าง security group
     - Type: SSH, Protocol: TCP, Port Range: 22, Source type: Custom, Source: 0.0.0.0/0
     - Type: SSH, Protocol: TCP, Port Range: 22, Source type: Custom, Source: ::/0
     - Type: HTTP, Protocol: TCP, Port Range: 80, Source type: Custom, Source: 0.0.0.0/0, ::/0
     - Type: HTTPS, Protocol: TCP, Port Range: 443, Source type: Custom, Source: 0.0.0.0/0, ::/0
     - Type: Custom TCP, Protocol: TCP, Port Range: 1337, Source type: Custom, Source: 0.0.0.0/0
   - Configure storage กำหนดให้เป็น 1 x 8 GiB gp2 Root volume
   - Launch instance

#### 2. Connect Instance

Console Home -> Click EC2 -> Instances -> Right Click on Instances desired -> Connect -> Copy code ตรง Example และแก้ directory key.pem ในโค้ดให้ตรงกับเครื่อง

#### 3. Update APT & Install package

```
sudo apt update # update apt
sudo apt install npm # install Node Package Manager
sudo npm install yarn -g # install Yarn
sudo apt install git # install Git
sudo npm install pm2 -g # install for manage process
```
#### 4. Create directory for run project

```
mkdir <Name directory> # Create directory
cd <Name directory> # Change directory
```

#### 5. Slone project from GitHub to EC2

```
git clone <remote repository URL> # clone project
cd <Name directory project> # change directory of project 
yarn install # install package
```

#### 6. Setup .env

```
cp .env.example .env # create .env by copy .env.example
nano .env # edit HOST, PORT, Key, Token in .env
```

#### 7. Build project

```
NODE_ENV=production yarn build
```

#### 8. Create file for run project

```
cd .. # leave directory
pm2 init # create ecosystem.config.js for run project
```

#### 9. Edit file for run project

```
sudo nano ecosystem.config.js # edit file for run project
module.exports = {
  apps: [
    {
      name: 'strapi-deploy',
      cwd: '/home/ubuntu/Purpose/Assignment1_CS360',
      script: 'yarn',
      args: 'start',
      env: {
        APP_KEYS: process.env.API_KEYS,
        API_TOKEN_SALT: process.env.API_TOKEN_SALT,
        ADMIN_JWT_SECRET: process.env.ADMIN_JWT_SECRET,
        JWT_SECRET: process.env.JWT_SECRET,
        NODE_ENV: 'production',
      },
    },
  ],
};
```

#### 10. Deploy Project

```
pm2 start ecosystem.config.js
```
