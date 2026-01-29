<div align="center">
  <h1>Project Coconut: Image Classification</h1>
  <p><b>MobileNetV2 Implementation with Transfer Learning for Efficient Visual Recognition</b></p>
  
  <img src="https://img.shields.io/badge/Model-MobileNetV2-blue" alt="Model">
  <img src="https://img.shields.io/badge/Framework-TensorFlow-orange" alt="Framework">
  <img src="https://img.shields.io/badge/Task-Classification-green" alt="Task">
</div>

<hr>

### 1. บทนำ (Introduction)
<p>
<b>Coconut</b> เป็นระบบจำแนกรูปภาพประสิทธิภาพสูงที่สร้างขึ้นบนสถาปัตยกรรม <b>MobileNetV2</b> โดยใช้เทคนิค <b>Transfer Learning</b> จากชุดข้อมูล ImageNet เพื่อให้ได้โมเดลที่มีขนาดเล็ก ประมวลผลได้รวดเร็ว และรักษาความแม่นยำในระดับสูง เหมาะสำหรับการใช้งานในสภาพแวดล้อมที่มีทรัพยากรจำกัด
</p>

### 2. ข้อมูลทางเทคนิค (Technical Specifications)
<ul>
  <li><b>Core Architecture:</b> MobileNetV2 (Pre-trained Weights)</li>
  <li><b>Optimization Strategy:</b> Transfer Learning (Feature Extraction)</li>
  <li><b>Data Augmentation:</b> Rotation, Shift, Shear, Zoom, Flip</li>
  <li><b>Inference System:</b> Graphical Confidence Score Output</li>
</ul>

### 3. โครงสร้างของโมเดล (Model Architecture)
<table width="100%">
  <thead>
    <tr>
      <th align="left">Layer Component</th>
      <th align="left">Description / Details</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>Base Model</b></td>
      <td>MobileNetV2 (Depthwise Separable Convolutions)</td>
    </tr>
    <tr>
      <td><b>Pooling Layer</b></td>
      <td>Global Average Pooling 2D (Prevent Overfitting)</td>
    </tr>
    <tr>
      <td><b>Output Layer</b></td>
      <td>Dense Layer (Sigmoid Activation)</td>
    </tr>
  </tbody>
</table>

### 4. ผลการทดลองและการแสดงผล (Experimental Results)
<table align="center" width="100%" style="border-collapse: collapse; table-layout: fixed;">
  <tr>
    <td align="center" style="padding: 10px; border: 1px solid #ddd; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/0b702ded-f870-45aa-a0f5-5ef0c48e7e4c" alt="Training Performance" style="width: 100%; height: 200px; object-fit: cover;">
      <br><br>
      <div style="min-height: 40px;"><b>Training History</b></div>
      <p align="left" style="font-size: 0.85em; line-height: 1.4;">กราฟแสดงแนวโน้ม Accuracy และ Loss เพื่อประเมินการเรียนรู้และตรวจสอบความเสถียรของโมเดล</p>
    </td>
    <td align="center" style="padding: 10px; border: 1px solid #ddd; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/0e160c1d-9b43-47d2-a634-3bfcbeee7bfc" alt="Augmentation Process" style="width: 100%; height: 200px; object-fit: cover;">
      <br><br>
      <div style="min-height: 40px;"><b>Data Augmentation</b></div>
      <p align="left" style="font-size: 0.85em; line-height: 1.4;">การจำลองความหลากหลายของข้อมูลเพื่อให้โมเดลทำงานได้ดีในสภาวะที่แตกต่างกัน</p>
    </td>
    <td align="center" style="padding: 10px; border: 1px solid #ddd; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/5bac8622-9878-4348-96ca-596fae657c48" alt="Prediction Output" style="width: 100%; height: 200px; object-fit: cover;">
      <br><br>
      <div style="min-height: 40px;"><b>Model Inference</b></div>
      <p align="left" style="font-size: 0.85em; line-height: 1.4;">การทำนายผลลัพธ์จริงพร้อมระบุค่าความเชื่อมั่นทางสถิติจากฟังก์ชัน Sigmoid</p>
    </td>
  </tr>
</table>

### 5. วิธีการดำเนินงาน (Workflow)
<ol>
  <li><b>Preprocessing:</b> ปรับขนาดภาพ 224x224 และ Rescale [0, 1]</li>
  <li><b>Training:</b> ฝึกฝนผ่าน ImageDataGenerator แบบขนาน</li>
  <li><b>Inference:</b> ประมวลผลและแสดงหมวดหมู่ผ่าน Matplotlib</li>
</ol>

<hr>

<div align="center">
  <p><i>Documentation for Project Coconut | Professional Use</i></p>
</div>
