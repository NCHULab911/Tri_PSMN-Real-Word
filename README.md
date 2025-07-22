# ***Tri-Scene-Real_2025***

本研究採用三目相機的立體相機系統，其架構主要延續由Sung-Yao Lan所提出的設計 L_tri_PSMN。使用的攝影機為 logitech C310，並如下圖所示，左右鏡頭與上下鏡頭間的光心距離皆設為 7.5 公分。在以照相者觀點定左右的假設下，我們將左側攝影機視為基準視角，並透過空間座標轉換的方式，將由 LiDAR 相機所推算出的深度資訊對齊至基準相機的座標架構之中。   
<img src="https://github.com/user-attachments/assets/26fd5fc9-4d6a-4a44-8dab-eab033356cd5" width="50%">  
深度相機: Intel RealSense Lidar Camera L515  
相機配置: L型三目相機  
參考相機: 左相機  
Baseline =7.5cm(左右、左下光心)   

資料集涵蓋了無人機真實世界飛行中可能遇到的多種典型環境，如宅區的電線、大樓、天空以及7公尺外的遠距離障礙物，更貼近實際應用需求。   

<img width="915" height="419" alt="1222" src="https://github.com/user-attachments/assets/a90ef7a0-869f-46c2-ac4a-ee46c864bdd9" />   
<img width="754" height="288" alt="1222222" src="https://github.com/user-attachments/assets/a0754d6e-6b94-46e8-8e31-a1343d490059" />   

Reference  
***潘裕升., & Pen, Y.-S. (2024). 建立三目深度相機導航環境與製作含水平線的現實場景資料集= Establishing a Trinocular Depth Camera Navigation Environment And Producing a Realistic Scene Dataset Containing Horizontal Lines. 國立中興大學.***  
***徐明志., & Hsu, M.-C. (2023). 偵測水平線的三目相機立體視覺: 演算法= Trinocular Vision to See Horizontal Wires: Algorithm. 國立中興大學.***  
***蘭松耀., & Lan, S.-Y. (2023). 偵測水平線的三目相機立體視覺: 現實世界測試= Trinocular Vision To See Horizontal Wires: Real World Testing. 國立中興大學.***  
