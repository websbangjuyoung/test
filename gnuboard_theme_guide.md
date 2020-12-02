## webs202003 테마
반응형 웹

### 브라우저 및 모바일 지원 범위
코드 베이스인 `bootstrap@4.5`의 지원 범위를 따른다.    
````
Chrome 45 이상
Firefox 38 이상
Edge 12 이상
iOS 9 이상
Safari 9 이상
Android 4.4 이상
Opera 30 이상
단, IE 11 이상부터
네이버 whale 최근 3년 이내
````

> 지원 범위 참고 https://getbootstrap.com/docs/4.5/getting-started/browsers-devices/

### 필수 라이브러리

- jquery
    - `jquery-3.5.1`
    - `jquery-migrate-3.3.2`
    > 문서참고 https://jquery.com/
    
- bootstrap
    - css: `bootstrap@4.5.3`
    - js: `bootstrap@4.5.3 bundle 버젼`
    > 문서참고 https://getbootstrap.com/docs/4.5/getting-started/introduction/
    
- 슬라이드
    - `OwlCarousel2 2.3.4`
        > 문서참고 http://owlcarousel2.github.io/OwlCarousel2
        
        

## 사이트 기본 메타 요소 확인
### 사이트 아이콘 등록
- 파일: `테마폴더/img/favicon.png`
- 사이즈: 가로 32px 세로 32px
> 브라우저 ie 10 이하 지원할 경우: `테마폴더/favicon.ico` (사이즈 가로 16px 세로 16px)

### 소셜 메타
- 카카오톡 (참고: [링크1](https://devtalk.kakao.com/t/topic/22238?source_topic_id=102650), [링크2](https://developers.kakao.com/docs/latest/ko/message/message-template#scrap]) )
> 이미지 권장 사이즈: 가로 800px 세로 800px
````
<meta property="og:url" content="https://devtalk.kakao.com/">
<meta property="og:title" content="Kakao DevTalk_">  
<meta property="og:type" content="website">
<meta property="og:image" content="https://devtalk.kakao.com/images/devtalk_.png">
<meta property="og:description" content="카카오 데브톡. 카카오 플랫폼 서비스 관련 질문 및 답변을 올리는 개발자 커뮤니티 사이트입니다.">
````
- 페이스북
> 이미지 권장 사이즈: 가로 1200px 세로 630px
````
<meta property="og:type" content="website">
<meta property="og:url" content="https://example.com/page.html">
<meta property="og:title" content="Content Title">
<meta property="og:image" content="https://example.com/image.jpg">
<meta property="og:description" content="Description Here">
<meta property="og:site_name" content="Site Name">
<meta property="og:locale" content="en_US">
<!-- Next tags are optional but recommended -->
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
````
- 트위터
````
<meta name="twitter:card" content="summary">
<meta name="twitter:site" content="@site_account">
<meta name="twitter:creator" content="@individual_account">
<meta name="twitter:url" content="https://example.com/page.html">
<meta name="twitter:title" content="Content Title">
<meta name="twitter:description" content="Content description less than 200 characters">
<meta name="twitter:image" content="https://example.com/image.jpg">
````

