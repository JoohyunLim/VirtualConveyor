# 인공지능 기반 분리수거 자동화 시스템 #

### 작품 소개 ###
> 분리수거 처리장에는 잘못된 분리배출로 인해 <b>쓰레기의 약 2~30%만이 재활용</b>되고 있으며, 제대로 된 재활용 폐기물을 선별하기 위한 별도의 선별작업이 필요하다. 사람이 직접 일일이 쓰레기를 선별하거나 비중관리선별기 등의 기계를 활용하고 있으나, 노동력과 비용적인 문제가 존재한다. 이 문제를 해결하고, 분리수거 시스템에 공학적으로 접근해보고자 <b>인공지능 기반 분리수거 자동화 컨베이어벨트</b>를 제작하고자 하였다. 
<br>
<img src = "https://user-images.githubusercontent.com/78129187/132122004-2bc32f8d-b29b-41f0-b912-a64fae7743c3.JPG" width="50%">
https://www.youtube.com/watch?v=f2Fym_h2EWw
<br><br>

### 기술 ###
> * <b>YOLO custom 모델 학습</b><br>
폐기물 분류에 적합한 class들을 선정하여 본 프로젝트의 목적에 맞는 YOLOv4 모델을 학습시켰다.

> * <b>빛 반사율 및 무게를 활용한 재질 판단 알고리즘</b> <br>
암실 환경에 조명을 설치해두고, 물체를 넣었을 때 물체가 빛을 반사해내는 정도를 활용하여 재질을 판단하였다. (조명으로 명확한 판별이 불가능할 경우 무게 기반의 분류 알고리즘도 도입함)
<br>
<p align="center">
<img src = "https://user-images.githubusercontent.com/78129187/150170429-6a7a0ad4-7adc-48aa-839b-69bb0ea7094a.png" width="60%">
</p><br>

> * <b>Unity 가상 컨베이어벨트</b> <br>
최근 주목받고 있는 디지털트윈 기술을 활용해 실제 선별장과 동일한 환경을 Unity 가상 환경에 제작하여 다양한 시뮬레이션을 진행하였고, 이 과정에서 본 기술을 실제 현장에 도입했을 때 발생할 수 있는 크고 작은 문제 상황들에 대해 파악하였다.
<br>
<p align="center">
<img src = "https://user-images.githubusercontent.com/78129187/150169683-e10845bd-bb4d-483e-a7cd-d4694ddefb29.jpg" width="60%">
</p><br>

> * <b>웹 & 앱서비스</b> <br>
서버와 데이터베이스를 구축하고, 관리자를 위한 웹 서비스 및 모바일 앱을 제작하였다. 실시간으로 재활용 현황을 알 수 있도록 ‘현재 재활용률’, ‘총 폐기물의 수’ 등의 데이터를 제공하고, 오류 발생 시 모바일 앱에 푸시 알림을 보내 빠른 대응이 가능하도록 개발하였다.
<br>
<p align="center">
<img src = "https://user-images.githubusercontent.com/78129187/150173054-2a0a59ab-3f65-4247-a17a-99bbd980b9d7.png" width="60%">
</p><br>
<br>
✔ 웹서비스 github
<br>
https://github.com/Jungchaeyeon/VirtualTrashCollectionConveyorbelt
<br><br>
✔ 재질판별 알고리즘 github
<br>
https://github.com/kim474/openCV_python
