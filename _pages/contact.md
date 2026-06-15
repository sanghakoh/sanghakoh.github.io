---
layout: page
title: Contact
permalink: /contact/
nav: true
nav_order: 4
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

<link rel="preconnect" href="https://fonts.googleapis.com" />
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />

<style>
  .post-header { display: none; }
  body { font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif; line-height: 1.72; -webkit-font-smoothing: antialiased; }

  h2 { color: #0e4a8a; border-bottom: 2px solid #e6eaef; padding-bottom: 0.35rem; margin-top: 2.2rem; }

  .lab-hero {
    border-radius: 18px; background: #0e4a8a; color: #fff; text-align: center;
    padding: 3rem 1.8rem; margin: 1.2rem 0 3rem; box-shadow: 0 10px 30px rgba(14, 74, 138, 0.22);
  }
  .lab-hero .lab-name { font-size: 1.9rem; font-weight: 800; line-height: 1.25; margin: 0 0 0.4rem; color: rgba(255, 255, 255, 0.9); letter-spacing: -0.02em; }
  .lab-hero .lab-name .sun { color: #fff; text-decoration: underline; text-underline-offset: 4px; text-decoration-thickness: 2px; }
  .lab-hero .lab-abbr { letter-spacing: 0.22em; font-weight: 700; color: #fff; opacity: 0.95; margin: 0.2rem 0 1.1rem; font-size: 0.95rem; }
  .lab-hero .lab-tagline { font-size: 1.08rem; max-width: 52ch; margin: 0 auto 0.8rem; color: rgba(255, 255, 255, 0.92); line-height: 1.65; }
  .lab-hero .lab-affil { font-size: 0.9rem; color: rgba(255, 255, 255, 0.72); margin: 0; }

  .research-grid { display: flex; flex-wrap: wrap; gap: 1.4rem; justify-content: center; margin: 1.5rem 0; }
  .research-card {
    flex: 1 1 240px; max-width: 320px; text-align: center; background: #fff;
    border: 1px solid #e6eaef; border-radius: 16px; padding: 2rem 1.5rem;
    box-shadow: 0 2px 10px rgba(14, 74, 138, 0.05); transition: transform 0.18s ease, box-shadow 0.18s ease;
  }
  .research-card:hover { transform: translateY(-4px); box-shadow: 0 12px 28px rgba(14, 74, 138, 0.12); }
  .research-card img { width: 150px; height: 150px; }
  .research-card h3 { margin: 1.1rem 0 0.5rem; color: #0e4a8a; font-size: 1.18rem; }
  .research-card p { font-size: 0.94rem; line-height: 1.6; color: #898c8e; }

  .joinus {
    border: 1px solid #e6eaef; border-top: 4px solid #0e4a8a; border-radius: 16px;
    background: #f7f9fc; text-align: center; padding: 2.6rem 1.8rem; margin: 2.4rem 0;
  }
  .joinus .joinus-title { color: #0e4a8a; font-size: 1.6rem; font-weight: 800; margin-bottom: 1.2rem; letter-spacing: -0.02em; }
  .joinus p { color: #898c8e; max-width: 56ch; margin: 0 auto 0.8rem; line-height: 1.65; }
  .joinus .email-btn {
    display: inline-block; margin-top: 1.4rem; background: #0e4a8a; color: #fff; font-weight: 600;
    padding: 0.75rem 1.7rem; border-radius: 999px; text-decoration: none;
    box-shadow: 0 4px 14px rgba(14, 74, 138, 0.28); transition: transform 0.15s ease, background 0.15s ease;
  }
  .joinus .email-btn:hover { background: #0c3e75; color: #fff; transform: translateY(-2px); }
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
</style>

<div class="contact-wrap">
  <div class="contact-card">
    <p class="lab-name">Security, Usability, and Networking Lab (SUNLab)</p>
    <div class="contact-row">
      <span class="label">Address</span>
      <span class="value">Room 614, College of Pharmacy Building,<br>
      Dept. of Computer Science and Engineering,<br>
      Hanyang University ERICA,<br>
      Ansan, Republic of Korea</span>
    </div>
    <div class="contact-row">
      <span class="label">Email</span>
      <span class="value"><a href="mailto:sanghak@hanyang.ac.kr">sanghak@hanyang.ac.kr</a></span>
    </div>
    <div class="contact-row">
      <span class="label">Phone</span>
      <span class="value">(+82)-31-400-1038</span>
    </div>
  </div>
  <div class="contact-map">
    <iframe src="https://maps.google.com/maps?q=Hanyang%20University%20ERICA&t=&z=16&ie=UTF8&iwloc=&output=embed" allowfullscreen></iframe>
  </div>
</div>
