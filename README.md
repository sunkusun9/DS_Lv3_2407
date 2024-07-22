# DS_Lv3_2407

## 실습 내용

||Day1|Day2|Day3|
|---|----|----|----|
|주제|최대수요전력 예측|스프링 내구력 테스트 통과/실패 예측|세탁 지수 예측|
|출제<br/>영역|**데이터 전처리**<br/>> Join, 표준화, 일자(date) 형식 처리, shifting<br/>**데이터 추출**<br/>> GroupBy, …<br/>**가설 검정**<br/>> Shapiro-Wilks, Bartlett, T,<br/>일원분산분석, Mann-Whitney U<br/>Chi2 독립성 검정, 이원분산분석<br/>**지도학습**<br/>> 결정트리, GBDT, SVM<br/>**비지도학습**<br/>> PCA, DBSCAN <br/>**이상치 탐색**<br/>> Isolation Forest, Local Outlier Factor|**결측치 처리**<br/>> 반복적 결측치 처리<br/>**가설 검정**<br/>> 베르눌리 분포,  정규 분포<br/>**속성 선택**<br/>> 필터법, 전진선택법<br/>**가설 검정**<br/>> Jarque-bera, Bartlett, 일원분산분석<br/>**지도학습**<br/>> 로지스틱 회귀, 랜덤 포레스트, LDA<br/>**비지도학습**<br/>> PCA<br/>**하이퍼 파라미터 최적화**<br/>> 그리드 서치|**데이터 전처리**<br/>> 치환, 문자열 결합, 표준화, 구간범주화, 가변수화<br/>**가설 검정**<br/>> Kolmogolov-Smironov, Bartlett, 일원분산분석<br/>**확률 통계**<br/>> 정규분포<br/>**지도학습**<br/>> Linear Regression, xgboost<br/>**비지도학습**<br/>> Agglomerative Clustering, PCA<br/>**하이퍼 파라미터 최적화**<br/>|

## 강의 시간표

|구분|강의 내용|시작|끝|
|----|---------|----|--|
|0|전처리|8시 30분| 9시 30분|
|1|문제 1|9시 40분| 10시 40분|
|2|문제 2|10시 50분| 11시 50분|
|3-1|문제 3|12시 00분| 12시 30분|
|3-2|문제 3|13시 30분| 14시 10분|
|4|문제 4|14시 20분| 15시 20분|
|5|문제 5|15시 30분| 16시 30분|
|6|문제 6|16시 40분| 17시 30분|

※ 점심시간 이외에는 강의 흐름에 따라 가변적으로 진행될 수 있습니다. 

## 시험장 환경을 가상 환경으로 구축

PC에 있는 Python 환경을 유지하면서, 시험장 환경의 Python환경을 별도로 구축하는 방법입니다.

OS: Windows 10 (Windows 11도 가능하지만 결과에 차이가 있을 수 있습니다.)

<div style="border: 1px solid #ddd; padding: 12px; margin-top: 10px;">

1. [패키지](https://drive.google.com/file/d/1zhyIoMbSq7ZTwf6AnwiIIXtQ1qMqEWlK/view?usp=drive_link) 압축 파일을 다운로드 받습니다.  C:\패키지 에 압축을 풉니다.

   (C:\패키지에 위치할 필요는 없지만, 이후 설명은 C:\패키지 를 기준으로 합니다.)


2. 패키지에 안에 있는 시험장 환경의 python(3.7.4 version) 설치 파일 python-3.7.4-amd64.exe을 실행시킵니다.


3. Python 설치 경로를 C:\python37로 합니다. (마찬가지로 따를 필요는 없지만, 설명은 C:\python37 를 기준으로 합니다.)


4. Python 가상 환경 구축

- 명령프롬프트를 실행시킵니다.(Windows 실행 → cmd.exe)


- 설치된 버젼의 python 실행 파일을 사용하여 python37이란 이름으로 가상환경을 만듭니다.

```
    C:\python37\python -m venv python37
```

- 성공하면 python37 경로가 생깁니다.


5. 패키지 설치

```
    python37\Scripts\activate
    cd c:\패키지
    pip install --upgrade --no-index --find-links . pip
    pip install --no-index --find-links . -r requirements.txt
```

-------------------------------------------------------------------
    
</div>

가상 환경 전환 

- 일단 가상환경이 구축이 되면, 이후에는 활성화를 통해 환경 전환이 가능합니다.

```
    python37\Scripts\activate 
```

----------------------------------

가상 환경 해제

- 가상환경 이전의 환경으로 돌아옵니다.

```
    deactivate
```
