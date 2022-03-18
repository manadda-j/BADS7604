
Project
  Image Classification ของขนมไทยทั้งหมด 10 ชนิด

Introduction
  Image Classification ของขนมไทยทั้งหมด 10 ชนิด โดยใช้ ImageNet Pre-trained CNN 
  โดยทำในลักษณะของ Fine-Tuning Transfer Learning ซึ่งจะทำการเปรียบเทียบประสิทธิภาพและประสิทธิผล
  ทั้งหมด 5 Models ประกอบด้วย VGG-16, ResNet152V2, MobileNet, DenseNet121 และ EfficientNetB0
  และการทำ Class Activation Mapping (CAM) เพื่อตรวจสอบว่า Model ได้ตรวจจับอยู่ในบริเวณของวัตถุหรือไม่


Dataset - 10 Classes of Thai Dessert
  1. Banana In Coconut Milk - Kluay Buat Chi (กล้วยบวชชี)
  2. Deep-Fried Rice Flour  - Fak Bua (ฝักบัว)
  3. Durian Sticky Rice     - Khao Niao Tu-rean (ข้าวเหนียวทุเรียน)
  4. Pandanus Pudding in Coconut Cream  - Piak Poon Krati Sod (เปียกปูนกระทิสด)
  5. Rice Balls in Sweet Coconut Milk   - Bua Loy (บัวลอย)
  6. Sweet Sticky Rice with Thai Custard - Khao Niao Sangkhaya (ข้าวเหนียวสังขยา)
  7. Tapioca Balls with Pork Filling    - Saku Sai Moo (สาคูไส้หมู)
  8. Thai Crispy Pancake topped with Golden Threads -  Khanom Buang Foi Thong (ขนมเบื้องฝอยทอง)
  9. Thai Style Fried Savory Dumplings with Fish Filling  - Pan Sib (ปั้นสิบ, ปั้นขลิบ)
  10. Toddy Palm Cake   - Khanom Tan (ขนมตาล)


Files Desciption
  1. Dataset ขนมไทย 10 Classes แต่ละ Class 200 รูป ทั้งหมดประมาณ 2,000 รูป
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



  12. Traditional_ML.ipynb: Source code of traditional machine learning (Random Forest Classifier) model
  13. churn_localcontractor.csv: Input data (Structured data)
  14. Report.pdf: Model comparison and recommendation

Members Percent Contribution and Responsibility
6220421004 Suwant Te (20%)
  -EDA and feature selection
  -training and tuning ML model
  -write pros and cons
  -write recommendation
6220421005 Ratchanat Sa (20%)
  -training and tuning MLP model
  -write pros and cons
  -write recommendation
6220421007 Manadda Ja (20%) 
  -provide dataset and giving dataset detail
  -training and tuning ML model
  -write ML report
  -write pros and cons
  -write recommendation 
6220422017 Kittipan Pi (20%)
  -training and tuning MLP model
  -retrain MLP model
  -write pros and cons
  -write recommendation 
6220422046 Krittin Sa (20%)
  -training and tuning MLP model
  -write MLP report
  -write discussion
  -write recommendation
