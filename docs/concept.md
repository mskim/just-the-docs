북치고는 "북치고 장구친다" 에서 유래된 이름이다.
즉 책을 혼자서 다 만든다는 뜻이다. Self Publishing, One man band...
'Book' 은 책을 뜻하며 'Go' 는 알파고(AlphaGo)와 같은 자동화를 의미 한다.

## 내용과 디자인을 분리해서 작업

북치고의 가장 핵심적인 개념은 편집을 보다 효율적으로 진행하기 위해서는 내용물과 디자인을 별도로 작업할 수 있게 하여야 한다는 것이다.

기존 편집 방식은 작가가 내용을 작성한 후 디자이너에게 전달하면 디자이너가 편집을 한 후 다시 작가에게 반복적으로 검토를 하면서 진행하는 방식이다. 이렇게 작업을 진행하다보니 작가와 디자이너가 다른 사람의 작업이 끝난 후에야 작업을 진행할 수 밖에 없는 형태로 작업을 하게되어 모든 공정의 시간이 늘어날 수 밖에 없었다. 시간이 길어질수록 비용도 커진다.

북치고는 새로운 편집 방식을 제공한다.
작가와 디자이너는 서로 다른 시간대에서 각자 자신의 작업을 진행하고 이를 컴퓨터가 자동으로 편집물을 합성 하는 방식이다. 
작가와 디자이너는 서로 약속된 방식으로 글과 디자인을 작성하고 디자이너도 이를 수용할 수 있는 디자인 작업을 하고  디자인과 원고를  컴퓨터가 자동 합성하게 하자는 것이다. 이렇게 되면 디자이너가 한번 작업한 디자인을 반복적으로 여러 개의 유사한 편집물에서 사용할 수 있게 되고 디자이너가 매번 모든 작업에 관여 하지 않고도 편집 작업을 작가 스스로 진행 할 수 있게 된다.
또한 웹 브라우저 상에서 작업을 할 수 있기 때문에 작가와 디자이너가 동시에 동일한 편집물에 작업을 하는 것도 가능하다.

### 약속된 방식의 내용물 작성

내용물 작성은  '마크다운(markdown)' 이라는 방식을 사용 하여 내용물을 작성 한다. 'book.md' 라는 파일에 책의 내용을 입력 하고  여러 명이 동시에 이것을 교정/교열 할 수 있다. 

### 모든 파일은 단순 텍스트 형태 으로 작성한다.

모든 문서의 내용은 단순 텍스트 형태의 파일로 저장 된다. 그 의미는 내용을 텍스트 수정이 가능한 프로그램을 사용해서 수정이 가능하다.  즉 메모장이나 카카오톡 등을 사용해서 원고 및 디자인 파일을 수정 할 수 있다.
기존의 방식은 특정업체에서 제작한 편집프로그램을 사용해야만 수정이 가능 했다. 즉 인디자인이나 아래한글 같은 프로그램이 있어야만 수정이 가능했다.
### 마스터페이지 작성

디자인 작성은 "YAML" 이라는 형태로 입력한다. 
```
```
```yaml
---
class: page
width: 350
height: 500
left_margin: 50
top_margin: 50
right_margin: 50
bottom_margin: 100
column_count: 2
```
위와 같이 입력 하여 마스터 페이지를 디자인 한다.




기존에 많이 사용하던 '디자인 템플릿' 방식과는 다른 방식이다.
'디자인 템플릿' 을 사용하여 자동편집을 할 경우, 수많은 템플릿들이 필요하다.
그리고 수많은 변수의 디자인 들을 수용할 수 없어 몇 개의 정해진 템플릿에서 선택을 해야 하는 방식을 사용해 왔다. 그래서 그 영역이 매우 제한적이었다. 즉 명함, 현수막, 사진첩, 등등 비교적 단순한 편집물에 국한 되어 왔었다.
그러나 스크립트 언어 방식을 사용하면 편집 영역을 보다 복잡한 형태의 편집물까지도 수용할 수 있게 된다. 소설, 신문, 잡지 등등의 편집물 들도 자동화가 가능 하다.
디자인 파일은 각각의 문서 단위로 작성한다. 즉 본문 장, 서문, 목차, 판권, 등등의 도큐멘트 별로 다른 디자인을 사용할 수 있다. 

즉 인디자인 이나 쿽의 사용방식과 비교 하자면 여러 개의 인디자인 파일을 책의 부분별로 작성해서 재활용하는 것 과 유사 하다고 생각 하면 된다. 

## 내용과 디자인을 자동으로 합성

디자인 파일은 여러 개의 부분별로 작성하고  내용물은 하나의 파일에 작성해서 수시로 원하는 내용과 디자인을 자동으로 합성한다.

약속된 형태의 내용물과 디자인을 다양한 형태로 합성이 가능하다. 일반인들이 쉽게 사용할 수 있는 웹기반에서 도 가능하며, 많은 양의 편집물을 서버에서 자동으로 처리하는 Batch 작업 형태로도  가능 사용이 가능하다.

