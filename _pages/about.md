---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
#main > article.page > .page__inner-wrap > header {
  display: none;
}

.masthead {
  display: none !important;
}

body {
  background:
    radial-gradient(1200px 620px at -10% -10%, rgba(37, 99, 235, 0.2) 0%, rgba(37, 99, 235, 0) 62%),
    radial-gradient(980px 560px at 110% 0%, rgba(14, 165, 233, 0.16) 0%, rgba(14, 165, 233, 0) 58%),
    linear-gradient(180deg, #f3f8ff 0%, #eef5ff 42%, #f7fbff 100%),
    repeating-linear-gradient(0deg, rgba(59, 130, 246, 0.06) 0 1px, transparent 1px 34px),
    repeating-linear-gradient(90deg, rgba(59, 130, 246, 0.06) 0 1px, transparent 1px 34px);
  background-attachment: fixed;
  padding-top: 0 !important;
  transition: background .45s ease;
}

body.rt-theme-dark {
  background:
    radial-gradient(1200px 620px at -10% -10%, rgba(59, 130, 246, 0.28) 0%, rgba(59, 130, 246, 0) 62%),
    radial-gradient(980px 560px at 110% 0%, rgba(34, 211, 238, 0.2) 0%, rgba(34, 211, 238, 0) 58%),
    linear-gradient(180deg, #020617 0%, #0b1223 46%, #0f172a 100%),
    repeating-linear-gradient(0deg, rgba(56, 189, 248, 0.08) 0 1px, transparent 1px 36px),
    repeating-linear-gradient(90deg, rgba(56, 189, 248, 0.08) 0 1px, transparent 1px 36px);
}

@media (min-width: 1024px) {
  #main {
    max-width: min(1720px, 97vw) !important;
  }

  .page {
    width: 82.5% !important;
    margin-right: 0 !important;
    padding-right: 0 !important;
  }
}

.rt-cyber-bg {
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: 0;
  overflow: hidden;
}

.rt-film-layer {
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: 1;
}

.rt-film-layer::before {
  content: "";
  position: absolute;
  inset: 0;
  background:
    radial-gradient(circle at 50% 45%, rgba(0, 0, 0, 0) 38%, rgba(2, 6, 23, 0.15) 100%),
    radial-gradient(circle at 0% 0%, rgba(15, 23, 42, 0.07) 0%, rgba(15, 23, 42, 0) 48%),
    radial-gradient(circle at 100% 0%, rgba(15, 23, 42, 0.07) 0%, rgba(15, 23, 42, 0) 48%);
}

.rt-film-layer::after {
  content: "";
  position: absolute;
  inset: 0;
  opacity: .14;
  mix-blend-mode: soft-light;
  background-image:
    radial-gradient(rgba(15, 23, 42, 0.28) .55px, transparent .7px),
    radial-gradient(rgba(30, 41, 59, 0.2) .45px, transparent .6px);
  background-size: 3px 3px, 5px 5px;
  background-position: 0 0, 1px 1px;
}

.rt-cyber-bg::before,
.rt-cyber-bg::after {
  content: "";
  position: absolute;
  width: 170vmax;
  height: 28vmax;
  left: -65vmax;
  top: 20vh;
  border-radius: 999px;
  transform: rotate(-11deg);
  filter: blur(16px);
}

.rt-cyber-bg::before {
  background: linear-gradient(100deg, rgba(37, 99, 235, 0) 8%, rgba(59, 130, 246, 0.22) 45%, rgba(14, 165, 233, 0.24) 55%, rgba(14, 165, 233, 0) 78%);
  animation: rt-cyber-scan 15s linear infinite;
}

.rt-cyber-bg::after {
  top: 63vh;
  background: linear-gradient(100deg, rgba(14, 165, 233, 0) 10%, rgba(56, 189, 248, 0.18) 46%, rgba(125, 211, 252, 0.2) 56%, rgba(125, 211, 252, 0) 80%);
  animation: rt-cyber-scan 19s linear infinite reverse;
  opacity: 0.72;
}

.rt-home {
  --rt-ink: #1f2937;
  --rt-soft-ink: #4b5563;/volume/math/users/rtliu/verl/recipe/lean_tts_async/1_7b_tts_async_first_wheelhouse.sh
  --rt-line: #dce7ef;
  --rt-blue: #2563eb;
  --rt-blue-2: #3b82f6;
  --rt-accent: #c2410c;
  --rt-surface: #ffffff;
  --rt-surface-soft: #f7fbff;
  --rt-panel-border: rgba(56, 189, 248, 0.44);
  --rt-panel-inner-border: rgba(125, 211, 252, 0.3);
  --rt-panel-bg: linear-gradient(135deg, rgba(248, 252, 255, 0.96) 0%, rgba(240, 248, 255, 0.92) 55%, rgba(255, 255, 255, 0.96) 100%);
  --rt-panel-shadow: 0 0 0 1px rgba(56, 189, 248, 0.14), inset 0 0 0 1px rgba(125, 211, 252, 0.22), 0 14px 26px rgba(15, 23, 42, 0.16);
  --rt-item-bg: linear-gradient(145deg, rgba(255, 255, 255, 0.94) 0%, rgba(245, 250, 255, 0.88) 100%);
  position: relative;
  z-index: 2;
  font-size: 1.035rem;
}

.rt-home[data-theme="dark"] {
  --rt-ink: #e2e8f0;
  --rt-soft-ink: #94a3b8;
  --rt-line: rgba(148, 163, 184, 0.35);
  --rt-panel-border: rgba(56, 189, 248, 0.48);
  --rt-panel-inner-border: rgba(125, 211, 252, 0.34);
  --rt-panel-bg: linear-gradient(135deg, rgba(15, 23, 42, 0.94) 0%, rgba(15, 23, 42, 0.88) 60%, rgba(30, 41, 59, 0.9) 100%);
  --rt-panel-shadow: 0 0 0 1px rgba(56, 189, 248, 0.2), inset 0 0 0 1px rgba(125, 211, 252, 0.22), 0 16px 28px rgba(2, 8, 23, 0.44);
  --rt-item-bg: linear-gradient(145deg, rgba(30, 41, 59, 0.9) 0%, rgba(15, 23, 42, 0.9) 100%);
}

.rt-home[data-theme="dark"] .rt-card,
.rt-home[data-theme="dark"] .rt-profile-block {
  background: linear-gradient(145deg, rgba(15, 23, 42, 0.95) 0%, rgba(30, 41, 59, 0.9) 100%);
  border-color: var(--rt-panel-border);
}

.rt-home[data-theme="dark"] .rt-intro-text,
.rt-home[data-theme="dark"] .rt-profile-sub,
.rt-home[data-theme="dark"] .rt-news-text,
.rt-home[data-theme="dark"] .rt-note,
.rt-home[data-theme="dark"] .rt-pub-authors,
.rt-home[data-theme="dark"] .rt-pub-meta {
  color: #94a3b8;
}

.rt-home[data-theme="dark"] .rt-profile-main,
.rt-home[data-theme="dark"] .rt-profile-main a,
.rt-home[data-theme="dark"] .rt-profile-company,
.rt-home[data-theme="dark"] .rt-pub-title,
.rt-home[data-theme="dark"] .rt-award strong {
  color: #e2e8f0;
}

.rt-home[data-theme="dark"] .rt-focus-pill,
.rt-home[data-theme="dark"] .rt-chip,
.rt-home[data-theme="dark"] .rt-pill {
  border-color: rgba(125, 211, 252, 0.45);
  background: linear-gradient(135deg, rgba(30, 41, 59, 0.92) 0%, rgba(15, 23, 42, 0.95) 100%);
  color: #dbeafe;
}

.rt-home[data-theme="dark"] .rt-time {
  border-color: rgba(125, 211, 252, 0.45);
  background: rgba(30, 41, 59, 0.86);
  color: #93c5fd;
}

.rt-home[data-theme="dark"] a {
  color: #93c5fd;
}

.rt-home[data-theme="dark"] a:hover {
  color: #67e8f9;
}

.rt-home[data-theme="dark"] .rt-overview-name,
.rt-home[data-theme="dark"] .rt-section-title,
.rt-home[data-theme="dark"] .rt-profile-head,
.rt-home[data-theme="dark"] .rt-profile-date,
.rt-home[data-theme="dark"] .rt-profile-time,
.rt-home[data-theme="dark"] .rt-service-title,
.rt-home[data-theme="dark"] .rt-counter-title {
  color: #7dd3fc;
}

.rt-home[data-theme="dark"] .rt-welcome-line,
.rt-home[data-theme="dark"] .rt-profile-role,
.rt-home[data-theme="dark"] .rt-service-text,
.rt-home[data-theme="dark"] .rt-counter-label,
.rt-home[data-theme="dark"] .rt-counter-value {
  color: #e2e8f0;
}

.rt-home[data-theme="dark"] .rt-overview-divider {
  border-top-color: rgba(125, 211, 252, 0.34);
}

.rt-home[data-theme="dark"] .rt-news-text strong,
.rt-home[data-theme="dark"] .rt-pub-authors strong,
.rt-home[data-theme="dark"] .rt-profile-role strong,
.rt-home[data-theme="dark"] .rt-award strong {
  color: #e2e8f0;
}

.rt-home[data-theme="dark"] .rt-award-list li,
.rt-home[data-theme="dark"] .rt-award-collapse summary,
.rt-home[data-theme="dark"] .rt-award-collapse summary::after {
  color: #cbd5e1;
}

.rt-home[data-theme="dark"] .rt-award-collapse {
  border-color: rgba(125, 211, 252, 0.34);
  background: rgba(15, 23, 42, 0.62);
}

.rt-home[data-theme="dark"] .rt-award {
  border-color: var(--rt-panel-inner-border);
  background: var(--rt-item-bg);
}

.rt-home[data-theme="dark"] .rt-news-zone .rt-time {
  color: #93c5fd;
}

.rt-home a {
  text-decoration: none;
}

.rt-home .rt-overview-card {
  margin-bottom: 2px;
  padding: 18px 18px 16px;
}

.rt-home .rt-overview-name {
  margin: 0 0 4px;
  font-size: 0.86rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: #1d4ed8;
  font-weight: 700;
}

.rt-home .rt-overview-title {
  margin: 0 0 10px;
  font-size: 1.6rem;
  line-height: 1.3;
  color: #0f172a;
  border: 0;
  padding: 0;
}

.rt-home .rt-overview-divider {
  border-top: 1px dashed #d8e5f3;
  margin: 14px 0 12px;
}

.rt-home .rt-chip-row {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 12px;
}

.rt-home .rt-chip {
  display: inline-flex;
  align-items: center;
  gap: 7px;
  background: linear-gradient(135deg, #f8fbff 0%, #ffffff 100%);
  border: 1px solid #d5e4f4;
  color: #1e3a8a;
  padding: 7px 12px;
  border-radius: 999px;
  font-size: 0.88rem;
  font-weight: 600;
  box-shadow: 0 8px 14px rgba(148, 163, 184, 0.12);
}

.rt-home .rt-chip:hover {
  background: linear-gradient(135deg, #ecf5ff 0%, #ffffff 100%);
}

.rt-home .rt-jump-nav {
  display: grid;
  grid-template-columns: repeat(5, minmax(0, 1fr));
  gap: 10px;
  margin: 4px 0 12px;
  padding: 9px 9px 13px;
  border-radius: 14px;
  border: 1px solid rgba(56, 189, 248, 0.5);
  background: linear-gradient(145deg, rgba(15, 23, 42, 0.72) 0%, rgba(15, 23, 42, 0.58) 100%);
  box-shadow: 0 0 0 1px rgba(14, 165, 233, 0.18) inset, 0 14px 28px rgba(2, 8, 23, 0.28);
  position: sticky;
  top: 10px;
  z-index: 15;
  overflow: hidden;
  -webkit-backdrop-filter: blur(8px);
  backdrop-filter: blur(8px);
}

.rt-theme-toggle {
  position: fixed;
  right: 14px;
  top: 14px;
  z-index: 28;
  display: inline-grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 4px;
  border: 1px solid rgba(56, 189, 248, 0.62);
  background: linear-gradient(135deg, rgba(15, 23, 42, 0.9) 0%, rgba(30, 41, 59, 0.9) 100%);
  border-radius: 999px;
  padding: 4px;
  box-shadow: 0 0 0 1px rgba(125, 211, 252, 0.2) inset, 0 12px 22px rgba(2, 8, 23, 0.3);
}

.rt-theme-option {
  appearance: none;
  border: 1px solid transparent;
  background: transparent;
  color: #bfdbfe;
  border-radius: 999px;
  padding: 5px 10px;
  min-width: 58px;
  font-size: 0.72rem;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  cursor: pointer;
  transition: color .2s ease, border-color .22s ease, box-shadow .22s ease, background .22s ease, transform .2s ease;
}

.rt-theme-option:hover {
  color: #e0f2fe;
}

.rt-theme-option.is-active {
  border-color: rgba(125, 211, 252, 0.86);
  background: linear-gradient(135deg, rgba(30, 64, 175, 0.82) 0%, rgba(37, 99, 235, 0.78) 100%);
  color: #e0f2fe;
  box-shadow: 0 0 0 1px rgba(191, 219, 254, 0.35) inset, 0 0 12px rgba(56, 189, 248, 0.34);
  transform: translateY(-1px);
}

.rt-theme-toggle.rt-theme-toggle--sidebar {
  position: relative;
  right: auto;
  top: auto;
  z-index: 12;
  width: 100%;
  margin: 10px 0 14px;
}

body.rt-theme-dark .rt-theme-toggle {
  border-color: rgba(125, 211, 252, 0.76);
  background: linear-gradient(135deg, rgba(2, 6, 23, 0.94) 0%, rgba(15, 23, 42, 0.9) 100%);
}

body.rt-theme-dark .rt-theme-option {
  color: #94a3b8;
}

body.rt-theme-dark .rt-theme-option.is-active {
  color: #e2e8f0;
  border-color: rgba(125, 211, 252, 0.88);
  background: linear-gradient(135deg, rgba(30, 58, 138, 0.9) 0%, rgba(30, 64, 175, 0.84) 100%);
}

.sidebar > div[itemscope] {
  position: relative;
  border: 1px solid rgba(56, 189, 248, 0.34);
  border-radius: 0;
  clip-path: polygon(0 0, calc(100% - 14px) 0, 100% 14px, 100% 100%, 0 100%);
  background: linear-gradient(145deg, rgba(248, 252, 255, 0.96) 0%, rgba(240, 248, 255, 0.93) 100%);
  box-shadow: 0 0 0 1px rgba(56, 189, 248, 0.12), inset 0 0 0 1px rgba(125, 211, 252, 0.2), 0 14px 22px rgba(15, 23, 42, 0.14);
  padding: 12px 12px 10px;
  overflow: hidden;
}

.sidebar > div[itemscope]::before {
  content: "";
  position: absolute;
  left: 12px;
  right: 12px;
  top: 10px;
  height: 2px;
  border-radius: 999px;
  background: linear-gradient(90deg, rgba(14, 165, 233, 0.2) 0%, rgba(224, 242, 254, 0.95) 50%, rgba(59, 130, 246, 0.2) 100%);
  box-shadow: 0 0 10px rgba(56, 189, 248, 0.34);
}

.sidebar .author__avatar {
  display: block;
  width: 100%;
}

.sidebar .author__avatar img {
  max-width: min(188px, 86%);
  border-radius: 14px !important;
  border: 1px solid rgba(125, 211, 252, 0.5) !important;
  background: linear-gradient(135deg, #eff6ff 0%, #ffffff 100%);
  padding: 6px !important;
  box-shadow: 0 10px 16px rgba(59, 130, 246, 0.16);
}

.sidebar .author__content {
  display: block;
  width: 100%;
  padding: 0 !important;
  margin-top: 8px;
}

.sidebar .author__name {
  color: #0f172a;
  font-size: 1.03rem !important;
  letter-spacing: 0.02em;
  margin-bottom: 6px !important;
}

.sidebar .author__bio {
  color: #475569;
  line-height: 1.55;
}

.sidebar .author__urls-wrapper {
  margin-top: 10px;
  display: block;
  cursor: default;
}

.sidebar .author__urls {
  display: block !important;
  position: relative;
  right: auto;
  margin: 0;
  padding: 0;
  border: 0;
  background: transparent;
  box-shadow: none;
}

.sidebar .author__urls li {
  margin: 0 0 8px;
  color: #475569;
  font-size: 0.82rem;
  line-height: 1.45;
}

.sidebar .author__urls li a {
  display: flex;
  align-items: center;
  gap: 8px;
  border: 1px solid #d7e7f8;
  border-radius: 9px;
  padding: 6px 8px;
  background: linear-gradient(135deg, #f8fbff 0%, #eef6ff 100%);
  color: #1e3a8a;
  font-size: 0.81rem;
  font-weight: 600;
  transition: transform .2s ease, box-shadow .22s ease, border-color .22s ease;
}

.sidebar .author__urls li a:hover {
  transform: translateY(-1px);
  border-color: #7dd3fc;
  box-shadow: 0 0 0 1px rgba(125, 211, 252, 0.44) inset, 0 8px 14px rgba(56, 189, 248, 0.2);
}

body.rt-theme-dark .sidebar > div[itemscope] {
  border-color: rgba(56, 189, 248, 0.5);
  background: linear-gradient(145deg, rgba(15, 23, 42, 0.95) 0%, rgba(30, 41, 59, 0.92) 100%);
  box-shadow: 0 0 0 1px rgba(56, 189, 248, 0.2), inset 0 0 0 1px rgba(125, 211, 252, 0.2), 0 16px 26px rgba(2, 8, 23, 0.4);
}

body.rt-theme-dark .sidebar .author__name {
  color: #e2e8f0;
}

body.rt-theme-dark .sidebar .author__bio {
  color: #94a3b8;
}

body.rt-theme-dark .sidebar .author__avatar img {
  border-color: rgba(125, 211, 252, 0.64) !important;
  background: linear-gradient(135deg, rgba(15, 23, 42, 0.86) 0%, rgba(30, 41, 59, 0.82) 100%);
}

body.rt-theme-dark .sidebar .author__urls li a {
  border-color: rgba(125, 211, 252, 0.38);
  background: linear-gradient(135deg, rgba(30, 41, 59, 0.9) 0%, rgba(15, 23, 42, 0.92) 100%);
  color: #cbd5e1;
}

body.rt-theme-dark .sidebar .author__urls li {
  color: #94a3b8;
}

.rt-home .rt-nav-progress {
  position: absolute;
  left: 11px;
  right: 11px;
  bottom: 7px;
  height: 2px;
  border-radius: 999px;
  background: rgba(56, 189, 248, 0.24);
  overflow: hidden;
  pointer-events: none;
  z-index: 0;
}

.rt-home .rt-nav-progress-fill {
  display: block;
  width: 100%;
  height: 100%;
  transform-origin: left center;
  transform: scaleX(0);
  background: linear-gradient(90deg, #22d3ee 0%, #60a5fa 42%, #38bdf8 100%);
  box-shadow: 0 0 10px rgba(56, 189, 248, 0.74);
  transition: transform .16s linear;
}

.rt-home .rt-jump-item {
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  overflow: hidden;
  gap: 7px;
  border: 1px solid rgba(56, 189, 248, 0.48);
  background: linear-gradient(135deg, rgba(30, 41, 59, 0.78) 0%, rgba(15, 23, 42, 0.9) 100%);
  color: #dbeafe;
  border-radius: 11px;
  padding: 10px 8px;
  font-size: 0.9rem;
  font-weight: 600;
  text-align: center;
  transition: transform .22s ease, box-shadow .24s ease, background .22s ease, border-color .22s ease;
  box-shadow: 0 8px 16px rgba(2, 8, 23, 0.24), 0 0 0 1px rgba(59, 130, 246, 0.15) inset;
  z-index: 1;
}

.rt-home .rt-jump-item > * {
  position: relative;
  z-index: 1;
}

.rt-home .rt-jump-item::before {
  content: "";
  position: absolute;
  top: -20%;
  left: -140%;
  width: 55%;
  height: 150%;
  background: linear-gradient(100deg, rgba(125, 211, 252, 0) 0%, rgba(125, 211, 252, 0.14) 20%, rgba(224, 242, 254, 0.85) 50%, rgba(125, 211, 252, 0.14) 80%, rgba(125, 211, 252, 0) 100%);
  transform: skewX(-22deg);
  opacity: 0;
  transition: transform .62s ease, opacity .22s ease;
}

.rt-home .rt-jump-item:hover {
  background: linear-gradient(135deg, rgba(30, 58, 138, 0.72) 0%, rgba(30, 64, 175, 0.62) 100%);
  transform: translateY(-2px) scale(1.02);
  border-color: rgba(125, 211, 252, 0.9);
  box-shadow: 0 0 0 1px rgba(125, 211, 252, 0.4) inset, 0 0 16px rgba(14, 165, 233, 0.38), 0 16px 24px rgba(37, 99, 235, 0.24);
}

.rt-home .rt-jump-item:hover::before {
  opacity: 1;
  transform: translateX(460%) skewX(-22deg);
}

.rt-home .rt-jump-item.is-active {
  background: linear-gradient(135deg, rgba(30, 58, 138, 0.8) 0%, rgba(30, 64, 175, 0.72) 100%);
  transform: translateY(-1px) scale(1.05);
  border-color: rgba(186, 230, 253, 0.98);
  box-shadow: 0 0 0 1px rgba(186, 230, 253, 0.5) inset, 0 0 18px rgba(56, 189, 248, 0.42), 0 18px 26px rgba(30, 64, 175, 0.3);
}

.rt-home .rt-jump-item.is-active::before {
  opacity: 1;
  transform: translateX(460%) skewX(-22deg);
}

.rt-home .rt-top-intro {
  margin: 14px 0 18px;
}

.rt-home .rt-card {
  background: var(--rt-surface);
  border: 1px solid var(--rt-line);
  border-radius: 14px;
  padding: 16px 16px 14px;
  box-shadow: 0 10px 20px rgba(148, 163, 184, 0.12);
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
  position: relative;
  overflow: hidden;
}

.rt-home .rt-card,
.rt-home .rt-profile-block,
.rt-home .rt-news-zone,
.rt-home .rt-awards-zone,
.rt-home .rt-pubs-zone,
.rt-home .rt-award,
.rt-home .rt-pub-card {
  border-radius: 0;
  clip-path: polygon(0 0, calc(100% - 14px) 0, 100% 14px, 100% 100%, 0 100%);
  box-shadow: 0 0 0 1px rgba(56, 189, 248, 0.18), inset 0 0 0 1px rgba(125, 211, 252, 0.24), 0 12px 24px rgba(15, 23, 42, 0.14);
}

.rt-home .rt-card::after {
  content: "";
  position: absolute;
  right: -34px;
  top: -30px;
  width: 90px;
  height: 90px;
  border-radius: 999px;
  background: radial-gradient(circle, rgba(37, 99, 235, 0.2) 0%, rgba(37, 99, 235, 0) 72%);
  opacity: 0;
  transition: opacity .24s ease;
}

.rt-home .rt-card:hover {
  transform: translateY(-3px) scale(1.015);
  border-color: #bfdbfe;
  box-shadow: 0 16px 26px rgba(96, 165, 250, 0.22);
}

.rt-home .rt-card:hover::after {
  opacity: 1;
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

.rt-home .rt-intro-text {
  margin: 0;
  color: #334155;
  line-height: 1.7;
}

.rt-home .rt-welcome-line {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  margin-right: 4px;
  font-weight: 700;
  color: #0f172a;
}

.rt-home .rt-wave-hand {
  display: inline-block;
  transform-origin: 72% 72%;
  color: #0ea5e9;
  text-shadow: 0 0 8px rgba(14, 165, 233, 0.45), 0 0 16px rgba(56, 189, 248, 0.28);
  animation: rt-wave 2s ease-in-out infinite;
}

.rt-home .rt-focus-row {
  display: flex;
  flex-wrap: wrap;
  gap: 9px;
  margin-top: 12px;
}

.rt-home .rt-focus-pill {
  display: inline-flex;
  align-items: center;
  border: 1px solid #c7dcf7;
  border-left: 3px solid #38bdf8;
  background: linear-gradient(135deg, #f3f9ff 0%, #ffffff 100%);
  color: #0f2f70;
  border-radius: 8px;
  padding: 4px 10px 4px 9px;
  font-size: 0.8rem;
  font-weight: 700;
  letter-spacing: 0.01em;
  text-transform: none;
}

.rt-home .rt-tag-card {
  position: relative;
}

.rt-home .rt-tag-pad {
  padding-top: 28px !important;
}

.rt-home .rt-corner-tag {
  position: absolute;
  top: 8px;
  right: 18px;
  z-index: 4;
  display: inline-flex;
  align-items: center;
  gap: 6px;
  height: 20px;
  padding: 0 9px 0 10px;
  border-radius: 999px;
  border: 1px solid #86efac;
  background: linear-gradient(135deg, #f0fdf4 0%, #dcfce7 100%);
  color: #166534;
  font-size: 0.64rem;
  font-weight: 800;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  box-shadow: 0 8px 14px rgba(34, 197, 94, 0.16);
  pointer-events: none;
}

.rt-home .rt-corner-tag::after {
  content: "";
  width: 8px;
  height: 8px;
  border-radius: 2px;
  border: 1px solid #16a34a;
  background: #bbf7d0;
  box-shadow: 0 0 0 1px rgba(255, 255, 255, 0.52) inset;
}

.rt-home .rt-corner-tag--blue {
  border-color: #93c5fd;
  background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
  color: #1e3a8a;
  box-shadow: 0 8px 14px rgba(59, 130, 246, 0.16);
}

.rt-home .rt-corner-tag--blue::after {
  border-color: #3b82f6;
  background: #bfdbfe;
}

.rt-home .rt-corner-tag--gold {
  border-color: #fdba74;
  background: linear-gradient(135deg, #fff7ed 0%, #ffedd5 100%);
  color: #9a3412;
  box-shadow: 0 8px 14px rgba(251, 146, 60, 0.16);
}

.rt-home .rt-corner-tag--gold::after {
  border-color: #ea580c;
  background: #fed7aa;
}

.rt-home .rt-corner-tag--cyan {
  border-color: #7dd3fc;
  background: linear-gradient(135deg, #ecfeff 0%, #cffafe 100%);
  color: #0c4a6e;
  box-shadow: 0 8px 14px rgba(6, 182, 212, 0.16);
}

.rt-home .rt-corner-tag--cyan::after {
  border-color: #0891b2;
  background: #a5f3fc;
}

.rt-home .rt-profile-stack {
  margin-top: 12px;
  display: grid;
  gap: 12px;
}

.rt-home .rt-profile-block {
  border: 1px solid #dbe7f5;
  border-radius: 12px;
  background: linear-gradient(145deg, rgba(255, 255, 255, 0.92) 0%, rgba(245, 250, 255, 0.88) 100%);
  padding: 12px 12px 11px;
  box-shadow: 0 9px 16px rgba(148, 163, 184, 0.14);
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
}

.rt-home .rt-profile-block:hover {
  transform: translateY(-3px) scale(1.008);
  border-color: #bfdbfe;
  box-shadow: 0 16px 24px rgba(96, 165, 250, 0.22);
}

.rt-home .rt-profile-head {
  margin: 0 0 8px;
  font-size: 0.76rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: #1e3a8a;
  font-weight: 800;
}

.rt-home .rt-profile-list {
  list-style: none;
  margin: 0;
  padding: 0;
  display: grid;
  gap: 8px;
}

.rt-home .rt-profile-list--intern {
  gap: 10px;
}

.rt-home .rt-profile-item {
  display: grid;
  grid-template-columns: 160px minmax(0, 1fr);
  gap: 12px;
  align-items: start;
  padding-top: 2px;
}

.rt-home .rt-profile-item + .rt-profile-item {
  border-top: 1px dashed #dbe7f5;
  padding-top: 10px;
}

.rt-home .rt-profile-date {
  color: #1e3a8a;
  font-size: 0.88rem;
  font-weight: 700;
  white-space: nowrap;
}

.rt-home .rt-profile-main {
  margin: 0 0 4px;
  color: #0f172a;
  font-weight: 700;
  line-height: 1.45;
}

.rt-home .rt-profile-main a {
  color: #0f172a;
}

.rt-home .rt-profile-main a:hover {
  color: #1d4ed8;
}

.rt-home .rt-profile-sub {
  margin: 0;
  color: #475569;
  font-size: 0.9rem;
  line-height: 1.5;
}

.rt-home .rt-profile-role-line {
  margin-top: 2px;
  display: flex;
  flex-wrap: wrap;
  gap: 7px;
  align-items: center;
}

.rt-home .rt-profile-role {
  display: inline;
  color: #334155;
  font-size: 0.93rem;
}

.rt-home .rt-profile-item--intern {
  display: block;
  padding-top: 2px;
}

.rt-home .rt-profile-item--intern + .rt-profile-item--intern {
  border-top: 1px dashed #dbe7f5;
  padding-top: 10px;
}

.rt-home .rt-profile-top {
  display: flex;
  align-items: baseline;
  gap: 10px;
}

.rt-home .rt-profile-company {
  margin: 0;
  color: #0f172a;
  font-weight: 700;
  line-height: 1.45;
}

.rt-home .rt-profile-time {
  margin-left: auto;
  color: #1e3a8a;
  font-size: 0.88rem;
  font-weight: 700;
  white-space: nowrap;
  text-align: right;
}

.rt-home .rt-spotlight {
  display: inline-block;
  margin-left: 0;
  padding: 1px 7px;
  border-radius: 999px;
  border: 1px solid #fda4af;
  background: #fff1f2;
  color: #be123c;
  font-weight: 800;
}

.rt-home .rt-section-title {
  border: 0;
  padding: 0;
  margin: 22px 0 12px;
  color: var(--rt-ink);
  font-size: 1.16rem;
  display: flex;
  align-items: center;
  gap: 8px;
}

.rt-home .rt-reveal {
  opacity: 0;
  transform: translateY(16px);
  transition: opacity .56s ease, transform .56s ease;
}

.rt-home .rt-reveal.is-inview {
  opacity: 1;
  transform: translateY(0);
}

.rt-home .rt-title-glitch {
  position: relative;
  display: inline-block;
  font-weight: 800;
  letter-spacing: 0.02em;
}

.rt-home .rt-title-glitch::before,
.rt-home .rt-title-glitch::after {
  content: attr(data-text);
  position: absolute;
  left: 0;
  top: 0;
  opacity: 0;
  pointer-events: none;
}

.rt-home .rt-title-glitch::before {
  color: #22d3ee;
  text-shadow: 0 0 12px rgba(34, 211, 238, 0.72);
}

.rt-home .rt-title-glitch::after {
  color: #f472b6;
  text-shadow: 0 0 12px rgba(244, 114, 182, 0.6);
}

.rt-home .rt-section-title:hover .rt-title-glitch::before {
  opacity: 0.75;
  animation: rt-glitch-a .36s steps(2, end) 1;
}

.rt-home .rt-section-title:hover .rt-title-glitch::after {
  opacity: 0.68;
  animation: rt-glitch-b .36s steps(2, end) 1;
}

.rt-home .rt-note {
  margin: 0 0 10px;
  color: #6b7280;
  font-size: 0.93rem;
}

.rt-home .rt-news-zone,
.rt-home .rt-awards-zone,
.rt-home .rt-pubs-zone {
  border-color: var(--rt-panel-border);
  background: var(--rt-panel-bg);
  box-shadow: var(--rt-panel-shadow);
}

.rt-home .rt-timeline li,
.rt-home .rt-award,
.rt-home .rt-pub-card {
  border-color: var(--rt-panel-inner-border);
  background: var(--rt-item-bg);
}

.rt-home .rt-timeline {
  list-style: none;
  margin: 0;
  padding: 0 0 0 24px;
  display: grid;
  gap: 12px;
  position: relative;
}

.rt-home .rt-timeline::before {
  content: "";
  position: absolute;
  left: 8px;
  top: 8px;
  bottom: 8px;
  width: 2px;
  border-radius: 999px;
  background: linear-gradient(180deg, rgba(56, 189, 248, 0.22) 0%, rgba(59, 130, 246, 0.88) 45%, rgba(14, 165, 233, 0.25) 100%);
  box-shadow: 0 0 10px rgba(56, 189, 248, 0.5);
}

.rt-home .rt-timeline::after {
  content: "";
  position: absolute;
  left: 7px;
  width: 4px;
  height: 50px;
  border-radius: 999px;
  background: linear-gradient(180deg, rgba(224, 242, 254, 0) 0%, rgba(224, 242, 254, 0.95) 50%, rgba(224, 242, 254, 0) 100%);
  box-shadow: 0 0 14px rgba(125, 211, 252, 0.82);
  animation: rt-rail-flow 5.8s linear infinite;
}

.rt-home .rt-news-zone {
  position: relative;
  border-radius: 16px;
  padding: 14px;
  margin-bottom: 6px;
  overflow: hidden;
  isolation: isolate;
  background: var(--rt-panel-bg);
  border: 1px solid var(--rt-panel-border);
  box-shadow: var(--rt-panel-shadow);
}

.rt-home .rt-news-zone::before {
  content: "";
  position: absolute;
  width: 280px;
  height: 280px;
  border-radius: 999px;
  top: -130px;
  right: -90px;
  background: radial-gradient(circle, rgba(37, 99, 235, 0.3) 0%, rgba(37, 99, 235, 0) 68%);
  filter: blur(4px);
  animation: rt-news-float 9s ease-in-out infinite;
  z-index: -1;
}

.rt-home .rt-news-zone::after {
  content: "";
  position: absolute;
  width: 220px;
  height: 220px;
  border-radius: 999px;
  bottom: -110px;
  left: -70px;
  background: radial-gradient(circle, rgba(14, 165, 233, 0.26) 0%, rgba(14, 165, 233, 0) 72%);
  filter: blur(3px);
  animation: rt-news-float 12s ease-in-out infinite reverse;
  z-index: -1;
}

.rt-home .rt-news-zone .rt-note {
  margin-bottom: 12px;
}

.rt-home .rt-timeline li {
  background: var(--rt-item-bg);
  border: 1px solid var(--rt-panel-inner-border);
  border-radius: 12px;
  padding: 12px 14px;
  position: relative;
  display: grid;
  grid-template-columns: 116px minmax(0, 1fr);
  column-gap: 12px;
  align-items: start;
  box-shadow: 0 10px 18px rgba(148, 163, 184, 0.14);
  transition: transform .22s ease, box-shadow .25s ease, border-color .25s ease;
  backdrop-filter: blur(5px);
  cursor: pointer;
}

.rt-home .rt-timeline li:hover {
  transform: translateY(-3px) scale(1.018);
  box-shadow: 0 18px 30px rgba(96, 165, 250, 0.24);
  border-color: #bfdbfe;
}

.rt-home .rt-timeline li:active {
  transform: translateY(-1px) scale(1.01);
}

.rt-home .rt-timeline li::before {
  content: "";
  position: absolute;
  left: -21px;
  top: 50%;
  width: 12px;
  height: 12px;
  border-radius: 999px;
  transform: translateY(-50%);
  border: 2px solid #38bdf8;
  background: #e0f2fe;
  box-shadow: 0 0 0 2px rgba(191, 219, 254, 0.45), 0 0 14px rgba(56, 189, 248, 0.78);
  animation: rt-node-pulse 2.4s ease-in-out infinite;
}

.rt-home .rt-timeline li::after {
  content: "";
  position: absolute;
  top: -18px;
  right: -14px;
  width: 84px;
  height: 84px;
  border-radius: 999px;
  background: radial-gradient(circle, rgba(191, 219, 254, 0.5) 0%, rgba(191, 219, 254, 0) 70%);
  opacity: 0;
  transition: opacity .25s ease;
}

.rt-home .rt-timeline li:hover::after {
  opacity: 1;
}

.rt-home .rt-timeline li:nth-child(2n)::before {
  animation-delay: .35s;
}

.rt-home .rt-timeline li:nth-child(3n)::before {
  animation-delay: .68s;
}

.rt-home .rt-time {
  display: inline-flex;
  align-items: center;
  justify-content: flex-start;
  min-height: 30px;
  font-size: 0.76rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--rt-blue);
  font-weight: 700;
  margin-bottom: 0;
  padding: 2px 10px;
  border-radius: 999px;
  border: 1px solid #bfdbfe;
  background: #eff6ff;
}

.rt-home .rt-news-text {
  color: #334155;
  line-height: 1.52;
}

.rt-home .rt-news-text strong {
  color: #1d4ed8;
}

.rt-home .rt-award-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
}

.rt-home .rt-awards-zone {
  position: relative;
  border-radius: 16px;
  padding: 14px;
  margin-bottom: 6px;
  overflow: hidden;
  isolation: isolate;
  background: var(--rt-panel-bg);
  border: 1px solid var(--rt-panel-border);
  box-shadow: var(--rt-panel-shadow);
}

.rt-home .rt-awards-zone::before {
  content: "";
  position: absolute;
  width: 260px;
  height: 260px;
  border-radius: 999px;
  top: -120px;
  right: -85px;
  background: radial-gradient(circle, rgba(251, 146, 60, 0.28) 0%, rgba(251, 146, 60, 0) 70%);
  filter: blur(3px);
  animation: rt-news-float 10s ease-in-out infinite;
  z-index: -1;
}

.rt-home .rt-awards-zone::after {
  content: "";
  position: absolute;
  width: 220px;
  height: 220px;
  border-radius: 999px;
  bottom: -100px;
  left: -70px;
  background: radial-gradient(circle, rgba(245, 158, 11, 0.24) 0%, rgba(245, 158, 11, 0) 72%);
  filter: blur(3px);
  animation: rt-news-float 12s ease-in-out infinite reverse;
  z-index: -1;
}

.rt-home .rt-award {
  border: 1px solid var(--rt-panel-inner-border);
  background: var(--rt-item-bg);
  border-radius: 12px;
  padding: 12px;
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
  box-shadow: 0 10px 18px rgba(251, 146, 60, 0.10);
  backdrop-filter: blur(4px);
  cursor: pointer;
}

.rt-home .rt-award:hover {
  transform: translateY(-3px) scale(1.015);
  border-color: #fdba74;
  box-shadow: 0 18px 28px rgba(251, 146, 60, 0.20);
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

.rt-home .rt-award-collapse {
  margin-top: 12px;
  border: 1px dashed #f2c9ad;
  border-radius: 12px;
  background: rgba(255, 255, 255, 0.72);
  overflow: hidden;
}

.rt-home .rt-award-collapse summary {
  list-style: none;
  cursor: pointer;
  padding: 12px 14px;
  font-weight: 700;
  color: #9a3412;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 8px;
}

.rt-home .rt-award-collapse summary::-webkit-details-marker {
  display: none;
}

.rt-home .rt-award-collapse summary::after {
  content: "+";
  font-size: 1.1rem;
  line-height: 1;
  transition: transform .22s ease;
}

.rt-home .rt-award-collapse[open] summary::after {
  content: "-";
}

.rt-home .rt-award-list {
  margin: 0;
  padding: 0 14px 14px 24px;
}

.rt-home .rt-award-list li {
  margin: 0 0 8px;
  color: #7c2d12;
}

.rt-home .rt-pub-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 12px;
}

.rt-home .rt-pubs-zone {
  position: relative;
  border-radius: 16px;
  padding: 14px;
  margin-bottom: 6px;
  overflow: hidden;
  isolation: isolate;
  background: var(--rt-panel-bg);
  border: 1px solid var(--rt-panel-border);
  box-shadow: var(--rt-panel-shadow);
}

.rt-home .rt-pubs-zone::before {
  content: "";
  position: absolute;
  width: 260px;
  height: 260px;
  border-radius: 999px;
  top: -120px;
  right: -85px;
  background: radial-gradient(circle, rgba(59, 130, 246, 0.28) 0%, rgba(59, 130, 246, 0) 70%);
  filter: blur(3px);
  animation: rt-news-float 10.5s ease-in-out infinite;
  z-index: -1;
}

.rt-home .rt-pubs-zone::after {
  content: "";
  position: absolute;
  width: 220px;
  height: 220px;
  border-radius: 999px;
  bottom: -100px;
  left: -70px;
  background: radial-gradient(circle, rgba(14, 165, 233, 0.24) 0%, rgba(14, 165, 233, 0) 72%);
  filter: blur(3px);
  animation: rt-news-float 11.8s ease-in-out infinite reverse;
  z-index: -1;
}

.rt-home .rt-pub-card {
  display: grid;
  grid-template-columns: minmax(260px, 320px) 1fr;
  align-items: start;
  border: 1px solid var(--rt-panel-inner-border);
  border-radius: 12px;
  overflow: hidden;
  background: var(--rt-item-bg);
  box-shadow: 0 8px 18px rgba(148, 163, 184, 0.12);
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
  backdrop-filter: blur(4px);
  position: relative;
}

.rt-home .rt-pub-card:hover {
  transform: translateY(-3px) scale(1.01);
  border-color: #bfdbfe;
  box-shadow: 0 20px 32px rgba(96, 165, 250, 0.22);
}

.rt-home .rt-pub-media {
  display: block;
  position: relative;
  isolation: isolate;
  align-self: start;
  overflow: hidden;
  aspect-ratio: 16 / 9;
  border-right: 1px solid #e5edf5;
  background: linear-gradient(135deg, #edf4ff 0%, #f8fbff 100%);
}

.rt-home .rt-pub-media::before {
  content: "";
  position: absolute;
  inset: 0;
  z-index: 1;
  pointer-events: none;
  opacity: 0.36;
  background:
    linear-gradient(180deg, rgba(2, 6, 23, 0.1) 0%, rgba(15, 23, 42, 0) 34%, rgba(2, 6, 23, 0.14) 100%),
    repeating-linear-gradient(0deg, rgba(148, 163, 184, 0.26) 0 1px, transparent 1px 14px),
    repeating-linear-gradient(90deg, rgba(148, 163, 184, 0.2) 0 1px, transparent 1px 14px);
  transition: opacity .26s ease;
}

.rt-home .rt-pub-media::after {
  content: "";
  position: absolute;
  left: -46%;
  top: -140%;
  width: 58%;
  height: 300%;
  z-index: 2;
  pointer-events: none;
  opacity: 0;
  background: linear-gradient(100deg, rgba(125, 211, 252, 0) 0%, rgba(224, 242, 254, 0.94) 48%, rgba(125, 211, 252, 0) 100%);
  transform: rotate(20deg) translateY(0);
}

.rt-home .rt-pub-thumb {
  display: block;
  width: 100%;
  height: 100%;
  aspect-ratio: 16 / 9;
  object-fit: cover;
  object-position: center;
  transition: transform .28s ease;
}

.rt-home .rt-pub-card:hover .rt-pub-thumb {
  transform: scale(1.03);
}

.rt-home .rt-pub-card:hover .rt-pub-media::before {
  opacity: 0.58;
}

.rt-home .rt-pub-card:hover .rt-pub-media::after {
  opacity: 1;
  animation: rt-pub-scan .92s ease 1;
}

.rt-home .rt-pub-status {
  position: absolute;
  right: 12px;
  bottom: 10px;
  z-index: 4;
  display: inline-flex;
  align-items: center;
  gap: 5px;
  height: 22px;
  padding: 0 9px;
  border-radius: 999px;
  border: 1px solid #93c5fd;
  background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
  color: #1e3a8a;
  font-size: 0.64rem;
  font-weight: 800;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  box-shadow: 0 8px 14px rgba(59, 130, 246, 0.2);
  pointer-events: none;
}

.rt-home .rt-pub-status::before {
  content: "";
  width: 7px;
  height: 7px;
  border-radius: 999px;
  background: currentColor;
  box-shadow: 0 0 8px currentColor;
}

.rt-home .rt-pub-status--review {
  border-color: #7dd3fc;
  background: linear-gradient(135deg, #ecfeff 0%, #cffafe 100%);
  color: #0c4a6e;
}

.rt-home .rt-pub-status--accepted {
  border-color: #86efac;
  background: linear-gradient(135deg, #f0fdf4 0%, #dcfce7 100%);
  color: #166534;
}

.rt-home .rt-pub-body {
  padding: 14px 13px 12px;
}

.rt-home .rt-pub-title {
  margin: 0 0 7px;
  font-size: 1.04rem;
  line-height: 1.38;
  color: #0f172a;
  font-weight: 760;
}

.rt-home .rt-pub-meta {
  margin: 0 0 11px;
  font-size: 0.74rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: #64748b;
  font-weight: 700;
}

.rt-home .rt-pub-authors {
  margin: 0 0 9px;
  font-size: 0.82rem;
  line-height: 1.5;
  color: #475569;
}

.rt-home .rt-pub-authors strong {
  color: #0f172a;
  font-weight: 800;
}

.rt-home .rt-pub-links {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 2px;
}

.rt-home .rt-pill {
  display: inline-block;
  border: 1px solid #c7d8eb;
  background: #f8fbff;
  color: #1d4ed8;
  border-radius: 999px;
  padding: 4px 10px;
  font-size: 0.76rem;
  font-weight: 700;
  letter-spacing: 0.05em;
  text-transform: uppercase;
}

.rt-home .rt-pill:hover {
  background: #eaf3ff;
}

.rt-home .rt-visitor-wrap {
  display: grid;
  grid-template-columns: 1fr;
  gap: 12px;
  max-width: 900px;
  margin: 0 auto;
}

.rt-home .rt-console-bar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 8px;
  border: 1px solid rgba(56, 189, 248, 0.5);
  background: linear-gradient(135deg, rgba(2, 6, 23, 0.86) 0%, rgba(15, 23, 42, 0.78) 100%);
  border-radius: 10px;
  padding: 8px 10px;
  box-shadow: 0 0 0 1px rgba(125, 211, 252, 0.2) inset, 0 10px 20px rgba(2, 8, 23, 0.26);
}

.rt-home .rt-console-chip {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  border: 1px solid rgba(125, 211, 252, 0.42);
  background: linear-gradient(135deg, rgba(30, 41, 59, 0.94) 0%, rgba(15, 23, 42, 0.9) 100%);
  color: #dbeafe;
  border-radius: 999px;
  padding: 4px 9px;
  font-size: 0.74rem;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  white-space: nowrap;
}

.rt-home .rt-console-chip--online {
  border-color: rgba(74, 222, 128, 0.6);
  color: #bbf7d0;
}

.rt-home .rt-console-dot {
  width: 7px;
  height: 7px;
  border-radius: 999px;
  background: #4ade80;
  box-shadow: 0 0 8px rgba(74, 222, 128, 0.92);
  animation: rt-online-pulse 1.8s ease-in-out infinite;
}

.rt-home .rt-visitor-card {
  border: 1px solid rgba(56, 189, 248, 0.45);
  border-radius: 0;
  clip-path: polygon(0 0, calc(100% - 14px) 0, 100% 14px, 100% 100%, 0 100%);
  background: linear-gradient(145deg, rgba(15, 23, 42, 0.94) 0%, rgba(30, 41, 59, 0.9) 100%);
  padding: 12px;
  text-align: center;
  color: #dbeafe;
  position: relative;
  overflow: hidden;
  box-shadow: 0 0 0 1px rgba(56, 189, 248, 0.18), inset 0 0 0 1px rgba(125, 211, 252, 0.24), 0 18px 30px rgba(2, 8, 23, 0.34);
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
}

.rt-home .rt-visitor-card:hover {
  transform: translateY(-3px) scale(1.012);
  border-color: rgba(125, 211, 252, 0.95);
  box-shadow: 0 0 0 1px rgba(125, 211, 252, 0.38), inset 0 0 0 1px rgba(186, 230, 253, 0.28), 0 22px 34px rgba(2, 8, 23, 0.38), 0 0 20px rgba(56, 189, 248, 0.26);
}

.rt-home .rt-visitor-card::before,
.rt-home .rt-service-card::before,
.rt-home .rt-counter-card::before {
  content: "";
  position: absolute;
  left: 12px;
  right: 12px;
  top: 10px;
  height: 2px;
  border-radius: 999px;
  background: linear-gradient(90deg, rgba(34, 211, 238, 0.24) 0%, rgba(224, 242, 254, 0.9) 48%, rgba(59, 130, 246, 0.24) 100%);
  box-shadow: 0 0 10px rgba(34, 211, 238, 0.45);
}

.rt-home .rt-map-caption {
  font-size: 0.86em;
  color: #93c5fd;
  margin-top: 6px;
}

.rt-home .rt-visitor-map {
  padding: 10px 10px 12px;
}

.rt-home .rt-map-embed {
  max-width: 620px;
  margin: 0 auto;
  border: 1px solid rgba(125, 211, 252, 0.3);
  border-radius: 10px;
  padding: 7px;
  background: linear-gradient(135deg, rgba(15, 23, 42, 0.62) 0%, rgba(15, 23, 42, 0.3) 100%);
}

.rt-home .rt-visitor-bottom {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
}

.rt-home .rt-service-card {
  border: 1px solid rgba(56, 189, 248, 0.42);
  border-radius: 0;
  clip-path: polygon(0 0, calc(100% - 14px) 0, 100% 14px, 100% 100%, 0 100%);
  background: linear-gradient(145deg, rgba(15, 23, 42, 0.93) 0%, rgba(30, 41, 59, 0.88) 100%);
  color: #dbeafe;
  padding: 15px 14px;
  position: relative;
  overflow: hidden;
  box-shadow: 0 0 0 1px rgba(56, 189, 248, 0.18), inset 0 0 0 1px rgba(125, 211, 252, 0.22), 0 14px 26px rgba(2, 8, 23, 0.34);
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
}

.rt-home .rt-service-card:hover {
  transform: translateY(-3px) scale(1.012);
  border-color: rgba(125, 211, 252, 0.95);
  box-shadow: 0 0 0 1px rgba(125, 211, 252, 0.38), inset 0 0 0 1px rgba(186, 230, 253, 0.28), 0 20px 30px rgba(2, 8, 23, 0.38), 0 0 20px rgba(56, 189, 248, 0.24);
}

.rt-home .rt-service-title {
  margin: 0 0 6px;
  font-size: 0.8rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: #7dd3fc;
  font-weight: 800;
}

.rt-home .rt-service-text {
  margin: 0;
  color: #dbeafe;
  line-height: 1.5;
  font-size: 0.93rem;
}

.rt-home .rt-counter-card {
  border: 1px solid rgba(56, 189, 248, 0.54);
  border-radius: 0;
  clip-path: polygon(0 0, calc(100% - 14px) 0, 100% 14px, 100% 100%, 0 100%);
  background: linear-gradient(135deg, rgba(2, 6, 23, 0.98) 0%, rgba(30, 58, 138, 0.88) 56%, rgba(37, 99, 235, 0.76) 100%);
  color: #eff6ff;
  text-align: center;
  padding: 16px 14px;
  position: relative;
  overflow: hidden;
  box-shadow: 0 0 0 1px rgba(56, 189, 248, 0.2), inset 0 0 0 1px rgba(125, 211, 252, 0.2), 0 14px 28px rgba(2, 8, 23, 0.4);
  transition: transform .22s ease, box-shadow .24s ease;
}

.rt-home .rt-counter-card:hover {
  transform: translateY(-3px) scale(1.012);
  box-shadow: 0 0 0 1px rgba(125, 211, 252, 0.42), inset 0 0 0 1px rgba(186, 230, 253, 0.3), 0 22px 36px rgba(2, 8, 23, 0.44), 0 0 24px rgba(56, 189, 248, 0.28);
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

@keyframes rt-news-float {
  0% {
    transform: translate3d(0, 0, 0) scale(1);
  }
  50% {
    transform: translate3d(0, -12px, 0) scale(1.06);
  }
  100% {
    transform: translate3d(0, 0, 0) scale(1);
  }
}

@keyframes rt-wave {
  0% { transform: rotate(0deg) scale(1); filter: drop-shadow(0 0 0 rgba(14, 165, 233, 0)); }
  10% { transform: rotate(14deg) scale(1.03); filter: drop-shadow(0 0 6px rgba(14, 165, 233, 0.55)); }
  20% { transform: rotate(-8deg) scale(1.02); filter: drop-shadow(0 0 8px rgba(56, 189, 248, 0.48)); }
  30% { transform: rotate(12deg) scale(1.04); filter: drop-shadow(0 0 9px rgba(56, 189, 248, 0.52)); }
  40% { transform: rotate(-5deg) scale(1.02); filter: drop-shadow(0 0 7px rgba(14, 165, 233, 0.45)); }
  50% { transform: rotate(8deg) scale(1.03); filter: drop-shadow(0 0 8px rgba(56, 189, 248, 0.45)); }
  60% { transform: rotate(0deg) scale(1); filter: drop-shadow(0 0 4px rgba(14, 165, 233, 0.3)); }
  100% { transform: rotate(0deg) scale(1); filter: drop-shadow(0 0 0 rgba(14, 165, 233, 0)); }
}

@keyframes rt-glitch-a {
  0% { transform: translate(0, 0); clip-path: inset(0 0 0 0); }
  35% { transform: translate(-2px, -1px); clip-path: inset(15% 0 62% 0); }
  65% { transform: translate(2px, 1px); clip-path: inset(58% 0 14% 0); }
  100% { transform: translate(0, 0); clip-path: inset(0 0 0 0); }
}

@keyframes rt-glitch-b {
  0% { transform: translate(0, 0); clip-path: inset(0 0 0 0); }
  40% { transform: translate(2px, 1px); clip-path: inset(8% 0 68% 0); }
  70% { transform: translate(-2px, -1px); clip-path: inset(64% 0 10% 0); }
  100% { transform: translate(0, 0); clip-path: inset(0 0 0 0); }
}

@keyframes rt-rail-flow {
  0% { top: 6px; opacity: 0; }
  12% { opacity: 1; }
  88% { opacity: 1; }
  100% { top: calc(100% - 56px); opacity: 0; }
}

@keyframes rt-node-pulse {
  0% { box-shadow: 0 0 0 2px rgba(191, 219, 254, 0.38), 0 0 8px rgba(56, 189, 248, 0.52); }
  50% { box-shadow: 0 0 0 4px rgba(125, 211, 252, 0.24), 0 0 16px rgba(56, 189, 248, 0.9); }
  100% { box-shadow: 0 0 0 2px rgba(191, 219, 254, 0.38), 0 0 8px rgba(56, 189, 248, 0.52); }
}

@keyframes rt-pub-scan {
  0% { transform: rotate(20deg) translateY(-14%); opacity: 0; }
  20% { opacity: 1; }
  100% { transform: rotate(20deg) translateY(64%); opacity: 0; }
}

@keyframes rt-online-pulse {
  0% { box-shadow: 0 0 4px rgba(74, 222, 128, 0.65); opacity: .75; }
  50% { box-shadow: 0 0 10px rgba(74, 222, 128, 1); opacity: 1; }
  100% { box-shadow: 0 0 4px rgba(74, 222, 128, 0.65); opacity: .75; }
}

@keyframes rt-cyber-scan {
  0% {
    transform: translateX(-35vw) rotate(-11deg);
    opacity: 0;
  }
  14% {
    opacity: 0.88;
  }
  65% {
    opacity: 0.35;
  }
  100% {
    transform: translateX(92vw) rotate(-11deg);
    opacity: 0;
  }
}

@media (max-width: 900px) {
  .rt-theme-toggle {
    right: 10px;
    top: 10px;
    padding: 3px;
  }

  .rt-theme-option {
    min-width: 50px;
    padding: 5px 8px;
    font-size: 0.68rem;
  }

  .rt-home .rt-jump-nav {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .rt-home .rt-award-grid,
  .rt-home .rt-pub-grid,
  .rt-home .rt-visitor-wrap,
  .rt-home .rt-visitor-bottom {
    grid-template-columns: 1fr;
  }

  .rt-home .rt-profile-item {
    grid-template-columns: 1fr;
    gap: 4px;
  }

  .rt-home .rt-pub-card {
    grid-template-columns: 1fr;
  }

  .rt-home .rt-pub-media {
    border-right: 0;
    border-bottom: 1px solid #e5edf5;
  }

  .rt-home .rt-pub-thumb {
    aspect-ratio: 16 / 9;
  }
}

@media (max-width: 640px) {
  .rt-home .rt-overview-card {
    padding: 15px 14px 14px;
  }

  .rt-home .rt-overview-title {
    font-size: 1.34rem;
  }

  .rt-home .rt-timeline li {
    grid-template-columns: 1fr;
    row-gap: 8px;
  }
}

@media (prefers-reduced-motion: reduce) {
  .rt-home .rt-news-zone::before,
  .rt-home .rt-news-zone::after,
  .rt-cyber-bg::before,
  .rt-cyber-bg::after {
    animation: none;
  }

  .rt-home .rt-timeline li {
    transition: none;
  }

  .rt-home .rt-timeline li:hover {
    transform: none;
  }

  .rt-home .rt-jump-item,
  .rt-home .rt-jump-item::before {
    transition: none;
  }

  .rt-home .rt-jump-item.is-active {
    transform: none;
  }

  .rt-home .rt-wave-hand {
    animation: none;
  }

  .rt-home .rt-timeline::after,
  .rt-home .rt-timeline li::before,
  .rt-home .rt-title-glitch::before,
  .rt-home .rt-title-glitch::after,
  .rt-home .rt-pub-card:hover .rt-pub-media::after {
    animation: none;
  }

  .rt-home .rt-nav-progress-fill {
    transition: none;
  }

  .rt-home .rt-console-dot {
    animation: none;
  }

  .rt-home .rt-reveal {
    transition: none;
    opacity: 1;
    transform: none;
  }
}
</style>

<div class="rt-cyber-bg" aria-hidden="true"></div>
<div class="rt-film-layer" aria-hidden="true"></div>
<div class="rt-home">
  <div class="rt-theme-toggle" id="rt-theme-toggle" role="group" aria-label="Theme switch">
    <button class="rt-theme-option" type="button" data-theme-choice="light" aria-pressed="true">Light</button>
    <button class="rt-theme-option" type="button" data-theme-choice="dark" aria-pressed="false">Dark</button>
  </div>
  <nav class="rt-jump-nav" aria-label="Section Navigation">
    <span class="rt-nav-progress" aria-hidden="true"><span class="rt-nav-progress-fill"></span></span>
    <a class="rt-jump-item" href="#section-overview"><i class="fa fa-compass" aria-hidden="true"></i> Overview</a>
    <a class="rt-jump-item" href="#section-news"><i class="fa fa-bolt" aria-hidden="true"></i> News</a>
    <a class="rt-jump-item" href="#section-awards"><i class="fa fa-trophy" aria-hidden="true"></i> Awards</a>
    <a class="rt-jump-item" href="#section-pubs"><i class="fa fa-book" aria-hidden="true"></i> Publications</a>
    <a class="rt-jump-item" href="#section-visitor"><i class="fa fa-globe" aria-hidden="true"></i> Visitor</a>
  </nav>

  <section class="rt-top-intro" id="section-overview">
    <article class="rt-card rt-overview-card rt-tag-card rt-tag-pad rt-reveal">
      <span class="rt-corner-tag rt-corner-tag--blue">overview</span>
      <p class="rt-overview-name">Ruitong Liu</p>
      <p class="rt-intro-text">
        <span class="rt-welcome-line">Welcome to my homepage! <span class="rt-wave-hand" aria-hidden="true">👋</span></span><br>
        I am currently a senior majoring at
        <a href="https://www.dlut.edu.cn/">Dalian University of Technology</a>. I will start my graduate studies at the
        <a href="https://www.math.pku.edu.cn/index.htm">School of Mathematical Sciences</a>,
        <a href="https://www.pku.edu.cn/">Peking University</a> in September 2026. My research focuses on Large Language Models (LLMs) and Multimodal Large Language Models (MLLMs), covering large-scale data engineering, complex reasoning optimization, training algorithms and full-stack training, KG+LLM, and mathematical formal reasoning. I am currently also working on research related to World Models(WMs).<br> Now i am interning in Beijing.
        If you are interested in academic cooperation or exchanges in related fields, please feel free to contact me via email at any time!
      </p>
      <div class="rt-focus-row">
        <span class="rt-focus-pill">LLM/MLLM Training (Full-Stack)</span>
        <span class="rt-focus-pill">Data-Centric AI</span>
        <span class="rt-focus-pill">MLLM Reasoning</span>
        <span class="rt-focus-pill">World Model</span>
        <span class="rt-focus-pill">Formal Math (Lean)</span>
        <span class="rt-focus-pill">Unify</span>
        <span class="rt-focus-pill">LLM Edit</span>
      </div>
      <div class="rt-chip-row">
        <a class="rt-chip" href="mailto:15668672116@163.com"><i class="fa fa-envelope" aria-hidden="true"></i> 15668672116@163.com</a>
        <a class="rt-chip" href="mailto:ruitong.jerry@gmail.com"><i class="fa fa-envelope-o" aria-hidden="true"></i> ruitong.jerry@gmail.com</a>
        <span class="rt-chip"><i class="fa fa-commenting" aria-hidden="true"></i> WeChat: ruitong_jerry</span>
      </div>
      <div class="rt-overview-divider"></div>
      <div class="rt-profile-stack">
        <section class="rt-profile-block rt-tag-card rt-tag-pad">
          <span class="rt-corner-tag rt-corner-tag--blue">education</span>
          <h3 class="rt-profile-head">Education</h3>
          <ul class="rt-profile-list">
            <li class="rt-profile-item">
              <div class="rt-profile-date">2026.09 - 2028.09</div>
              <div>
                <p class="rt-profile-main"><a href="https://www.math.pku.edu.cn/index.htm">School of Mathematical Sciences, Peking University</a></p>
                <p class="rt-profile-sub">Data Science and Big Data Technology (Graduate Studies, Planned)</p>
              </div>
            </li>
            <li class="rt-profile-item">
              <div class="rt-profile-date">2022.09 - 2026.07</div>
              <div>
                <p class="rt-profile-main"><a href="https://math.dlut.edu.cn/">School of Mathematical Sciences, Dalian University of Technology</a></p>
                <p class="rt-profile-sub">Mathematics and Applied Mathematics (B.S.)</p>
              </div>
            </li>
          </ul>
        </section>
      </div>
    </article>
  </section>

  <h2 class="rt-section-title rt-reveal" id="section-news"><i class="fa fa-bolt" aria-hidden="true"></i><span class="rt-title-glitch" data-text="What's New">What's New</span></h2>
  <div class="rt-news-zone rt-tag-card rt-tag-pad rt-reveal">
    <span class="rt-corner-tag">news</span>
    <ul class="rt-timeline">
      <li>
        <span class="rt-time">2026-05</span>
        <div class="rt-news-text">One paper was submitted to <strong>NIPS 2026</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2026-04</span>
        <div class="rt-news-text">Two papers were accepted to <strong>ACL 2026 (One Main, One Findings.)</strong>. Congratulations to all co-authors.!</div>
      </li>
      <li>
        <span class="rt-time">2026-03</span>
        <div class="rt-news-text">One paper was submitted to <strong>EMNLP 2026</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2026-02</span>
        <div class="rt-news-text">A survey on LLM data preparation was accepted by <strong>JCST's 40th Anniversary Special Issue</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2026-01</span>
        <div class="rt-news-text">Two papers were submitted to <strong>ICML 2026</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2025-08</span>
        <div class="rt-news-text">A paper was submitted to <strong>TPAMI</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2025-07</span>
        <div class="rt-news-text">I was pre-admitted to PKU through the postgraduate recommendation program (Bao Yan).</div>
      </li>
    </ul>
  </div>

  <h2 class="rt-section-title rt-reveal" id="section-awards"><i class="fa fa-trophy" aria-hidden="true"></i><span class="rt-title-glitch" data-text="Awards">Awards</span></h2>
  <div class="rt-awards-zone rt-tag-card rt-tag-pad rt-reveal">
    <span class="rt-corner-tag rt-corner-tag--gold">awards</span>
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

    <details class="rt-award-collapse">
      <summary>Show All Awards & Honors</summary>
      <ul class="rt-award-list">
        <li>October 2025: First-Class Academic Excellence Scholarship</li>
        <li>May 2025: Third Prize in the National Network Technology Track of the China University Computer Competition</li>
        <li>January 2025: Excellent League Cadre, School of Mathematical Sciences</li>
        <li>January 2025: Excellent Communist Youth League Member, Dalian University of Technology</li>
        <li>October 2024: Top 10 College Students, School of Mathematical Sciences (&lt;=2%)</li>
        <li>October 2024: Excellent Merit Student, Dalian University of Technology</li>
        <li>October 2024: Four individual scholarships (Spiritual Civilization, Social Work, Social Practice, Cultural &amp; Sports Activities)</li>
        <li>October 2024: First-Class Academic Excellence Scholarship</li>
        <li>September 2024: Top 10 Volunteers, School of Mathematical Sciences (&lt;=2%)</li>
        <li>July 2024: University-level Gold Award, China International Internet Plus Innovation &amp; Entrepreneurship Competition</li>
        <li>July 2024: Became a full member of CPC after one-year probation</li>
        <li>December 2023: Excellent Merit Student, Dalian University of Technology</li>
        <li>December 2023: Excellent Communist Youth League Member, Dalian University of Technology</li>
        <li>November 2023: Sunshine Education Scholarship</li>
        <li>November 2023: Practical team received a national-level award</li>
        <li>November 2023: Excellent Young Volunteer, Dalian University of Technology (&lt;=4%)</li>
        <li>October 2023: Four individual scholarships (Spiritual Civilization, Cultural &amp; Sports Activities, Scientific &amp; Technological Innovation, Social Practice)</li>
        <li>October 2023: Second-Class Academic Excellence Scholarship</li>
        <li>October 2023: Practical team won University-level Second Prize</li>
        <li>September 2023: Top 10 Volunteers, School of Mathematical Sciences (&lt;=2%)</li>
        <li>June 2023: First Prize, Dalian Mathematics Competition</li>
      </ul>
    </details>
  </div>

  <h2 class="rt-section-title rt-reveal" id="section-pubs"><i class="fa fa-book" aria-hidden="true"></i><span class="rt-title-glitch" data-text="Publications">Publications</span></h2>
  <p class="rt-note">*: co-first authors. #: corresponding author.</p>
  <div class="rt-pubs-zone rt-tag-card rt-tag-pad rt-reveal">
    <span class="rt-corner-tag rt-corner-tag--blue">publications</span>
    <div class="rt-pub-grid">
      
      <article class="rt-pub-card">
        <span class="rt-pub-status rt-pub-status--accepted">Accepted</span>
        <a class="rt-pub-media" href="https://arxiv.org/pdf/2510.26495">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/06.png' | relative_url }}" alt="Text-to-SQL paper teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Rethinking Text-to-SQL: Dynamic Multi-turn SQL Interaction for Real-world Database Exploration</h3>
          <p class="rt-pub-authors">Linzhuang Sun*, Tianyu Guo*, Hao Liang*, <strong>Ruitong Liu</strong>, Yuying Li, Qifeng Cai, Jingxuan Wei, Yuchen Wu, Bihui Yu, Xiangxiang Zhang, Wentao Zhang#, Bin CUI#</p>
          <p class="rt-pub-meta">ACL 2026 Findings</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://arxiv.org/pdf/2510.26495">PDF</a>
            <a class="rt-pill" href="https://github.com/Aurora-slz/DySQL-Bench.git">Code</a>
          </div>
        </div>
      </article>

      <article class="rt-pub-card">
        <span class="rt-pub-status rt-pub-status--accepted">Accepted</span>
        <a class="rt-pub-media" href="https://arxiv.org/pdf/2602.12389">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/07.png' | relative_url }}" alt="Temporal KGF paper teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Evolving Beyond Snapshots: Harmonizing Structure and Sequence via Entity State Tuning for Temporal Knowledge Graph Forecasting</h3>
          <p class="rt-pub-authors">Siyuan Li#*, Yunjia Wu*, yiyong xiao*, Huang Pingyang, Peize Li, <strong>Ruitong Liu#</strong>, Yan Wen, Te Sun</p>
          <p class="rt-pub-meta">ACL 2026 Main</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://arxiv.org/pdf/2602.12389">PDF</a>
            <a class="rt-pill" href="https://github.com/yuanwuyuan9/Evolving-Beyond-Snapshots.git">Code</a>
          </div>
        </div>
      </article>

      <article class="rt-pub-card">
        <span class="rt-pub-status rt-pub-status--accepted">Accepted</span>
        <a class="rt-pub-media" href="https://link.springer.com/article/10.1007/s11390-026-5948-8">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/05.png' | relative_url }}" alt="LLM data preparation survey teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Data Preparation for Large Language Models: A Survey</h3>
          <p class="rt-pub-authors">Hao Liang, Zhen Hao Wong, <strong>Ruitong Liu</strong>, Yuhan Wang, Meiyi Qiang, Zhengyang Zhao, Chengyu Shen, Conghui He#, Wentao Zhang#, Bin Cui#</p>
          <p class="rt-pub-meta">JCST 40th Anniversary Special Issue</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://link.springer.com/article/10.1007/s11390-026-5948-8">PDF</a>
          </div>
        </div>
      </article>
      
      <article class="rt-pub-card">
        <span class="rt-pub-status rt-pub-status--review">Under Review</span>
        <a class="rt-pub-media" href="https://arxiv.org/pdf/2602.04290">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/01.png' | relative_url }}" alt="Guided Verifier teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Guided Verifier: Collaborative Multimodal Reasoning via Dynamic Process Supervision</h3>
          <p class="rt-pub-authors">Lingzhuang Sun*, <strong>Ruitong Liu*</strong>, Yuxia Zhu*, Xiaohan Xu, Jingxuan Wei, Xiangxiang Zhang, Bihui Yu, Wentao Zhang#</p>
          <p class="rt-pub-meta">ICML 2026 Under Review</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://arxiv.org/pdf/2602.04290">PDF</a>
            <a class="rt-pill" href="https://github.com/tongruiliu/Guided-GRPO">Code</a>
            <a class="rt-pill" href="https://huggingface.co/ruitongl/Guided-Verifier-8B">Model</a>
          </div>
        </div>
      </article>

      <article class="rt-pub-card">
        <span class="rt-pub-status rt-pub-status--review">Under Review</span>
        <a class="rt-pub-media" href="https://arxiv.org/pdf/2602.10494">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/02.png' | relative_url }}" alt="Canvas-of-Thought teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Canvas-of-Thought: Grounding Reasoning via Mutable Structured States</h3>
          <p class="rt-pub-authors">Lingzhuang Sun*, Yuxia Zhu*, <strong>Ruitong Liu*</strong>, Hao Liang, Zheng Sun, Caijun Jia, Honghao He, Yuchen Wu, Siyuan Li, Jingxuan Wei, Xiangxiang Zhang, Bihui Yu, Wentao Zhang#</p>
          <p class="rt-pub-meta">ICML 2026 Under Review</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://arxiv.org/pdf/2602.10494">PDF</a>
            <a class="rt-pill" href="https://github.com/Zzzyxii/Canvas-CoT">Code</a>
          </div>
        </div>
      </article>

      <article class="rt-pub-card">
        <span class="rt-pub-status rt-pub-status--review">Under Review</span>
        <a class="rt-pub-media" href="https://arxiv.org/pdf/2510.08966">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/03.png' | relative_url }}" alt="Semantic-Condition Tuning teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Semantic-Condition Tuning: Fusing Graph Context with Large Language Models for Knowledge Graph Completion</h3>
          <p class="rt-pub-authors"><strong>Ruitong Liu</strong>, Yan Wen, Te Sun, Yunjia Wu, Pingyang Huang, Zihang Yu, Siyuan Li</p>
          <p class="rt-pub-meta">EMNLP 2026 Under Review</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://arxiv.org/pdf/2510.08966">PDF</a>
            <a class="rt-pill" href="https://github.com/tongruiliu/GMT">Code</a>
          </div>
        </div>
      </article>

      <article class="rt-pub-card">
        <span class="rt-pub-status rt-pub-status--review">Under Review</span>
        <a class="rt-pub-media" href="https://arxiv.org/pdf/2506.23137">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/04.png' | relative_url }}" alt="Flow-Modulated Scoring teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Flow-Modulated Scoring for Semantic-Aware Knowledge Graph Completion</h3>
          <p class="rt-pub-authors">Siyuan Li, <strong>Ruitong Liu</strong>, Yan Wen, Te Sun, Andi Zhang, Yanbiao Ma#, Xiaoshuai Hao#</p>
          <p class="rt-pub-meta">TPAMI Under Review</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://arxiv.org/pdf/2506.23137">PDF</a>
            <a class="rt-pill" href="https://github.com/yuanwuyuan9/FMS">Code</a>
          </div>
        </div>
      </article>
      
    </div>
  </div>

  <h2 class="rt-section-title rt-reveal" id="section-visitor"><i class="fa fa-globe" aria-hidden="true"></i><span class="rt-title-glitch" data-text="Visitor">Visitor</span></h2>
  <div class="rt-visitor-wrap rt-reveal">
    <div class="rt-console-bar" aria-label="Visitor Console">
      <span class="rt-console-chip"><i class="fa fa-microchip" aria-hidden="true"></i> Runtime</span>
      <span class="rt-console-chip"><i class="fa fa-clock-o" aria-hidden="true"></i> <span id="rt-console-time">--:--:--</span></span>
      <span class="rt-console-chip rt-console-chip--online"><span class="rt-console-dot" aria-hidden="true"></span> Online</span>
    </div>
    <div class="rt-visitor-card rt-visitor-map rt-tag-card rt-tag-pad">
      <span class="rt-corner-tag rt-corner-tag--cyan">map</span>
      <div class="rt-map-embed">
        <script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?d=wWuKIsCZO2yYZA7sXQVVhdoENIGHAUsZCAy6ZjG-Uhk&cl=ffffff&w=a"></script>
      </div>
      <div class="rt-map-caption">Visitor Geography</div>
    </div>
    <div class="rt-visitor-bottom">
      <div class="rt-service-card rt-tag-card rt-tag-pad">
        <span class="rt-corner-tag rt-corner-tag--gold">service</span>
        <div class="rt-service-title">Service</div>
        <p class="rt-service-text">Reviewer/PC Member: Transactions on Knowledge Discovery from Data (TKDD), Journal of Communications Software and Systems (JCOMSS)</p>
      </div>
      <div class="rt-counter-card rt-tag-card rt-tag-pad">
        <span class="rt-corner-tag rt-corner-tag--cyan">counter</span>
        <div class="rt-counter-title">Visit Counter</div>
        <div id="busuanzi_value_site_pv" data-offset="27" class="rt-counter-value">--</div>
        <div class="rt-counter-label">Page Views (PV)</div>
      </div>
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
<script>
(function () {
  var homeEl = document.querySelector('.rt-home');
  var toggleWrap = document.getElementById('rt-theme-toggle');
  var toggleOptions = Array.prototype.slice.call(document.querySelectorAll('#rt-theme-toggle .rt-theme-option'));
  var prefersReduced = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  var desktopMedia = window.matchMedia('(min-width: 1024px)');
  var storageKey = 'rt-home-theme';

  if (!homeEl || !toggleWrap || !toggleOptions.length) {
    return;
  }

  function readStoredTheme() {
    try {
      return localStorage.getItem(storageKey);
    } catch (err) {
      return null;
    }
  }

  function writeStoredTheme(theme) {
    try {
      localStorage.setItem(storageKey, theme);
    } catch (err) {
      return;
    }
  }

  function updateToggleUi(theme) {
    toggleOptions.forEach(function (option) {
      var isActive = option.getAttribute('data-theme-choice') === theme;
      option.classList.toggle('is-active', isActive);
      option.setAttribute('aria-pressed', isActive ? 'true' : 'false');
    });
    toggleWrap.setAttribute('data-active-theme', theme);
  }

  function applyTheme(theme) {
    var safeTheme = theme === 'dark' ? 'dark' : 'light';
    homeEl.setAttribute('data-theme', safeTheme);
    document.body.classList.toggle('rt-theme-dark', safeTheme === 'dark');
    updateToggleUi(safeTheme);
    writeStoredTheme(safeTheme);
  }

  var initialTheme = readStoredTheme() || 'light';
  applyTheme(initialTheme);

  function placeThemeToggle() {
    var sidebarUrls = document.querySelector('.sidebar .author__urls-wrapper');
    var navEl = homeEl.querySelector('.rt-jump-nav');

    if (desktopMedia.matches && sidebarUrls && sidebarUrls.parentNode) {
      if (toggleWrap.parentNode !== sidebarUrls.parentNode || toggleWrap.previousElementSibling !== sidebarUrls) {
        sidebarUrls.parentNode.insertBefore(toggleWrap, sidebarUrls.nextSibling);
      }
      toggleWrap.classList.add('rt-theme-toggle--sidebar');
      return;
    }

    if (navEl && toggleWrap.parentNode !== homeEl) {
      homeEl.insertBefore(toggleWrap, navEl);
    }
    toggleWrap.classList.remove('rt-theme-toggle--sidebar');
  }

  placeThemeToggle();

  toggleOptions.forEach(function (option) {
    option.addEventListener('click', function () {
      var choice = option.getAttribute('data-theme-choice');
      if (choice === 'light' || choice === 'dark') {
        applyTheme(choice);
      }
    });
  });

  if (typeof desktopMedia.addEventListener === 'function') {
    desktopMedia.addEventListener('change', placeThemeToggle);
  } else if (typeof desktopMedia.addListener === 'function') {
    desktopMedia.addListener(placeThemeToggle);
  }

  window.addEventListener('resize', placeThemeToggle);

  var revealTargets = Array.prototype.slice.call(document.querySelectorAll('.rt-home .rt-reveal'));
  if (!revealTargets.length) {
    return;
  }

  if (prefersReduced || !('IntersectionObserver' in window)) {
    revealTargets.forEach(function (el) {
      el.classList.add('is-inview');
    });
    return;
  }

  var observer = new IntersectionObserver(function (entries, obs) {
    entries.forEach(function (entry) {
      if (!entry.isIntersecting) {
        return;
      }
      entry.target.classList.add('is-inview');
      obs.unobserve(entry.target);
    });
  }, {
    threshold: 0.18,
    rootMargin: '0px 0px -8% 0px'
  });

  revealTargets.forEach(function (el) {
    observer.observe(el);
  });
})();
</script>
<script>
(function () {
  var navLinks = Array.prototype.slice.call(document.querySelectorAll('.rt-jump-nav .rt-jump-item[href^="#"]'));
  var progressFill = document.querySelector('.rt-jump-nav .rt-nav-progress-fill');
  if (!navLinks.length) {
    return;
  }

  var sections = navLinks
    .map(function (link) {
      var id = link.getAttribute('href');
      var el = id ? document.querySelector(id) : null;
      return el ? { link: link, el: el } : null;
    })
    .filter(Boolean);

  if (!sections.length) {
    return;
  }

  function setActive(targetLink) {
    sections.forEach(function (item) {
      var active = item.link === targetLink;
      item.link.classList.toggle('is-active', active);
      if (active) {
        item.link.setAttribute('aria-current', 'true');
      } else {
        item.link.removeAttribute('aria-current');
      }
    });
  }

  function updateActiveLink() {
    var trigger = 130;
    var current = sections[0];

    for (var i = 0; i < sections.length; i += 1) {
      var rect = sections[i].el.getBoundingClientRect();
      if (rect.top <= trigger) {
        current = sections[i];
      } else {
        break;
      }
    }

    if (current) {
      setActive(current.link);
    }
  }

  function updateScrollProgress() {
    if (!progressFill) {
      return;
    }
    var doc = document.documentElement;
    var scrollTop = window.pageYOffset || doc.scrollTop || 0;
    var maxScroll = Math.max(1, doc.scrollHeight - window.innerHeight);
    var ratio = Math.min(1, Math.max(0, scrollTop / maxScroll));
    progressFill.style.transform = 'scaleX(' + ratio + ')';
  }

  var ticking = false;
  function onScroll() {
    if (ticking) {
      return;
    }
    ticking = true;
    requestAnimationFrame(function () {
      updateActiveLink();
      updateScrollProgress();
      ticking = false;
    });
  }

  window.addEventListener('scroll', onScroll, { passive: true });
  window.addEventListener('resize', onScroll);
  window.addEventListener('hashchange', function () {
    setTimeout(updateActiveLink, 50);
  });

  updateActiveLink();
  updateScrollProgress();
})();
</script>
<script>
(function () {
  var timeEl = document.getElementById('rt-console-time');

  function updateConsoleTime() {
    if (!timeEl) {
      return;
    }
    var now = new Date();
    var dateText = now.toLocaleDateString('en-CA');
    var timeText = now.toLocaleTimeString('en-GB', { hour12: false });
    timeEl.textContent = dateText + ' ' + timeText;
  }

  if (timeEl) {
    updateConsoleTime();
    setInterval(updateConsoleTime, 1000);
  }
})();
</script>
