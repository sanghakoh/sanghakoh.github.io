---
layout: page
title: People
permalink: /people/
nav: true
nav_order: 2

profiles:
  # if you want to include more than one profile, just replicate the following block
  # and create one content file for each profile inside _pages/
  - align: right
    image: prof_pic.jpg
    content: about_einstein.md
    image_circular: false # crops the image to make it circular
    more_info: >
      <p>555 your office number</p>
      <p>123 your address street</p>
      <p>Your City, State 12345</p>
  - align: left
    image: prof_pic.jpg
    content: about_einstein.md
    image_circular: false # crops the image to make it circular
    more_info: >
      <p>555 your office number</p>
      <p>123 your address street</p>
      <p>Your City, State 12345</p>
---

<link rel="preconnect" href="https://fonts.googleapis.com" />
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />

<style>
  body { font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif; line-height: 1.72; -webkit-font-smoothing: antialiased; }
  a { color: #0e4a8a; }
  a:hover { color: #0c3e75; }
  h1 { color: #0e4a8a; }

  .contact-wrap { display: flex; flex-wrap: wrap; gap: 1.5rem; align-items: stretch; margin-top: 1.5rem; }
  .contact-card { flex: 1 1 320px; background: #f7f9fc; border: 1px solid #e6eaef; border-radius: 16px; padding: 2rem; }
  .contact-card .lab-name { color: #0e4a8a; font-size: 1.3rem; font-weight: 700; margin: 0 0 1.4rem; }
  .contact-row { display: flex; gap: 1rem; margin-bottom: 1.1rem; line-height: 1.55; }
  .contact-row .label { color: #0e4a8a; font-weight: 700; min-width: 72px; }
  .contact-row .value { color: #898c8e; }
  .contact-row .value a { color: #0e4a8a; }
  .contact-map { flex: 1 1 360px; min-height: 340px; }
  .contact-map iframe { width: 100%; height: 100%; min-height: 340px; border: 0; border-radius: 16px; }
</style>

<style>
  /* SUNLab 로고: 네비게이션 왼쪽 위 (전 페이지 공통, 자동으로 home 링크) */
  .navbar-brand {
    display: inline-block !important;
    width: 110px !important;        /* 로고 가로폭, 필요하면 조절 */
    height: 44px !important;        /* 네비바 높이에 맞춤 */
    padding: 0 !important;
    font-size: 0 !important;        /* 테마 기본 "SUNLab" 글자 숨김 */
    background: url("/assets/img/sunlab_icon_with_white_background.png") left center / contain no-repeat;
  }
  #navbar .nav-link,
  .navbar-nav .nav-link { font-weight: 700 !important; }
</style>
