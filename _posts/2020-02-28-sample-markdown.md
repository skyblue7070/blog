---
layout: post
title: Sample blog post to learn markdown tips [한국어]
subtitle: 배울 것이 많아요! 


tags: [sample]
comments: true
mathjax: true
author: Bill Smith
last-updated: 2025-01-03
readtime: true
---
<!-- gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow] -->

{: .box-warning}
이 글은 원본 게시물이 아니며 일부 콘텐츠가 수정되어 있습니다. 원본은 [여기](https://beautifuljekyll.com/2020-02-28-sample-markdown)를 참조해주십시오.

{: .box-success}
이것은 마크다운으로 블로그 게시물을 작성하는 방법을 보여주는 데모 게시물입니다. [5분 동안 마크다운으로 작성하는 방법](https://markdowntutorial.com/)을 배우는 것을 강력히 권장합니다. - 이 게시물은 일반 텍스트를 볼드/이탤릭/테이블 등으로 변환하는 방법을 알려줄 것입니다.<br/>또한 [이 게시물을 만든 코드](https://raw.githubusercontent.com/skyblue7070/blog/master/_posts/2025-01-21-sample-markdown.md)를 참고하여 Beautiful Jekyll에서 마크다운 사용에 대한 고급 팁을 배우는 것도 권장합니다.

**이것은 굵은 글씨입니다**

## 이것은 두번째 제목입니다

[이것은 다른 (이 테마 개발자)웹사이트로 이동](https://deanattali.com/)하고, [이것은 이 페이지의 섹션으로 이동](#local-urls)됩니다.

이건 테이블:

| 숫자 | 다음 숫자 | 이전 숫자 |
| :------ |:--- | :--- |
| 다섯 | 여섯 | 넷 |
| 열 | 열하나 | 아홉 |
| 일곱 | 여덟 | 여섯 |
| 둘 | 셋 | 하나 |

[MathJax](https://www.mathjax.org/) 을 사용하여 LaTeX 표현을 사용할 수 있습니다. 예시:
\\(a \ne 0\\)일 때, \\(ax^2 + bx + c = 0\\) 또는 $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}$$으로 해는 두가지이다.

이 맛있는 크레페 어떠세요?

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg)

가운데에 놓을 수도 있습니다!

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg){: .mx-auto.d-block :}

여기는 코드가 있습니다:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

그리고 여기 문법 하이라이트가 있는 같은 코드:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

그리고 여기 또 같은 코드지만 줄번호가 있음:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## 박스
알림, 경고, 오류 박스를 다음과 같이 추가할 수 있음:

### 알림

{: .box-note}
**노트:** 이것은 알림 박스입니다.

### 경고

{: .box-warning}
**경고:** 이것은 경고 박스입니다.

### 오류

{: .box-error}
**오류:** 이것은 오류 박스입니다.

## 프로젝트 사이트의 로컬 URL {#local-urls}

GitHub Pages에서 *프로젝트 사이트*를 호스팅할 때(예시, `https://USERNAME.github.io/MyProject`, 그리고 이 웹사이트), URL은 루트 URL(/)이 GitHub Pages에서 어떻게 해석되는지에 따라 올바르게 작동하지 않을 수 있습니다. 더 자세히 알고 싶으시면 [FAQ](https://beautifuljekyll.com/faq/#links-in-project-page)에서 확인하세요. 이 문제를 설명하기 위해, **이 웹사이트가 프로젝트 사이트인 경우** 다음 로컬 이미지가 손상될 것입니다:

![Crepe](/assets/img/crepe.jpg)

만약에 위의 이미지가 손상되었다면 [FAQ](https://beautifuljekyll.com/faq/#links-in-project-page)의 지침을 따르세요. 아래는 고쳐지면 보인다는 증거입니다:

![Crepe]({{ '/assets/img/crepe.jpg' | relative_url }})
