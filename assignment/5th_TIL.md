# Fifth Study Week

- 39강: [LOD](#39강-lod)

- 40강: [EXCLUDE](#40-lod-exclude)

- 41강: [INCLUDE](#41-lod-include)

- 42강 : [매개변수](#42-매개변수)

- 43강 : [매개변수 실습](#43-매개변수-실습) 
![링크](https://youtu.be/GJvB8hBqeE8?si=3jIj1iymZHZ7mBam)

- 44강: [매개변수 실습](#44-매개변수-실습)

- 45강: [마크카드](#45-워크시트-마크카드)

- 46강: [서식계층](#46-서식-계층)

- 47강: [워크시트](#47-워크시트-서식)

- [문제1](#문제-1)

- [문제2](#문제-2)

## Study Schedule

| 강의 범위     | 강의 이수 여부 | 링크                                                                                                        |
|--------------|---------|-----------------------------------------------------------------------------------------------------------|
| 1~9강        |  ✅      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=84)       |
| 10~19강      | ✅      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=75)       |
| 20~29강      | ✅      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=65)       |
| 30~38강      | ✅      | [링크](https://www.youtube.com/watch?v=e6J0Ljd6h44&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=55)       |
| 39~47강      | ✅      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=45)       |
| 48~59강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=35)       |
| 60~69강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=25)       |
| 70~79강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=15)       |
| 80~89강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=5)        |


<!-- 여기까진 그대로 둬 주세요-->

> **🧞‍♀️ 오늘의 스터디는 지니와 함께합니다.**


## 39강. LOD

<!-- INCLUDE, EXCLUDE, FIXED 등 본 강의에서 알게 된 LOD 표현식에 대해 알게 된 점을 적어주세요. -->
Level Of Detail: 뷰의 세부 수준을 나타냄. 계산할 수준을 세부적으로 제어 가능

FIXED: 현재 뷰에 있는 차원과 상관 없이 계산된 필드에서 원하는 차원을 따라 계산

예시)
![5th_TIL39(1)](./img/5th_TIL39(1).png) 1. FIXED에서 설정한 차원 ⊂ 뷰 | ![5th_TIL39(2)](./img/5th_TIL39(2).png) 2. FIXED에서 설정한 차원 ⊄ 뷰
--| --|


![5th_TIL39(3)](./img/5th_TIL39(3).png) <p align="center"> **3. 퀵 테이블 계산을 통해 구성 비율 표현** </p>

## 40. LOD EXCLUDE

<!-- INCLUDE, EXCLUDE, FIXED 등 본 강의에서 알게 된 LOD 표현식에 대해 알게 된 점을 적고, 아래 두 질문에 답해보세요 :) -->
EXCLUDE: 현재 뷰에서 특정 차원을 제외하여 계산할 때 사용

> **🧞‍♀️ FIXED와 EXCLUDE을 사용하는 경우의 차이가 무엇인가요?**

```
- FIXED: 현재 뷰와 상관 없이 특정 차원을 사용하여 계산하기 때문에 필터의 영향X
- EXCLUDE: 뷰에 있는 차원을 따라 계산하기 때문에 관련 차원을 필터로 걸어보면 영향을 받음
```
예시) 제품의 범주 별 매출 보기
![5th_TIL40(1)](./img/5th_TIL40(1).png) | ![5th_TIL40(2)](./img/5th_TIL40(2).png)
--| --|

예시) 하위 범주에 있는 제품 중 한 제품(액세서리) 매출을 기준으로 다른 제품들의 매출과 차이 비교
![5th_TIL40(3)](./img/5th_TIL40(3).png)
> **🧞‍♀️ 왜 ATTR 함수를 사용하나요?**

***SUM([매출]) - ATTR([EXCLUDE 하위 범주 매출])***

```
- ATTR: 그룹의 모든 행에 대해 단일 값만 포함하면 주어진 식의 값을 반환하고, 그렇지 않으면 (*)표시. 
- 여기서는 각 제품들의 매출과 액세서리의 매출 차이를 계산하기 위해 사용 되었는데,
  [EXCLUDE 하위 범주 매출]이 단일 값만 반환되도록 하기 위해 사용한다. 
```

## 41. LOD INCLUDE

<!-- INCLUDE, EXCLUDE, FIXED 등 본 강의에서 알게 된 LOD 표현식에 대해 알게 된 점을 적고, 아래 두 질문에 답해보세요 :) -->
INCLUDE: 현재 뷰에서 특정 차원을 추가하여 계산, 차원 필터를 통해 해당 값 변경 가능

예) 각 도시의 고객 당 평균 매출 표시
![5th_TIL41(1)](./img/5th_TIL41(1).png) 분석-총계-평균을 이용한 고객 당 평균 매출 표시| ![5th_TIL41(2)](./img/5th_TIL41(2).png) 주문 ID 차원을 포함한 합계 매출의 평균을 반환:<br>AVG({INCLUDE [주문 Id]:SUM([매출])}) |![5th_TIL41(3)](./img/5th_TIL41(3).png)AVG({INCLUDE [주문 Id]:SUM([매출])})<br>=AVG({FIXED [주문 Id]:SUM([매출])})
--| --| --|

