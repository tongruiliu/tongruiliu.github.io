---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
.rt-home {
  --rt-ink: #1f2937;
  --rt-soft-ink: #4b5563;
  --rt-line: #dce7ef;
  --rt-blue: #2563eb;
  --rt-blue-2: #3b82f6;
  --rt-accent: #c2410c;
  --rt-surface: #ffffff;
  --rt-surface-soft: #f7fbff;
}

.rt-home a {
  text-decoration: none;
}

.rt-home .rt-hero {
  background: linear-gradient(125deg, #0f172a 0%, #1e3a8a 55%, #2563eb 100%);
  color: #e2e8f0;
  border-radius: 18px;
  padding: 30px 26px;
  box-shadow: 0 16px 36px rgba(15, 23, 42, 0.2);
  position: relative;
  overflow: hidden;
  margin-bottom: 18px;
}

.rt-home .rt-hero::after {
  content: "";
  position: absolute;
  width: 220px;
  height: 220px;
  right: -70px;
  top: -70px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(255, 255, 255, 0.22) 0%, rgba(255, 255, 255, 0) 72%);
}

.rt-home .rt-eyebrow {
  margin: 0 0 6px;
  font-size: 0.82rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  font-weight: 600;
  color: #bfdbfe;
}

.rt-home .rt-hero h1 {
  margin: 0 0 8px;
  color: #f8fafc;
  border: 0;
  padding: 0;
  font-size: 1.8rem;
  line-height: 1.25;
}

.rt-home .rt-hero p {
  margin: 0;
  color: #dbeafe;
}

.rt-home .rt-chip-row {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 18px;
}

.rt-home .rt-chip {
  display: inline-flex;
  align-items: center;
  gap: 7px;
  background: rgba(255, 255, 255, 0.14);
  border: 1px solid rgba(255, 255, 255, 0.26);
  color: #eff6ff;
  padding: 7px 12px;
  border-radius: 999px;
  font-size: 0.88rem;
  font-weight: 500;
}

.rt-home .rt-chip:hover {
  background: rgba(255, 255, 255, 0.24);
}

.rt-home .rt-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 14px;
  margin: 14px 0 18px;
}

.rt-home .rt-card {
  background: var(--rt-surface);
  border: 1px solid var(--rt-line);
  border-radius: 14px;
  padding: 16px 16px 14px;
  box-shadow: 0 10px 20px rgba(148, 163, 184, 0.12);
}

.rt-home .rt-card h2,
.rt-home .rt-card h3 {
  border: 0;
  padding: 0;
  margin: 0 0 10px;
  color: var(--rt-ink);
  font-size: 1.08rem;
}

.rt-home .rt-card p,
.rt-home .rt-card li {
  color: var(--rt-soft-ink);
}

.rt-home .rt-quick-list {
  list-style: none;
  margin: 0;
  padding: 0;
}

.rt-home .rt-quick-list li {
  padding: 8px 0;
  border-bottom: 1px dashed #e2e8f0;
}

.rt-home .rt-quick-list li:last-child {
  border-bottom: 0;
}

.rt-home .rt-section-title {
  border: 0;
  padding: 0;
  margin: 22px 0 12px;
  color: var(--rt-ink);
  font-size: 1.16rem;
}

.rt-home .rt-note {
  margin: 0 0 10px;
  color: #6b7280;
  font-size: 0.93rem;
}

.rt-home .rt-timeline {
  list-style: none;
  margin: 0;
  padding: 0;
}

.rt-home .rt-timeline li {
  background: var(--rt-surface-soft);
  border: 1px solid var(--rt-line);
  border-radius: 12px;
  padding: 12px 14px;
  margin-bottom: 10px;
  position: relative;
}

.rt-home .rt-timeline li::before {
  content: "";
  position: absolute;
  left: -1px;
  top: -1px;
  bottom: -1px;
  width: 4px;
  border-radius: 12px 0 0 12px;
  background: linear-gradient(180deg, var(--rt-blue-2), #0ea5e9);
}

.rt-home .rt-time {
  display: inline-block;
  font-size: 0.8rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--rt-blue);
  font-weight: 700;
  margin-bottom: 4px;
}

.rt-home .rt-award-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
}

