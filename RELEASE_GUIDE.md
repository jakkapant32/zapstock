# 🚀 คู่มือการปล่อยแอพ ZapStock แบบฟรี

## 📋 สิ่งที่ต้องเตรียม

### 1. 🎨 ไอคอนและรูปภาพ (ต้องสร้าง)
สร้างไฟล์เหล่านี้ในโฟลเดอร์ `assets/`:

- `icon.png` - ไอคอนหลัก 1024x1024 pixels
- `adaptive-icon.png` - ไอคอน Android 1024x1024 pixels  
- `splash.png` - หน้าจอเริ่มต้น 1284x2778 pixels
- `favicon.png` - ไอคอนเว็บ 32x32 pixels

### 2. 📝 ข้อมูลแอพ
- ชื่อ: ZapStock
- คำอธิบาย: แอพจัดการสต็อกสินค้า
- หมวดหมู่: Business/Productivity
- ภาษา: ไทย

### 3. 🔧 การตั้งค่า Build

#### Android APK
```bash
# ติดตั้ง EAS CLI
npm install -g @expo/eas-cli

# ตั้งค่า EAS
eas build:configure

# สร้าง APK
eas build --platform android --profile preview
```

#### iOS IPA (ถ้าต้องการ)
```bash
# สร้าง IPA
eas build --platform ios --profile preview
```

## 🌐 แพลตฟอร์มการแจกจ่ายฟรี

### 1. 📱 APK Mirror
- **เว็บไซต์**: https://www.apkmirror.com/
- **ข้อดี**: ฟรี, ไม่ต้องสมัครสมาชิก
- **วิธีใช้**: อัปโหลด APK ไฟล์

### 2. 📦 GitHub Releases
- **เว็บไซต์**: https://github.com/
- **ข้อดี**: ฟรี, ควบคุมได้เต็มที่
- **วิธีใช้**: สร้าง repository และอัปโหลดไฟล์

### 3. 🔗 Direct Download
- **วิธีใช้**: อัปโหลด APK ไปยัง Google Drive, Dropbox
- **ข้อดี**: ฟรี, ง่าย
- **ข้อเสีย**: ต้องแชร์ลิงก์เอง

### 4. 📱 F-Droid (Open Source)
- **เว็บไซต์**: https://f-droid.org/
- **ข้อดี**: ฟรี, เน้นความเป็นส่วนตัว
- **ข้อกำหนด**: ต้องเป็น Open Source

### 5. 🌍 APKPure
- **เว็บไซต์**: https://apkpure.com/
- **ข้อดี**: ฟรี, มีผู้ใช้เยอะ
- **วิธีใช้**: อัปโหลด APK ไฟล์

## 🛠️ ขั้นตอนการสร้าง APK

### 1. ติดตั้ง Dependencies
```bash
npm install -g @expo/eas-cli
```

### 2. ตั้งค่า EAS
```bash
eas build:configure
```

### 3. สร้าง APK
```bash
eas build --platform android --profile preview
```

### 4. ดาวโหลด APK
- ไปที่ https://expo.dev/
- เข้าสู่บัญชี
- ดาวโหลด APK ไฟล์

## 📋 Checklist ก่อนปล่อย

- [ ] สร้างไอคอนและรูปภาพ
- [ ] ทดสอบแอพให้ครบทุกฟีเจอร์
- [ ] ตรวจสอบ API connection
- [ ] สร้าง APK
- [ ] ทดสอบ APK บนอุปกรณ์จริง
- [ ] เตรียมคำอธิบายแอพ
- [ ] อัปโหลดไปยังแพลตฟอร์มที่เลือก

## 🔒 ข้อควรระวัง

1. **API Server**: ต้องแน่ใจว่า server ทำงานได้
2. **Database**: ต้องมี database ที่เสถียร
3. **Security**: ตรวจสอบการเข้ารหัสข้อมูล
4. **Testing**: ทดสอบบนอุปกรณ์จริงหลายเครื่อง

## 📞 การสนับสนุน

หากมีปัญหาในการสร้าง APK หรือการปล่อยแอพ สามารถติดต่อได้ที่:
- GitHub Issues
- Email Support
- Community Forums