> **🧞‍♀️ 그렇다면 어떤 경우에 각 표현식을 사용하나요? 예시와 함께 적어보아요**

```
뷰에 표시되는 값이 차원이면, 차원과 측정값을 반환할 수 있는 FIXED LOD 표현식만 사용 가능
(측정값만 반환하는 INCLUDE, EXCLUDE 표현식은 사용 불가)

반환 값이 차원 필터의 영향을 받게 되는 경우, 차원 필터에 영향을 받는 INCLUDE, EXCLUDE 표현식 사용
(FIXED 표현식은 차원 필터 영향X)
```

## 42. 매개변수

<!-- 매개변수에 대해 알게 된 점을 적어주세요 -->
매개변수: 고정된 상수 값이 아닌 동적인 값으로 변경하기 위해서 활용하는 기능
반드시 **계산식, 필터, 참조선**과 함께 사용된다.

매개 변수를 만드는 방법
![5th_TIL42(1)](./img/5th_TIL42(1).png) 1. 필터| ![5th_TIL42(2)](./img/5th_TIL42(2).png) 2. 필드 위에 우클릭| ![5th_TIL42(3)](./img/5th_TIL42(3).png) 3. 데이터 패널
--| --| --|

![5th_TIL42(4)](./img/5th_TIL42(4).png)

예시) 매출이 높은 상위 5개 제품 표시하기
![5th_TIL42(5)](./img/5th_TIL42(5).png)| ![5th_TIL42(6)](./img/5th_TIL42(6).png)| ![5th_TIL42(7)](./img/5th_TIL42(7).png)필터를 적용해야 작동!| ![5th_TIL42(8)](./img/5th_TIL42(8).png)
--| --| --| --|

![5th_TIL42(9)](./img/5th_TIL42(9).png)

> **🧞‍♀️ 집합에도 매개변수를 적용할 수 있나요? 시도해봅시다**

![5th_TIL42(10)](./img/5th_TIL42(10).png) | ![5th_TIL42(11)](./img/5th_TIL42(11).png)
--| --|

![5th_TIL42(12)](./img/5th_TIL42(12).png)

## 43. 매개변수 실습
<!-- 영상 묶음에 포함되지 않아 찾기 어려우실까 링크를 아래에 첨부하겠습니다. 수강 후 삭제해주세요-->

https://www.youtube.com/watch?v=GJvB8hBqeE8

## 44. 매개변수 실습

<!-- 매개변수에 대해 알게 된 점을 적어주세요 -->

## 45. 워크시트 마크카드

<!-- 마크카드에 대해 알게 된 점을 적어주세요 -->


## 46. 서식 계층

<!-- 서식계층에 대해 알게 된 점을 적어주세요 -->

> **🧞‍♀️ 서식계층을 일반적인 것에서 구체적인 것 순서로 기입해보세요**


```
여기에 답을 적어주세요!
```


## 47. 워크시트 서식

<!-- 워크시트 서식에 대해 알게 된 점을 적어주세요!-->



## 문제 리스트



## 문제 1.

```
가장 많이 주문한 사람들은 물건 배송을 빨리 받았을까요?
조건을 준수하여 아래 이미지를 만들어봆시다.
1) 국가/지역별(이하 '나라'로 통칭), 범주별로 배송일자가 다를 수 있으니 먼저, 나라별/범주별로 평균 배송일자를 설정한 뒤,
2) 각 나라에서 가장 많이 주문한 사람의 이름을 첫 번째 열,
3) 그 사람이 주문한 제품 이름을 2번째 열,
4) 각 상품이 배송까지 걸린 날 수를 표현하고
5) 그리고 만약 배송이 각 나라/범주별 평균보다 빨랐다면 '빠름', 같다면 '평균', 느리다면 '느림' 으로 print 해주세요. 
```

![이미지주소](https://github.com/yousrchive/BUSINESS-INTELLIGENCE-TABLEAU/blob/main/study/img/2nd%20study/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202024-08-13%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2010.12.36.png?raw=true)

<!-- 여기까지 오는 과정 중 알게 된 점을 기입하고, 결과는 시트 명을 본인 이름으로 바꾸어 표시해주세요.-->

## 문제 2.

```
채원이는 태블로를 쓰실 수 없는 상사분께 보고하기 위한 대시보드를 만들고 싶어요. 

제품 중분류별로 구분하되 매개변수로써 수익, 매출, 수량을 입력하면 저절로 각각 지표에 해당하는 그래프로 바뀌도록 설계하고자 해요.

 어떤 값이 각 지표의 평균보다 낮은 값을 갖고 있다면 색깔을 주황색으로, 그것보다 높다면 파란색으로 표시하고 싶어요. 그 평균값은 각 지표별로 달라야 해요.
```

![example](https://github.com/yousrchive/BUSINESS-INTELLIGENCE-TABLEAU/blob/main/study/img/2nd%20study/%E1%84%83%E1%85%A1%E1%84%8B%E1%85%AE%E1%86%AB%E1%84%85%E1%85%A9%E1%84%83%E1%85%B3.png?raw=true)

<!-- 예시 사진은 지워주세요-->
