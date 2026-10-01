---
title: The KHAN's App Studio
---

<!--
  마크다운 안에 HTML 과 <style> 을 그대로 둘 수 있다. Jekyll(kramdown)은 블록으로 시작하는
  HTML 을 손대지 않고 내보내므로, 아래 히어로는 적은 그대로 페이지에 들어간다.

  배경은 앱 메인 헤더와 같은 벡터(assets/header-wave.svg)다. 테마(jekyll-theme-primer)가
  내주는 가운데 정렬 컨테이너 안에 있어서, 화면 끝까지 늘리려면 음수 마진으로 한 번
  빠져나가야 한다. 자세한 내용은 아래 CSS 주석에 적었다.
-->

<style>
/* 100vw 는 스크롤바 폭까지 세므로 그만큼 가로가 넘친다. 이 페이지엔 sticky 가 없어 잘라도 된다. */
body { overflow-x: hidden; background: #F8FAFC; }

/* 테마가 맨 위에 넣는 저장소 이름 제목. 히어로가 그 자리를 대신한다. */
.markdown-body > h1:first-child { display: none; }

.qb-hero {
  /* -32px 은 테마 컨테이너의 my-5(32px)를 걷어내 히어로를 화면 맨 위에 붙이는 값이다. */
  margin: -32px 0 32px;
  /* 컨테이너 안에서 화면 폭으로 빠져나간다. 컨테이너가 가운데 정렬이라 좌우가 맞는다. */
  width: 100vw;
  margin-left: calc(50% - 50vw);
  background: #F8FAFC url("./assets/header-wave.svg") no-repeat;
  background-size: 100% 100%;   /* 앱의 ImageView fitXY 와 같게 늘린다 */
}
.qb-hero__inner {
  max-width: 1012px;            /* 테마의 container-lg */
  margin: 0 auto;
  padding: 40px 16px 52px;
  box-sizing: border-box;
}
.qb-hero__mark { display: block; width: 56px; height: 56px; }
.qb-hero__title {
  margin: 16px 0 0;
  padding: 0;
  border: 0;                    /* markdown-body 가 h1 밑에 긋는 선을 지운다 */
  font-size: 30px;
  line-height: 1.25;
  font-weight: 700;
  color: #0F172A;               /* brand_text */
}
.qb-hero__sub {
  margin: 6px 0 0;
  font-size: 14px;
  color: #8D8EDB;               /* toolbar_slogan */
}

/*
  테마는 투명 PNG 가 어두운 바탕에서 묻히지 않게 `.markdown-body img` 에 흰 배경을
  깔아 둔다. 우리 마크에는 그 흰 판이 네모로 그대로 보인다. 선택자에
  `.markdown-body` 를 같이 적는 것은 특이도 때문이다 — 클래스만으로는 테마 규칙에
  밀려 안 먹는다.
*/
.markdown-body img.qb-hero__mark { background: none; }

@media (max-width: 600px) {
  .qb-hero__inner { padding: 28px 16px 40px; }
  .qb-hero__mark  { width: 48px; height: 48px; }
  .qb-hero__title { font-size: 24px; }
}
</style>

<div class="qb-hero">
  <div class="qb-hero__inner">
    <img class="qb-hero__mark" src="./assets/quickbar-mark.svg" width="56" height="56" alt="">
    <h1 class="qb-hero__title">The KHAN&rsquo;s App Studio</h1>
    <p class="qb-hero__sub">Your favorites. One slide away.</p>
  </div>
</div>

## QuickBar (퀵바)

알림바에 자주 쓰는 앱·웹주소·연락처를 놓고 한 번에 여는 런처입니다.

- [Google Play](https://play.google.com/store/apps/details?id=kr.co.two_khan.quickbar)
- [개인정보처리방침 / Privacy Policy](https://khansappstudio.github.io/privacy.html)

## 문의

khans.appstudio@gmail.com
