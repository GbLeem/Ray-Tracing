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

### 8. Diffuse material
![image](https://user-images.githubusercontent.com/86725870/173000934-0a3ee038-4e14-45fc-bc1f-0f859221b7ea.png)

* diffuse with gamma correction

![image](https://user-images.githubusercontent.com/86725870/173004545-539da6ca-cfbf-4361-b0aa-25b9cb2d923f.png)

* fix shadow acne

![image](https://user-images.githubusercontent.com/86725870/173004951-7fadf950-076b-4f09-b86c-4e1a88f1c59d.png)
* true lambertian reflection

![image](https://user-images.githubusercontent.com/86725870/173006182-9d417e72-ac9c-4414-b184-c18e2ac915f8.png)
* alternative diffuse formulation

![image](https://user-images.githubusercontent.com/86725870/173007178-3b53a7c9-7f17-4f95-adeb-193acc41d437.png)

### 9. Metal
![image](https://user-images.githubusercontent.com/86725870/173102500-56a23e39-c96c-4d01-a7af-e87494a4becb.png)
* Fuzzy reflection

![image](https://user-images.githubusercontent.com/86725870/173103720-fe7c0b47-0564-4d82-8f36-b62a6d162a26.png)

### 10. Dielectrics
* Glass Sphere that always refracts

![image](https://user-images.githubusercontent.com/86725870/173176107-8425dd4d-c2c6-4552-b55f-81b9bb7e5564.png)
* Total internal refraction -> Glass sphere that sometimes refracts

![image](https://user-images.githubusercontent.com/86725870/173176349-05328ec0-f80d-4449-ad81-2ce32005916f.png)
* A hollow glass sphere by Schlick Approximation

![image](https://user-images.githubusercontent.com/86725870/173176607-b2cc3e95-7e3d-478f-9d7f-37710a290c41.png)