.rt-home .rt-award {
  border: 1px solid #f1d2bf;
  background: linear-gradient(135deg, #fff9f5 0%, #fff 100%);
  border-radius: 12px;
  padding: 12px;
}

.rt-home .rt-award strong {
  color: #7c2d12;
}

.rt-home .rt-service {
  border-left: 4px solid var(--rt-accent);
  background: #fff9f3;
  border-radius: 10px;
  padding: 10px 12px;
  color: #7c2d12;
  margin-top: 8px;
}

.rt-home .rt-pub-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
}

.rt-home .rt-pub-card {
  border: 1px solid var(--rt-line);
  border-radius: 12px;
  overflow: hidden;
  background: #fff;
  box-shadow: 0 8px 18px rgba(148, 163, 184, 0.12);
}

.rt-home .rt-pub-thumb {
  display: block;
  width: 100%;
  height: 160px;
  object-fit: cover;
  border-bottom: 1px solid #e5edf5;
}

.rt-home .rt-pub-body {
  padding: 12px;
}

.rt-home .rt-pub-title {
  margin: 0 0 6px;
  font-size: 0.98rem;
  line-height: 1.35;
  color: #1f2937;
}

.rt-home .rt-pub-meta {
  margin: 0 0 10px;
  font-size: 0.85rem;
  color: #64748b;
}

