
# Bank of Judy - ระบบธนาคารอย่างง่าย

## ภาษาไทย

### 📌 คำอธิบายโปรแกรม
Bank of Judy เป็นโปรแกรมระบบธนาคารอย่างง่ายที่พัฒนาด้วยภาษา C โดยมีฟังก์ชันการทำงานพื้นฐานดังนี้:
- **ฝากเงิน** (Deposite)
- **ถอนเงิน** (Withdraw)
- **ตรวจสอบยอดเงินคงเหลือ** (Check Balance)

### 🚀 วิธีการใช้งาน
1. **ยอดเงินเริ่มต้น**: ระบบจะเริ่มต้นด้วยยอดเงิน 1,000 บาท
2. **เมนูหลัก**: ผู้ใช้สามารถเลือกทำรายการได้ 4 อย่าง:
   - กด `1` เพื่อฝากเงิน
   - กด `2` เพื่อถอนเงิน
   - กด `3` เพื่อดูยอดเงินคงเหลือ
   - กด `4` เพื่อออกจากโปรแกรม

3. **การทำรายการ**:
   - เมื่อเลือกฝากหรือถอนเงิน ระบบจะถามจำนวนเงินที่ต้องการทำรายการ
   - ระบบจะตรวจสอบความถูกต้องของจำนวนเงิน (ต้องมากกว่า 0)
   - สำหรับการถอนเงิน ระบบจะตรวจสอบว่ามียอดเงินเพียงพอหรือไม่

4. **การแสดงผล**:
   - หลังทำรายการทุกครั้งจะแสดงยอดเงินปัจจุบัน
   - หากเกิดข้อผิดพลาดจะแสดงข้อความ "Judy Error" พร้อมคำอธิบาย

### ⚠️ ข้อควรรู้
- โปรแกรมนี้ใช้ตัวแปร global เก็บยอดเงิน (`balance`)
- มีระบบเคลียร์ input buffer เพื่อป้องกันข้อผิดพลาดในการรับค่า
- ข้อความแสดงผลทั้งหมดเป็นภาษาไทย

### 📝 ตัวอย่างการใช้งาน
```
--- ระบบบัญชีธนาคารอย่างง่าย ---
ยอดเงินเริ่มต้น: 1000 บาท

เลือกทำรายการ:
1. ฝากเงิน
2. ถอนเงิน
3. ดูยอดเงินคงเหลือ
4. ออกจากโปรแกรม
กรุณาเลือก (1-4): 1
ป้อนจำนวนเงินที่ต้องการฝาก: 500
ฝากเงินสำเร็จ: +500 บาท
ยอดเงินปัจจุบัน: 1500 บาท
```

## English

### 📌 Program Description
Bank of Judy is a simple banking system developed in C language with basic functions:
- **Deposit money**
- **Withdraw money**
- **Check balance**

### 🚀 How to Use
1. **Initial Balance**: The system starts with 1,000 THB
2. **Main Menu**: Users can choose 4 options:
   - Press `1` to deposit
   - Press `2` to withdraw
   - Press `3` to check balance
   - Press `4` to exit

3. **Transactions**:
   - When selecting deposit or withdraw, the system will ask for amount
   - The system validates the amount (must be greater than 0)
   - For withdrawals, the system checks sufficient balance

4. **Display**:
   - Current balance is shown after every transaction
   - Errors display "Judy Error" with explanation

### ⚠️ Notes
- This program uses global variable for balance (`balance`)
- Includes input buffer clearing to prevent input errors
- All messages are in Thai language

### 📝 Usage Example
```
--- Simple Banking System ---
Initial balance: 1000 THB

Select transaction:
1. Deposit
2. Withdraw
3. Check balance
4. Exit
Please choose (1-4): 1
Enter amount to deposit: 500
Deposit successful: +500 THB
Current balance: 1500 THB
```

## 🛠️ ฟังก์ชันหลัก / Main Functions
- `deposite(int value)`: ฝากเงิน / Deposit money
- `withdraw(int amount)`: ถอนเงิน / Withdraw money
- `getbalance()`: ดูยอดเงินคงเหลือ / Check balance
- `clearInputBuffer()`: เคลียร์ input buffer / Clear input buffer

