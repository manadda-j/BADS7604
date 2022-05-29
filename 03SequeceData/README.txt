Project
  Human Activity Recognition (HAR) using Traditional Machine Learning and Deep Learning

Introduction
  งานนี้เกี่ยวข้องกับ Human Activity Recognition (HAR) ที่รวบรวมจากเซ็นเซอร์ของ Smartphone เพื่อแบ่งแยก
  ประเภทของกิจกรรมทั้งหมด 6 ประเภท โดยได้เปรียบเทียบประสิทธิภาพของ Model ระหว่าง การใช้ Traditional ML
  อย่าง Logistic Regrssion และ การใช้ Deep Learning ประกอบด้วย LSTM, GRU และ LSTM+CNN

Highlight
  - ในส่วนของ Validation Set จะเห็นได้ว่า Model จากฝั่ง Deep Learning นั้นทำนายข้อมูลได้ดีกว่า Traditional Machine Learning
โดยมี F1 Score อยู่ที่ 0.87 – 0.92 ในขณะที่ฝั่ง Traditional Machine Learning อยู่ที่ 0.80 แต่เมื่อนำ Model ไปทำนายกับ Test Set
ผลลัพธ์กลายเป็นว่า Model จากฝั่ง Traditional Machine Learning สามารถให้ผลลัพธ์ที่ดีกว่า ซึ่งถือได้ว่าผิดคาดจากที่ทางกลุ่ม
ได้ตั้งสมมติฐานไว้ในตอนแรก
  - เมื่อพิจารณาในส่วนของ Confusion Matrix ของทุก Model จะพบว่ากิจกรรมที่ Model สามารถแยกประเภทได้แย่ที่สุดคือ
Downstairs กับ Upstairs อาจเกิดจากข้อมูลของทั้งสองกิจกรรมมีพฤติกรรมที่คล้ายคลึงกันจึงส่งผลให้ Model ทำนายผิด
ในขณะที่กิจกรรมอื่นมีพฤติกรรมที่ชัดเจนเลยสามารถทำนายออกมาได้ถูกต้องแม่นยำกว่า
  - จากการทดสอบของแต่ละ Model กับ Test Set พบว่า Logistic Regression เป็น Model ที่สามารถแยกประเภทกิจกรรม
ได้ดีที่สุด โดยมีค่า F1 Score สูงสุดอยู่ที่ 0.9186 แต่หากพิจารณาในเรื่องของการทำ Feature Engineering ประกอบไปด้วยนั้น
ทางกลุ่มเห็นว่าการใช้ Model Deep Learning อย่าง LSTM+CNN ที่ให้ค่า F1 Score อยู่ที่ 0.9179 นั้นดีกว่าการใช้ Logistic Regression
เพราะประหยัดเวลากว่า และไม่ได้ต้องการที่จะใช้กระบวนการทำงานของ Model ไปอธิบายต่อ 

Dataset
  https://www.cis.fordham.edu/wisdm/dataset.php
  (WISDM_ar_v1.1)

Files Desciption
  1. Folder TraditionalMachine Learning
      ข้อมูลการ Train, Validate, Test และ Result ของLogistic Regression
  2. Folder Deep Leraning
      ข้อมูลการ Train, Validate, Test และ Result ของทั้ง 3 Models ประกอบด้วย
      LSTM, GRU และ LSTM+CNN
  3. Report.pdf
      รายละเอียดทั้งหมดเกี่ยวกับ Project  

Members Percent Contribution and Responsibility
6220421004 Suwant Te (20%)
  -Logistic Regression with Feature Engineering
  -Report
6220421005 Ratchanat Sa (20%)
  -Logistic Regression
  -Report
6220421007 Manadda Ja (20%) 
  -LSTM
  -Report
6220422017 Kittipan Pi (20%)
  -GRU
  -Report
6220422046 Krittin Sa (20%)
  -LSTM+CNN
  -Report
