# Disease-Leaf-2-Layer-Detector
งานนี้เป็นส่วนหนึ่งของโครงการ IRAIC2023(Innovation Robotic AI & IOT Contest 2023) ที่จัดโดยมหาวิทยาลัยเกษตรศาสตร์และได้รับรางวัลรองชนะเริศอันดับ 2 ในหัวข้อ ออกแบบระบบ IoT System สำหรับระบบเกษตร
แม่นยำสูง(Precision Argriculture)

โดย Project จะเกี่ยวกับการสร้าง DashBoard ที่ติดตามค่าสถานะต่างๆของฟาร์มเช่น อุณหภูมิ ความชื้น ความสว่าง รวมถึงการใช้ Deep learning มาประยุกต์ใช้เข้ากับ smart farm เพื่อให้มีประสิทธิภาพมากยิ่งขึ้น

ชื่อทีม:El gato

## DashBoard

DashBoard ที่เราเลือกใช้คือ Grafa(grafana.com) ซึ่งสามารถใช้ได้ดีกับข้อมูลประเภท Real-Time
    

## Sensor

Sensor ทั้งหมดที่เลือกจะแสดงผลมี 7 ตัวได้แก่
    - 
    - 
    - 
    - 
    - 
    - 
    -
    - 

## Dataset
พืชที่ใช้สำหรับการทดสอบคือแตงกวาจึงต้องหา Dataset สำหรับใบแตงกวาสำหรับการ train
Dataset ที่ใช้สำหรับ train แบ่งออกได้เป็น 2 ส่วน:
  - https://www.kaggle.com/datasets/farahseifeld/greenhouse-cucumber-growth-stages (for Object detection model)
  - https://data.mendeley.com/datasets/y6d3z6f8z9/1 (for Classifier model) 

## Model
  - Object detection model ใช้สำหรับตรวจจับใบเพื่อเพิ่มความแม่นยำในการแยก label และ model ที่ใช้คือ YOLOv8(https://github.com/ultralytics/ultralytics)
        ![Yolo Result](images/Yoloresult.png)
    
  - Classifier model หลังจากแยกใบเราจะใช้ model ตัวนี้สำหรับแยกระหว่าง ใบที่ Healthy  และ Unhealthy
        ![Classifier Result](images/ดาวน์โหลด (2).png)

## Last Result
        ![Last Result](images/image (1).png)
