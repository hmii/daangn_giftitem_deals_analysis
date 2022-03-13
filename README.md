# daangn_giftitem_deals_analysis
당근마켓 명절 선물세트 미개봉 중고거래 분석

## 개요
- 명절 미개봉 선물세트 중고거래 데이터에서 유용한 인사이트를 도출하다

## 프로젝트 설명
- 명절 기간 당근마켓에 미개봉 선물세트가 쏟아져 나오는 현상을 발견하여 이를 파헤쳐보았다. 
- 연간 및 월간 물량 추이, 끌올, 인기 카테고리, 가격변화, 제목 키워드 가중치, 거래 장소 분석을 진행했다.
- 스팸은 명절 기간 물량이 가장 많음에도 불구하고 가격은 다른 기간보다 10% 높았다. 
- 게시글 제목에는 '마지막', '가격내림'이라는 키워드를 포함하면 관심과 조회수를 모두 높일 수 있었다.
- 이 외에도 관계자, 구매자, 판매자 등 당근마켓을 이용하는 사람들이 눈여겨볼 여러 인사이트를 도출하였다.

## 프로젝트 목차
- 데이터 수집 및 전처리
- 데이터 분석 내용
  1. 선물세트 물량 분석, 끌올 분석
  2. 카테고리 분석
  3. 인기 매물 집중 분석
  4. 제목 키워드 가중치 분석, 키워드 실험 
  5. 거래 장소 분석
- 결론


## 주요 역할
- **[데이터 수집](https://github.com/hmii/daangn_giftitem_deals_analysis/blob/dc943e55fb8b1a95a995cfd50b4f4339621d6011/1.%20scraping/Carrot_scrapping_BS.ipynb)**
  : 당근마켓 홈페이지에서 서울시 25개구에서 '선물세트'로 등록된 일년치 물량 스크래핑 
 
- **전처리**
  - [날짜 전처리](https://github.com/hmii/daangn_giftitem_deals_analysis/blob/dc943e55fb8b1a95a995cfd50b4f4339621d6011/2.%20preprocessing/preprocessing_25gu_timedelta_year.ipynb)
  - [제목 텍스트 전처리 및 카테고리 분류](https://github.com/hmii/daangn_giftitem_deals_analysis/blob/dc943e55fb8b1a95a995cfd50b4f4339621d6011/2.%20preprocessing/BPE_token_year.ipynb) 
    - BPE(Byte Pair Encoding) 토크나이징 - 딕셔너리 제작 - 카테고리 분류 및 컬럼 생성
- **[EDA](https://github.com/hmii/daangn_giftitem_deals_analysis/tree/master/3.%20EDA)** 
- **데이터 분석**
  - 명절 기간에 선물세트 물량은 얼마나 증가할까? 선물세트를 팔아야 하는 좋은 시점은? [월별/일별/시간대별 물량추이](https://github.com/hmii/daangn_giftitem_deals_analysis/blob/dc943e55fb8b1a95a995cfd50b4f4339621d6011/3.%20EDA/time_series_EDA.ipynb)
  - 어떤 키워드를 제목에 넣으면 사람들이 많이 클릭하고 하트(관심)를 누를까? [제목 텍스트 가중치 분석](https://github.com/hmii/daangn_giftitem_deals_analysis/blob/dc943e55fb8b1a95a995cfd50b4f4339621d6011/4.%20modeling/weight_modeling.ipynb)
    
  
- **실험** : 분석 결과에 따라 실제로 가중치가 높은 키워드를 넣으면 조회수와 관심도가 올라갈까? (제목텍스트에 따른 조회수와 관심도 비교 실험)

## 발표 자료 및 영상
- 발표 영상: [https://youtu.be/JPZETe3eab0](https://youtu.be/JPZETe3eab0)
- 발표 평가: [https://youtu.be/JPZETe3eab0?t=1049](https://youtu.be/JPZETe3eab0?t=1049)
