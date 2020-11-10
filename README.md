# 이상치 데이터 탐지

쇼핑몰 리뷰를 바탕으로 Word Embedding을 활용하여 가짜 리뷰를 태깅하는 프로젝트 입니다.

### 개발환경
* Windows
* Python 3.6

### 데이터 셋

* 데이터 셋: Blouse_Review_Data
* 언어: 한국어

* 총 6813개, 7개 컬럼
* item_no(상품 번호): int
* title(리뷰 제목): string
* contents(리뷰 내용): string
* style_1(카테고리): string . ex) 격식차린, 바캉스룩, 야외활동, 이국적인, 이지웨어, 프레피룩
* style_2(카테고리): string . ex) 스포티한, 일상복, 힙합
* style_3(카테고리): string . ex) 걸리쉬, 매니쉬, 섹시한, 우아한, 유니섹스
* style_4(카테고리): string . ex) 유니크한, 장식이 없는, 포멀한

The DataSet Used is Blouse Review in korea. Final results are anomaly scores based on dimension or style.


# STEP 
 
 1. download fasttext (https://github.com/facebookresearch/fastText) for word embedding.
    
    (1) pip uninstall fasttext
  
    (2) cd fastText
  
    (3) pip install .
  
    Ref) https://fasttext.cc/docs/en/crawl-vectors.html

 2. download sister (https://github.com/NAMSOO-KIM/sister) for sentence embedding.
    
    (1) git clone https://github.com/NAMSOO-KIM/sister.git
  
    (2) cd sister
  
    (3) pip install .

 3. Use this iforest_RealData.
 
    py3.6 version
    
    
