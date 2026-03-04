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
}

.rt-cyber-bg {
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: 0;
  overflow: hidden;
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
  --rt-soft-ink: #4b5563;
  --rt-line: #dce7ef;
  --rt-blue: #2563eb;
  --rt-blue-2: #3b82f6;
  --rt-accent: #c2410c;
  --rt-surface: #ffffff;
  --rt-surface-soft: #f7fbff;
  position: relative;
  z-index: 1;
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

.rt-home .rt-jump-nav {
  display: grid;
  grid-template-columns: repeat(5, minmax(0, 1fr));
  gap: 10px;
  margin: 14px 0 10px;
}

.rt-home .rt-jump-item {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 7px;
  border: 1px solid #d5e4f4;
  background: linear-gradient(135deg, #f8fbff 0%, #ffffff 100%);
  color: #1e3a8a;
  border-radius: 11px;
  padding: 10px 8px;
  font-size: 0.9rem;
  font-weight: 600;
  text-align: center;
  transition: transform .22s ease, box-shadow .24s ease, background .22s ease, border-color .22s ease;
  box-shadow: 0 8px 14px rgba(148, 163, 184, 0.14);
}

.rt-home .rt-jump-item:hover {
  background: linear-gradient(135deg, #ecf5ff 0%, #ffffff 100%);
  transform: translateY(-2px) scale(1.02);
  border-color: #bfdbfe;
  box-shadow: 0 14px 22px rgba(96, 165, 250, 0.22);
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

.rt-home .rt-focus-row {
  display: flex;
  flex-wrap: wrap;
  gap: 9px;
  margin-top: 12px;
}

.rt-home .rt-focus-pill {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  border: 1px solid #d5e4f4;
  background: linear-gradient(135deg, #f8fbff 0%, #ffffff 100%);
  color: #1e3a8a;
  border-radius: 999px;
  padding: 5px 11px;
  font-size: 0.83rem;
  font-weight: 600;
}

.rt-home .rt-snapshot-row {
  margin-top: 12px;
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(0, 1.8fr);
  gap: 12px;
}

.rt-home .rt-snapshot-item {
  border: 1px solid #dbe7f5;
  border-radius: 12px;
  background: linear-gradient(145deg, rgba(255, 255, 255, 0.92) 0%, rgba(245, 250, 255, 0.88) 100%);
  padding: 12px 12px 11px;
  box-shadow: 0 9px 16px rgba(148, 163, 184, 0.14);
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
}

.rt-home .rt-snapshot-item:hover {
  transform: translateY(-3px) scale(1.012);
  border-color: #bfdbfe;
  box-shadow: 0 16px 24px rgba(96, 165, 250, 0.22);
}

.rt-home .rt-snapshot-item--internship {
  padding: 12px 13px;
}

.rt-home .rt-snapshot-kicker {
  margin: 0 0 5px;
  font-size: 0.76rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: #1e3a8a;
  font-weight: 800;
}

.rt-home .rt-snapshot-main {
  margin: 0 0 6px;
  color: #0f172a;
  font-weight: 700;
  line-height: 1.45;
}

.rt-home .rt-snapshot-sub {
  margin: 0;
  color: #475569;
  font-size: 0.9rem;
  line-height: 1.5;
}

.rt-home .rt-role-meta {
  color: #475569;
  font-size: 0.88rem;
}

.rt-home .rt-snapshot-line {
  margin-top: 5px;
  display: flex;
  flex-wrap: wrap;
  gap: 7px;
  align-items: center;
}

.rt-home .rt-snapshot-role {
  display: inline-flex;
  color: #334155;
  font-size: 0.93rem;
}

.rt-home .rt-snapshot-stack {
  display: grid;
  gap: 8px;
}

.rt-home .rt-snapshot-entry {
  padding-top: 2px;
}

.rt-home .rt-snapshot-entry + .rt-snapshot-entry {
  border-top: 1px dashed #dbe7f5;
  padding-top: 10px;
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
  display: grid;
  gap: 12px;
}

.rt-home .rt-news-zone {
  position: relative;
  border-radius: 16px;
  padding: 14px;
  margin-bottom: 6px;
  overflow: hidden;
  isolation: isolate;
  background: linear-gradient(135deg, #edf5ff 0%, #f8fbff 52%, #ffffff 100%);
  border: 1px solid #dbe8f6;
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
  background: linear-gradient(145deg, rgba(255, 255, 255, 0.88) 0%, rgba(247, 251, 255, 0.8) 100%);
  border: 1px solid rgba(223, 234, 246, 0.9);
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
  left: -1px;
  top: -1px;
  bottom: -1px;
  width: 4px;
  border-radius: 12px 0 0 12px;
  background: linear-gradient(180deg, var(--rt-blue-2), #0ea5e9);
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
  background: linear-gradient(135deg, #fff8f2 0%, #fffcf8 52%, #ffffff 100%);
  border: 1px solid #f7dfcf;
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
  border: 1px solid #f1d2bf;
  background: linear-gradient(135deg, rgba(255, 249, 245, 0.88) 0%, rgba(255, 255, 255, 0.9) 100%);
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
  background: linear-gradient(135deg, #f3f8ff 0%, #f9fbff 56%, #ffffff 100%);
  border: 1px solid #dbe8f7;
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
  border: 1px solid var(--rt-line);
  border-radius: 12px;
  overflow: hidden;
  background: linear-gradient(145deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 252, 255, 0.84) 100%);
  box-shadow: 0 8px 18px rgba(148, 163, 184, 0.12);
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
  backdrop-filter: blur(4px);
}

.rt-home .rt-pub-card:hover {
  transform: translateY(-3px) scale(1.01);
  border-color: #bfdbfe;
  box-shadow: 0 20px 32px rgba(96, 165, 250, 0.22);
}

.rt-home .rt-pub-media {
  display: block;
  align-self: start;
  overflow: hidden;
  aspect-ratio: 16 / 9;
  border-right: 1px solid #e5edf5;
  background: linear-gradient(135deg, #edf4ff 0%, #f8fbff 100%);
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

.rt-home .rt-pub-authors {
  margin: 0 0 8px;
  font-size: 0.84rem;
  line-height: 1.45;
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
  grid-template-columns: 1fr;
  gap: 12px;
  max-width: 900px;
  margin: 0 auto;
}

.rt-home .rt-visitor-card {
  border: 1px solid var(--rt-line);
  border-radius: 12px;
  background: #fff;
  padding: 12px;
  text-align: center;
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
}

.rt-home .rt-visitor-card:hover {
  transform: translateY(-3px) scale(1.012);
  border-color: #bfdbfe;
  box-shadow: 0 16px 26px rgba(96, 165, 250, 0.2);
}

.rt-home .rt-visitor-map {
  padding: 10px 10px 12px;
}

.rt-home .rt-map-embed {
  max-width: 620px;
  margin: 0 auto;
}

.rt-home .rt-visitor-bottom {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
}

.rt-home .rt-service-card {
  border: 1px solid var(--rt-line);
  border-radius: 12px;
  background: linear-gradient(145deg, rgba(255, 255, 255, 0.95) 0%, rgba(245, 250, 255, 0.9) 100%);
  color: #1f2937;
  padding: 15px 14px;
  box-shadow: 0 10px 20px rgba(148, 163, 184, 0.16);
  transition: transform .22s ease, box-shadow .24s ease, border-color .22s ease;
}

.rt-home .rt-service-card:hover {
  transform: translateY(-3px) scale(1.012);
  border-color: #bfdbfe;
  box-shadow: 0 18px 28px rgba(96, 165, 250, 0.22);
}

.rt-home .rt-service-title {
  margin: 0 0 6px;
  font-size: 0.8rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: #1e3a8a;
  font-weight: 800;
}

.rt-home .rt-service-text {
  margin: 0;
  color: #334155;
  line-height: 1.5;
  font-size: 0.93rem;
}

.rt-home .rt-counter-card {
  border: 1px solid #1e3a8a;
  border-radius: 12px;
  background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 55%, #2563eb 100%);
  color: #eff6ff;
  text-align: center;
  padding: 16px 14px;
  box-shadow: 0 12px 24px rgba(15, 23, 42, 0.22);
  transition: transform .22s ease, box-shadow .24s ease;
}

.rt-home .rt-counter-card:hover {
  transform: translateY(-3px) scale(1.012);
  box-shadow: 0 20px 34px rgba(37, 99, 235, 0.34);
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
  .rt-home .rt-jump-nav {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .rt-home .rt-snapshot-row,
  .rt-home .rt-award-grid,
  .rt-home .rt-pub-grid,
  .rt-home .rt-visitor-wrap,
  .rt-home .rt-visitor-bottom {
    grid-template-columns: 1fr;
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
  .rt-home .rt-hero {
    padding: 22px 16px;
  }

  .rt-home .rt-hero h1 {
    font-size: 1.45rem;
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
}
</style>

<div class="rt-cyber-bg" aria-hidden="true"></div>
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

  <nav class="rt-jump-nav" aria-label="Section Navigation">
    <a class="rt-jump-item" href="#section-overview"><i class="fa fa-compass" aria-hidden="true"></i> Overview</a>
    <a class="rt-jump-item" href="#section-news"><i class="fa fa-bolt" aria-hidden="true"></i> News</a>
    <a class="rt-jump-item" href="#section-awards"><i class="fa fa-trophy" aria-hidden="true"></i> Awards</a>
    <a class="rt-jump-item" href="#section-pubs"><i class="fa fa-book" aria-hidden="true"></i> Publications</a>
    <a class="rt-jump-item" href="#section-visitor"><i class="fa fa-globe" aria-hidden="true"></i> Visitor</a>
  </nav>

  <section class="rt-top-intro" id="section-overview">
    <article class="rt-card">
      <h2><i class="fa fa-flask" aria-hidden="true"></i> Research Overview</h2>
      <p class="rt-intro-text">
        My research centers on Data-Centric AI for Large Language Models (LLMs) and Multimodal LLMs, spanning scalable data synthesis,
        data quality filtering, alignment optimization, and structure-aware reasoning with Knowledge Graphs to improve reliability and factual consistency.
      </p>
      <div class="rt-focus-row">
        <span class="rt-focus-pill"><i class="fa fa-database" aria-hidden="true"></i> Data Synthesis &amp; Filtering</span>
        <span class="rt-focus-pill"><i class="fa fa-sliders" aria-hidden="true"></i> LLM/MMLM Alignment</span>
        <span class="rt-focus-pill"><i class="fa fa-sitemap" aria-hidden="true"></i> KG Reasoning</span>
      </div>
    </article>
    <div class="rt-snapshot-row">
      <article class="rt-snapshot-item">
        <div class="rt-snapshot-kicker">Education</div>
        <p class="rt-snapshot-main">Incoming Graduate Student</p>
        <p class="rt-snapshot-sub">Big Data Program, School of Mathematical Sciences, <a href="https://www.pku.edu.cn/">Peking University</a></p>
      </article>
      <article class="rt-snapshot-item rt-snapshot-item--internship">
        <div class="rt-snapshot-kicker">Internship</div>
        <div class="rt-snapshot-stack">
          <div class="rt-snapshot-entry">
            <p class="rt-snapshot-main">Ubiquant-IQuest <span class="rt-role-meta">2026.02 - Present</span></p>
            <div class="rt-snapshot-line">
              <span class="rt-snapshot-role">LLM Algorithm Intern</span>
              <span class="rt-spotlight">Talent Program</span>
            </div>
          </div>
          <div class="rt-snapshot-entry">
            <p class="rt-snapshot-main">Institute for Advanced Algorithms Research (IAAR), Shanghai <span class="rt-role-meta">2025.09 - 2026.02</span></p>
            <div class="rt-snapshot-line">
              <span class="rt-snapshot-role">LLM Algorithm Research Intern</span>
            </div>
          </div>
        </div>
      </article>
    </div>
  </section>

  <h2 class="rt-section-title" id="section-news"><i class="fa fa-bolt" aria-hidden="true"></i> What's New</h2>
  <div class="rt-news-zone">
    <p class="rt-note">For detailed paper information, please check the <a href="/Publications.html">Publications</a> page.</p>
    <ul class="rt-timeline">
      <li>
        <span class="rt-time">2026-02</span>
        <div class="rt-news-text">A survey on LLM data preparation was accepted by <strong>JCST's 40th Anniversary Special Issue</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2026-01</span>
        <div class="rt-news-text">A paper was submitted to <strong>IJCAI 2026</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2026-01</span>
        <div class="rt-news-text">The first paper was submitted to <strong>ICML 2026</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2026-01</span>
        <div class="rt-news-text">The second paper was submitted to <strong>ICML 2026</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2026-01</span>
        <div class="rt-news-text">The first paper was submitted to <strong>ACL 2026</strong>.</div>
      </li>
      <li>
        <span class="rt-time">2026-01</span>
        <div class="rt-news-text">The second paper was submitted to <strong>ACL 2026</strong>.</div>
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

  <h2 class="rt-section-title" id="section-awards"><i class="fa fa-trophy" aria-hidden="true"></i> Selected Awards</h2>
  <div class="rt-awards-zone">
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

  <h2 class="rt-section-title" id="section-pubs"><i class="fa fa-book" aria-hidden="true"></i> Publications</h2>
  <div class="rt-pubs-zone">
    <div class="rt-pub-grid">
      <article class="rt-pub-card">
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
        <a class="rt-pub-media" href="https://arxiv.org/pdf/2510.08966">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/03.png' | relative_url }}" alt="Semantic-Condition Tuning teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Semantic-Condition Tuning: Fusing Graph Context with Large Language Models for Knowledge Graph Completion</h3>
          <p class="rt-pub-authors"><strong>Ruitong Liu</strong>, Yan Wen, Te Sun, Yunjia Wu, Pingyang Huang, Zihang Yu, Siyuan Li</p>
          <p class="rt-pub-meta">IJCAI 2026 Under Review</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://arxiv.org/pdf/2510.08966">PDF</a>
            <a class="rt-pill" href="https://github.com/tongruiliu/GMT">Code</a>
          </div>
        </div>
      </article>

      <article class="rt-pub-card">
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

      <article class="rt-pub-card">
        <a class="rt-pub-media" href="https://drive.google.com/file/d/1TqwULwmD8f-cpokfcfYfapuC9bNxrztA/view?usp=sharing">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/05.png' | relative_url }}" alt="LLM data preparation survey teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Data Preparation for Large Language Models: A Survey</h3>
          <p class="rt-pub-authors">Hao Liang, Zhen Hao Wong, <strong>Ruitong Liu</strong>, Yuhan Wang, Meiyi Qiang, Zhengyang Zhao, Chengyu Shen, Conghui He#, Wentao Zhang#, Bin Cui#</p>
          <p class="rt-pub-meta">JCST 40th Anniversary Special Issue</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://drive.google.com/file/d/1TqwULwmD8f-cpokfcfYfapuC9bNxrztA/view?usp=sharing">PDF</a>
          </div>
        </div>
      </article>

      <article class="rt-pub-card">
        <a class="rt-pub-media" href="https://arxiv.org/pdf/2510.26495">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/06.png' | relative_url }}" alt="Text-to-SQL paper teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Rethinking Text-to-SQL: Dynamic Multi-turn SQL Interaction for Real-world Database Exploration</h3>
          <p class="rt-pub-authors">Linzhuang Sun*, Tianyu Guo*, Hao Liang*, <strong>Ruitong Liu</strong>, Yuying Li, Qifeng Cai, Jingxuan Wei, Yuchen Wu, Bihui Yu, Xiangxiang Zhang, Wentao Zhang#, Bin CUI#</p>
          <p class="rt-pub-meta">ACL 2026 Under Review</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://arxiv.org/pdf/2510.26495">PDF</a>
            <a class="rt-pill" href="https://github.com/Aurora-slz/DySQL-Bench.git">Code</a>
          </div>
        </div>
      </article>

      <article class="rt-pub-card">
        <a class="rt-pub-media" href="https://arxiv.org/pdf/2602.12389">
          <img class="rt-pub-thumb" src="{{ '/images/home_pubs/07.png' | relative_url }}" alt="Temporal KGF paper teaser">
        </a>
        <div class="rt-pub-body">
          <h3 class="rt-pub-title">Evolving Beyond Snapshots: Harmonizing Structure and Sequence via Entity State Tuning for Temporal Knowledge Graph Forecasting</h3>
          <p class="rt-pub-authors">Yunjia Wu, yiyong xiao, Huang Pingyang, Peize Li, Siyuan Li#, <strong>Ruitong Liu#</strong>, Yan Wen, Te Sun, Fangyi Pei</p>
          <p class="rt-pub-meta">ACL 2026 Under Review</p>
          <div class="rt-pub-links">
            <a class="rt-pill" href="https://arxiv.org/pdf/2602.12389">PDF</a>
            <a class="rt-pill" href="https://github.com/yuanwuyuan9/Evolving-Beyond-Snapshots.git">Code</a>
          </div>
        </div>
      </article>
    </div>
  </div>

  <h2 class="rt-section-title" id="section-visitor"><i class="fa fa-globe" aria-hidden="true"></i> Visitor</h2>
  <div class="rt-visitor-wrap">
    <div class="rt-visitor-card rt-visitor-map">
      <div class="rt-map-embed">
        <script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?d=wWuKIsCZO2yYZA7sXQVVhdoENIGHAUsZCAy6ZjG-Uhk&cl=ffffff&w=a"></script>
      </div>
      <div style="font-size:0.86em;color:#64748b;margin-top:6px;">Visitor Geography</div>
    </div>
    <div class="rt-visitor-bottom">
      <div class="rt-service-card">
        <div class="rt-service-title">Service</div>
        <p class="rt-service-text">Reviewer/PC Member: Transactions on Knowledge Discovery from Data (TKDD)</p>
      </div>
      <div class="rt-counter-card">
        <div class="rt-counter-title">Visit Counter</div>
        <div id="busuanzi_value_site_pv" data-offset="20" class="rt-counter-value">--</div>
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
