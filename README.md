# Slip-Robust InEKF for Wheeled Robots

This project aims to estimate the states of a wheel robot in outdoor environments using IMU data, wheel encoder data. An InEKF based approach is taken to achieve the objective. This project is developed based on the ["Legged Robot State Estimation in Slippery Environments Using Invariant Extended Kalman Filter with Velocity Update"](https://arxiv.org/abs/2104.04238) and the open source code of ["In-EKF"](https://github.com/RossHartley/invariant-ekf).

<p align="center">
  <img width="750" height="500" src="results/husky_new_inekf.PNG">
</p>


## Getting Started
To run the Python code, the following environment and dependencies are required: 
- Python == 3.6
- numpy == 1.20.3
- matplotlib == 3.4.3
- scipy == 1.7.1
- pandas == 1.3.4

## Code organization
    .
    ├── results                     # Folder contains final results images
    ├── src                         # Matlab and Python scripts
    │   ├── Matlab                  # Matlab scripts
    │   │   ├── main.m              # Main script of state estimation with In-EKF in indoor environment
    │   ├── Python                  # Python scripts
    │   │   ├── helper_func.py          # Helper function
    │   │   ├── husky_inekf_indoor.py   # Main script of state estimation with In-EKF in indoor environment
    │   │   ├── husky_inekf_light.py    # Main script of state estimation with In-EKF in parking lot environment
    │   │   ├── inekf_imu_cameraPos.py	# In-EKF with encoder and camera measurements
    └── README.md

## Running the code
To run the Python code, run `husky_inekf_light.py`for parking lot environment

To run the Matlab code, run `main.m`for parking lot environment
<!-- or `husky_inekf_indoor.py` for indoor environment. -->


## Implementations

* See the [report](ROB_530_Team_13_Project.pdf) for detailed implementations.

## Results

The following video shows how our proposed algorithms (encoder-only and encoder-pseudo measurement) work well compared to ORB-SLAM2, Visual Odometry and GPS.

<p align="center">
  <img src="results/final_gif.gif" alt="animated" />
</p>



## Contributors
* Theodor Chakhachiro: [Github](https://github.com/Theochiro), [Linkedin](https://www.linkedin.com/in/teochiro/), [Google Scholar](https://scholar.google.com/citations?user=GFfVbcQAAAAJ&hl=en), [Homepage](https://theodorchakhachiro.netlify.app/)

* Ryan Feng: [Linkedin](https://www.linkedin.com/in/ryan-feng-54646722a/), [Homepage](https://rzfeng.xyz/)

* Vladimir Krokhmal: [Github](https://github.com/VladKrokhmal), [Linkedin](https://www.linkedin.com/in/krokhmalvladimir/)

* Xihang Yu: [Github](https://github.com/XihangYU630), [Linkedin](https://www.linkedin.com/in/xihang-yu-291511207/)

* Hongyu Zhou: [Github](https://github.com/Hongyu-ZHOU), [Linkedin](https://www.linkedin.com/in/hongyu-zhou-2398761a9/), [Google Scholar](https://scholar.google.com/citations?user=byfB4H8AAAAJ&hl=en&authuser=1), [Homepage](https://hongyu-zhou.github.io/)

<!-- <a href = "https://github.com/XihangYU630">
  <img src = "https://avatars.githubusercontent.com/u/94797458?s=48&v=4.png?size=50"/>
</a>

<a href = "https://github.com/Theochiro">
  <img src = "https://avatars.githubusercontent.com/u/74928553?s=48&v=4.png?size=50"/>
</a>

<a href = "https://github.com/Hongyu-ZHOU">
  <img src = "https://avatars.githubusercontent.com/u/62939586?s=48&v=4.png?size=50"/>
</a> -->

<!-- <iframe src="https://umich-my.sharepoint.com/personal/teochiro_umich_edu/_layouts/15/Doc.aspx?sourcedoc={b58d029a-1b85-45da-8555-0aa1cb9df0c2}&amp;action=embedview&amp;wdAr=1.7777777777777777" width="476px" height="288px" frameborder="0">This is an embedded <a target="_blank" href="https://office.com">Microsoft Office</a> presentation, powered by <a target="_blank" href="https://office.com/webapps">Office</a>.</iframe> -->
<!-- <p align="center">
  <img width="800" height="500" src="result/path1.png">
</p>
<p align="center">
  <img width="800" height="500" src="result/gif1.gif">
</p>
<p align="center">
  <img width="800" height="500" src="result/path1_3d.png">
</p>
Results for data set 2 (Downtown):
<p align="center">
  <img width="800" height="500" src="result/path2.png">
</p>
<p align="center">
  <img width="800" height="500" src="result/gif2.gif">
</p>
<p align="center">
  <img width="800" height="500" src="result/path2_3d.png">
</p>
Results for data set 3 (Rural Area):
<p align="center">
  <img width="800" height="500" src="result/path3.png">
</p>
<p align="center">
  <img width="800" height="500" src="result/gif3.gif">
</p>
<p align="center">
  <img width="800" height="500" src="result/path3_3d.png">
</p> -->
