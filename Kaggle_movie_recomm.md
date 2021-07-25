
EDA 시작하고 생각이 파생된 과정

## kaggle movies dataset contents based recomsys 과정

1. 데이터셋 모두를 불러와 데이터를 탐색했다
2. 영화 타이틀을 보기 위해 movieid 를 키로 merge 
3. overview에 대한 전처리 Tokenizing 후  
4. linear_kernel cosine_similarity를 계산하여 추천 영화를 리턴 하는 함수를 참고하여 만들었다
 &nbsp;



### Tokenizer 라이브러리와 Tfidvectorizer 의 활용 형태
  * Tokenizer는 정수 인코딩을 할 수 있게 만들어 주지만 Ttidvectorizer는 matrix를 return 하므로 cosine_similar 활용에 쓰인다

### cosine_similarity 를 만들 때는 linear_kernel을 활용

### dataframe과 series를 필요한 형태로 만들기
 
