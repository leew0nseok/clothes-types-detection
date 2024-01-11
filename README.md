# 패션 이미지를 보고 패션 아이템 탐지 프로젝트
> OOTD, 착샷 등 패션에 관한 스타일 이미지를 보고 어떤 옷 종류에 해당하는지 탐지하는 프로젝트 

데이터 수집부터 라벨링까지 직접 해보고싶어 진행한 프로젝트입니다.
프로젝트 아이디어와 전체적인 진행은 아래 블로그 포스트를 보고 진행했습니다.

1200장을 수집하였지만 라벨링을 직접 진행해 Object Detection 프로젝트를 진행하려고했지만 수집부터 라벨링, 훈련을 진행하는 경험을 해보고자 약 270장의 데이터만 라벨링 후 훈련에 사용하였습니다.

https://velog.io/@kimsoohyun/18%EC%9D%BC-%EC%B0%A8-YOLO-Mini-Project
## 데이터 수집

[무신사 브랜드 스냅](https://www.musinsa.com/mz/brandsnap) 에서 크롤링 코드를 통해 이미지를 수집하였습니다.



## 데이터 라벨링

데이터 라벨링은 LabelImg를 통해 진행하였습니다.

(https://github.com/tzutalin/labelImg)

<img width="1626" alt="image" src="https://github.com/leew0nseok/clothes-types-detection/assets/101381258/55224abd-cba9-47b6-a696-0cb163b9b54f">


다음과 같이 진행하였으며 라벨은 32개로 아래와 같습니다.

<details>
  <summary>Label</summary>
  <div markdown="1">
    <ul>
      <li>Beanie</li>
      <li>Buckethat</li>
      <li>Cap</li>
      <li>Hat</li>
      <li>Glasses</li>
      <li>Coat</li>
      <li>Bubble jacket</li>
      <li>Outer</li>
      <li>Jacket</li>
      <li>Shorts</li>
      <li>Skirt</li>
      <li>Croptop</li>
      <li>T-shirts</li>
      <li>Sweatshirt</li>
      <li>Shirt</li>
      <li>Vest</li>
      <li>Hoodie</li>
      <li>Top</li>
      <li>Jeans</li>
      <li>Training pants</li>
      <li>Pants</li>
      <li>Shoes</li>
      <li>Boots</li>
      <li>Sandal</li>
      <li>Muffler</li>
      <li>Tie</li>
      <li>Mask</li>
      <li>Headphone</li>
      <li>Accessories</li>
      <li>Handbag</li>
      <li>Backpack</li>
      <li>Bag</li>
    </ul>
  </div>
</details>


## 모델

YOLOv5s version

https://github.com/ultralytics/yolov5.git

## 결과

데이터 수집부터 라벨링, 모델 훈련 경험을 얻고싶어서 진행한 프로젝트라서 성능측정이나 이런 부분은 신경쓰지 않고 진행하였다. 

<img width="559" alt="image" src="https://github.com/leew0nseok/clothes-types-detection/assets/101381258/c3cd4a91-91eb-4d47-972d-1332515a9845">

## 결과화면
