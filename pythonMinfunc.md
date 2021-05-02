### 파이썬 min() 함수  


  
##  <br/>:question: 카카오 문자열 압축 문제를 풀다가 생긴 의문  



####   <br/><br/> compressed_list = ['2ab2cd2ab2cd',  '22222222ababcdcdababcdcd', 'ababcdcdababcdcd', 'ababcdcdababcdcd', '2ababcdcd']


#### <br/><br/>이 리스트에 대해 min(compress_list) 에 대한 값으로 마지막 값인 '2ababcdcd'를 기대 했는데 
     

<br/>`min(compressed_list) =  2ab2cd2ab2cd` 값이 나온다

#### <br/> 파이썬 내장 함수인 min 함수는 문자열 비교 시 오로지 문자만 비교 한다!. ( python 3.8.3 verison 기준)

## <br/><br/> 📖 그래서 내 마음대로 만들었다 . 문자열 비교 하도록
  
#### <br/><br/> 정규표현식을 이용하여 리스트를 통째로 str 로 바꾼 후

#### 비탐욕적 방식으로 패턴의 가장 짧은 문자열 추출을 하려고 했지만 핀트가 맞지 않아 iterator 방식 사용. <br/><br/>

```{.python} <br/><br/>
  def min_str_in_list(compressed_list): 
    for i in compressed_list:    
      if min_len > len(i):  
        min_len = len(i)  
    return min_len  
```
