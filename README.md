# Groundwater-Quality-Potential-Database
โปรเจคนี้มีสองส่วนหลักคือ "Groundwater Quality-Potential Database" และ "Phuket Island Map Interpolation".
Groundwater Quality-Potential Database:

โดยส่วนนี้มุ่งเน้นการวิเคราะห์และการแสดงผลข้อมูลคุณภาพน้ำใต้ดิน โดยใช้ข้อมูลจากฐานข้อมูลที่เกี่ยวข้องกับค่าความเข้มข้นของ Cl (chloride) และ TDS (total dissolved solids) ซึ่งเป็นตัวบ่งชี้สำคัญในการประเมินคุณภาพของน้ำใต้ดิน
ฟังก์ชัน determine_zone() ถูกใช้เพื่อกำหนดโซนของคุณภาพน้ำใต้ดินตามค่า Cl และ TDS
ฟังก์ชัน analyze_and_plot() จะทำการวิเคราะห์และพล็อตกราฟสำหรับแต่ละพื้นที่ย่อย (sub-district) โดยแสดงข้อมูล Cl vs TDS พร้อมกับแสดงโซนความเข้มข้นของ Cl และ TDS แต่ละโซนบนกราฟ
Phuket Island Map Interpolation:

ส่วนนี้มุ่งเน้นการสร้างแผนที่ที่มีการประมาณค่าข้อมูลโดยใช้เทคนิคการ interpolation จากข้อมูลจุดบนพื้นผิว Phuket Island
ใช้เทคนิคการ interpolation โดยใช้ Rbf (Radial Basis Function) และ IDW (Inverse Distance Weighting) เพื่อประมาณค่าข้อมูลระหว่างจุดข้อมูลที่มีอยู่
ผลลัพธ์ที่ได้คือแผนที่ที่แสดงค่าที่ประมาณได้บนพื้นผิวของเกาะภูเก็ต รวมถึงการแสดงข้อมูลจุดที่ใช้ในการประมาณค่าลงบนแผนที่ด้วย
