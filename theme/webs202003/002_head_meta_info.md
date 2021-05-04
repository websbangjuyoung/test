## HEAD 메타 정보
사이트에 맞게 아이콘과 이미지는 제작 후 다시 업로드 해야 하며, 경우에 따라 소스 수정이 필요할 수 있습니다.

### 사이트 아이콘
- 기본: `테마폴더/img/favicon.png` (사이즈 가로 32px 세로 32px)
- ie 10 이하 지원: `테마폴더/favicon.ico` (사이즈 가로 16px 세로 16px)

### 소셜 메타
- `head.sub.php` 파일 내 삽입된 공통 코드
    > `og_image.jpg` 는 가로 800px 세로 800px (카카오톡 이미지 권장 사이즈)로 기본 제작합니다.  
    > 페이스북 또는 트위터 동시 사용시 적정 이미지 또는 추가 작업이 필요할 수 있습니다.   
````
<meta property="og:url" content="<?php echo G5_URL; ?>">
<meta property="og:title" content="<?php echo $g5_head_title; ?>">
<meta property="og:image" content="<?php echo G5_THEME_IMG_URL; ?>/og_image.jpg">
<meta property="og:site_name" content="<?php echo $config['cf_title']; ?>">
````

- 관리자 페이지 내 환경설정 - 레이아웃 추가설정 영역 내 `추가 script, css` 에 메타 태그 등록
    > 사이트 설명 입력은 각 사이트에 맞는 적절한 문구를 넣어 주세요.  
````
<meta name="description" content="사이트 설명 입력 (75자 이내)">
<meta property="og:description" content="사이트 설명 입력 (75자 이내)">

// 트위터 카드 사용시
<meta name="twitter:card" content="summary">

// 이 외 사이트에 필요한 메타 태그 추가
````
#### 오픈 그래프 메타 태그 관련 공식 문서
- 오픈그래프 [링크](https://ogp.me/)
- 카카오톡
    - 메타 태그 구성 - 스크랩 메세지 내용 참고 [링크](https://developers.kakao.com/docs/latest/ko/message/message-template#scrap])
    - 메타 태그 추가 설명 참고 [링크](https://devtalk.kakao.com/t/topic/22238?source_topic_id=102650)
    - 미리보기(스크랩) 캐시 삭제(로그인 필요) [링크](https://developers.kakao.com/tool/clear/og)

- 페이스북 
    - 메태 태그 구성 [링크](https://developers.facebook.com/docs/sharing/webmasters#markup)
    - 미리보기(스크랩) 확인(로그인 필요) [링크](https://developers.facebook.com/tools/debug)
- 트위터 [링크](https://developer.twitter.com/en/docs/twitter-for-websites/cards/guides/getting-started)
