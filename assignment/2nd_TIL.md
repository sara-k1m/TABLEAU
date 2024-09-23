# Second Study Week

- 10강: [차원과 측정값](#10강-차원과-측정값)

- 11강: [시각화](#11강-시각화)

- 12강: [막대그래프](#12강-막대그래프)

- 13강: [누적막대그래프](#13강-누적막대그래프)

- 14강: [병렬막대그래프](#14강-병렬막대그래프)

- 15강: [누적병렬막대그래프](#15강-누적병렬막대그래프)

- 16강: [라인그래프](#16강-라인그래프)

- 17강: [맵작성](#17강-맵작성)

- 18강: [텍스트테이블](#18강-텍스트테이블)

- 19강: [트리맵과 하이라이트테이블](#19강-트리맵과-하이라이트테이블)

- 문제1 : [문제1](#문제1)

- 문제2 : [문제2](#문제2)

- 참고자료 : [참고자료](#참고-자료)



## Study Schedule

| 강의 범위     | 강의 이수 여부 | 링크                                                                                                        |
|--------------|---------|-----------------------------------------------------------------------------------------------------------|
| 1~9강        |  ✅      | [링크](https://youtu.be/3ovkUe-TP1w?si=CRjj99Qm300unSWt)       |
| 10~19강      | ✅      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=75)       |
| 20~29강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=65)       |
| 30~39강      | 🍽️      | [링크](https://www.youtube.com/watch?v=e6J0Ljd6h44&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=55)       |
| 40~49강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=45)       |
| 50~59강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=35)       |
| 60~69강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=25)       |
| 70~79강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=15)       |
| 80~89강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=5)        |


<!-- 여기까진 그대로 둬 주세요-->
<!-- 이 안에 들어오는 텍스트는 주석입니다. -->

# Second Study Week

## 10강: 차원과 측정값

<!-- 차원과 측정값에 관해 배우게 된 점을 적어주세요 -->
데이터의 열을 필드로 만들고 데이터의 유형에 따라 필드를 차원 또는 측정값으로 할당한다.

차원과 측정값은 영역을 기준으로 구분하고 불연속은 파란색과 녹색으로 구분한다.

> **🧞‍♀️ 차원과 측정값의 고유한 특성에 대해 설명해주세요.**

```
차원: 정성적인 값을 가진 필드로 집계되거나 개산되지 않는 독립적인 필드이다. 기본적으로 불연속형 필드. (이름, 카테고리 등)
측정값: 정량적인 값을 가진 필드로 집계될 수 있는 값을 가진다. 기본적으로 연속형 필드. (매출 수익 등)
```

*Quiz: 차원은 불연속형이고, 측정값은 연속형이다 (x)*

- 차원이 연속형 필드가 될 수도 있다. 시각화하고자 하는 방식에 짜라서 필드를 적절히 활용할 수 있어야 한다.

## 11강: 시각화

<!-- 시각화 관해 배우게 된 점을 적어주세요 -->
필드 추가 방법</br>
* 더블 클릭
* 열, 행 선반으로 드래그&드롭
* ctrl 누르고 필드 선택 후 시트로 필드 추가 
* 마크창 활용

*Quiz: 차원은 대부분 불연속형이며 표 형태로 시각화했을 때 머리글로 표시되고, 측정값은 대부분 연속형이므로 표 형태로 시각화 진행했을 때 패널로 추가된다.(o)*

## 12강: 막대그래프

<!-- 막대그래프에 관해 배우게 된 점을 적어주세요 -->
![2nd_TIL#12](./img/2nd_TIL12.png)

## 13강: 누적막대그래프

<!-- 누적막대그래프에 관해 배우게 된 점을 적어주세요 -->
![2nd_TIL#13](./img/2nd_TIL13.png)
<!-- 테이블(아래로)와 테이블(옆으로)의 계산 방식을 습득해보세요. 이에 관련해 아래 참고자료도 있습니다 :) -->
```
테이블(옆으로)는 카테고리 전체 합을 기준으로 백분율을 계산하고
테이블(아래로)는 개별 카테고리별로 백분율을 계산한다.
```

## 14강: 병렬막대그래프

<!-- 병렬막대그래프에 관해 배우게 된 점을 적어주세요 -->
![2nd_TIL#14](./img/2nd_TIL14.png)
데이터 유형 변경 시 데이터 원본을 변경하면 표현하려는 뷰마다 데이터를 변경해야한느 번거로움과 데이터 유형 간 충돌 발생 위험이 있다. 그러므로 표시하려는 데이터 뷰에서 변경하는 것이 좋다.

![그라데이션](https://github.com/yousrchive/BUSINESS-INTELLIGENCE-TABLEAU/blob/main/study/img/2nd%20study/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202024-09-12%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%201.54.19.png?raw=true)

> *🧞‍♀️ 끊어진 색상으로 배치되어 표현되는 경우와 이어지는 그라데이션 색으로 표현되는 경우 두 가지가 있습니다. 위 사진의 경우 왜 색깔이 끊어지는 색상으로 표시되지 않고 그라데이션으로 표시되었나요? 데이터의 특성과 관련하여 이야기해 봅시다.*

```
데이터 유형이 연속형이기 때문이다.
```

## 15강: 누적병렬막대그래프

<!-- 누적병렬막대그래프에 관해 배우게 된 점을 적어주세요 -->
![2nd_TIL#15_1](./img/2nd_TIL15_1.png) |![2nd_TIL#15_2](./img/2nd_TIL15_2.png)
--| --|

![screen](https://github.com/yousrchive/BUSINESS-INTELLIGENCE-TABLEAU/blob/main/study/img/2nd%20study/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202024-09-12%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%201.57.52.png?raw=true)


> *🧞‍♀️ 위 사진에서는 Profit과 Sales를 측정값으로 두었습니다.  개별 칼럼(태블로에서는 #필드라 명칭합니다)을 열/행에 두는 대신, '측정값'을 사용하고 측정값 선반에 필드를 올려둡니다. 이런 방식을 사용하는 이유가 무엇일지, 어떻게 사용할 수 있을지 고민해보세요*

```
'측정값' 선반을 사용하여 Profit과 Sales 두 값을 모두 포함한 시각화를 만들 수 있으며 데이터를 한 번에 비교할 때 효과적입니다. 
```

<!-- 정답은 없습니다 -->

## 16강: 라인그래프

<!-- 라인그래프에 관해 배우게 된 점을 적어주세요 -->
![2nd_TIL#16](./img/2nd_TIL16.png)

## 17강: 맵작성

<!-- 맵차트 관해 배우게 된 점을 적어주세요 -->
![2nd_TIL#17_1](./img/2nd_TIL17_1.png)
![2nd_TIL#17_2](./img/2nd_TIL17_2.png)
![2nd_TIL#17_3](./img/2nd_TIL17_3.png)

```js
## 참고
Country/Region - 나라/지역
State/Province - 시/도
City - 시
County - 군
Postal Code - 우편번호
Area Code - 지역 코드
Airport - 공항
MSA/CBSA (Metropolitan Statistical Area) - 광역 통계 지역
Longitude - 경도
Latitude - 위도
```

## 18강: 텍스트테이블

<!-- 텍스트테이블에 관해 배우게 된 점을 적어주세요-->
![2nd_TIL#18](./img/2nd_TIL18.png)

## 19강: 트리맵과 하이라이트테이블
![2nd_TIL#19_1](./img/2nd_TIL19_1.png) |![2nd_TIL#19_2](./img/2nd_TIL19_2.png)
--| --| --|

```
트리맵을 사용할 때에는 나타내야하는 데이터의 수를 잘 조절해야 함
```

> *🧞‍♀️하이라이트 테이블 등에서 두개 이상의 측정값을 사용하는 경우, 함께 색을 표현하게 되면 단위가 달라 정확한 값을 표현할 수 없습니다. 이때 클릭해야 하는 항목은?*

```
별도의 범례 사용
```
![2nd_TIL#19_3](./img/2nd_TIL19_3.png) |![2nd_TIL#19_4](./img/2nd_TIL19_4.png)|![2nd_TIL#19_5](./img/2nd_TIL19_5.png)
--| --|

## 문제1

```js
지민이는 superstore의 한국 수출 관리 업무를 맡고 있습니다. 국가/지역이 우리나라, 즉 'South Korea'인 데이터만을 필터링하여, 상품 하위범주 별로 각 하위범주가 매출의 비율 중 얼마만큼을 차지하는지를 트리맵으로 확인하고 싶습니다. 트리맵의 각 네모 안에 표시되는 텍스트에는 **해당 범주의 이름과 전체에서 해당 범주가 차지하는 비율**이 표시되었으면 합니다.

지민이를 도와주세요! (풀이를 찾아가는 과정을 기술해주세요)
```


![2nd_TIL_Q1_1](./img/2nd_TIL_Q1_1.png)
```
'South Korea'인 데이터만을 필터링
```
![2nd_TIL_Q1_2](./img/2nd_TIL_Q1_2.png)
```
하위 범주 이름, 전체 중 차지 비율을 표시한 트리맵
```

## 문제2

```js
주현이는 국가/지역별로 매출과 수익의 증감을 시간에 흐름에 따라 표현하고자 합니다. 특히 **한국/중국/일본**을 비교하고자 해당 3국을 남기고 필터링했고, 3개 국가를 매출과 수익이라는 두 가지 지표로 확인해보았습니다.

아래는 위 설명을 표현해본 예시입니다.
```

![스크린샷](
https://github.com/yousrchive/BUSINESS-INTELLIGENCE-TABLEAU/blob/main/study/img/3rd%20study/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202024-09-12%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%203.13.22.png?raw=true)

```js
레퍼런스와 꼭 같지 않아도 자유롭게 표현하고, 그 과정을 기술해주세요.
```


![2nd_TIL_Q2_1](./img/2nd_TIL_Q2_1.png)
```
'South Korea, China, Japan'인 데이터만을 필터링
```
![2nd_TIL_Q2_2](./img/2nd_TIL_Q2_2.png)
```
열에 필터의 국가 지역 드래그&드랍, 분기 추가 후 연속형 범주(분기)로 변경
행에 매출, 수익 추가 후 이중축 설정하여 두 필드를 한번에 비교
```

### 참고 자료

```js
테이블 계산에서 '다음을 사용하여 계산'에는 테이블 당 계산과 패널 당 계산이 있습니다. 이에 대해 이해하는 것이 꼭 필요하기 때문에, 외부 레퍼런스를 참고하여 이 단계에서 꼭! 학습 후, 넘어가주세요 :)
```

![테이블계산](https://velog.velcdn.com/images/eunsuh/post/8a56ab15-930d-4ad6-b5ab-74513863115f/image.png
)

[참고 외부자료 링크는여기를클릭하십시다](https://velog.io/@eunsuh/Tableau-%EB%A0%88%EB%B2%A8UP-%EA%B0%95%EC%9D%98-%EC%A0%95%EB%A6%AC-1-%ED%85%8C%EC%9D%B4%EB%B8%94-%EA%B3%84%EC%82%B0)