# ***Tri-Scene-Real_2025***

本研究採用三目相機的立體相機系統，其架構主要延續由Sung-Yao Lan所提出的設計 L_Tri_PSMN。使用的攝影機為 logitech C310，並如下圖所示，左右鏡頭與上下鏡頭間的光心距離皆設為 7.5 公分。在以照相者觀點定左右的假設下，我們將左側攝影機視為基準視角，並透過空間座標轉換的方式，將由 LiDAR 相機所推算出的深度資訊對齊至基準相機的座標架構之中。   
<img src="https://github.com/user-attachments/assets/26fd5fc9-4d6a-4a44-8dab-eab033356cd5" width="50%">  
深度相機: Intel RealSense Lidar Camera L515  
相機配置: L型三目相機  
參考相機: 左相機  
Baseline =7.5cm(左右、左下光心)   

資料集涵蓋了無人機真實世界飛行中可能遇到的多種典型環境，如宅區的電線、大樓、天空以及7公尺外的遠距離障礙物，更貼近實際應用需求。   
資料集分為兩種方式來建立   
1: 7公尺以內使用Intel RealSense Lidar Camera L515   
2: 7公尺以上使用:L_Tri_PSMN預測搭配雷射測距儀驗證其準確度   

以下展示使用Intel RealSense Lidar Camera L515所建立資料集範例，左圖為參考相機RGB圖、右圖為Ground Truth   

<img width="701" height="794" alt="1222222222222222" src="https://github.com/user-attachments/assets/d32b0702-6f2d-405e-940c-b900ff2e7395" />   


這邊則展示使用L_Tri_PSMN預測搭配雷射測距範例。  

<img width="705" height="518" alt="12222222" src="https://github.com/user-attachments/assets/449a8fd5-e916-4bcb-b7f3-9ad06fc4df7a" />   



資料集總共586組，分別為481組的Traning和104組的Testing   


Reference  
***潘裕升., & Pen, Y.-S. (2024). 建立三目深度相機導航環境與製作含水平線的現實場景資料集= Establishing a Trinocular Depth Camera Navigation Environment And Producing a Realistic Scene Dataset Containing Horizontal Lines. 國立中興大學.***  
***徐明志., & Hsu, M.-C. (2023). 偵測水平線的三目相機立體視覺: 演算法= Trinocular Vision to See Horizontal Wires: Algorithm. 國立中興大學.***  
***蘭松耀., & Lan, S.-Y. (2023). 偵測水平線的三目相機立體視覺: 現實世界測試= Trinocular Vision To See Horizontal Wires: Real World Testing. 國立中興大學.***  
