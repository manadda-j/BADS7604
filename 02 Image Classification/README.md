Project
  Image Classification ของขนมไทยทั้งหมด 10 ชนิด

Introduction
  Image Classification ของขนมไทยทั้งหมด 10 ชนิด โดยใช้ ImageNet Pre-trained CNN 
  โดยทำในลักษณะของ Fine-Tuning Transfer Learning ซึ่งจะทำการเปรียบเทียบประสิทธิภาพและประสิทธิผล
  ทั้งหมด 5 Models ประกอบด้วย VGG-16, ResNet152V2, MobileNet, DenseNet121 และ EfficientNetB0
  และการทำ Class Activation Mapping (CAM) เพื่อตรวจสอบว่า Model ได้ตรวจจับอยู่ในบริเวณของวัตถุหรือไม่

Highlight
  -จากผลของการทดสอบ Model ด้วย Validation และ Test Set ทำให้สมมติฐานที่เราคิดไว้นั้นไม่เป็นไปตามคาด
เนื่องจาก ทางกลุ่มมองว่า Model ที่มีประสิทธิผลดีกับ Validation Set อย่าง DenseNet121 และ EfficientNetB0
ที่มีค่า Accuracy สูงถึง 0.91 ควรจะ ให้ Accuracy กับ Test Set ได้ดีเช่นกัน แต่หลังจากที่เราทดสอบกับ Test Set
Model ที่ดีที่สุดคือ MobileNet ทั้งในด้านประสิทธิภาพและประสิทธิผล
  -ทางด้านความเร็วในการ Train Modelเป็นไปตามที่ทางกลุ่มประเมินไว้ คือ Model ที่มีจำนวน Layer และ
Parameter น้อยจะ train ได้เร็วกว่า Model ที่มีจำนวน Layer และ Parameter มาก จะเห็นว่า MobileNet 
นั้นเป็น Model ขนาดเล็กเมื่อเทียบกับ Model อื่นๆ จึงมีประสิทธิภาพที่ดีกว่า
  -ข้อมูลรูปภาพที่นามสกุลไฟล์ .JFIF นั้นไม่สามารถนำมาใช้ได้ จำเป็นที่จะต้องกรองออกก่อน
ที่จะนำข้อมูลเข้า Model
  -การเพิ่มจำนวนรูปภาพในการ Train ไม่ได้ทำให้ประสิทธิผลของ Model เพิ่มขึ้นอย่างมีนัยสำคัญ

Files Desciption
  1. Dataset 
      รูปภาพของขนมไทย 10 Classes แต่ละ Class 200 รูป ทั้งหมดประมาณ 2,000 รูป
      - Banana In Coconut Milk - Kluay Buat Chi (กล้วยบวชชี)
      - Deep-Fried Rice Flour  - Fak Bua (ฝักบัว)
      - Durian Sticky Rice     - Khao Niao Tu-rean (ข้าวเหนียวทุเรียน)
      - Pandanus Pudding in Coconut Cream  - Piak Poon Krati Sod (เปียกปูนกระทิสด)
      - Rice Balls in Sweet Coconut Milk   - Bua Loy (บัวลอย)
      - Sweet Sticky Rice with Thai Custard - Khao Niao Sangkhaya (ข้าวเหนียวสังขยา)
      - Tapioca Balls with Pork Filling    - Saku Sai Moo (สาคูไส้หมู)
      - Thai Crispy Pancake topped with Golden Threads -  Khanom Buang Foi Thong (ขนมเบื้องฝอยทอง)
      - Thai Style Fried Savory Dumplings with Fish Filling  - Pan Sib (ปั้นสิบ, ปั้นขลิบ)
      - Toddy Palm Cake   - Khanom Tan (ขนมตาล)
     แต่ละ Class ถูกแบ่งเป็น Train Set, Validation Set และ Test Set ด้วยสัดส่วน 80:10:10
     ภายใน Folder นี้ประกอบไปด้วย 3 Folders ย่อย
     1.1 Train Set - ประกอบไปด้วยรูปภาพสำหรับ Train Model
     1.2 Validate Set - ประกอบไปด้วยรูปภาพสำหรับ Validate Model
     1.3 Test Set - ประกอบไปด้วยรูปภาพสำหรับ Test Model
     1.4 Datasource.xlsx - ไฟล์ที่รวม URLs Source ของ Dataset ทั้งหมด
  2. Model
      ข้อมูลการ Train, Validate, Test และ Result ของทั้ง 5 Models ประกอบด้วย
      VGG-16, ResNet152V2, MobileNet, DenseNet121 และ EfficientNetB0

Members Percent Contribution and Responsibility
6220421004 Suwant Te (20%)
  -รวบรวมรูปภาพ Class สาคูไส้หมู และ ขนมฝักบัว
  -รับผิดชอบในส่วนของ ResNet152V2
6220421005 Ratchanat Sa (20%)
  -รวบรวมรูปภาพ Class บัวลอย และ ปั้นขลิบ
  -รับผิดชอบในส่วนของ DenseNet121
6220421007 Manadda Ja (20%) 
  -รวบรวมรูปภาพ Class เปียกปูนกะทิสด และ กล้วยบวชชี
  -รับผิดชอบในส่วนของ VGG-16
6220422017 Kittipan Pi (20%)
  -รวบรวมรูปภาพ Class ข้าวเหนียวสังขยา และ ขนมเบื้องฝอยทอง
  -รับผิดชอบในส่วนของ MobileNet
6220422046 Krittin Sa (20%)
  -รวบรวมรูปภาพ Class ข้าวเหนียวมะม่วง และ ขนมตาล
  -รับผิดชอบในส่วนของ EfficientNetB0
