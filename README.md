1. โจทย์ H-Bridge (ควบคุมมอเตอร์ + ปุ่มกลับทาง)
สร้าง Tiles (ช่อง) ทั้งหมด 6 อัน ดังนี้ครับ:

Tile 1: สั่งหมุนซ้าย (Button)
Type: Button (Publish)

Topic: my_project_user1/motor/control

Payload: left

Label: หมุนซ้าย

Icon: (รูปลูกศรซ้าย)

Tile 2: สั่งหมุนขวา (Button)
Type: Button (Publish)

Topic: my_project_user1/motor/control

Payload: right

Label: หมุนขวา

Icon: (รูปลูกศรขวา)

Tile 3: สั่งหยุด (Button)
Type: Button (Publish)

Topic: my_project_user1/motor/control

Payload: stop

Label: หยุด

Icon: (รูปสี่เหลี่ยมหยุด)

Tile 4: สั่ง LED ติด (เพื่อกลับทางหมุน) (Button)
Type: Button (Publish)

Topic: my_project_user1/led/control

Payload: on

Label: LED ON (กลับทาง)

Icon: (รูปหลอดไฟ)

Tile 5: แสดงสถานะมอเตอร์ (Text)
Type: Text (Subscribe)

Topic: my_project_user1/motor/status

Label: สถานะ Motor

Tile 6: แสดงสถานะ LED (Text)
Type: Text (Subscribe)

Topic: my_project_user1/led/status

Label: สถานะไฟ

2. โจทย์ LDR + Transistor (ระบบอัตโนมัติ + Emergency)
สร้าง Tiles (ช่อง) ทั้งหมด 6 อัน ดังนี้ครับ:

Tile 1: แสดงค่าแสง (Text)
Type: Text (Subscribe)

Topic: my_project_user1/ldr

Label: ค่าแสง (LDR)

Tile 2: สถานะมอเตอร์ (Text)
Type: Text (Subscribe)

Topic: my_project_user1/motor/status

Label: มอเตอร์ทำงาน?

Tile 3: สถานะ LED1 (ทำงาน) (Text)
Type: Text (Subscribe)

Topic: my_project_user1/led1/status

Label: LED1 (Run)

Tile 4: สถานะ LED2 (หยุด) (Text)
Type: Text (Subscribe)

Topic: my_project_user1/led2/status

Label: LED2 (Stop)

Tile 5: ปุ่มฉุกเฉิน (Button - Emergency)
Type: Button (Publish)

Topic: my_project_user1/emergency

Payload: press

Label: 🚨 EMERGENCY STOP

Color: (แนะนำเลือกสีแดง)

Tile 6: ปุ่มรีเซ็ต (Button - Reset)
Type: Button (Publish)

Topic: my_project_user1/reset

Payload: press

Label: 🔄 RESET SYSTEM

Color: (แนะนำเลือกสีเขียวหรือน้ำเงิน)
