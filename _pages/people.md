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
</style>
