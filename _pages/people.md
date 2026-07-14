---
layout: page
title: People
permalink: /people/
nav: true
nav_order: 2
---

<link rel="preconnect" href="https://fonts.googleapis.com" />
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />

<style>
  body { font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif; line-height: 1.72; -webkit-font-smoothing: antialiased; }
  h2 { color: #0e4a8a; border-bottom: 2px solid #e6eaef; padding-bottom: 0.35rem; margin-top: 2.2rem; }

  /* 네비바 공통 (다른 페이지와 동일) */
  .navbar-brand {
    display: inline-block !important;
    width: 110px !important;
    height: 44px !important;
    padding: 0 !important;
    font-size: 0 !important;
    background: url("/assets/img/sunlab_icon_with_white_background.png") left center / contain no-repeat;
  }
  #navbar .nav-link,
  .navbar-nav .nav-link { font-weight: 700 !important; }

  /* PI 카드 */
  .pi-card { display: flex; flex-wrap: wrap; gap: 1.8rem; align-items: flex-start; background: #f7f9fc; border: 1px solid #e6eaef; border-radius: 16px; padding: 1.8rem; margin: 1.2rem 0; }
  .pi-photo img { width: 180px; height: 220px; object-fit: cover; border-radius: 12px; border: 1px solid #e6eaef; }
  .pi-info { flex: 1 1 320px; }
  .pi-name { font-size: 1.5rem; font-weight: 800; color: #0e4a8a; margin: 0 0 0.2rem; }
  .pi-title { font-weight: 600; color: #1f2937; margin: 0 0 0.1rem; }
  .pi-affil { color: #898c8e; margin: 0 0 0.1rem; }
  .pi-bio { margin: 1rem 0; line-height: 1.65; }
  .pi-links { display: flex; flex-wrap: wrap; gap: 0.6rem; margin-top: 1rem; }
  .pi-links a { display: inline-block; background: #0e4a8a; color: #fff; font-weight: 600; font-size: 0.85rem; padding: 0.4rem 0.9rem; border-radius: 999px; text-decoration: none; transition: background 0.15s ease; }
  .pi-links a:hover { background: #0c3e75; color: #fff; }

  /* 학생 그리드 */
  .member-grid { display: flex; flex-wrap: wrap; gap: 1.4rem; margin: 1.2rem 0; }
  .member { flex: 0 0 150px; text-align: center; }
  .member img { width: 120px; height: 120px; object-fit: cover; border-radius: 50%; border: 1px solid #e6eaef; }
  .member .m-name { font-weight: 700; color: #0e4a8a; margin-top: 0.6rem; }
  .member .m-role { font-size: 0.85rem; color: #898c8e; }
  .empty-note { color: #898c8e; font-style: italic; }

  /* Open positions callout */
    .openings {
      border: 1px solid #dbe4f0;
      border-left: 5px solid #0e4a8a;
      background: #fafcff;
      border-radius: 12px;
      padding: 1.6rem 1.8rem;
      margin: 1.4rem 0 2rem;
    }
    .openings .openings-title { color: #0e4a8a; font-size: 1.15rem; font-weight: 700; margin: 0 0 0.5rem; }
    .openings p { color: #4b5563; margin: 0; line-height: 1.65; }
    .openings a { color: #0e4a8a; font-weight: 600; text-decoration: none; }
    .openings a:hover { text-decoration: underline; }
</style>

## Faculty

<div class="pi-card">
  <div class="pi-photo">
    <img src="/assets/img/sanghak_oh.jpg" alt="Sanghak Oh" />
  </div>
  <div class="pi-info">
    <p class="pi-name">Sanghak Oh</p>
    <p class="pi-title">Assistant Professor</p>
    <p class="pi-affil">Department of Computer Science and Engineering</p>
    <p class="pi-affil">Hanyang University ERICA, Ansan, Korea</p>
    <p class="pi-bio">
      Sanghak Oh is an Assistant Professor at Hanyang University ERICA, where he leads SUNLab. 
      His research spans network security, usable security, and AI security. He received his 
      Ph.D. from Sungkyunkwan University and previously served as an Assistant Professor at 
      the Korea Military Academy. <!-- 필요하면 수정 -->
    </p>
    <div class="pi-links">
      <a href="mailto:sanghak@hanyang.ac.kr">Email</a>
      <a href="https://scholar.google.com/citations?user=2ipInUsAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
      <a href="https://dblp.org/pid/195/6446.html" target="_blank" rel="noopener">DBLP</a>
      <a href="/assets/pdf/cv.pdf" target="_blank" rel="noopener">CV</a>
    </div>
  </div>
</div>

## Students

<div class="openings">
  <p class="openings-title">Open Positions</p>
  <p>
    We are looking for motivated undergraduate and graduate (M.S. and Ph.D.) students. If you are interested in our lab, please email: <a href="mailto:sanghak@hanyang.ac.kr">sanghak@hanyang.ac.kr</a>
  </p>
</div>

<div class="member-grid">
  <div class="member">
    <img src="/assets/img/students/eunjung_jang.jpg" alt="Eunjung Jang" />
    <div class="m-name">Eunjung Jang</div>
    <div class="m-role">Undergraduate</div>
  </div>
  <div class="member">
    <img src="/assets/img/students/jooyoung_kim.jpg" alt="Jooyoung Kim" />
    <div class="m-name">Jooyoung Kim</div>
    <div class="m-role">Undergraduate</div>
  </div>
  <div class="member">
    <img src="/assets/img/students/bohyun_kim.jpg" alt="Bohyun Kim" />
    <div class="m-name">Bohyun Kim</div>
    <div class="m-role">Undergraduate</div>
  </div>  
</div>


<!-- 학생이 생기면 아래 틀을 복사해서 채우세요
<div class="member-grid">
  <div class="member">
    <img src="/assets/img/member1.jpg" alt="Name" />
    <div class="m-name">Hong Gildong</div>
    <div class="m-role">Ph.D. Student</div>
  </div>
</div>
-->
