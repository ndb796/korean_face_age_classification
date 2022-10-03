### Korean Face Age Classification

> 한국인 얼굴이 주어졌을 때 나이(age)를 예측하는 인공지능

#### 데이터 세트 소개

* 전체 데이터 세트는 13,068개의 이미지로 구성된다.
<pre>
F0001_AGE_D_18_a1.jpg
F0001_AGE_D_18_a2.jpg
...
F0900_AGE_M_57_f1.jpg
F0900_AGE_M_57_f2.jpg
</pre>

<img src="/resources/dataset.png" width="600px">

* custom_dataset.csv는 각 이미지에 대한 메타 정보를 가진다.
  * 속성(attribute) 목록: 'family_id', 'person_id', 'age_class', 'image_path'

* 전체 이미지를 학습(training), 검증(validation), 테스트(test) 목적으로 나눈다.
  * 학습 데이터 세트: (F0001 ~ F0299) folders have 10,025 images.
  * 검증 데이터 세트: (F0801 ~ F0850) folders have 1,539 images.
  * 테스트 데이터 세트: (F0851 ~ F0900) folders have 1,504 images.

* 본 저장소에서는 각 이미지와 나이 정보(age class)만 사용한다.
  * 주어진 한 장의 한국인 얼굴 이미지가 어떠한 나이군에 해당하는지 예측한다.

* 데이터 세트 다운로드: [custom_korean_family_dataset_resolution_128.zip](https://postechackr-my.sharepoint.com/:u:/g/personal/dongbinna_postech_ac_kr/EbMhBPnmIb5MutZvGicPKggBWKm5hLs0iwKfGW7_TwQIKg)
* 전체 소스코드 [링크](/age_class_estimation.ipynb)

#### 최종 테스트 결과

<img src="/resources/result.png" width="300px">
