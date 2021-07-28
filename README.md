# markdown 작성방법

## 마크다운의 장점
* `읽기 쉽다.` 확실히 마크다운은 다른 마크업 언어에 비해 가독성이 좋습니다. 문법도 단순하고, HTML은 작성하면서 브라우저에서 어떻게 보여질지 예상하는게 쉽지 않지만, 마크다운을 사용한 텍스트는 브라우저에 보여질 내용을 쉽게 상상할 수 있습니다.
* `익히기 쉽다.` 존 그루버는 사람들이 많이 사용하는 것은 마크다운으로 사용하고, 복잡한 것은 HTML로 사용하기 바랬습니다. 그래서 문법이 매우 간단합니다. 그리고 마크다운으로 글을 작성할 때, 제한적인 기능 몇 개를 제외하고 HTML을 함께 사용해도 상관없습니다.
* `모바일 친화적이다.` 단순히 텍스트만 작성하는 것이 아닌 에디터를 이용해 모바일로 작성하는 것은 쉽지 않습니다. 하지만 마크다운을 이용하면 모바일에서도 태그로 쉽게 서식을 넣을 수 있어서, 에디터보다 훨씬 편합니다.

## 마크다운 단점
* `문법이 너무 단순하다.` 문법이 단순한 나머지 결국에는 HTML을 써야하는 경우가 생깁니다. 테이블 정렬 기능은 있지만, 이미지 정렬 기능이 없어서 HTML의 img 태그를 사용해야합니다. 태그에 클래스 지정등이 불가능하기 때문에, 클래스나 id를 지정하려면 HTML을 사용해야합니다.
* `표준이 없어 사용자마다 문법이 상이할 수 있다.` 문법이 단순하다 보니, 이러한 점을 해결하기 위해 확장문법들이 생겼고, 이러한 것들 때문에 한 곳에서 작동하는 마크다운 문서가 다른 곳에서는 잘 작동하지 않는 경우가 생기기도 합니다.

***

## 1. 헤더 (headers)
* `#`으로 시작하는 텍스트.
* `#`은 하나부터 여섯개까지 가능.
* `#`이 늘어날때마다 제목의 스케일 낮아집니다.

### 제목 사용방법
```
# This is an H1; 부(parts)에 사용<br>
## This is an H2; 장(chapters)에 사용<br>
### This is an H3; 페이지 섹션에 사용<br>
#### This is an H4; 하위 섹션에 사용<br>
##### This is an H5; 하위 섹션 아래의 하위 섹션에 사용<br>
###### This is an H6; 문단에 사용<br>
```

***

## 2. 강조 (emphasis)
* 기울여 쓰기(italic) : `*` 또는 `_`로 감싼 텍스트.
* 두껍게 쓰기(bold) : `**` 또는 `__`로 감싼 텍스트.
* 취소선 : `~~`로 감싼 텍스트.
* 이탤릭체와 두껍게를 같이 사용할 수 있습니다.

### 강조 사용법
```
*This text will be italic*
_This will also be italic_
**This text will be bold**
__This will also be bold__
~~This is canceled~~
*You **can** combine them*
```

***

## 3. 인용문 (blockquotes)
* ">"으로 시작하는 텍스트
* ">"는 3개까지 가능합니다.
* 1개는 인용문
* 2개는 2중첩 인용문
* 3개는 3중첩 인용문

### 인용 사용방법
```
As Grace Hopper said:
> I’ve always been more interested in the future than in the past.    
> This is a first blockquote.
> > This is a second blockquote.
> > > This is a third blockquote.
```

***

## 4.목록 (list)
### 순서가 없는 목록 (ul)
* "*", "+", "-" 를 이용해서 순서가 없는 목록을 만들 수 있습니다.
* 들여쓰기를 하면 모양을 바뀝니다.

### 순서가 있는 목록 (ol)
* 숫자를 기입하면 순서가 있는 목록이 됩니다. 
* 들여쓰기를 하면 모양이 바뀝니다.

#### 목록 사용법
```
* Item 1
* Item 2
  * Item 1
  * Item 2
 1. Item 1
 2. Item 2
 3. Item 3
   1. Item 1
   2. Item 2
   3. Item 3
```

***

## 5. 줄바꿈 (line break)
* "<br>"을 활용하여 줄바꿈을 할 수 있습니다.

### 줄바꿈 사용방법
```
I just wanna set you free <br>
C'mon, c'mon, c'mon <br>
You and me can make it up, anyway <br>
For now, we can stay here for a while <br>
Cause you know, I just wanna see your smile <br>
No matter where you go, know you're not alone <br>
```

***

## 6. 표 (tabel)
* 헤더와 셀을 구분할 때 3개 이상의 -(hyphen/dash) 기호가 필요합니다.
* 헤더 셀을 구분하면서 :(Colons) 기호로 셀(열/칸) 안에 내용을 정렬할 수 있습니다.
* 가장 좌측과 가장 우측에 있는 |(vertical bar) 기호는 생략 가능합니다.

### 표 사용방법
```
헤더1|헤더2|헤더3|헤더4
---|---|---|---
셀1|셀2|셀3|셀4
셀5|셀6|셀7|셀8
셀9|셀10|셀11|셀12

테이블 정렬

헤더1|헤더2|헤더3
:---|:---:|---:
Left|Center|Right
1|2|3
4|5|6
7|8|9
```

### 실행 결과
헤더1|헤더2|헤더3|헤더4
---|---|---|---
셀1|셀2|셀3|셀4
셀5|셀6|셀7|셀8
셀9|셀10|셀11|셀12

테이블 정렬

헤더1|헤더2|헤더3
:---|:---:|---:
Left|Center|Right
1|2|3
4|5|6
7|8|9

***

## 7. 🎈이모지 (emoji)
* 마크다운을 이용해 이모티콘 표현가능.
* 깃허브도 적용가능.
* 더 많은 리스트 아래의 사이트로 방문.
* www.emoji-cheat-sheet.com

### 이모지 사용방법
```
GitHub supports emoji!
:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat:
```

***

## 8. 체크리스트 (task list)
* 줄 앞에 "- [x]" 를 써서 완료된 리스트 표시.
* 줄 앞에 "- [ ]" 를 써서 미완료된 리스트 표시.

### 체크리스트 사용방법
```
- [x] this is a complete item
- [ ] this is an incomplete item
- [x] @mentions, #refs, [links]()
```

***

## 9. 내부 링크
```
[보여지는 내용](#이동할 헤드(제목))
괄호 안의 링크를 쓸 때는 띄어쓰기는 -로 연결, 영어는 모두 소문자로 작성
```

### 내부 링크 사용방법
```
[1. Headers 헤더](#1-헤더-headers)
[2. Emphasis 강조](#2-강조-emphasis))
[3. Blockquotes 인용](#3-인용문-blockquotes)
```