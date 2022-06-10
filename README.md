# Ray-Tracing

## DAY 1
### 1. Overview
### 2. Output an Image
#### 2.1. The PPM Image Format
#### 2.2. Creating an Image File
* .ppm 형식을 이용하여 데이터를 시각화 하기

![image](https://user-images.githubusercontent.com/86725870/172625459-aa761851-1355-4f85-932b-1018045c09bc.png)
### 3. The vec3 Class
### 4. Rays, a Simple Camera, and Background
![image](https://user-images.githubusercontent.com/86725870/172440941-b310efdd-dd2e-4ed4-983c-b9d205a8d929.png)
### 5. Adding a Sphere
* 이차방정식을 통해 빛(ray)이 구와 겹치는 부분을 확인하여 빨간색으로 나타냄

![image](https://user-images.githubusercontent.com/86725870/172537389-7987b8ca-56bd-49bd-b61a-7370b6e74076.png)

### 6. Surface Normals and Multiple Normals
* 빛이 없기 때문에 노말값을 시각화하여 구 형태가 나타나도록 함

![image](https://user-images.githubusercontent.com/86725870/172539749-dd5e6e30-3c52-4922-8f7e-fd2294fa046f.png)

![image](https://user-images.githubusercontent.com/86725870/172609554-cff5ea29-fea8-422d-99cb-1ceeb18e3a1e.png)

### 7. Antialiasing
* 안티 앨리어싱 이전과 비교하여 가장자리 픽셀의 차이 발생(좀 더 부드러운 곡선이 생성)
* 각 픽셀 안에 있는 샘플의 묶음을 평균화함으로써 가장자리가 jaggy 한 것을 방지

![image](https://user-images.githubusercontent.com/86725870/172623475-ec45bd65-e99c-417b-9f50-322c6f083767.png)

![image](https://user-images.githubusercontent.com/86725870/173000934-0a3ee038-4e14-45fc-bc1f-0f859221b7ea.png)

