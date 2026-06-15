---
layout: about
title: Home
permalink: /
subtitle:
nav: true
nav_order: 1
---

<style>
.post-header { display: none; }
.lab-hero {
  border-radius: 16px;
  background: #0E4A8A;
  color: #ffffff;
  text-align: center;
  padding: 2.6rem 1.6rem;
  margin: 1rem 0 2.5rem;
  box-shadow: 0 2px 8px rgba(14, 74, 138, .18);
}
.lab-hero .lab-name { font-size: 1.7rem; font-weight: 700; line-height: 1.3; margin: 0 0 .3rem; color: rgba(255,255,255,.85); }
.lab-hero .lab-name .sun { color: #ffffff; }
.lab-hero .lab-abbr { letter-spacing: .18em; font-weight: 600; color: #ffffff; margin: .1rem 0 1rem; }
.lab-hero .lab-tagline { font-size: 1.05rem; max-width: 48ch; margin: 0 auto .7rem; color: rgba(255,255,255,.9); }
.lab-hero .lab-affil { font-size: .9rem; color: rgba(255,255,255,.7); margin: 0; }

.research-grid { display: flex; flex-wrap: wrap; gap: 1.5rem; justify-content: center; margin: 1.5rem 0; }
.research-card {
  flex: 1 1 240px; max-width: 320px; text-align: center;
  background: #ffffff;
  border: 1px solid #e3e6e9;
  border-radius: 14px;
  padding: 1.8rem 1.4rem;
  box-shadow: 0 1px 4px rgba(14, 74, 138, .07);
}
.research-card img { width: 150px; height: 150px; }
.research-card h3 { margin: 1.1rem 0 .4rem; color: #0E4A8A; }
.research-card p { font-size: .95rem; line-height: 1.55; color: #898C8E; }

.joinus {
  border: 1.5px solid #0E4A8A; border-radius: 14px; background: #f7f8fa;
  text-align: center; padding: 2.4rem 1.6rem; margin: 2.2rem 0;
}
.joinus .joinus-title { color: #0E4A8A; font-size: 1.5rem; font-weight: 700; margin-bottom: 1.2rem; }
.joinus p { color: #898C8E; max-width: 56ch; margin: 0 auto .8rem; line-height: 1.6; }
.joinus .email-btn {
  display: inline-block; margin-top: 1.2rem; background: #0E4A8A; color: #ffffff;
  font-weight: 600; padding: .7rem 1.5rem; border-radius: 8px; text-decoration: none;
}
.joinus .email-btn:hover { background: #0c3e75; color: #ffffff; }
</style>

<div class="lab-hero">
  <h1 class="lab-name"><span class="sun">S</span>ecurity, <span class="sun">U</span>sability, and <span class="sun">N</span>etworking Lab</h1>
  <p class="lab-abbr">SUNLab</p>
  <p class="lab-tagline">We develop fundamental techniques to make real-world systems secure, usable, and trustworthy. We cover diverse topics across network security, usable security, and AI security.</p>
  <p class="lab-affil">Dept. of Computer Science and Engineering · Hanyang University ERICA</p>
</div>

## Research Areas

<div class="research-grid">
  <div class="research-card">
    <img src="/assets/img/icon-network-security.png" alt="Network Security" />
    <h3>Network Security</h3>
    <p>We analyze and protect networked systems and the traffic that flows
    through them, including encrypted and tunneled communications, to uncover
    attacks and keep real-world networks reliable and trustworthy.</p>
  </div>
  <div class="research-card">
    <img src="/assets/img/icon-usable-security.png" alt="Usable Security" />
    <h3>Usable Security</h3>
    <p>We study how people perceive, adopt, and interact with security and
    privacy mechanisms, and design protections that work in practice without
    burdening the people who rely on them.</p>
  </div>
  <div class="research-card">
    <img src="/assets/img/icon-ai-security.png" alt="AI Security" />
    <h3>AI Security</h3>
    <p>We investigate the security and robustness of AI and machine learning
    systems, including the risks of poisoned or compromised models, to defend
    learning-based systems against adversarial manipulation.</p>
  </div>
</div>

## News

- **Mar 2026** · SUNLab officially launches at Hanyang University ERICA!
- **Jan 2026** · Two papers accepted to ASIACCS 2026 (CCA-Droid, PP-Vul).

<div class="joinus">
  <div class="joinus-title">Join Us</div>
  <p>SUNLab is actively recruiting motivated M.S. and Ph.D. students, as well as undergraduate interns, who are interested in security, usability, and networking.</p>
  <p>If you are passionate about solving challenging problems across networks, machine learning, and human factors, please reach out!</p>
  <a class="email-btn" href="mailto:sanghak@hanyang.ac.kr">sanghak@hanyang.ac.kr</a>
</div>
