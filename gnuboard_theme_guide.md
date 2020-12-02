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
        
        

## 사이트 메타 기본 요소 확인
사이트에 맞게 아이콘과 이미지는 제작 후 다시 업로드 해야 하며, 경우에 따라 소스 수정이 필요할 수 있습니다.

### 사이트 아이콘
- 기본: `테마폴더/img/favicon.png` (사이즈 가로 32px 세로 32px)
- ie 10 이하용: `테마폴더/favicon.ico` (사이즈 가로 16px 세로 16px)

### 소셜 메타
- `head.sub.php` 파일 내 삽입된 공통 코드
> `og_image.jpg` 는 가로 800px 세로 800px (카카오톡 이미지 권장 사이즈)로 기본 제작합니다.  
> 페이스북 또는 트위터 공유도 같이 사용시 적정 이미지 또는 추가 작업이 필요할 수 있습니다.   
````
<meta property="og:url" content="<?php echo G5_URL; ?>">
<meta property="og:title" content="<?php echo $g5_head_title; ?>">
<meta property="og:image" content="<?php echo G5_THEME_IMG_URL; ?>/og_image.jpg">
<meta property="og:site_name" content="<?php echo $config['cf_title']; ?>">
````

- 관리자 페이지 내 환경설정 - 레이아웃 추가설정 영역 내 `추가 script, css` 에 메타 태그 등록
> 사이트 설명 입력은 각 사이트에 맞는 적절한 문구를 넣어 주세요.  
> 기타 추가적으로 필요한 메타 태그
````
<meta name="description" content="사이트 설명 입력 (75자 이내)">
<meta property="og:description" content="사이트 설명 입력 (75자 이내)">

// 트위터 카드 사용시
<meta name="twitter:card" content="summary">
````
#### 소셜 메타 태그 관련 문서
- 카카오톡: [링크1](https://devtalk.kakao.com/t/topic/22238?source_topic_id=102650), [링크2](https://developers.kakao.com/docs/latest/ko/message/message-template#scrap])
- 페이스북: [링크1](https://developers.facebook.com/docs/sharing/webmasters#markup)
- 트위터: [링크1](https://developer.twitter.com/en/docs/twitter-for-websites/cards/guides/getting-started)

