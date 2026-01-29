# Image-Classification-using-MobileNetV2-with-Transfer-Learning
ระบบจำแนกภาพประสิทธิภาพสูงด้วย MobileNetV2 และ Transfer Learning (ImageNet) ออกแบบเพื่ออุปกรณ์ทรัพยากรจำกัด ใช้ Data Augmentation เพิ่มความแม่นยำด้วยการหมุนและซูมภาพ โครงสร้างใช้ Global Average Pooling ลด Overfitting และ Output ด้วย Sigmoid รองรับการทำนายผลพร้อมแสดง Confidence Score ในตัว

<div align="center">
  <h1>Coconut: Image Classification Project</h1>
  <p><b>MobileNetV2 Implementation with Transfer Learning</b></p>
  
  <img src="https://img.shields.io/badge/Model-MobileNetV2-blue" alt="Model">
  <img src="https://img.shields.io/badge/Framework-TensorFlow-orange" alt="Framework">
  <img src="https://img.shields.io/badge/Task-Classification-green" alt="Task">
</div>

<hr>

### 1. บทนำ (Introduction)
<p>
โปรเจกต์ <b>Coconut</b> เป็นระบบจำแนกรูปภาพประสิทธิภาพสูงที่สร้างขึ้นบนสถาปัตยกรรม <b>MobileNetV2</b> โดยใช้เทคนิค <b>Transfer Learning</b> จากชุดข้อมูล ImageNet เพื่อให้ได้โมเดลที่มีขนาดเล็ก ประมวลผลได้รวดเร็ว และรักษาความแม่นยำในระดับสูง เหมาะสำหรับการใช้งานในสภาพแวดล้อมที่มีทรัพยากรจำกัด
</p>

### 2. คุณสมบัติทางเทคนิค (Technical Specifications)
<ul>
  <li><b>Architecture:</b> MobileNetV2 (Pre-trained Weights)</li>
  <li><b>Optimization:</b> ใช้การถ่ายโอนความรู้เพื่อลดระยะเวลาการฝึกฝนและเพิ่มความสามารถในการจำแนก</li>
  <li><b>Data Augmentation:</b> มีการปรับแต่งข้อมูลภาพด้วยเทคนิค Rotation, Width/Height Shift, Shear, Zoom และ Horizontal Flip</li>
  <li><b>Inference System:</b> รองรับการวิเคราะห์ภาพเดี่ยวพร้อมแสดงค่าความมั่นใจ (Confidence Score)</li>
</ul>



### 3. โครงสร้างของโมเดล (Model Architecture)
<table>
  <thead>
    <tr>
      <th>Layer Type</th>
      <th>Details / Parameters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>Base Model</b></td>
      <td>MobileNetV2 (Feature Extractor)</td>
    </tr>
    <tr>
      <td><b>Pooling Layer</b></td>
      <td>Global Average Pooling 2D</td>
    </tr>
    <tr>
      <td><b>Final Output</b></td>
      <td>Dense Layer (Sigmoid Activation)</td>
    </tr>
  </tbody>
</table>

### 4. วิธีการทำงาน (Workflow)
<ol>
  <li><b>Data Preprocessing:</b> ปรับขนาดภาพเข้าที่ 224x224 พิกเซล และทำการ Rescale ค่าพิกเซลให้อยู่ในช่วง 0-1</li>
  <li><b>Training:</b> ใช้ชุดข้อมูลจากระบบไฟล์ที่แบ่งหมวดหมู่ไว้ชัดเจนผ่าน ImageDataGenerator</li>
  <li><b>Evaluation:</b> แสดงผลการทำนายผ่านกราฟิก Matplotlib พร้อมระบุระดับความเชื่อมั่นของโมเดล</li>
</ol>

<hr>

<p align="center">
<i>Documentation for Project Coconut | Developed for Professional Use</i>
</p>
