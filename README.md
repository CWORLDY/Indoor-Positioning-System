**该项目资源仅限学习，作者能力有限 若有建议 请留言**




# 项目简介
“面向室内场馆的智能定位系统”是一个能够针对多种室内场景，采用低功耗蓝牙（Bluetooth Low Energy, BLE）/MEMS融合技术，达到低功耗性能，实现高精度定位功能的室内定位系统。该系统的创新点在于自适应布局信号接入点（Access Point，AP）、快速构建位置指纹数据库、指纹库自动更新和精准定位算法等，避免了传统指纹定位系统的指纹库构建工作繁重、保持高定位精度困难等缺点。  
实验结果表明，本系统利用自主设计的服务器及手机终端APP，能够对多种室内环境自适应快速部署定位系统并保持较高的定位精度。相比传统的指纹定位系统，本套定位系统的建库工作量减小80%以上，定位精度达到1.5米，实时响应时间为1秒。综上，本作品积极响应国家对导航与位置服务的新要求和节能减排的战略需求，成功研制了一整套智能定位系统，实现低功耗性能，同时突破了多项室内高精度定位关键技术问题，具有较大的应用前景。


<div align=center>

![1](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/2.png)    

  
![2](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/9.png)      


![3](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/1.png)    
  
<div align=left>       
  
## 主要工作
1 **提出自适应AP布局算法**  
     提出一种基于贪心算法的自适应AP布局算法，以仿真指纹库的区分度为目标函数优化AP布局，经过多次迭代达到最优布局或者接近最优布局，较传统布局方法准确性更高且节约大量成本。  
2 **快速构建位置指纹数据库**  
     提出一种快速采集指纹联合径向基函数插值的建库方法。在目标环境中动态采集部分指纹样本，然后利用径向基函数插值算法对指纹库进行扩充建立完整指纹库，建库时间开销较普通建库方法减小80%以上。   
3 **指纹库自适应更新**  
     提出一种指纹数据库更新算法，使初期建立的指纹库一直保持较高的定位精度  
4 **室内高精度融合定位**  
     基于BLE定位结果和MEMS定位结果，选择扩展卡尔曼滤波器对两者进行融合定位，可达到1.5米以内的定位精度。


# 框架原理
本系统主要由四个模块组成，分别为速度与航向角解算模块、蓝牙指纹定位模块、融合定位模块和指纹库自适应更新模块。



<div align=left>    
  
**系统框架**     

  <div align=center>
  
  
![4](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/3.png)        

     
<div align=left>    
  
**速度解算**   

<div align=center>



  ![5](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/4.png)       
       
      
  
<div align=left>    
  
 **MEMS航向解算**   

<div align=center>
 
 
![6](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/5.png)     
        
      

<div align=left>    
  
   **指纹建库**   

<div align=center>
  
  ![7](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/6.png)    
       
       
<div align=left>    
  
**指纹库更新**  

<div align=center>
  
  ![8](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/7.png)    
    
<div align=left> 
    
# 实验结果


<div align=left>    
  
 **融合定位**   

<div align=center> 



![7](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/16.png)  


![7](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/17.png)  
    
      

<div align=left>    
  
 **指纹库自适应更新**    

<div align=center> 

    
![8](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/14.png)  
  
  ![9](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/15.png)  
        
           
  
<div align=left>    
  
 **快速构建位置指纹数据库**    

<div align=center> 


 
![10](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/13.png)  
       
       
       
   
<div align=left>    
  
  **自适应AP布局**    

<div align=center>       
  
![11](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/10.png)
  
 ![12](https://github.com/CWORLDY/Indoor-Positioning-System/blob/master/document/experiment%20photo/12.png)  
   

