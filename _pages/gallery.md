---
layout: page
title: Gallery
permalink: /gallery/
nav: true
nav_order: 5
---

<link rel="preconnect" href="https://fonts.googleapis.com" />
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />

<style>
  body { font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif; line-height: 1.72; -webkit-font-smoothing: antialiased; }
  h1 { color: #0e4a8a; }
  h2 { color: #0e4a8a; border-bottom: 2px solid #e6eaef; padding-bottom: 0.35rem; margin-top: 2.4rem; }

  /* 행사 캐러셀 2열 레이아웃 (왼쪽부터 채움) */
  .gallery-columns { display: flex; flex-wrap: wrap; gap: 2rem; align-items: flex-start; justify-content: flex-start; margin: 1.2rem 0 2rem; }
  .carousel { flex: 1 1 340px; max-width: calc(50% - 1rem); margin: 0; }
  @media (max-width: 680px) {
    .carousel { max-width: 100%; flex-basis: 100%; }
  }
  .carousel-title { text-align: center; color: #0e4a8a; font-weight: 700; font-size: 1.15rem; margin: 0 0 0.9rem; }
  .carousel-stage { position: relative; }
  .carousel-track { position: relative; aspect-ratio: 4 / 3; border-radius: 12px; overflow: hidden; border: 1px solid #e6eaef; background: #f7f9fc; }
  .carousel-track img { position: absolute; inset: 0; width: 100%; height: 100%; object-fit: cover; opacity: 0; transition: opacity 0.3s ease; cursor: zoom-in; }
  .carousel-track img.active { opacity: 1; }
  .car-btn { position: absolute; top: 50%; transform: translateY(-50%); z-index: 3; background: rgba(14, 74, 138, 0.82); color: #fff; border: none; width: 40px; height: 40px; border-radius: 50%; font-size: 1.1rem; cursor: pointer; transition: background 0.15s ease; }
  .car-btn:hover { background: #0e4a8a; }
  .car-prev { left: 10px; }
  .car-next { right: 10px; }
  .carousel-dots { text-align: center; margin-top: 0.8rem; }
  .carousel-dots span { display: inline-block; width: 9px; height: 9px; border-radius: 50%; background: #d6e2f0; margin: 0 4px; cursor: pointer; transition: background 0.15s ease; }
  .carousel-dots span.active { background: #0e4a8a; }

  /* Lightbox */
  .lightbox { position: fixed; inset: 0; z-index: 1000; background: rgba(0, 0, 0, 0.9); display: none; align-items: center; justify-content: center; }
  .lightbox.open { display: flex; }
  .lightbox .lb-img { max-width: 90vw; max-height: 84vh; border-radius: 8px; box-shadow: 0 10px 40px rgba(0, 0, 0, 0.5); }
  .lightbox .lb-btn { position: absolute; top: 50%; transform: translateY(-50%); background: rgba(255, 255, 255, 0.14); color: #fff; border: none; width: 48px; height: 48px; border-radius: 50%; font-size: 1.4rem; cursor: pointer; transition: background 0.15s ease; }
  .lightbox .lb-btn:hover { background: rgba(255, 255, 255, 0.3); }
  .lightbox .lb-prev { left: 18px; }
  .lightbox .lb-next { right: 18px; }
  .lightbox .lb-close { position: absolute; top: 16px; right: 20px; background: none; border: none; color: #fff; font-size: 2.1rem; line-height: 1; cursor: pointer; }
  .lightbox .lb-caption { position: absolute; bottom: 20px; left: 0; right: 0; text-align: center; color: rgba(255, 255, 255, 0.9); font-size: 0.9rem; }
</style>

<style>
  /* SUNLab 로고 + 메뉴 (다른 페이지와 동일) */
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
</style>

<div class="gallery-columns">

  <!-- 새 행사(최신)는 이 자리, 맨 앞에 추가하면 기존 것이 오른쪽/아래로 밀립니다 -->

  <div class="carousel" data-title="CISC-W 2026">
    <p class="carousel-title">CISC-W 2026</p>
    <div class="carousel-stage">
      <div class="carousel-track">
        <img src="/assets/img/gallery/cisc-2026w/1.jpg" alt="CISC-W 2026 1" class="active" loading="lazy" />
        <img src="/assets/img/gallery/cisc-2026w/2.jpg" alt="CISC-W 2026 2" loading="lazy" />
        <img src="/assets/img/gallery/cisc-2026w/3.jpg" alt="CISC-W 2026 3" loading="lazy" />
        <img src="/assets/img/gallery/cisc-2026w/4.jpg" alt="CISC-W 2026 4" loading="lazy" />
        <img src="/assets/img/gallery/cisc-2026w/5.jpg" alt="CISC-W 2026 5" loading="lazy" />
      </div>
      <button class="car-btn car-prev" aria-label="Previous">&#10094;</button>
      <button class="car-btn car-next" aria-label="Next">&#10095;</button>
    </div>
    <div class="carousel-dots"></div>
  </div>

  <!-- 행사 추가 틀 (복사해서 제목·사진 경로만 바꾸세요)
  <div class="carousel" data-title="행사명">
    <p class="carousel-title">행사명</p>
    <div class="carousel-stage">
      <div class="carousel-track">
        <img src="/assets/img/gallery/행사폴더/1.jpg" alt="행사명 1" class="active" loading="lazy" />
        <img src="/assets/img/gallery/행사폴더/2.jpg" alt="행사명 2" loading="lazy" />
      </div>
      <button class="car-btn car-prev" aria-label="Previous">&#10094;</button>
      <button class="car-btn car-next" aria-label="Next">&#10095;</button>
    </div>
    <div class="carousel-dots"></div>
  </div>
  -->

</div>

<div class="lightbox" id="lightbox" aria-hidden="true">
  <button class="lb-close" aria-label="Close">&times;</button>
  <button class="lb-btn lb-prev" aria-label="Previous">&#10094;</button>
  <img class="lb-img" src="" alt="" />
  <button class="lb-btn lb-next" aria-label="Next">&#10095;</button>
  <div class="lb-caption"></div>
</div>

<script>
  (function () {
    function init() {
      var lb = document.getElementById("lightbox");
      var lbImg = lb ? lb.querySelector(".lb-img") : null;
      var lbCap = lb ? lb.querySelector(".lb-caption") : null;
      var lbGroup = [], lbIdx = 0;

      function lbShow(i) {
        if (!lbGroup.length) return;
        lbIdx = (i + lbGroup.length) % lbGroup.length;
        lbImg.src = lbGroup[lbIdx].src;
        lbImg.alt = lbGroup[lbIdx].alt || "";
        lbCap.textContent = (lbGroup[lbIdx].alt ? lbGroup[lbIdx].alt + "   " : "") + "(" + (lbIdx + 1) + " / " + lbGroup.length + ")";
      }
      function lbOpen(g, i) { lbGroup = g; lb.classList.add("open"); document.body.style.overflow = "hidden"; lbShow(i); }
      function lbClose() { lb.classList.remove("open"); document.body.style.overflow = ""; }

      if (lb) {
        lb.querySelector(".lb-next").addEventListener("click", function (e) { e.stopPropagation(); lbShow(lbIdx + 1); });
        lb.querySelector(".lb-prev").addEventListener("click", function (e) { e.stopPropagation(); lbShow(lbIdx - 1); });
        lb.querySelector(".lb-close").addEventListener("click", function (e) { e.stopPropagation(); lbClose(); });
        lb.addEventListener("click", function (e) { if (e.target === lb) lbClose(); });
        document.addEventListener("keydown", function (e) {
          if (!lb.classList.contains("open")) return;
          if (e.key === "ArrowRight") lbShow(lbIdx + 1);
          else if (e.key === "ArrowLeft") lbShow(lbIdx - 1);
          else if (e.key === "Escape") lbClose();
        });
      }

      document.querySelectorAll(".carousel").forEach(function (car) {
        var imgs = Array.prototype.slice.call(car.querySelectorAll(".carousel-track img"));
        if (!imgs.length) return;
        var group = imgs.map(function (im) { return { src: im.getAttribute("src"), alt: im.getAttribute("alt") }; });
        var dotsWrap = car.querySelector(".carousel-dots");
        var cur = 0;

        imgs.forEach(function (im, i) {
          var dot = document.createElement("span");
          dot.addEventListener("click", function () { show(i); });
          dotsWrap.appendChild(dot);
          im.addEventListener("click", function () { lbOpen(group, cur); });
        });
        var dots = Array.prototype.slice.call(dotsWrap.querySelectorAll("span"));

        function show(i) {
          cur = (i + imgs.length) % imgs.length;
          imgs.forEach(function (im, j) { im.classList.toggle("active", j === cur); });
          dots.forEach(function (d, j) { d.classList.toggle("active", j === cur); });
        }

        car.querySelector(".car-prev").addEventListener("click", function () { show(cur - 1); });
        car.querySelector(".car-next").addEventListener("click", function () { show(cur + 1); });
        show(0);
      });
    }
    if (document.readyState === "loading") document.addEventListener("DOMContentLoaded", init);
    else init();
  })();
</script>
