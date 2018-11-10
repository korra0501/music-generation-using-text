# deeplearning_project
2018-2 고려대학교 딥러닝 수업(주재걸 교수님) 프로젝트

# 프로젝트 양식
https://www.overleaf.com/latex/templates/template-for-neural-information-processing-systems-nips-2018/zxpdbfpqgxss

## 프로젝트 평가 기준
**후보가 다음의 조건을 만족하는지 평가해야 합니다.**
1. 목표가 무엇인가? 정확하고 간결하게 설명할 수 있어야 한다.
2. 해당 분야의 현재 진척 상황은 어떠며, 현재 연구의 문제점이나 한계는 무엇인가?
3. 당신의 접근이 새로운 이유와 성공적이라고 생각하는 이유는 무엇인가?
4. 누가 당신의 연구를 필요로 하는가?
5. 성공한다면, 어떤 변화를 만들어 낼 수 있을 것인가?-> 비지니스 및 기술적 변화 서술
6. 성공을 위한 중간과 마지막 체크리스트는 무엇인가?

### Project 주제 후보군

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

## 참고자료
- [AttnGAN](https://arxiv.org/pdf/1711.10485.pdf)
- [AttnGAN의 간단한 한글설명](https://blog.naver.com/PostView.nhn?blogId=blogstock&logNo=221189113859&parentCategoryNo=&categoryNo=&viewDate=&isShowPopularPosts=false&from=postView)
- [Chinese Paintings by GAN](http://cs231n.stanford.edu/reports/2017/pdfs/311.pdf)
- [CycleGAN](https://arxiv.org/pdf/1703.10593.pdf)
  - [Pytorch Implementation](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)
- [ArtGAN](https://arxiv.org/pdf/1702.03410.pdf)
## 데이터셋
- [The Behance Artistic Media Dataset](https://bam-dataset.org/)
  - 아마추어 작가들의 그림과, 캡션을 모아놓은 사이트(75000여건)
- [WIKIART](https://www.wikiart.org/en/wu-daozi)
  - 서양화 및 동양화를 모아놓은 사이트(캡션 있음)
- [Chinese Paintings Dataset](https://github.com/ychen93/Chinese-Painting-Dataset)
  - CS231n 텀프로젝트에서 스탠포드 학생들이 모은 중국화(5200여장)
- [우키요에(일본 목판화) 데이터베이스](https://ukiyo-e.org/)
  - 22만건의 방대한 데이터 
