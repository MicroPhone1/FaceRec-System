# FaceRec-System
โครงการนี้เกี่ยวข้องกับการพัฒนาระบบการรู้จำใบหน้าที่ใช้เทคโนโลยีปัญญาประดิษฐ์ (AI) และการเรียนรู้ของเครื่อง (Machine Learning) เพื่อทำให้คอมพิวเตอร์สามารถระบุและจำแนกใบหน้าได้อย่างแม่นยำ ซึ่งมีขั้นตอนหลักๆ ดังนี้:

1.การรวบรวมข้อมูล:
  ข้อมูลใบหน้าได้รับการรวบรวมและจัดเก็บในโฟลเดอร์ที่แยกเป็นกลุ่ม เช่น person1 และ unknown โดยใช้กล้องเพื่อจับภาพใบหน้าและบันทึกเป็นไฟล์รูปภาพ

2.การเตรียมข้อมูล:
  ใช้ ImageDataGenerator ของ TensorFlow เพื่อเพิ่มข้อมูล (Data Augmentation) เช่น การหมุน การเปลี่ยนขนาด และการสะท้อน เพื่อทำให้โมเดลมีความทนทานต่อความหลากหลายของข้อมูล

3.การสร้างและฝึกโมเดล:
  สร้างโมเดล Convolutional Neural Network (CNN) ซึ่งเป็นรูปแบบของโมเดลที่นิยมใช้ในการรู้จำภาพ
ฝึกโมเดลด้วยข้อมูลใบหน้าเพื่อให้มันสามารถจำแนกใบหน้าเป็น "รู้จัก" หรือ "ไม่รู้จัก" ได้

4.การทดสอบระบบ:
  ใช้กล้องเพื่อจับภาพใบหน้าในเวลาจริงและใช้โมเดลที่ฝึกแล้วในการคาดการณ์ว่าใบหน้าที่ตรวจพบเป็นใบหน้าที่รู้จักหรือไม่
แสดงผลลัพธ์ด้วยการวาดกรอบสี่เหลี่ยมรอบใบหน้าและใช้สีวงกลมที่มุมขวาบนของหน้าต่างเพื่อแสดงสถานะ (สีเขียว: ใบหน้าที่รู้จัก, สีแดง: ใบหน้าที่ไม่รู้จัก)

5.การใช้งานและพัฒนาเพิ่มเติม:
  ระบบนี้สามารถนำไปใช้ในหลายๆ แอปพลิเคชัน เช่น ระบบรักษาความปลอดภัย, การจัดการการเข้าถึง, และระบบตรวจสอบผู้ใช้
โครงการนี้มีจุดมุ่งหมายในการสร้างระบบที่สามารถทำงานได้ในเวลาจริงและมีความแม่นยำสูงในการระบุใบหน้า ซึ่งเป็นการนำเทคโนโลยี AI มาประยุกต์ใช้ในชีวิตประจำวันเพื่อเพิ่มความสะดวกและความปลอดภัย

This project focuses on developing a face recognition system that utilizes artificial intelligence (AI) and machine learning technologies to enable computers to accurately identify and classify faces. The key steps involved in the project are as follows:

1.Data Collection:
  Faces are captured and stored in folders, such as person1 and unknown, using a camera to take pictures and save them as image files.

2.Data Preparation:
  TensorFlow’s ImageDataGenerator is used for data augmentation, including operations like rotation, resizing, and flipping, to make the model robust against variations in the data.

3.Model Creation and Training:
  A Convolutional Neural Network (CNN) model is created, a common type of model used for image recognition tasks.
The model is trained with the collected face data to classify faces as "known" or "unknown."

4.System Testing:
  A camera is used to capture real-time face images, which are then fed into the trained model for prediction.
Results are displayed by drawing rectangles around detected faces and using a color-coded circle in the top-right corner of the window to indicate status (green circle for known faces, red circle for unknown faces).

5.Application and Further Development:
  The system can be applied to various applications such as security systems, access control, and user verification.
The project aims to create a real-time system with high accuracy for face identification, showcasing the practical use of AI technology in everyday life to enhance convenience and security.
