# Rap-Lyrics-Generator
2019-2 'NLP and Deep Learning' Class Project
### 한국 가요 가사를 바탕으로 새로운 가사를 생성하는 모델
* 멜론에서 BeautifulSoup를 활용해 모든 장르의 가사 10000개 수집
> * 랩 가사는 비문과 영어가 너무 섞여 제대로 된 가사가 생성되지 못함
> * 동요가 운율이 잘 맞아 학습의 성능이 좋을 것이라 예상했으나 오히려 성능이 하락
> * 결국 모든 장르의 가사 활용

* LSTM 모델로 주어진 가사 학습 후 새로운 가사 Generating
> * 최초로 일정 숫자의 text 랜덤하게 생성 후 과거 텍스트의 순서를 반영해 다음 글자 예측을 반복 
> > * Char-level langauge model
