# 빅데이터자연어처리기술 Final Report(20년도 2학기)
[1] 임희석 교수님 빅데이터자연어처리기술 과목 기말고사 대체과제입니다.

[2] Natural Language Processing Final Project

# 파일 설명
[1] EmotionLines_friends_annotation.tar.gz
- 영어 학습 Corpus 데이터
- "Friends_감정분석기.ipynb" 파일 내의 소스코드에서 !git clone https://github.com/dolphz/2020-2nd-NLP 을 통해 해당 Corpus 데이터를 다운받기 위한 용도

[2] Friends_감정분석기.ipynb
- 영어 발화에 대한 감정 분석 알고리즘을 구현한 소스코드
- Google Colab 기반으로 작성하여 .ipynb 파일로 첨부

[3] NSMC_감정분석기.ipynb
- 한국어 발화에 대한 감정 분석 알고리즘을 구현한 소스코드
- Google Colab 기반으로 작성하여 .ipynb 파일로 첨부

[4] README.md
- 페이지 소개를 위한 README File

[5] kaggle.json
- "Friends_감정분석기.ipynb" 파일과 "NSMC_감정분석기.ipynb" 파일 내의 소스코드에서 Colab과 Kaggle 간의 연동 API를 사용하기 위한 JSON File
- 상기 2개의 한국어/영어 감정분석기 소스코드 실행을 위해서는 kaggle.json 파일을 우선적으로 다운받아야 합니다.

# 한국어 감정분석기 실행 방법
[1] 파일 2개 다운로드
- NSMC_감정분석기.ipynb
- kaggle.json

[2] Google Colab 접속 및 로그인

[3] 파일 > 노트 업로드 > 업로드 Tab > 파일 선택 > NSMC_감정분석기.ipynb > 열기

[4] 소스코드를 순차적으로 실행하되, 아래 코드 실행 시 명령어 프롬프트에서 파일 선택 > kaggle.json > 열기
- !pip install kaggle
- from google.colab import files
- files.upload()

[5] kaggle.json 파일이 정상적으로 Import 된 것을 확인한 후 다음 소스코드 순차적으로 실행

[6] 실행 완료 후 생성된 sample.csv 파일을 보면 모델이 Kaggle Competition Test Set에 대해 예측한 Label 값이 ID 순서대로 기입되어 있다.

# 영어 감정분석기 실행 방법
[1] 파일 2개 다운로드
- Friends_감정분석기.ipynb
- kaggle.json

[2] Google Colab 접속 및 로그인

[3] 파일 > 노트 업로드 > 업로드 Tab > 파일 선택 > Friends_감정분석기.ipynb > 열기

[4] 소스코드를 순차적으로 실행하되, 아래 코드 실행 시 명령어 프롬프트에서 파일 선택 > kaggle.json > 열기
- !pip install kaggle
- from google.colab import files
- files.upload()

[5] kaggle.json 파일이 정상적으로 Import 된 것을 확인한 후 다음 소스코드 순차적으로 실행

[6] 실행 완료 후 생성된 sample.csv 파일을 보면 모델이 Kaggle Competition Test Set에 대해 예측한 Label 값이 ID 순서대로 기입되어 있다.

# 참고 문헌 및 소스코드
[1] Google Colab 개발환경
https://colab.research.google.com/

[2] 한국어 NSMC Corpus 데이터
https://github.com/e9t/nsmc

[3] 영어 Friends Corpus 데이터
http://doraemon.iis.sinica.edu.tw/emotionlines/

[4] 빅데이터자연어처리 과목 실습 동영상
https://kulms.korea.ac.kr/ultra/courses/_210990_1/cl/outline

[5] Yoon Kim, “Convolutional Neural Networks for Sentence Classification” 논문 참조
http://emnlp2014.org/papers/pdf/EMNLP2014181.pdf

[6] Ratsgo’s Blog (CNN으로 문장 분류하기)
https://ratsgo.github.io/natural%20language%20processing/2017/03/19/CNN/

[7] 1D CNN으로 IMDB 리뷰 분류하기
https://wikidocs.net/80783

[8] 네이버 영화 리뷰 감성 분류하기
https://wikidocs.net/44249

[9] 모델 학습 완료 후 저장하기
https://hansonminlearning.tistory.com/12

[10] CNN의 성능을 높이기 위한 기법들
https://mrsyee.github.io/image%20processing/2018/11/28/cnn_technique/

[11] 영화 리뷰를 사용한 텍스트 분류(Tensorflow)
https://www.tensorflow.org/tutorials/keras/text_classification?hl=ko

[12] 모델 학습 시 Callback 옵션 사용법(Overfitting 방지를 위한 Early Stopping 등)
https://jins-sw.tistory.com/27

[13] 문서 분류를 위한 CNN 모델
https://www.sallys.space/blog/2018/05/18/cnn-for-doc/
