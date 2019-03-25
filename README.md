# deeplearning_project
2018-2 고려대학교 딥러닝 수업(주재걸 교수님) 프로젝트

# 프로젝트 양식
https://www.overleaf.com/latex/templates/template-for-neural-information-processing-systems-nips-2018/zxpdbfpqgxss

## 연구 Timeline
### 반드시 1주일에 적어도 한번씩 만나고, 제대로 기한에 맞추어 진행할 것
#### 11월 3주
- **계획: 딥러닝 모델 구체적으로 결정(감정분석, 음악생성), 모델에 대해 정확하고 자세하게 알아오기**
- 실제: 
### 감정분석 데이터셋
#### 문제점: 인간의 다양한 감정을 분류할 수 있는 데이터셋이 없음(대부부 긍정-부정 분류)
- 데이터셋: [무료 감정분석 데이셋 15개](https://gengo.ai/datasets/15-free-sentiment-analysis-datasets-for-machine-learning/?utm_campaign=c&utm_medium=quora&utm_source=rei)
- **Stanford140(140만개의 트위터 데이터셋, 감정 종류:긍정, 부정, 중립)**
    - [Standford140 분석 글목록](https://towardsdatascience.com/search?q=Another%20Twitter%20sentiment%20analysis%20with%20Python%E2%80%8A) 
    - [Word2Vec+CNN](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-11-cnn-word2vec-41f5e28eda74)
    - [iPython파일](https://github.com/tthustla/twitter_sentiment_analysis_part11/blob/master/Capstone_part11.ipynb)
    - [Stanford 140 논문](https://cs.stanford.edu/people/alecmgo/papers/TwitterDistantSupervision09.pdf) 

- **네이버 영화리뷰 데이터셋(감정 종류: 긍정, 부정)**
- [BiLSTM을 이용한 영화 감성분류](https://github.com/MSWon/Sentimental-Analysis)

### 음악생성 모델 
- [문학 기반 음악생성](http://www.aclweb.org/anthology/W14-0901)
- [Composing music with RNN](http://www.hexahedria.com/2015/08/03/composing-music-with-recurrent-neural-networks/)
- 모이기로 한 날: 11월 18일 일요일
- 실제 모인 날: 11월 18일 일요일

#### 11월 4주
- **계획: 감정분석 모델 구현 및 실험, 음악 데이터 수집**

#### 11월 5주
- **계획: 감정에 따른 음악생성 모델 구현**

#### 12월 1주
- **계획: 감정에 따른 음악생성 실험, 보고서 집필**

#### 12월 2주(딥러닝 프로젝트 발표)


## 프로젝트 평가 기준
**후보가 다음의 조건을 만족하는지 평가해야 합니다.**
1. 목표가 무엇인가? 정확하고 간결하게 설명할 수 있어야 한다.
2. 해당 분야의 현재 진척 상황은 어떠며, 현재 연구의 문제점이나 한계는 무엇인가?
3. 당신의 접근이 새로운 이유와 성공적이라고 생각하는 이유는 무엇인가?
4. 누가 당신의 연구를 필요로 하는가?

## Project 주제 후보군

**1. Draw Oriental Paintings**
  - 목표: 글에 어울리는 동양화 생성
  - 이 분야의 진척 상황: AttnGAN 
  
**2. Generate music by text sentiment analysis**
- 입력 텍스트에 대한 sentiment analysis 진행
  - [참조](https://ratsgo.github.io/natural%20language%20processing/2017/08/16/deepNLP/#e-감성분류)
- [WaveNet](https://deepmind.com/blog/wavenet-generative-model-raw-audio/) 모델 사용
- [표정에서 읽은 감정에 기반한 음악 생성](http://www.scitepress.org/Papers/2018/65977/65977.pdf)
- 음악은 동양음악으로 설정?
- [C-RNN-GAN](https://medium.com/cindicator/music-generation-with-neural-networks-gan-of-the-week-b66d01e28200)

## 참고자료
- [AttnGAN](https://arxiv.org/pdf/1711.10485.pdf)
- [AttnGAN의 간단한 한글설명](https://blog.naver.com/PostView.nhn?blogId=blogstock&logNo=221189113859&parentCategoryNo=&categoryNo=&viewDate=&isShowPopularPosts=false&from=postView)
- [Chinese Paintings by GAN](http://cs231n.stanford.edu/reports/2017/pdfs/311.pdf)
- [CycleGAN](https://arxiv.org/pdf/1703.10593.pdf)
  - [Pytorch Implementation](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)
- [ArtGAN](https://arxiv.org/pdf/1702.03410.pdf)
- [MuseGAN](https://salu133445.github.io/musegan/pdf/musegan-aaai2018-slides.pdf)
  - Pop music 생성기
- [Music Gen. with Keras](https://towardsdatascience.com/how-to-generate-music-using-a-lstm-neural-network-in-keras-68786834d4c5)
- [GAN 참고자료](https://github.com/nashory/gans-awesome-applications)
- [Music Gen. from MIDI datasets](https://neuro.cs.ut.ee/wp-content/uploads/2018/02/MIDI_music.pdf)
- [cs224d Deep Learning for Music](https://cs224d.stanford.edu/reports/allenh.pdf)
- [Training GAN on small dataset of images](https://stackoverflow.com/questions/48601991/training-gan-on-small-dataset-of-images)
  - 적은 image dataset일 때의 질문이지만, 해결책은 music에도 적용 가능하리라 생각
- [Music Comp. using RNN](https://web.stanford.edu/class/cs224n/reports/2762076.pdf)
## 데이터셋
- [The Behance Artistic Media Dataset](https://bam-dataset.org/)
  - 아마추어 작가들의 그림과, 캡션을 모아놓은 사이트(75000여건)
- [WIKIART](https://www.wikiart.org/en/wu-daozi)
  - 서양화 및 동양화를 모아놓은 사이트(캡션 있음)
- [Chinese Paintings Dataset](https://github.com/ychen93/Chinese-Painting-Dataset)
  - CS231n 텀프로젝트에서 스탠포드 학생들이 모은 중국화(5200여장)
- [우키요에(일본 목판화) 데이터베이스](https://ukiyo-e.org/)
  - 22만건의 방대한 데이터 
- [Open Datasets](https://skymind.ai/wiki/open-datasets)
  - Music dataset 외에도 다양
  
### 이 외의 아이디어들

3. Text to Handwriting
- 나의 손글씨로 문장을 변환해보자...!
- http://www.cs.toronto.edu/~graves/handwriting.html
- https://github.com/szcom/rnnlib

4. Deep to Deep
- 딥러닝 네트워크를 이용한 딥러닝 코드작성
- 이것보다는 파이썬의 코드나 C 코드를 생성해주는 딥러닝 네트워크는 어떨까
- 또는 동일 기능의 python 코드와 c코드를 작성하여 프로그래밍 언어 번역기 만들기...!
- https://github.com/kootenpv/neural_complete

5. Sample to Full
- 미리듣기 음악으로 전체 음악을 구성할 수 있을까...?
- 구성한다면 기존의 원본 음악과의 차이는?

6. Hide and Seek
- 여러 환경에 적합한 위장패턴을 생성
- 검출은 인물구별용 딥러닝 모델을 사용한다

7. Fake news detection
- 기사의 내용이 진짜인지 탐지
- MIT 해커톤에서 만든 것으로는 90%이상의 정확도 보여줌
- 한국어 기사에 적용할 시 정확도는...?
