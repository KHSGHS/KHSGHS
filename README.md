---
marp: true
footer: Created by fls2134
paginate: true
theme: gaia
style: |
  section{background:rgb(241, 237, 234)}
  p{font-size:24px;}
  li{font-size:18pt}
  table{font-size:20px;}
---

# 9주차

---

# MarkDown

---

### Goal

- Markdown 문법을 이해하고 문서 작성에 활용할 수 있다

---

### Markdown이란?

- **간단한 문법으로 문서 구조를 표현**할 수 있는 경량 마크업 언어
- README, 블로그, 문서화, 발표자료 등에 널리 사용됨
- `.md` 확장자 사용

---

### 개요

Markdown은 텍스트 기반의 마크업언어로 2004년 존그루버에 의해 만들어졌으며 쉽게 쓰고 읽을 수 있으며 HTML로 변환이 가능하다.

특수기호와 문자를 이용한 매우 간단한 구조의 문법을 사용하여 웹에서도 보다 빠르게 컨텐츠를 작성하고 보다 직관적으로 인식할 수 있다.

---

### Title

```
# Header1 - h1
## Header2 - h2
### Header3 - h3
```

# Header1 - h1

## Header2 - h2

### Header3 - h3

---

### Title

```
#### Header4 - h4
##### Header5 - h5
###### Header6 - h6
```

#### Header4 - h4

##### Header5 - h5

###### Header6 - h6

---

### 인용구

```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```

> This is a first blockqute.

> > This is a second blockqute.

> > > This is a third blockqute.

---

### 리스트

```
1. list item 1
3. list item 2
8. list item 3
```

1. list item 1
2. list item 2
3. list item 3

---

### 순서없는 리스트

```
- Index
    - Category 1
        - Sub Category 1
        - Sub Category 2
```

- Index
  - Category 1
    - Sub Category 1
    - Sub Category 2

---

### 코드 블럭

```
indent로 들여쓰기를 하면 자동으로 코드블럭 생성

    # include <stdio.h>
    int main(){printf("Hello World!);}

파이썬처럼 indent 닫으면 코드블럭 끝남
```

indent로 들여쓰기를 하면 자동으로 코드블럭 생성

    # include <stdio.h>
    int main(){printf("Hello World!);}

파이썬처럼 indent 닫으면 코드블럭 끝남

---

### 코드 블럭

indent를 사용한 코드 블럭은 indent가 들어간 영역 위, 아래로 개행을 해둬야만 적용됨.

##### 보다 일반적인 사용 예 : "`" 3개 사용하기

````
    ```python
    # write your code
    ```
````

---

### 키워드 강조

- \`keyword\` : `keyword`

- \*keyword\* : _keyword_

- keyword* : \_keyword*

- \*\*keyword\*\* : **keyword**

- ~\~keyword\~\~ : ~~keyword~~

---

### image 삽입

```
![Alt text](/path/to/img.jpg)

> 예시: ![height:100](/img/logo.png)
> 높이를 100 사이즈만큼, 이미지의 경로
```

![height:100](/img/logo.png)

---

# Marp

---

### Marp란?

- **Markdown 기반 발표 슬라이드 생성 도구**
- 마크다운 문법으로 슬라이드를 작성하고 HTML, PDF 등으로 출력 가능
- VS Code 확장 또는 CLI 사용

---

### Marp의 특징

| 특징                | 설명                                        |
| ------------------- | ------------------------------------------- |
| 간편한 문법         | 마크다운 기반으로 쉽게 작성 가능            |
| 다양한 테마         | 기본 테마 외에 커스텀 테마 적용 가능        |
| 코드 하이라이팅     | 코드 블럭에 문법 강조 지원 (`highlight.js`) |
| PDF 내보내기        | `--pdf` 옵션 또는 VS Code로 바로 저장 가능  |
| 이미지, 수학식 지원 | LaTeX 수식(`KaTeX`), 이미지 첨부 지원       |

---

### 슬라이드 작성 구조

- 슬라이드 구분은 `---` 사용
- 제목과 내용은 마크다운 문법 그대로 작성

---

# TIPS

---

### 자기소개

github repo 이름을 본인 계정 이름으로 만들면 자기소개 페이지가 생성된다.

해당 repo에 `readme.md`를 수정하면 자기소개 페이지를 관리할 수 있다.

---

### 기타 팁

shilds.io로 뱃지 넣기 - [LINK](https://shields.io/badges)

![Static Badge](https://img.shields.io/badge/:badgeContent)

| 이거 쓰면 좀 가오가 있어보인다.

![height:280](img/image.png)

---

### 기타 팁

##### ✅ 내 계정의 깃허브 스택을 보여줄 수 있다.

```
#![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=본인깃계정명&show_icons=true&theme=radical)
```

##### ✅ 내 백준 티어를 자랑할 수 있다

```
[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=본인백준계정)](https://solved.ac/본인백준계정/)
```