.rt-home .rt-pub-links {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.rt-home .rt-pill {
  display: inline-block;
  border: 1px solid #c7d8eb;
  background: #f8fbff;
  color: #1d4ed8;
  border-radius: 999px;
  padding: 4px 9px;
  font-size: 0.8rem;
  font-weight: 600;
}

.rt-home .rt-pill:hover {
  background: #eaf3ff;
}

.rt-home .rt-visitor-wrap {
  display: grid;
  grid-template-columns: 1.2fr 1fr;
  gap: 12px;
}

.rt-home .rt-visitor-card {
  border: 1px solid var(--rt-line);
  border-radius: 12px;
  background: #fff;
  padding: 12px;
  text-align: center;
}

.rt-home .rt-counter-card {
  border: 1px solid #1e3a8a;
  border-radius: 12px;
  background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 55%, #2563eb 100%);
  color: #eff6ff;
  text-align: center;
  padding: 18px 12px;
  box-shadow: 0 12px 24px rgba(15, 23, 42, 0.22);
}

.rt-home .rt-counter-title {
  font-size: 0.76rem;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  opacity: 0.85;
}

.rt-home .rt-counter-value {
  font-size: 2.2rem;
  font-weight: 700;
  margin: 2px 0;
}

.rt-home .rt-counter-label {
  font-size: 0.86rem;
  opacity: 0.85;
}

@media (max-width: 900px) {
  .rt-home .rt-grid,
  .rt-home .rt-award-grid,
  .rt-home .rt-pub-grid,
  .rt-home .rt-visitor-wrap {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 640px) {
  .rt-home .rt-hero {
    padding: 22px 16px;
  }

  .rt-home .rt-hero h1 {
    font-size: 1.45rem;
  }
}
</style>

<div class="rt-home">
  <section class="rt-hero">
    <p class="rt-eyebrow">Ruitong Liu</p>
    <h1>Data-Centric AI for LLMs and Multimodal Intelligence</h1>
    <p>
      Senior undergraduate at
      <a href="https://www.dlut.edu.cn/" style="color:#f8fafc; text-decoration: underline;">Dalian University of Technology</a>
      (Mathematics and Applied Mathematics), working on scalable data synthesis, filtering, alignment, and structure-aware reasoning for trustworthy AI systems.
    </p>
    <div class="rt-chip-row">
      <a class="rt-chip" href="mailto:15668672116@163.com"><i class="fa fa-envelope" aria-hidden="true"></i> 15668672116@163.com</a>
      <a class="rt-chip" href="mailto:ruitong.jerry@gmail.com"><i class="fa fa-envelope-o" aria-hidden="true"></i> ruitong.jerry@gmail.com</a>
      <span class="rt-chip"><i class="fa fa-commenting" aria-hidden="true"></i> WeChat: ruitong_jerry</span>
    </div>
  </section>

  <section class="rt-grid">
    <article class="rt-card">
      <h2><i class="fa fa-flask" aria-hidden="true"></i> Research Overview</h2>
      <p>
        My research centers on Data-Centric AI for Large Language Models (LLMs) and Multimodal LLMs, spanning from
        large-scale data engineering to complex reasoning optimization.
      </p>
      <p>
        I focus on scalable frameworks for automated data synthesis and quality filtering, and design advanced alignment
        algorithms to enhance model intelligence and reliability.
      </p>
      <p>
        I also investigate Knowledge Graphs (KGs) for structure-aware modeling to improve factual consistency and logical reasoning.
      </p>
    </article>
    <article class="rt-card">
      <h2><i class="fa fa-rocket" aria-hidden="true"></i> Snapshot</h2>
      <ul class="rt-quick-list">
        <li><strong>Incoming Graduate Student</strong><br>Big Data program, School of Mathematical Sciences, <a href="https://www.pku.edu.cn/">Peking University</a></li>
        <li><strong>Current Role</strong><br>Intern at a top-tier quantitative firm in Beijing</li>
        <li><strong>Service</strong><br>Reviewer/PC Member: Transactions on Knowledge Discovery from Data (TKDD)</li>
      </ul>
    </article>
  </section>

  <h2 class="rt-section-title"><i class="fa fa-bolt" aria-hidden="true"></i> What's New</h2>
  <p class="rt-note">For detailed paper information, please check the <a href="/Publications.html">Publications</a> page.</p>
  <ul class="rt-timeline">
    <li>
      <span class="rt-time">February 2026</span><br>
      A survey on LLM data preparation was accepted by <strong>JCST's 40th Anniversary Special Issue</strong>.
    </li>
    <li>
      <span class="rt-time">January 2026</span><br>
      One paper submitted to <strong>IJCAI 2026</strong>; two papers submitted to <strong>ICML 2026</strong>; two papers submitted to <strong>ACL 2026</strong>.
    </li>
    <li>
      <span class="rt-time">August 2025</span><br>
      One paper submitted to <strong>TPAMI</strong>.
    </li>
    <li>
      <span class="rt-time">July 2025</span><br>
      One paper accepted by <strong>ICONIP 2025</strong>; pre-admitted to PKU through recommendation program (Bao Yan).
    </li>
  </ul>

  <h2 class="rt-section-title"><i class="fa fa-trophy" aria-hidden="true"></i> Selected Awards</h2>
  <p class="rt-note">For full honors and details, please visit <a href="/Awards/">Awards</a>.</p>
  <div class="rt-award-grid">
    <article class="rt-award">
      <strong>2025 Model Excellent Communist Youth League Member</strong><br>
      Dalian University of Technology (only 7 undergraduates university-wide)
    </article>
    <article class="rt-award">
      <strong>2025 Five-Star Volunteer</strong><br>
      Dalian University of Technology (600+ volunteer hours in 3 years)
    </article>
    <article class="rt-award">
      <strong>2024 Top 10 Volunteers</strong><br>
      Dalian University of Technology (all degree levels, only 10 students)
    </article>
    <article class="rt-award">
      <strong>2024 National Scholarship</strong><br>
      National-level competitive scholarship
    </article>
  </div>

  <div class="rt-service">
    <strong>Academic Service:</strong> Reviewer/PC Member, Transactions on Knowledge Discovery from Data (TKDD)
  </div>

  <h2 class="rt-section-title"><i class="fa fa-book" aria-hidden="true"></i> Selected Publications</h2>
  <p class="rt-note">Auto synced from your existing <a href="/publications/">Publications</a> page.</p>
  <div class="rt-pub-grid">
    <article class="rt-pub-card">
      <a href="https://arxiv.org/pdf/2602.04290">
        <img class="rt-pub-thumb" src="{{ '/images/pub_icml_guide.png' | relative_url }}" alt="Guided Verifier teaser">
      </a>
      <div class="rt-pub-body">
        <h3 class="rt-pub-title">Guided Verifier: Collaborative Multimodal Reasoning via Dynamic Process Supervision</h3>
        <p class="rt-pub-meta">ICML 2026 Under Review</p>
        <div class="rt-pub-links">
          <a class="rt-pill" href="https://arxiv.org/pdf/2602.04290">PDF</a>
          <a class="rt-pill" href="https://github.com/tongruiliu/Guided-GRPO">Code</a>
          <a class="rt-pill" href="https://huggingface.co/ruitongl/Guided-Verifier-8B">Model</a>
        </div>
      </div>
    </article>

    <article class="rt-pub-card">
      <a href="https://arxiv.org/pdf/2602.10494">
        <img class="rt-pub-thumb" src="{{ '/images/pub_canvas_cot.png' | relative_url }}" alt="Canvas-of-Thought teaser">
      </a>
      <div class="rt-pub-body">
        <h3 class="rt-pub-title">Canvas-of-Thought: Grounding Reasoning via Mutable Structured States</h3>
        <p class="rt-pub-meta">ICML 2026 Under Review</p>
        <div class="rt-pub-links">
          <a class="rt-pill" href="https://arxiv.org/pdf/2602.10494">PDF</a>
          <a class="rt-pill" href="https://github.com/Zzzyxii/Canvas-CoT">Code</a>
        </div>
      </div>
    </article>

    <article class="rt-pub-card">
      <a href="https://arxiv.org/pdf/2510.08966">
        <img class="rt-pub-thumb" src="{{ '/images/pub_www.png' | relative_url }}" alt="Semantic-Condition Tuning teaser">
      </a>
      <div class="rt-pub-body">
        <h3 class="rt-pub-title">Semantic-Condition Tuning: Fusing Graph Context with LLMs for KGC</h3>
        <p class="rt-pub-meta">IJCAI 2026 Under Review</p>
        <div class="rt-pub-links">
          <a class="rt-pill" href="https://arxiv.org/pdf/2510.08966">PDF</a>
          <a class="rt-pill" href="https://github.com/tongruiliu/GMT">Code</a>
        </div>
      </div>
    </article>

    <article class="rt-pub-card">
      <a href="https://arxiv.org/pdf/2506.23137">
        <img class="rt-pub-thumb" src="{{ '/images/pub_tpami.png' | relative_url }}" alt="Flow-Modulated Scoring teaser">
      </a>
      <div class="rt-pub-body">
        <h3 class="rt-pub-title">Flow-Modulated Scoring for Semantic-Aware Knowledge Graph Completion</h3>
        <p class="rt-pub-meta">TPAMI Under Review</p>
        <div class="rt-pub-links">
          <a class="rt-pill" href="https://arxiv.org/pdf/2506.23137">PDF</a>
          <a class="rt-pill" href="https://github.com/yuanwuyuan9/FMS">Code</a>
        </div>
      </div>
    </article>

    <article class="rt-pub-card">
      <a href="https://drive.google.com/file/d/1TqwULwmD8f-cpokfcfYfapuC9bNxrztA/view?usp=sharing">
        <img class="rt-pub-thumb" src="{{ '/images/pub_survey.png' | relative_url }}" alt="LLM data preparation survey teaser">
      </a>
      <div class="rt-pub-body">
        <h3 class="rt-pub-title">Data Preparation for Large Language Models: A Survey</h3>
        <p class="rt-pub-meta">JCST 40th Anniversary Special Issue</p>
        <div class="rt-pub-links">
          <a class="rt-pill" href="https://drive.google.com/file/d/1TqwULwmD8f-cpokfcfYfapuC9bNxrztA/view?usp=sharing">PDF</a>
        </div>
      </div>
    </article>
  </div>

  <h2 class="rt-section-title"><i class="fa fa-globe" aria-hidden="true"></i> Visitor</h2>
  <div class="rt-visitor-wrap">
    <div class="rt-visitor-card">
      <div style="display:inline-block; zoom:5;">
        <script type="text/javascript" id="clstr_globe" src="https://clustrmaps.com/globe.js?d=wWuKIsCZO2yYZA7sXQVVhdoENIGHAUsZCAy6ZjG-Uhk"></script>
      </div>
      <div style="font-size:0.86em;color:#64748b;margin-top:6px;">Visitor Geography</div>
    </div>
    <div class="rt-counter-card">
      <div class="rt-counter-title">Visit Counter</div>
      <div id="busuanzi_value_site_pv" data-offset="20" class="rt-counter-value">--</div>
      <div class="rt-counter-label">Page Views (PV)</div>
    </div>
  </div>
</div>

<script async src="//busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js"></script>
<script>
(function () {
  var counterEl = document.getElementById('busuanzi_value_site_pv');
  if (!counterEl) {
    return;
  }
  var attempts = 0;
  var timer = setInterval(function () {
    attempts += 1;
    if (counterEl.getAttribute('data-offset-applied') === 'true') {
      clearInterval(timer);
      return;
    }
    var raw = (counterEl.textContent || '').replace(/,/g, '');
    var value = parseInt(raw, 10);
    if (Number.isNaN(value)) {
      if (attempts >= 20) {
        clearInterval(timer);
      }
      return;
    }
    var offset = parseInt(counterEl.getAttribute('data-offset') || '0', 10);
    counterEl.textContent = (value + offset).toLocaleString();
    counterEl.setAttribute('data-offset-applied', 'true');
    clearInterval(timer);
  }, 500);
})();
</script>
