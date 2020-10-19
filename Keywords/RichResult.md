## [ Featured snippets && Rich snippets => Rich Result ]

> 구글 검색에서 활용되는 구조화된 데이터 형식과  
> 구글이 권장하는('가능한 경우 구조화된 데이터에는 JSON-LD를 사용하는 것이 좋습니다.')라고 말하고 있는 JSON-LD에 관하여 정리해보자.

#### | 공식 schema.org

https://schema.org

> @type, @context 확인

#### | 구조화된 데이터 작동 방식의 이해

https://developers.google.com/search/docs/guides/intro-structured-data

> JSON+ld sample

```html
<html>
  <head>
    <title>Apple Pie by Grandma</title>
    <script type="application/ld+json">
      {
        "@context": "https://schema.org/",
        "@type": "Recipe",
        "name": "Apple Pie by Grandma",
        "author": "Elaine Smith",
        "image": "http://images.edge-generalmills.com/56459281-6fe6-4d9d-984f-385c9488d824.jpg",
        "description": "A classic apple pie.",
        "aggregateRating": {
          "@type": "AggregateRating",
          "ratingValue": "4.8",
          "reviewCount": "7462",
          "bestRating": "5",
          "worstRating": "1"
        },
        "prepTime": "PT30M",
        "totalTime": "PT1H30M",
        "recipeYield": "8",
        "nutrition": {
          "@type": "NutritionInformation",
          "calories": "512 calories"
        },
        "recipeIngredient": [
          "1 box refrigerated pie crusts, softened as directed on box",
          "6 cups thinly sliced, peeled apples (6 medium)"
        ]
      }
    </script>
  </head>
  <body></body>
</html>
```

#### | 구조화된 데이터 가이드라인

https://developers.google.com/search/docs/guides/sd-policies

#### | 구조화된 데이터 생성

https://developers.google.com/search/docs/guides/generate-structured-data-with-javascript

> Google 태그 관리자(GTM)를 사용하여 동적으로 JSON-LD 생성이 가능하다고 나와있다

#### | 구조화된 데이터 마크업 도우미

https://www.google.com/webmasters/markup-helper/u/0/?hl=ko

#### | Google Rich snippets tester 링크

https://search.google.com/test/rich-results

#### | 구조화 데이터 관련 정리 블로그

https://brunch.co.kr/@springboot/131

#### | JSON-LD 위키백과 정의

https://ko.wikipedia.org/wiki/JSON-LD

```
JSON-LD(JavaScript Object Notation for Linked Data)는 JSON을 사용하여 링크드 데이터를 인코딩하는 방식이다.
목적은 개발자들이 기존의 JSON을 JSON-LD로 변환하는데 들어가는 노력을 가능한 최소화시키는 것이었다.
이로써 데이터가 전통적인 JSON과 유사한 방식으로 직렬화할 수 있게 된다.
월드 와이드 웹 컨소시엄 권고안의 하나이다. 검토, 개선, 표준화를 위해 RDF 워킹 그룹으로 이전되기 전까지는
처음에 JSON 포 링킹 데이터 커뮤니티 그룹(JSON for Linking Data Community Group)에 의해 개발되었다.

JSON-LD는 JSON→RDF 모델의 추가적인 매핑을 제공하기 위한 컨텍스트의 개념으로 설계되어 있다.
이 컨텍스트는 JSON 문서 내의 객체 속성을 온톨로지의 개념에 연결시킨다.
JSON-LD 문법을 RDF에 매핑시키기 위해 JSON-LD는 값들을 특정한 유형에 강제시키거나 특정 언어에 태그할 수 있게 허용한다.
컨텍스트는 JSON-LD 문서에 직접 추가하거나 별도 파일에 넣거나 다른 문서들로부터(HTTP 링크 헤더를 통해 전통적인 JSON 문서로부터) 참조할 수 있다.
```
