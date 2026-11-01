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

  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 0.8rem;
    margin: 1.1rem 0 1.5rem;
  }
  .gallery-grid img {
    width: 100%;
    aspect-ratio: 4 / 3;
    object-fit: cover;
    border-radius: 10px;
    border: 1px solid #e6eaef;
    cursor: pointer;
    transition: transform 0.15s ease, box-shadow 0.15s ease;
  }
  .gallery-grid img:hover { transform: translateY(-3px); box-shadow: 0 10px 24px rgba(14, 74, 138, 0.15); }
  @media (max-width: 640px) {
    .gallery-grid { grid-template-columns: repeat(2, 1fr); gap: 0.6rem; }
  }

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

## SUNLab Launch (Jun 2026)

<div class="gallery-grid">
  <img src="/assets/img/gallery/launch/1.jpg" alt="SUNLab launch 1" loading="lazy" />
  <img src="/assets/img/gallery/launch/2.jpg" alt="SUNLab launch 2" loading="lazy" />
  <img src="/assets/img/gallery/launch/3.jpg" alt="SUNLab launch 3" loading="lazy" />
  <img src="/assets/img/gallery/launch/4.jpg" alt="SUNLab launch 4" loading="lazy" />
  <img src="/assets/img/gallery/launch/5.jpg" alt="SUNLab launch 5" loading="lazy" />
  <img src="/assets/img/gallery/launch/6.jpg" alt="SUNLab launch 6" loading="lazy" />
</div>

## Group Outing (Jul 2026)

<div class="gallery-grid">
  <img src="/assets/img/gallery/outing/1.jpg" alt="Group outing 1" loading="lazy" />
  <img src="/assets/img/gallery/outing/2.jpg" alt="Group outing 2" loading="lazy" />
  <img src="/assets/img/gallery/outing/3.jpg" alt="Group outing 3" loading="lazy" />
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
    function initGallery() {
      var lb = document.getElementById("lightbox");
      if (!lb) return;
      var lbImg = lb.querySelector(".lb-img");
      var lbCap = lb.querySelector(".lb-caption");
      var group = [], idx = 0;

      function show(i) {
        if (!group.length) return;
        idx = (i + group.length) % group.length;
        lbImg.src = group[idx].src;
        lbImg.alt = group[idx].alt || "";
        lbCap.textContent = (group[idx].alt ? group[idx].alt + "   " : "") + "(" + (idx + 1) + " / " + group.length + ")";
      }
      function open(g, i) { group = g; lb.classList.add("open"); document.body.style.overflow = "hidden"; show(i); }
      function close() { lb.classList.remove("open"); document.body.style.overflow = ""; }

      document.querySelectorAll(".gallery-grid").forEach(function (grid) {
        var imgs = Array.prototype.slice.call(grid.querySelectorAll("img"));
        var g = imgs.map(function (im) { return { src: im.getAttribute("src"), alt: im.getAttribute("alt") }; });
        imgs.forEach(function (im, i) { im.addEventListener("click", function () { open(g, i); }); });
      });

      lb.querySelector(".lb-next").addEventListener("click", function (e) { e.stopPropagation(); show(idx + 1); });
      lb.querySelector(".lb-prev").addEventListener("click", function (e) { e.stopPropagation(); show(idx - 1); });
      lb.querySelector(".lb-close").addEventListener("click", function (e) { e.stopPropagation(); close(); });
      lb.addEventListener("click", function (e) { if (e.target === lb) close(); });
      document.addEventListener("keydown", function (e) {
        if (!lb.classList.contains("open")) return;
        if (e.key === "ArrowRight") show(idx + 1);
        else if (e.key === "ArrowLeft") show(idx - 1);
        else if (e.key === "Escape") close();
      });
    }
    if (document.readyState === "loading") document.addEventListener("DOMContentLoaded", initGallery);
    else initGallery();
  })();
</script>
