<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Redwan-ul Karim Ratul - Professional Accountant & Data Analyst based in Dhaka, Bangladesh">
<meta name="keywords" content="accountant, data analyst, bookkeeping, financial statements, data visualization, Dhaka">
<title>Redwan-ul Karim Ratul | Accountant & Data Analyst</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Hind+Siliguri:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,700;0,800;1,700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
<script src="https://cdn.tailwindcss.com"></script>
<style>
/* ============================================================
   CONFIGURATION — Change these variables to customize site
   ============================================================ */
:root {
  --primary: #3a86ff;
  --primary-dark: #1a65d6;
  --primary-glow: rgba(58,134,255,0.35);
  --accent: #ff6b6b;
  --accent2: #06d6a0;
  --bg-dark: #060b14;
  --bg-mid: #0d1628;
  --bg-card: rgba(13,22,40,0.75);
  --glass: rgba(255,255,255,0.055);
  --glass-border: rgba(255,255,255,0.10);
  --text-primary: #f0f4ff;
  --text-secondary: #8fa3c8;
  --text-muted: #4a6080;
  --font-body: 'Hind Siliguri', sans-serif;
  --font-display: 'Playfair Display', serif;
  --radius: 16px;
  --shadow-card: 0 8px 40px rgba(0,0,0,0.45), 0 1px 0 rgba(255,255,255,0.06) inset;
  --transition: 0.4s cubic-bezier(0.16,1,0.3,1);
}

/* ============================================================
   BASE RESET & GLOBAL
   ============================================================ */
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; font-size: 16px; }
body {
  background: var(--bg-dark);
  color: var(--text-primary);
  font-family: var(--font-body);
  overflow-x: hidden;
  line-height: 1.65;
}
::selection { background: var(--primary); color: #fff; }
::-webkit-scrollbar { width: 6px; }
::-webkit-scrollbar-track { background: var(--bg-dark); }
::-webkit-scrollbar-thumb { background: var(--primary); border-radius: 3px; }

img { max-width: 100%; display: block; }
a { text-decoration: none; color: inherit; }

/* ============================================================
   BACKGROUND MESH / GRID
   ============================================================ */
body::before {
  content: '';
  position: fixed; inset: 0;
  background:
    radial-gradient(ellipse 80% 60% at 20% 10%, rgba(58,134,255,0.12) 0%, transparent 60%),
    radial-gradient(ellipse 60% 40% at 80% 80%, rgba(6,214,160,0.08) 0%, transparent 55%),
    radial-gradient(ellipse 40% 30% at 60% 40%, rgba(255,107,107,0.06) 0%, transparent 50%);
  pointer-events: none; z-index: 0;
}
.grid-overlay {
  position: fixed; inset: 0;
  background-image:
    linear-gradient(rgba(58,134,255,0.04) 1px, transparent 1px),
    linear-gradient(90deg, rgba(58,134,255,0.04) 1px, transparent 1px);
  background-size: 60px 60px;
  pointer-events: none; z-index: 0;
}

/* ============================================================
   UTILITY
   ============================================================ */
.container { max-width: 1200px; margin: 0 auto; padding: 0 24px; }
.section-tag {
  display: inline-flex; align-items: center; gap: 8px;
  font-size: 11px; font-weight: 600; letter-spacing: 3px; text-transform: uppercase;
  color: var(--primary); background: rgba(58,134,255,0.1);
  border: 1px solid rgba(58,134,255,0.25);
  padding: 6px 16px; border-radius: 30px; margin-bottom: 20px;
}
.section-title {
  font-family: var(--font-display);
  font-size: clamp(2rem, 4vw, 3rem);
  font-weight: 800; line-height: 1.15;
  background: linear-gradient(135deg, #f0f4ff 0%, var(--primary) 100%);
  -webkit-background-clip: text; -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 16px;
}
.section-subtitle {
  color: var(--text-secondary); font-size: 1.05rem;
  max-width: 540px; line-height: 1.75;
}
.gradient-text {
  background: linear-gradient(135deg, var(--primary) 0%, var(--accent2) 100%);
  -webkit-background-clip: text; -webkit-text-fill-color: transparent;
  background-clip: text;
}
.glow-btn {
  display: inline-flex; align-items: center; gap: 10px;
  padding: 14px 32px; border-radius: 50px;
  font-family: var(--font-body); font-size: 0.95rem; font-weight: 600;
  cursor: pointer; transition: var(--transition);
  border: none; position: relative; overflow: hidden;
}
.glow-btn::after {
  content: ''; position: absolute; inset: 0;
  background: rgba(255,255,255,0.15);
  transform: translateX(-100%); transition: transform 0.5s ease;
}
.glow-btn:hover::after { transform: translateX(100%); }
.btn-primary {
  background: linear-gradient(135deg, var(--primary) 0%, #1a65d6 100%);
  color: #fff;
  box-shadow: 0 4px 24px var(--primary-glow), 0 1px 0 rgba(255,255,255,0.15) inset;
}
.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 32px rgba(58,134,255,0.5);
}
.btn-outline {
  background: transparent;
  color: var(--text-primary);
  border: 1px solid var(--glass-border);
  backdrop-filter: blur(10px);
}
.btn-outline:hover {
  border-color: var(--primary);
  color: var(--primary);
  transform: translateY(-2px);
  box-shadow: 0 0 20px rgba(58,134,255,0.15);
}
.glass-card {
  background: var(--glass);
  backdrop-filter: blur(20px) saturate(180%);
  border: 1px solid var(--glass-border);
  border-radius: var(--radius);
  box-shadow: var(--shadow-card);
  position: relative; overflow: hidden;
}
.glass-card::before {
  content: '';
  position: absolute; top: 0; left: 0; right: 0; height: 1px;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.15), transparent);
}

/* ============================================================
   NAVBAR
   ============================================================ */
#navbar {
  position: fixed; top: 0; left: 0; right: 0; z-index: 1000;
  padding: 20px 0;
  transition: all 0.4s ease;
}
#navbar.scrolled {
  background: rgba(6,11,20,0.85);
  backdrop-filter: blur(24px);
  padding: 12px 0;
  border-bottom: 1px solid var(--glass-border);
  box-shadow: 0 4px 30px rgba(0,0,0,0.4);
}
.nav-inner {
  display: flex; align-items: center; justify-content: space-between;
}
.nav-logo {
  font-family: var(--font-display);
  font-size: 1.5rem; font-weight: 700;
  background: linear-gradient(135deg, #fff 0%, var(--primary) 100%);
  -webkit-background-clip: text; -webkit-text-fill-color: transparent;
  background-clip: text;
}
.nav-logo span {
  display: inline-block;
  width: 8px; height: 8px; border-radius: 50%;
  background: var(--primary);
  margin-left: 3px; vertical-align: super;
}
.nav-links { display: flex; align-items: center; gap: 36px; list-style: none; }
.nav-links a {
  font-size: 0.875rem; font-weight: 500; letter-spacing: 0.5px;
  color: var(--text-secondary);
  transition: color 0.3s, opacity 0.3s;
  position: relative;
}
.nav-links a::after {
  content: ''; position: absolute; bottom: -4px; left: 0; right: 0;
  height: 2px; background: var(--primary);
  transform: scaleX(0); transform-origin: right;
  transition: transform 0.35s ease;
}
.nav-links a:hover, .nav-links a.active { color: #fff; }
.nav-links a:hover::after, .nav-links a.active::after { transform: scaleX(1); transform-origin: left; }
.nav-cta { display: flex; align-items: center; gap: 16px; }
#menu-toggle {
  display: none; flex-direction: column; gap: 5px;
  cursor: pointer; padding: 4px;
}
#menu-toggle span {
  display: block; width: 24px; height: 2px;
  background: var(--text-primary); border-radius: 2px;
  transition: var(--transition);
}
#mobile-menu {
  display: none; position: fixed; inset: 0; z-index: 999;
  background: rgba(6,11,20,0.97);
  backdrop-filter: blur(30px);
  flex-direction: column; align-items: center; justify-content: center;
  gap: 32px;
}
#mobile-menu.open { display: flex; }
#mobile-menu a {
  font-family: var(--font-display);
  font-size: 2rem; font-weight: 700;
  color: var(--text-secondary);
  transition: color 0.3s;
}
#mobile-menu a:hover { color: var(--primary); }
#mobile-close {
  position: absolute; top: 24px; right: 24px;
  font-size: 1.5rem; color: var(--text-secondary);
  cursor: pointer; transition: color 0.3s;
}
#mobile-close:hover { color: var(--primary); }

/* ============================================================
   HERO SECTION
   ============================================================ */
#hero {
  min-height: 100vh;
  display: flex; align-items: center;
  position: relative; overflow: hidden;
  padding: 120px 0 80px;
}
.hero-bg {
  position: absolute; inset: 0;
  background: radial-gradient(ellipse 100% 80% at 50% -10%, rgba(58,134,255,0.18) 0%, transparent 60%);
}
.hero-particles {
  position: absolute; inset: 0; overflow: hidden;
}
.hero-particles span {
  position: absolute; border-radius: 50%;
  background: var(--primary); opacity: 0.12;
  animation: float-particle linear infinite;
}
@keyframes float-particle {
  0% { transform: translateY(100vh) rotate(0deg); opacity: 0; }
  10% { opacity: 0.12; }
  90% { opacity: 0.12; }
  100% { transform: translateY(-100px) rotate(720deg); opacity: 0; }
}
.hero-inner {
  display: grid; grid-template-columns: 1fr 1fr;
  gap: 80px; align-items: center;
  position: relative; z-index: 1;
}
.hero-badge {
  display: inline-flex; align-items: center; gap: 8px;
  background: rgba(58,134,255,0.12); border: 1px solid rgba(58,134,255,0.3);
  padding: 8px 18px; border-radius: 30px;
  font-size: 0.8rem; font-weight: 600; letter-spacing: 2px;
  text-transform: uppercase; color: var(--primary);
  margin-bottom: 28px;
  animation: fade-up 0.8s ease both;
}
.hero-badge i { font-size: 0.75rem; animation: pulse 2s ease infinite; }
@keyframes pulse { 0%,100% { opacity:1; } 50% { opacity:0.4; } }
.hero-name {
  font-family: var(--font-display);
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  font-weight: 800; line-height: 1.1;
  color: #fff; margin-bottom: 12px;
  animation: fade-up 0.8s 0.15s ease both;
}
.hero-name .line2 {
  display: block;
  background: linear-gradient(135deg, var(--primary) 0%, var(--accent2) 100%);
  -webkit-background-clip: text; -webkit-text-fill-color: transparent;
  background-clip: text;
}
.hero-roles {
  font-size: 1.25rem; color: var(--text-secondary);
  margin-bottom: 20px; min-height: 2em;
  animation: fade-up 0.8s 0.3s ease both;
}
.hero-roles .static { color: var(--text-secondary); }
.hero-roles .dynamic {
  color: var(--primary); font-weight: 600;
  border-right: 2px solid var(--primary);
  animation: blink-cursor 0.75s step-end infinite;
}
@keyframes blink-cursor { 0%,100%{border-color:var(--primary)} 50%{border-color:transparent} }
.hero-desc {
  color: var(--text-secondary); font-size: 1.0rem;
  max-width: 480px; line-height: 1.8; margin-bottom: 36px;
  animation: fade-up 0.8s 0.45s ease both;
}
.hero-actions {
  display: flex; align-items: center; gap: 16px; flex-wrap: wrap;
  margin-bottom: 48px;
  animation: fade-up 0.8s 0.6s ease both;
}
.hero-socials {
  display: flex; align-items: center; gap: 12px;
  animation: fade-up 0.8s 0.75s ease both;
}
.hero-socials a {
  width: 44px; height: 44px;
  display: flex; align-items: center; justify-content: center;
  border-radius: 50%; font-size: 1rem;
  border: 1px solid var(--glass-border);
  color: var(--text-secondary);
  transition: var(--transition);
  background: var(--glass); backdrop-filter: blur(10px);
}
.hero-socials a:hover {
  border-color: var(--primary); color: var(--primary);
  background: rgba(58,134,255,0.1);
  transform: translateY(-3px);
  box-shadow: 0 8px 20px rgba(58,134,255,0.25);
}
.hero-image-wrap {
  position: relative;
  animation: fade-left 1s 0.3s ease both;
}
.hero-image-ring {
  position: absolute; inset: -20px;
  border: 2px dashed rgba(58,134,255,0.3);
  border-radius: 50%;
  animation: spin-slow 20s linear infinite;
}
.hero-image-ring2 {
  position: absolute; inset: -40px;
  border: 1px dashed rgba(6,214,160,0.2);
  border-radius: 50%;
  animation: spin-slow 30s linear infinite reverse;
}
@keyframes spin-slow { to { transform: rotate(360deg); } }
.hero-image-blob {
  position: absolute; inset: -10px;
  background: radial-gradient(circle, rgba(58,134,255,0.2) 0%, transparent 70%);
  border-radius: 50%; filter: blur(20px);
  animation: pulse-glow 3s ease infinite;
}
@keyframes pulse-glow { 0%,100% { transform:scale(1); opacity:0.6; } 50% { transform:scale(1.1); opacity:1; } }
.hero-image-frame {
  width: 380px; height: 380px; border-radius: 50%;
  overflow: hidden; position: relative; margin: 0 auto;
  border: 3px solid rgba(58,134,255,0.4);
  box-shadow: 0 0 60px rgba(58,134,255,0.3), 0 0 120px rgba(58,134,255,0.1);
}
.hero-image-frame img {
  width: 100%; height: 100%; object-fit: cover;
  object-position: center top;
}
.hero-stat-pill {
  position: absolute;
  display: flex; align-items: center; gap: 10px;
  background: rgba(13,22,40,0.85);
  backdrop-filter: blur(20px);
  border: 1px solid var(--glass-border);
  border-radius: 50px; padding: 10px 20px;
  box-shadow: 0 8px 32px rgba(0,0,0,0.4);
  white-space: nowrap;
}
.hero-stat-pill .icon {
  width: 36px; height: 36px; border-radius: 50%;
  display: flex; align-items: center; justify-content: center;
  font-size: 0.9rem;
}
.hero-stat-pill .num { font-weight: 700; font-size: 1.1rem; }
.hero-stat-pill .lbl { font-size: 0.7rem; color: var(--text-secondary); }
.pill-top-left { top: 5%; left: -10%; animation: float-bob 4s ease infinite; }
.pill-bottom-right { bottom: 8%; right: -8%; animation: float-bob 4s 2s ease infinite; }
.pill-top-right { top: 30%; right: -12%; animation: float-bob 4s 1s ease infinite; }
@keyframes float-bob { 0%,100% { transform:translateY(0); } 50% { transform:translateY(-10px); } }
@keyframes fade-up { from { opacity:0; transform:translateY(30px); } to { opacity:1; transform:translateY(0); } }
@keyframes fade-left { from { opacity:0; transform:translateX(50px); } to { opacity:1; transform:translateX(0); } }

/* ============================================================
   SECTION WRAPPER
   ============================================================ */
section { padding: 100px 0; position: relative; z-index: 1; }
.section-header { text-align: center; margin-bottom: 64px; }

/* ============================================================
   ABOUT SECTION
   ============================================================ */
.about-grid {
  display: grid; grid-template-columns: 1fr 1.3fr;
  gap: 64px; align-items: center;
}
.about-image-wrap { position: relative; }
.about-img-outer {
  border-radius: 24px; overflow: hidden;
  border: 1px solid var(--glass-border);
  box-shadow: var(--shadow-card);
  position: relative;
}
.about-img-outer::after {
  content: '';
  position: absolute; inset: 0;
  background: linear-gradient(180deg, transparent 50%, rgba(6,11,20,0.8) 100%);
}
.about-img-outer img { width: 100%; height: 420px; object-fit: cover; object-position: center top; }
.about-badge-float {
  position: absolute; bottom: -20px; right: -20px;
  background: linear-gradient(135deg, var(--primary), #1a65d6);
  padding: 20px 24px; border-radius: 16px;
  text-align: center;
  box-shadow: 0 8px 32px rgba(58,134,255,0.4);
}
.about-badge-float .num { font-size: 2.5rem; font-weight: 800; line-height: 1; }
.about-badge-float .lbl { font-size: 0.7rem; letter-spacing: 1px; opacity: 0.85; }
.about-info h2 { margin-bottom: 20px; }
.about-info p { color: var(--text-secondary); line-height: 1.85; margin-bottom: 20px; }
.about-pills { display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 32px; }
.about-pill {
  font-size: 0.8rem; font-weight: 500;
  padding: 6px 16px; border-radius: 30px;
  border: 1px solid var(--glass-border);
  background: var(--glass); color: var(--text-secondary);
  transition: 0.3s;
}
.about-pill:hover { border-color: var(--primary); color: var(--primary); }
.about-facts { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
.about-fact {
  padding: 20px; border-radius: 12px;
  background: var(--glass); border: 1px solid var(--glass-border);
  transition: var(--transition);
}
.about-fact:hover { border-color: rgba(58,134,255,0.3); transform: translateY(-2px); }
.about-fact i { font-size: 1.2rem; color: var(--primary); margin-bottom: 8px; }
.about-fact h4 { font-weight: 700; margin-bottom: 4px; }
.about-fact p { font-size: 0.8rem; color: var(--text-secondary); margin: 0; }

/* ============================================================
   SKILLS SECTION
   ============================================================ */
#skills { background: rgba(13,22,40,0.4); }
.skills-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 24px; }
.skill-card {
  padding: 32px; border-radius: var(--radius);
  background: var(--glass); border: 1px solid var(--glass-border);
  backdrop-filter: blur(20px);
  transition: var(--transition);
  position: relative; overflow: hidden;
  cursor: default;
}
.skill-card::before {
  content: ''; position: absolute; top: 0; left: 0; right: 0; bottom: 0;
  background: radial-gradient(circle at 50% 0%, rgba(58,134,255,0.08), transparent 60%);
  opacity: 0; transition: opacity 0.4s;
}
.skill-card:hover { border-color: rgba(58,134,255,0.35); transform: translateY(-6px); box-shadow: 0 20px 60px rgba(0,0,0,0.4); }
.skill-card:hover::before { opacity: 1; }
.skill-icon {
  width: 56px; height: 56px; border-radius: 14px;
  display: flex; align-items: center; justify-content: center;
  font-size: 1.4rem; margin-bottom: 20px;
}
.skill-card h3 { font-size: 1.1rem; font-weight: 700; margin-bottom: 12px; }
.skill-list { list-style: none; }
.skill-list li {
  font-size: 0.875rem; color: var(--text-secondary);
  padding: 5px 0; display: flex; align-items: center; gap: 8px;
}
.skill-list li::before {
  content: ''; width: 5px; height: 5px; border-radius: 50%;
  background: var(--primary); flex-shrink: 0;
}

/* ============================================================
   PORTFOLIO / PROJECTS
   ============================================================ */
.projects-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 28px; }
.project-card {
  border-radius: var(--radius);
  border: 1px solid var(--glass-border);
  background: var(--glass);
  backdrop-filter: blur(20px);
  overflow: hidden;
  transition: var(--transition);
  box-shadow: var(--shadow-card);
}
.project-card:hover { border-color: rgba(58,134,255,0.35); transform: translateY(-8px); box-shadow: 0 24px 64px rgba(0,0,0,0.5); }
.project-img {
  height: 220px; overflow: hidden; position: relative;
  background: #0d1628;
}
.project-img img {
  width: 100%; height: 100%; object-fit: cover;
  transition: transform 6s cubic-bezier(0.25,0.46,0.45,0.94);
  transform: translateY(0);
}
.project-card:hover .project-img img { transform: translateY(-30%); }
.project-overlay {
  position: absolute; inset: 0;
  background: linear-gradient(180deg, transparent 40%, rgba(6,11,20,0.95) 100%);
  display: flex; align-items: flex-end; padding: 20px;
  opacity: 0; transition: opacity 0.4s;
}
.project-card:hover .project-overlay { opacity: 1; }
.project-overlay-btns { display: flex; gap: 10px; }
.project-overlay-btn {
  padding: 8px 20px; border-radius: 30px; font-size: 0.8rem; font-weight: 600;
  display: flex; align-items: center; gap: 6px;
  cursor: pointer; transition: 0.3s; border: none;
}
.project-body { padding: 24px; }
.project-tag {
  font-size: 0.72rem; font-weight: 600; letter-spacing: 1.5px;
  text-transform: uppercase; color: var(--primary);
  margin-bottom: 10px; display: block;
}
.project-body h3 { font-weight: 700; font-size: 1.1rem; margin-bottom: 8px; }
.project-body p { font-size: 0.875rem; color: var(--text-secondary); line-height: 1.7; }

/* ============================================================
   CERTIFICATIONS
   ============================================================ */
#certifications { background: rgba(13,22,40,0.4); }
.certs-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; }
.cert-card {
  border-radius: var(--radius); overflow: hidden;
  border: 1px solid var(--glass-border);
  background: var(--glass); backdrop-filter: blur(20px);
  transition: var(--transition); cursor: pointer;
  position: relative;
}
.cert-card:hover { border-color: rgba(58,134,255,0.4); transform: scale(1.04); box-shadow: 0 16px 48px rgba(58,134,255,0.25); }
.cert-card img { width: 100%; height: 180px; object-fit: cover; transition: 0.4s; }
.cert-card:hover img { transform: scale(1.05); }
.cert-label {
  padding: 14px 16px; font-size: 0.82rem; font-weight: 600;
  text-align: center; color: var(--text-secondary);
}
.cert-badge-icon {
  position: absolute; top: 12px; right: 12px;
  width: 32px; height: 32px; border-radius: 50%;
  background: var(--primary); display: flex; align-items: center; justify-content: center;
  font-size: 0.8rem; color: #fff;
}

/* ============================================================
   EXPERIENCE / TIMELINE
   ============================================================ */
.timeline { position: relative; max-width: 800px; margin: 0 auto; }
.timeline::before {
  content: ''; position: absolute; left: 32px; top: 0; bottom: 0;
  width: 2px; background: linear-gradient(to bottom, var(--primary), var(--accent2));
}
.timeline-item {
  display: flex; gap: 32px; padding-left: 0; margin-bottom: 48px;
  position: relative;
}
.timeline-dot {
  flex-shrink: 0; width: 64px; height: 64px;
  border-radius: 50%;
  background: var(--bg-mid); border: 2px solid var(--primary);
  display: flex; align-items: center; justify-content: center;
  font-size: 1.3rem; color: var(--primary);
  position: relative; z-index: 1;
  transition: 0.3s;
  box-shadow: 0 0 20px rgba(58,134,255,0.3);
}
.timeline-item:hover .timeline-dot {
  background: var(--primary); color: #fff;
  box-shadow: 0 0 32px rgba(58,134,255,0.5);
}
.timeline-content {
  flex: 1; padding: 24px;
  background: var(--glass); border: 1px solid var(--glass-border);
  border-radius: var(--radius); backdrop-filter: blur(20px);
  transition: var(--transition);
}
.timeline-item:hover .timeline-content { border-color: rgba(58,134,255,0.3); transform: translateX(4px); }
.timeline-content .period {
  font-size: 0.75rem; color: var(--primary); font-weight: 600;
  letter-spacing: 1px; margin-bottom: 8px; display: block;
}
.timeline-content h3 { font-weight: 700; font-size: 1.1rem; margin-bottom: 4px; }
.timeline-content .company { color: var(--text-secondary); font-size: 0.875rem; margin-bottom: 12px; }
.timeline-content p { font-size: 0.875rem; color: var(--text-secondary); line-height: 1.7; }

/* ============================================================
   CONTACT
   ============================================================ */
.contact-grid {
  display: grid; grid-template-columns: 1fr 1.4fr; gap: 64px; align-items: start;
}
.contact-info-items { margin-top: 32px; display: flex; flex-direction: column; gap: 20px; }
.contact-item {
  display: flex; align-items: center; gap: 16px;
  padding: 20px; border-radius: 12px;
  background: var(--glass); border: 1px solid var(--glass-border);
  backdrop-filter: blur(10px); transition: 0.3s;
}
.contact-item:hover { border-color: rgba(58,134,255,0.3); transform: translateX(4px); }
.contact-item .icon {
  width: 44px; height: 44px; border-radius: 50%;
  display: flex; align-items: center; justify-content: center;
  background: rgba(58,134,255,0.12); color: var(--primary); font-size: 1rem;
  flex-shrink: 0;
}
.contact-item .detail span { font-size: 0.75rem; color: var(--text-secondary); display: block; }
.contact-item .detail strong { font-size: 0.95rem; }
.contact-form { display: flex; flex-direction: column; gap: 20px; }
.form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
.form-group { display: flex; flex-direction: column; gap: 8px; }
.form-group label { font-size: 0.8rem; font-weight: 600; color: var(--text-secondary); letter-spacing: 0.5px; }
.form-group input,
.form-group textarea {
  background: var(--glass); border: 1px solid var(--glass-border);
  border-radius: 10px; padding: 14px 18px;
  color: var(--text-primary); font-family: var(--font-body); font-size: 0.95rem;
  transition: 0.3s; outline: none; resize: none;
}
.form-group input:focus,
.form-group textarea:focus {
  border-color: var(--primary);
  box-shadow: 0 0 0 3px rgba(58,134,255,0.15);
  background: rgba(58,134,255,0.05);
}
.form-group input::placeholder,
.form-group textarea::placeholder { color: var(--text-muted); }
#form-status {
  padding: 14px 20px; border-radius: 10px;
  font-size: 0.9rem; font-weight: 500;
  text-align: center; display: none;
}
#form-status.success { background: rgba(6,214,160,0.15); border: 1px solid rgba(6,214,160,0.3); color: var(--accent2); }
#form-status.error { background: rgba(255,107,107,0.1); border: 1px solid rgba(255,107,107,0.3); color: var(--accent); }

/* ============================================================
   MAP SECTION
   ============================================================ */
#map-section { padding: 0; }
.map-wrap {
  position: relative;
  height: 400px; overflow: hidden;
  border-top: 1px solid var(--glass-border);
}
.map-wrap::before {
  content: ''; position: absolute; inset: 0;
  background: linear-gradient(to right, var(--bg-dark) 0%, transparent 30%, transparent 70%, var(--bg-dark) 100%);
  z-index: 1; pointer-events: none;
}
.map-wrap::after {
  content: ''; position: absolute; top: 0; left: 0; right: 0; height: 60px;
  background: linear-gradient(to bottom, var(--bg-dark), transparent);
  z-index: 1; pointer-events: none;
}
.map-wrap iframe { width: 100%; height: 100%; filter: invert(90%) hue-rotate(180deg) saturate(0.4) brightness(0.8); border: none; }

/* ============================================================
   FOOTER
   ============================================================ */
footer {
  background: rgba(6,11,20,0.95);
  border-top: 1px solid var(--glass-border);
  padding: 40px 0 28px;
  position: relative; z-index: 1;
}
.footer-inner {
  display: flex; align-items: center; justify-content: space-between;
  flex-wrap: wrap; gap: 20px;
}
.footer-links { display: flex; gap: 24px; }
.footer-links a { font-size: 0.875rem; color: var(--text-secondary); transition: color 0.3s; }
.footer-links a:hover { color: var(--primary); }
.footer-copy { font-size: 0.8rem; color: var(--text-muted); text-align: center; margin-top: 20px; }

/* ============================================================
   SCROLL REVEAL
   ============================================================ */
.reveal {
  opacity: 0; transform: translateY(40px);
  transition: opacity 0.7s ease, transform 0.7s ease;
}
.reveal.visible { opacity: 1; transform: translateY(0); }
.reveal-delay-1 { transition-delay: 0.1s; }
.reveal-delay-2 { transition-delay: 0.2s; }
.reveal-delay-3 { transition-delay: 0.3s; }
.reveal-delay-4 { transition-delay: 0.4s; }

/* ============================================================
   BACK TO TOP
   ============================================================ */
#back-top {
  position: fixed; bottom: 28px; right: 28px; z-index: 99;
  width: 48px; height: 48px; border-radius: 50%;
  background: linear-gradient(135deg, var(--primary), #1a65d6);
  color: #fff; display: flex; align-items: center; justify-content: center;
  font-size: 1rem; cursor: pointer;
  box-shadow: 0 4px 20px rgba(58,134,255,0.45);
  opacity: 0; transform: translateY(20px);
  transition: var(--transition); border: none;
}
#back-top.show { opacity: 1; transform: translateY(0); }
#back-top:hover { transform: translateY(-4px); box-shadow: 0 8px 28px rgba(58,134,255,0.6); }

/* ============================================================
   MODAL (Cert lightbox)
   ============================================================ */
#modal-overlay {
  display: none; position: fixed; inset: 0; z-index: 2000;
  background: rgba(0,0,0,0.85); backdrop-filter: blur(10px);
  align-items: center; justify-content: center; padding: 20px;
}
#modal-overlay.open { display: flex; }
#modal-img { max-width: 90vw; max-height: 90vh; border-radius: 12px; box-shadow: 0 20px 80px rgba(0,0,0,0.8); }
#modal-close {
  position: absolute; top: 20px; right: 24px;
  font-size: 2rem; color: #fff; cursor: pointer; opacity: 0.8; transition: 0.3s;
}
#modal-close:hover { opacity: 1; color: var(--accent); }

/* ============================================================
   RESPONSIVE
   ============================================================ */
@media (max-width: 1024px) {
  .hero-inner { grid-template-columns: 1fr; gap: 60px; text-align: center; }
  .hero-desc { max-width: none; }
  .hero-actions { justify-content: center; }
  .hero-socials { justify-content: center; }
  .hero-image-wrap { order: -1; }
  .hero-image-frame { width: 280px; height: 280px; }
  .pill-top-left,.pill-bottom-right,.pill-top-right { display: none; }
  .about-grid { grid-template-columns: 1fr; gap: 40px; }
  .contact-grid { grid-template-columns: 1fr; gap: 40px; }
}
@media (max-width: 768px) {
  section { padding: 70px 0; }
  .nav-links, .nav-cta { display: none; }
  #menu-toggle { display: flex; }
  .form-row { grid-template-columns: 1fr; }
  .about-facts { grid-template-columns: 1fr; }
  .timeline::before { left: 24px; }
  .timeline-dot { width: 48px; height: 48px; font-size: 1rem; }
}
@media (max-width: 480px) {
  .hero-name { font-size: 2.2rem; }
  .hero-image-frame { width: 220px; height: 220px; }
}
</style>
</head>
<body>
<div class="grid-overlay"></div>

<!-- ============================================================
     JAVASCRIPT DATA — EDIT THESE VARIABLES TO CUSTOMIZE
     ============================================================ -->
<script>
const SITE_DATA = {
  // Personal Info
  name: "Redwan-ul Karim Ratul",
  title: "Chartered Accountant & Data Analyst",
  tagline: "Transforming Complex Financial Data into Actionable Insights",
  phone: "01913665046",
  email: "redwanratul027@gmail.com",
  location: "Dhaka, Bangladesh",
  yearsExp: "3.5+",
  projectsDone: "50+",
  clientsServed: "30+",

  // Profile Image
  profileImage: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEijdHkzABLb6Qwu928T3_4ErI70McDfp64aZreiQrNlkrR1SMgjQGcTuqtQc3LW0fJwUK6XhyTfLvlk3PM3Vmhm5wGcbgdd3LffzMocJeHgY7Vu4J3fYEsn7jR2Du0WlGAP3Y38_bS_6cfyreS1dGKcFyh-Kbe48W2nVFmtETY_s-ENN30odYnnlX22z1Q/s320/WhatsApp%20Image%202026-05-24%20at%2011.37.23%20AM.jpeg",

  // Social Links
  social: {
    facebook: "https://www.facebook.com/share/1GRu1AKdKp/",
    linkedin: "https://www.linkedin.com/in/redwanul-karim-ratul-839074253",
    instagram: "https://www.instagram.com/redwan3403?igsh=MXhxYW5oZDc2Mm5ydA=="
  },

  // Typing Roles (hero rotation text)
  roles: [
    "Chartered Accountant (CA)",
    "Data Analyst",
    "Tax & VAT Specialist",
    "Financial Statement Expert",
    "Data Visualization Expert",
    "Audit & Compliance Pro"
  ],

  // About Summary
  aboutText: [
    "Chartered Accountant & Data-Driven Financial Professional with over 3.5 years of progressive experience in financial accounting, taxation, auditing, and advanced data analytics. Currently associated with a reputed Chartered Accountancy Firm registered with the Institute of Chartered Accountants of Bangladesh (ICAB) since November 2022.",
    "I specialize in preparing complete sets of financial statements, managing month-end and year-end closings, corporate and individual tax computations, VAT & direct tax compliance, regulatory reporting, and audit support. My expertise spans multiple industries including manufacturing, trading, services, and telecommunications.",
    "Passionate about leveraging both accounting precision and modern data analytics, I transform complex financial data into actionable insights using predictive modeling, statistical analysis, and dynamic data visualization — helping businesses enhance decision-making, optimize performance, and achieve operational efficiency."
  ],

  // Skills Categories
  skills: [
    {
      icon: "fa-solid fa-calculator",
      color: "#3a86ff",
      bg: "rgba(58,134,255,0.12)",
      title: "Accounting & Finance",
      items: ["Data Entry & Bookkeeping", "Ledger Management", "Bank Reconciliation", "Financial Statement Prep", "Cloud Accounting (QuickBooks/Xero)"]
    },
    {
      icon: "fa-solid fa-chart-line",
      color: "#06d6a0",
      bg: "rgba(6,214,160,0.12)",
      title: "Data Analytics",
      items: ["Data Collection & Cleaning", "Data Exploration (EDA)", "Statistical Analysis", "Insight Generation", "Report Building"]
    },
    {
      icon: "fa-solid fa-chart-pie",
      color: "#ff6b6b",
      bg: "rgba(255,107,107,0.12)",
      title: "Data Visualization",
      items: ["Power BI", "Tableau", "Excel Dashboards", "Google Data Studio", "Python (Matplotlib/Seaborn)"]
    },
    {
      icon: "fa-solid fa-brain",
      color: "#f7b731",
      bg: "rgba(247,183,49,0.12)",
      title: "Advanced Analytics",
      items: ["Predictive Modeling", "Performance Monitoring", "Decision Support", "Business Intelligence", "SQL Queries"]
    }
  ],

  // Projects
  projects: [
    {
      tag: "Marketing Analytics",
      title: "Marketing Performance Dashboard",
      desc: "Comprehensive marketing analytics dashboard tracking campaign ROI, customer acquisition, and engagement metrics.",
      image: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiIatZOQmjtJwg6fx47gq1QRmmEnhGQO7glJONT5GA0AGrf9gDyPXBVlFX3PbtU2hTwlz4bN1r8iwCVQdkSP9XO2pYUSd1YupATS5O6sGKklyPwCkA74vdT27Gu-KcQnX_a71dUxHcyUCOLNDl7fXGxlIKCUyGNs9LcVoYOPlUuOkgVHBhl22hQ-j9AO20/s320/05_marketing_analytics.png",
      previewLink: "#"
    },
    {
      tag: "Healthcare Analytics",
      title: "Healthcare Data Analysis Report",
      desc: "Statistical analysis of patient data to identify trends, reduce costs, and improve operational efficiency in healthcare.",
      image: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg3NSa6zypuhPS81GH7v40ITOydukQcO54eyPzG0KBT1sfO8KwlYBFd4Gr8P9FVwslJO6ldnS3xvHJehqOE5319_w60a_586HNYKvUiLUJy5FPDi_hdP_U5Ye1lWdx_PfwQ1KS8_iYnihMJLdP2LVWSeUI5A7OaBxFN7cHlIadBdo09PxPIR-BiOVd_DWY/s320/04_healthcare_analytics.png",
      previewLink: "#"
    },
    {
      tag: "Finance Analytics",
      title: "Financial Performance Analysis",
      desc: "In-depth financial analysis covering P&L statements, cash flow projections, and variance analysis for strategic planning.",
      image: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj4nm7i1EiY2kNKGGiUU9cdHKhbF4WkIdKgQtbdYSg-bMrWIEzLPDgIxwtpPFT4vq-ls0Gq4IsBx83KuJngfS09087QmknNNJJv8Gt9OPWiErXKcAAq4dM9sSHr3BkGgmj5pRQKaXEu3YJaaH2M6tDHZWITwgc6sGNmgcIkXYzXbuSv761vq44BHM4qMsU/s320/03_finance_analytics.png",
      previewLink: "#"
    },
    {
      tag: "E-Commerce Analytics",
      title: "E-Commerce Sales Dashboard",
      desc: "Real-time sales tracking, inventory management, and customer behavior analysis for e-commerce businesses.",
      image: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgiZg0r2blmor1TIFOZ3SkxqfF03oy9lbTNi3VntUetiSFxToCJ2tYR15PihURRJa7Pglneubqw7eGczfljO7UI4KXTTsvcC0VOjsl0r_ic71z24j2BcKrGXwvhDr8Z8YHNt2Om92HJrC2yIAYVvx4_9at7Z7SRJibUEW3wfCcEq0S9GwRsz3j-fBVuMQM/s320/01_ecommerce_analytics.png",
      previewLink: "#"
    },
    {
      tag: "HR Analytics",
      title: "HR Workforce Analytics",
      desc: "Employee performance tracking, attrition analysis, and workforce planning dashboard for HR decision-makers.",
      image: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiMLt-goDrXFwk4Kyw9FydoBPx9FOH8hpq5YSokfYWv8yB6DAaTo1dDvlAR3-LYop4ucHEQDP-mOrVc6E4_JL8IoU5vAjbkM9qxw7DEtMKSdCVjxP3OqMMOcaCXf7KkejLhorRyx9HooTJF3YWLOf4nR__QtjKL7V53RmoX2Qv1J6Wp1hi41TOfSKmn4wA/s320/02_hr_analytics.png",
      previewLink: "#"
    },
   {
                    title: "Business Insights Report",
                    category: "Report Building",
                    image: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhavxOSPXZdqbxKNMJUa4AIBB55jr8VQHh1I2t03kpJFdNiqx7C5NudWQE5jS8DFhzXghB0oQmvUXFO1yBggUrAnIcw6wYGJKjuHVylBmkLgDvLfYrPhlYto9kZImVdHKGNvt41Gs_vqLberU4uHAvyLF3T6yNz2Bgg3k01k7BMn6R_CTl4EYWBrhbbIjc/s320/WhatsApp%20Image%202026-05-17%20at%202.50.41%20PM.jpeg",
                    previewLink: "#", githubLink: "#"
                },
                {
                    title: "Sales Forecasting Model",
                    category: "Insight Generation",
                    image: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhpLNMaKxUGoI9uZI_2h2tAiWhF9HQGRXQ4XdVn6rmobr2dglyjJ5NrHkN4KqimuialmCcAXvrma8wU5scSGPqclvZx4LvCbjVz0b3usYswaYtgMswMc7SYfs-9yl-equbII7bXpJMjwj5x5pnavx33PmQ_abvzja3QS6yaluDk8A-okTvob0w_PZmOtwk/s320/WhatsApp%20Image%202026-05-17%20at%202.50.41%20PM%20(1).jpeg",
                    previewLink: "#", githubLink: "#"
                },
                {
                    title: "Data Cleaning Framework",
                    category: "Data Processing",
                    image: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjdVthmKotcdhjke9STFsMEEaUvPraUgilJyIA3ca_PXqW9sH05_XQ55NZMBL9WGImsDhVDM_n8ysBs0nanDmF935TJ878zJG0ifUapr870qFkKuiC9EMnqs-bZTVmho06i76CNvi5FB-3pCDUNlvt9_M9iborIuslukY1g33p-wVFjborcRS5YS2ELXlY/s320/WhatsApp%20Image%202026-05-17%20at%201.54.49%20PM%20(1).jpeg",
                    previewLink: "#", githubLink: "#"
                },
                {
                    title: "Ledger & Bookkeeping",
                    category: "Accounting",
                    image: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgoxYagqyneOzt1BnlAFjLAiRdSExkyLKF2_ycucCk4jDYrHGiXqQgaZ5TFIIQfv0fEEIw403SIT4iaM6waAEXo2sJPABOgK5RiVLjt8v1uk45GDamv0IN-nZqGgchIe4WrQ7TCcElWNzIpCOoMUOFo2X8W0KxpceBtBDWGfrF0PQ21f3FKhjzdLA2GbXQ/s320/WhatsApp%20Image%202026-05-17%20at%201.54.49%20PM.jpeg",
                    previewLink: "#", githubLink: "#"
                }
  ],

  // Certifications
  certifications: [
    { img: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEh2RRBGjIhK8FxH81QKui_w8MXDXT7x4NnzEwq9axUe1VPoHkl7uHUUQtEYKWCQ9w5BSpC4fUE21fy7CMDSYKB-KXycOfdyY_jUtlxuSk1NEkn0WoE-xXA9P8itHWj24aStWqHNjKM8rWBYE4rxRtoPYN4sPaRHaMPzMSKGmLjRbiTim0zy0fViwtlU-q0/s320/WhatsApp%20Image%202026-05-24%20at%2011.52.12%20AM.jpeg", label: "Professional Certification 1" },
    { img: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhYel8But3pkDY-Bks8Nilrk_cjTDjC7of76v1y98sUIl-O34iLnchskpjdtyAY7-GHP_o0g00s6rNX5LAsaphHhaPlBNcJ13F7TBiR6jZ6d9dBqb9HT4Ku9N0oWfVoHfAH4SDs-yKl9B9GmS-kXsyMobQ-CeBCFQUfUnx6X7X7hzsnNDYy5gansvJBF6A/s320/WhatsApp%20Image%202026-05-24%20at%2011.52.13%20AM%20(1).jpeg", label: "Professional Certification 2" },
    { img: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgleSBF5DmdJlFs8ocnCVmHFo6xH0E4lcpvdJ9SywRdRAmuA18K0kv5mJxykJs_zXHEHYp0O6CSq7k5ptDq5nIfVk-JoNOocMlQVes9rdOUBYzxsfZHAVzMUsDqf7E64sa18IvUp5VGxJgPVr2hyphenhyphenmq3YRWKAszh173DnYZtRjnobxARNngYpcDQkrlDPEI/s320/WhatsApp%20Image%202026-05-24%20at%2011.52.13%20AM%20(2).jpeg", label: "Professional Certification 3" },
    { img: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhTH7iDSfZgHjXGA8zr6u2JT52sjyrGT2KJXnPEg0Jy6PEFmSpwINQ_wlCoBBUQEheme7LrGhiW7Zr79QaNFSRvY7eYeUCL6QBu7WfehgaVkCx4XmtZUxgz15xzLWj635KpN0m-8yZaIKbxppT3oA6zUt5b2wfqbET1K33JHB6lrpjZVmyW7Tky1IWBKqQ/s320/WhatsApp%20Image%202026-05-24%20at%2011.52.13%20AM.jpeg", label: "Professional Certification 4" },
    { img: "https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjCIEOQNJvuWPCSZQ0g6bpfHXneruXPTLIWcr_YMFY5ejt6ROGok01_viJMYgHYDj-RntViXA-eSBBhcb5sBnM4gQoMHRMnECoHPChS3xsqqZc2fJ4_MSWTPabhKk2AMsGW1T1_pFy87IYz48mAi1jA6ju_7suNR7okFKNXi5gF1LvmvY8KKGDxSv70V10/s320/WhatsApp%20Image%202026-05-24%20at%2011.52.14%20AM.jpeg", label: "Professional Certification 5" }
  ],

  // Google Script URL — replace with your deployed Google Apps Script URL
  googleScriptURL: "https://script.google.com/macros/s/YOUR_SCRIPT_ID/exec",

  // Telegram Bot — replace with your bot token and chat ID
  telegramBotToken: "YOUR_BOT_TOKEN",
  telegramChatId: "YOUR_CHAT_ID",

  // Google Map embed src — replace to change location
  googleMapSrc: "https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d233668.43779825457!2d90.27923583437499!3d23.780572800000015!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3755b8b087026b81%3A0x8fa563bbdd5904c2!2sDhaka!5e0!3m2!1sen!2sbd!4v1716550000000!5m2!1sen!2sbd"
};
</script>

<!-- ============================================================ NAVBAR ============================================================ -->
<nav id="navbar">
  <div class="container nav-inner">
    <a href="#hero" class="nav-logo">RKRatul<span></span></a>
    <ul class="nav-links">
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#certifications">Certificates</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
    <div class="nav-cta">
      <a href="mailto:redwanratul027@gmail.com" class="glow-btn btn-primary" style="padding:10px 24px;font-size:0.85rem">
        <i class="fa-solid fa-envelope"></i> Hire Me
      </a>
    </div>
    <div id="menu-toggle" onclick="openMobile()">
      <span></span><span></span><span></span>
    </div>
  </div>
</nav>

<!-- Mobile Menu -->
<div id="mobile-menu">
  <i class="fa-solid fa-xmark" id="mobile-close" onclick="closeMobile()"></i>
  <a href="#about" onclick="closeMobile()">About</a>
  <a href="#skills" onclick="closeMobile()">Skills</a>
  <a href="#portfolio" onclick="closeMobile()">Portfolio</a>
  <a href="#certifications" onclick="closeMobile()">Certificates</a>
  <a href="#contact" onclick="closeMobile()">Contact</a>
  <a href="mailto:redwanratul027@gmail.com" class="glow-btn btn-primary">
    <i class="fa-solid fa-envelope"></i> Hire Me
  </a>
</div>

<!-- ============================================================ HERO ============================================================ -->
<section id="hero">
  <div class="hero-bg"></div>
  <div class="hero-particles" id="hero-particles"></div>
  <div class="container">
    <div class="hero-inner">
      <div class="hero-text">
        <div class="hero-badge">
          <i class="fa-solid fa-circle-dot"></i>
          Available for Work
        </div>
        <h1 class="hero-name">
          Hello, I'm<br>
          <span class="line2" id="hero-name"></span>
        </h1>
        <div class="hero-roles">
          <span class="static">I am a </span>
          <span class="dynamic" id="typing-text"></span>
        </div>
        <p class="hero-desc" id="hero-tagline"></p>
        <div class="hero-actions">
          <a href="#portfolio" class="glow-btn btn-primary">
            <i class="fa-solid fa-briefcase"></i> View My Work
          </a>
          <a href="#contact" class="glow-btn btn-outline">
            <i class="fa-solid fa-paper-plane"></i> Get In Touch
          </a>
        </div>
        <div class="hero-socials" id="hero-socials"></div>
      </div>
      <div class="hero-image-wrap">
        <div class="hero-image-ring2"></div>
        <div class="hero-image-ring"></div>
        <div class="hero-image-blob"></div>
        <div class="hero-image-frame">
          <img id="hero-img" src="" alt="Redwan-ul Karim Ratul">
        </div>
        <div class="hero-stat-pill pill-top-left glass-card">
          <div class="icon" style="background:rgba(58,134,255,0.15)">
            <i class="fa-solid fa-briefcase" style="color:#3a86ff"></i>
          </div>
          <div>
            <div class="num" id="stat-projects"></div>
            <div class="lbl">Projects Done</div>
          </div>
        </div>
        <div class="hero-stat-pill pill-top-right glass-card">
          <div class="icon" style="background:rgba(6,214,160,0.15)">
            <i class="fa-solid fa-users" style="color:#06d6a0"></i>
          </div>
          <div>
            <div class="num" id="stat-clients"></div>
            <div class="lbl">Happy Clients</div>
          </div>
        </div>
        <div class="hero-stat-pill pill-bottom-right glass-card">
          <div class="icon" style="background:rgba(255,107,107,0.15)">
            <i class="fa-solid fa-star" style="color:#ff6b6b"></i>
          </div>
          <div>
            <div class="num" id="stat-exp"></div>
            <div class="lbl">Years Exp.</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============================================================ ABOUT ============================================================ -->
<section id="about">
  <div class="container">
    <div class="about-grid">
      <div class="about-image-wrap reveal">
        <div class="about-img-outer">
          <img id="about-img" src="" alt="About Redwan">
        </div>
        <div class="about-badge-float">
          <div class="num" id="about-exp-num"></div>
          <div class="lbl">Years of Experience</div>
        </div>
      </div>
      <div class="about-info">
        <div class="section-tag reveal"><i class="fa-solid fa-user"></i> About Me</div>
        <h2 class="section-title reveal">Crafting Financial <br><span class="gradient-text">Clarity from Data</span></h2>
        <div id="about-texts" class="reveal"></div>
        <div class="about-pills reveal" id="about-pills"></div>
        <div class="about-facts reveal">
          <div class="about-fact">
            <i class="fa-solid fa-phone"></i>
            <h4 id="fact-phone"></h4>
            <p>Phone Number</p>
          </div>
          <div class="about-fact">
            <i class="fa-solid fa-envelope"></i>
            <h4 id="fact-email"></h4>
            <p>Email Address</p>
          </div>
          <div class="about-fact">
            <i class="fa-solid fa-location-dot"></i>
            <h4 id="fact-location"></h4>
            <p>Location</p>
          </div>
          <div class="about-fact">
            <i class="fa-solid fa-circle-check" style="color:#06d6a0"></i>
            <h4>Available Now</h4>
            <p>Open for Projects</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============================================================ SKILLS ============================================================ -->
<section id="skills">
  <div class="container">
    <div class="section-header">
      <div class="section-tag reveal"><i class="fa-solid fa-code"></i> Expertise</div>
      <h2 class="section-title reveal">Skills & <span class="gradient-text">Specializations</span></h2>
      <p class="section-subtitle reveal" style="margin:0 auto">From raw numbers to refined narratives — my skill set covers every layer of accounting and data analytics.</p>
    </div>
    <div class="skills-grid" id="skills-grid"></div>
  </div>
</section>

<!-- ============================================================ PORTFOLIO ============================================================ -->
<section id="portfolio">
  <div class="container">
    <div class="section-header">
      <div class="section-tag reveal"><i class="fa-solid fa-folder-open"></i> Work</div>
      <h2 class="section-title reveal">Featured <span class="gradient-text">Projects</span></h2>
      <p class="section-subtitle reveal" style="margin:0 auto">A curated selection of my data analytics and accounting projects that delivered measurable impact.</p>
    </div>
    <div class="projects-grid" id="projects-grid"></div>
  </div>
</section>

<!-- ============================================================ CERTIFICATIONS ============================================================ -->
<section id="certifications">
  <div class="container">
    <div class="section-header">
      <div class="section-tag reveal"><i class="fa-solid fa-award"></i> Credentials</div>
      <h2 class="section-title reveal">Professional <span class="gradient-text">Certifications</span></h2>
      <p class="section-subtitle reveal" style="margin:0 auto">Industry-recognized certifications validating my expertise in accounting and data analytics.</p>
    </div>
    <div class="certs-grid" id="certs-grid"></div>
  </div>
</section>

<!-- ============================================================ EXPERIENCE TIMELINE ============================================================ -->
<section id="experience">
  <div class="container">
    <div class="section-header">
      <div class="section-tag reveal"><i class="fa-solid fa-timeline"></i> Journey</div>
      <h2 class="section-title reveal">Professional <span class="gradient-text">Experience</span></h2>
      <p class="section-subtitle reveal" style="margin:0 auto">3.5+ years of progressive growth across accounting, taxation, auditing, and data analytics.</p>
    </div>

    <!-- Professional Summary Card -->
    <div class="glass-card reveal" style="padding:40px;margin-bottom:64px;position:relative;overflow:hidden;">
      <div style="position:absolute;top:-40px;right:-40px;width:200px;height:200px;border-radius:50%;background:radial-gradient(circle,rgba(58,134,255,0.12),transparent 70%);pointer-events:none;"></div>
      <div style="position:absolute;bottom:-30px;left:-30px;width:150px;height:150px;border-radius:50%;background:radial-gradient(circle,rgba(6,214,160,0.08),transparent 70%);pointer-events:none;"></div>
      <div style="display:flex;align-items:flex-start;gap:20px;margin-bottom:28px;">
        <div style="flex-shrink:0;width:52px;height:52px;border-radius:14px;background:rgba(58,134,255,0.12);display:flex;align-items:center;justify-content:center;font-size:1.4rem;color:var(--primary);">
          <i class="fa-solid fa-id-badge"></i>
        </div>
        <div>
          <h3 style="font-family:var(--font-display);font-size:1.4rem;font-weight:700;margin-bottom:4px;">Professional Summary</h3>
          <span style="font-size:0.78rem;color:var(--primary);font-weight:600;letter-spacing:1.5px;text-transform:uppercase;">Chartered Accountant & Data Analyst</span>
        </div>
      </div>
      <p style="color:var(--text-secondary);line-height:1.9;font-size:0.97rem;margin-bottom:20px;">
        Chartered Accountant & Data-Driven Financial Professional with over <strong style="color:var(--text-primary);">3.5 years of progressive experience</strong> in financial accounting, taxation, auditing, and advanced data analytics. Currently associated with a reputed Chartered Accountancy Firm registered with the <strong style="color:var(--primary);">Institute of Chartered Accountants of Bangladesh (ICAB)</strong> since November 2022.
      </p>
      <p style="color:var(--text-secondary);line-height:1.9;font-size:0.97rem;margin-bottom:20px;">
        I specialize in preparing complete sets of financial statements, managing month-end and year-end closings, corporate and individual tax computations, VAT & direct tax compliance, regulatory reporting, and audit support. My expertise spans multiple industries including <strong style="color:var(--text-primary);">manufacturing, trading, services, and telecommunications</strong>.
      </p>
      <p style="color:var(--text-secondary);line-height:1.9;font-size:0.97rem;margin-bottom:32px;">
        Passionate about leveraging both accounting precision and modern data analytics, I transform complex financial data into actionable insights using <strong style="color:var(--text-primary);">predictive modeling, statistical analysis, and dynamic data visualization</strong>. This integrated approach helps businesses enhance decision-making, optimize performance, and achieve operational efficiency in dynamic environments.
      </p>
      <!-- Key Expertise Tags -->
      <div style="display:flex;flex-wrap:wrap;gap:10px;">
        <span style="font-size:0.78rem;font-weight:600;padding:6px 14px;border-radius:30px;background:rgba(58,134,255,0.1);border:1px solid rgba(58,134,255,0.25);color:var(--primary);"><i class="fa-solid fa-check-circle" style="margin-right:5px;"></i>Financial Statements</span>
        <span style="font-size:0.78rem;font-weight:600;padding:6px 14px;border-radius:30px;background:rgba(58,134,255,0.1);border:1px solid rgba(58,134,255,0.25);color:var(--primary);"><i class="fa-solid fa-check-circle" style="margin-right:5px;"></i>Corporate Tax & VAT</span>
        <span style="font-size:0.78rem;font-weight:600;padding:6px 14px;border-radius:30px;background:rgba(58,134,255,0.1);border:1px solid rgba(58,134,255,0.25);color:var(--primary);"><i class="fa-solid fa-check-circle" style="margin-right:5px;"></i>Audit Support</span>
        <span style="font-size:0.78rem;font-weight:600;padding:6px 14px;border-radius:30px;background:rgba(6,214,160,0.1);border:1px solid rgba(6,214,160,0.25);color:#06d6a0;"><i class="fa-solid fa-check-circle" style="margin-right:5px;"></i>Predictive Modeling</span>
        <span style="font-size:0.78rem;font-weight:600;padding:6px 14px;border-radius:30px;background:rgba(6,214,160,0.1);border:1px solid rgba(6,214,160,0.25);color:#06d6a0;"><i class="fa-solid fa-check-circle" style="margin-right:5px;"></i>Data Visualization</span>
        <span style="font-size:0.78rem;font-weight:600;padding:6px 14px;border-radius:30px;background:rgba(6,214,160,0.1);border:1px solid rgba(6,214,160,0.25);color:#06d6a0;"><i class="fa-solid fa-check-circle" style="margin-right:5px;"></i>Statistical Analysis</span>
        <span style="font-size:0.78rem;font-weight:600;padding:6px 14px;border-radius:30px;background:rgba(255,107,107,0.1);border:1px solid rgba(255,107,107,0.25);color:#ff6b6b;"><i class="fa-solid fa-check-circle" style="margin-right:5px;"></i>ICAB Registered</span>
        <span style="font-size:0.78rem;font-weight:600;padding:6px 14px;border-radius:30px;background:rgba(255,107,107,0.1);border:1px solid rgba(255,107,107,0.25);color:#ff6b6b;"><i class="fa-solid fa-check-circle" style="margin-right:5px;"></i>Regulatory Reporting</span>
      </div>
    </div>

    <!-- Industry Expertise Row -->
    <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:16px;margin-bottom:64px;">
      <div class="glass-card reveal reveal-delay-1" style="padding:24px;text-align:center;transition:var(--transition);" onmouseover="this.style.borderColor='rgba(58,134,255,0.4)';this.style.transform='translateY(-6px)'" onmouseout="this.style.borderColor='var(--glass-border)';this.style.transform='translateY(0)'">
        <div style="width:50px;height:50px;border-radius:12px;background:rgba(58,134,255,0.12);display:flex;align-items:center;justify-content:center;margin:0 auto 14px;font-size:1.3rem;color:var(--primary);"><i class="fa-solid fa-industry"></i></div>
        <h4 style="font-weight:700;margin-bottom:6px;">Manufacturing</h4>
        <p style="font-size:0.8rem;color:var(--text-secondary);">Cost accounting, inventory & production reporting</p>
      </div>
      <div class="glass-card reveal reveal-delay-2" style="padding:24px;text-align:center;transition:var(--transition);" onmouseover="this.style.borderColor='rgba(6,214,160,0.4)';this.style.transform='translateY(-6px)'" onmouseout="this.style.borderColor='var(--glass-border)';this.style.transform='translateY(0)'">
        <div style="width:50px;height:50px;border-radius:12px;background:rgba(6,214,160,0.12);display:flex;align-items:center;justify-content:center;margin:0 auto 14px;font-size:1.3rem;color:#06d6a0;"><i class="fa-solid fa-store"></i></div>
        <h4 style="font-weight:700;margin-bottom:6px;">Trading</h4>
        <p style="font-size:0.8rem;color:var(--text-secondary);">Revenue tracking, margin analysis & compliance</p>
      </div>
      <div class="glass-card reveal reveal-delay-3" style="padding:24px;text-align:center;transition:var(--transition);" onmouseover="this.style.borderColor='rgba(255,107,107,0.4)';this.style.transform='translateY(-6px)'" onmouseout="this.style.borderColor='var(--glass-border)';this.style.transform='translateY(0)'">
        <div style="width:50px;height:50px;border-radius:12px;background:rgba(255,107,107,0.12);display:flex;align-items:center;justify-content:center;margin:0 auto 14px;font-size:1.3rem;color:#ff6b6b;"><i class="fa-solid fa-briefcase"></i></div>
        <h4 style="font-weight:700;margin-bottom:6px;">Services</h4>
        <p style="font-size:0.8rem;color:var(--text-secondary);">Project-based accounting & service revenue recognition</p>
      </div>
      <div class="glass-card reveal reveal-delay-4" style="padding:24px;text-align:center;transition:var(--transition);" onmouseover="this.style.borderColor='rgba(247,183,49,0.4)';this.style.transform='translateY(-6px)'" onmouseout="this.style.borderColor='var(--glass-border)';this.style.transform='translateY(0)'">
        <div style="width:50px;height:50px;border-radius:12px;background:rgba(247,183,49,0.12);display:flex;align-items:center;justify-content:center;margin:0 auto 14px;font-size:1.3rem;color:#f7b731;"><i class="fa-solid fa-tower-broadcast"></i></div>
        <h4 style="font-weight:700;margin-bottom:6px;">Telecom</h4>
        <p style="font-size:0.8rem;color:var(--text-secondary);">Regulatory compliance & telecom financial reporting</p>
      </div>
    </div>

    <!-- Timeline -->
    <div class="timeline">
      <div class="timeline-item reveal">
        <div class="timeline-dot"><i class="fa-solid fa-building-columns"></i></div>
        <div class="timeline-content">
          <span class="period">November 2022 — Present</span>
          <h3>Article Student (CA Trainee)</h3>
          <div class="company">Chartered Accountancy Firm — ICAB Registered, Dhaka</div>
          <p>Currently completing articleship training at an ICAB-registered CA firm, gaining hands-on experience in statutory auditing, financial statement preparation, tax assessments, and client advisory across manufacturing, trading, services, and telecommunications industries.</p>
        </div>
      </div>
      <div class="timeline-item reveal">
        <div class="timeline-dot"><i class="fa-solid fa-file-invoice-dollar"></i></div>
        <div class="timeline-content">
          <span class="period">2022 — Present</span>
          <h3>Tax, VAT & Regulatory Compliance</h3>
          <div class="company">CA Firm Practice, Dhaka</div>
          <p>Handling corporate and individual income tax computations, VAT return filings, direct tax compliance, regulatory submissions, and supporting clients through tax audits and assessments in compliance with Bangladesh tax laws.</p>
        </div>
      </div>
      <div class="timeline-item reveal">
        <div class="timeline-dot"><i class="fa-solid fa-chart-line"></i></div>
        <div class="timeline-content">
          <span class="period">2023 — Present</span>
          <h3>Data Analytics & Financial Intelligence</h3>
          <div class="company">Integrated Practice — Analytics + Accounting</div>
          <p>Leveraging advanced data analytics alongside accounting expertise — building predictive models, financial dashboards, and statistical reports that transform raw financial data into strategic business insights for decision-makers.</p>
        </div>
      </div>
      <div class="timeline-item reveal">
        <div class="timeline-dot"><i class="fa-solid fa-graduation-cap"></i></div>
        <div class="timeline-content">
          <span class="period">Pre-2022</span>
          <h3>Foundation in Accounting & Finance</h3>
          <div class="company">Academic & Early Career</div>
          <p>Built a strong foundation in financial accounting principles, ledger management, bank reconciliation, and data entry operations — the bedrock that supports today's complex financial and analytical work.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============================================================ CONTACT ============================================================ -->
<section id="contact">
  <div class="container">
    <div class="section-header">
      <div class="section-tag reveal"><i class="fa-solid fa-paper-plane"></i> Contact</div>
      <h2 class="section-title reveal">Let's Work <span class="gradient-text">Together</span></h2>
      <p class="section-subtitle reveal" style="margin:0 auto">Have a project in mind? I'd love to hear from you. Send a message and I'll get back within 24 hours.</p>
    </div>
    <div class="contact-grid">
      <div class="reveal">
        <h3 style="font-size:1.4rem;font-weight:700;margin-bottom:12px">Get in Touch</h3>
        <p style="color:var(--text-secondary);font-size:0.95rem;line-height:1.75">
          Whether you need financial clarity, data-driven insights, or a complete analytics solution — I'm here to help you make smarter decisions.
        </p>
        <div class="contact-info-items">
          <div class="contact-item">
            <div class="icon"><i class="fa-solid fa-phone"></i></div>
            <div class="detail">
              <span>Phone</span>
              <strong id="contact-phone"></strong>
            </div>
          </div>
          <div class="contact-item">
            <div class="icon"><i class="fa-solid fa-envelope"></i></div>
            <div class="detail">
              <span>Email</span>
              <strong id="contact-email"></strong>
            </div>
          </div>
          <div class="contact-item">
            <div class="icon"><i class="fa-solid fa-location-dot"></i></div>
            <div class="detail">
              <span>Location</span>
              <strong id="contact-location"></strong>
            </div>
          </div>
        </div>
      </div>
      <div class="glass-card reveal" style="padding:36px">
        <div class="contact-form" id="contact-form">
          <div class="form-row">
            <div class="form-group">
              <label for="f-name"><i class="fa-solid fa-user" style="margin-right:6px"></i>Full Name</label>
              <input type="text" id="f-name" placeholder="Your full name" required>
            </div>
            <div class="form-group">
              <label for="f-phone"><i class="fa-solid fa-phone" style="margin-right:6px"></i>Phone</label>
              <input type="tel" id="f-phone" placeholder="Your phone number">
            </div>
          </div>
          <div class="form-group">
            <label for="f-email"><i class="fa-solid fa-envelope" style="margin-right:6px"></i>Email Address</label>
            <input type="email" id="f-email" placeholder="your@email.com" required>
          </div>
          <div class="form-group">
            <label for="f-msg"><i class="fa-solid fa-message" style="margin-right:6px"></i>Message</label>
            <textarea id="f-msg" rows="5" placeholder="Tell me about your project or inquiry..." required></textarea>
          </div>
          <div id="form-status"></div>
          <button class="glow-btn btn-primary" style="width:100%;justify-content:center;padding:16px" onclick="submitForm()">
            <i class="fa-solid fa-paper-plane"></i> Send Message
          </button>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============================================================ MAP ============================================================ -->
<div id="map-section">
  <div class="map-wrap">
    <iframe id="map-iframe" src="" allowfullscreen="" loading="lazy"></iframe>
  </div>
</div>

<!-- ============================================================ FOOTER ============================================================ -->
<footer>
  <div class="container">
    <div class="footer-inner">
      <div class="nav-logo" style="font-family:'Playfair Display',serif;font-size:1.4rem">RKRatul<span style="display:inline-block;width:8px;height:8px;border-radius:50%;background:#3a86ff;margin-left:3px;vertical-align:super"></span></div>
      <div class="footer-links">
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#contact">Contact</a>
      </div>
      <div class="hero-socials" id="footer-socials"></div>
    </div>
    <div class="footer-copy" id="footer-copy"></div>
  </div>
</footer>

<!-- Back to Top -->
<button id="back-top" onclick="window.scrollTo({top:0,behavior:'smooth'})" title="Back to Top">
  <i class="fa-solid fa-chevron-up"></i>
</button>

<!-- Modal for Certs -->
<div id="modal-overlay" onclick="closeModal()">
  <span id="modal-close">&times;</span>
  <img id="modal-img" src="" alt="Certificate">
</div>

<!-- ============================================================ SCRIPTS ============================================================ -->
<script>
/* ============================================================
   BUILD PAGE FROM SITE_DATA
   ============================================================ */
function buildPage() {
  const d = SITE_DATA;

  // Hero
  document.getElementById('hero-name').textContent = d.name;
  document.getElementById('hero-tagline').textContent = d.tagline;
  document.getElementById('hero-img').src = d.profileImage;
  document.getElementById('about-img').src = d.profileImage;
  document.getElementById('stat-projects').textContent = d.projectsDone;
  document.getElementById('stat-clients').textContent = d.clientsServed;
  document.getElementById('stat-exp').textContent = d.yearsExp;

  // Social icons
  const socials = [
    { key: 'facebook', icon: 'fa-brands fa-facebook-f' },
    { key: 'linkedin', icon: 'fa-brands fa-linkedin-in' },
    { key: 'instagram', icon: 'fa-brands fa-instagram' }
  ];
  ['hero-socials','footer-socials'].forEach(id => {
    const el = document.getElementById(id);
    el.innerHTML = socials.map(s =>
      d.social[s.key] ? `<a href="${d.social[s.key]}" target="_blank" rel="noopener" aria-label="${s.key}"><i class="${s.icon}"></i></a>` : ''
    ).join('');
  });

  // About
  document.getElementById('about-exp-num').textContent = d.yearsExp;
  const aboutTexts = document.getElementById('about-texts');
  aboutTexts.innerHTML = d.aboutText.map(t => `<p>${t}</p>`).join('');
  const pills = ['ICAB Registered','Tax & VAT Compliance','Audit Support','Financial Statements','Bookkeeping','Data Analytics','Power BI','Predictive Modeling','Cloud Accounting','Regulatory Reporting'];
  document.getElementById('about-pills').innerHTML = pills.map(p => `<span class="about-pill">${p}</span>`).join('');
  document.getElementById('fact-phone').textContent = d.phone;
  document.getElementById('fact-email').textContent = d.email;
  document.getElementById('fact-location').textContent = d.location;

  // Contact
  document.getElementById('contact-phone').textContent = d.phone;
  document.getElementById('contact-email').textContent = d.email;
  document.getElementById('contact-location').textContent = d.location;

  // Skills
  const sg = document.getElementById('skills-grid');
  sg.innerHTML = d.skills.map((s,i) => `
    <div class="skill-card reveal reveal-delay-${(i%4)+1}">
      <div class="skill-icon" style="background:${s.bg}; color:${s.color}">
        <i class="${s.icon}"></i>
      </div>
      <h3>${s.title}</h3>
      <ul class="skill-list">
        ${s.items.map(item => `<li>${item}</li>`).join('')}
      </ul>
    </div>
  `).join('');

  // Projects
  const pg = document.getElementById('projects-grid');
  pg.innerHTML = d.projects.map((p,i) => `
    <div class="project-card reveal reveal-delay-${(i%3)+1}">
      <div class="project-img">
        <img src="${p.image}" alt="${p.title}" loading="lazy">
        <div class="project-overlay">
          <div class="project-overlay-btns">
            <a href="${p.previewLink}" class="project-overlay-btn" style="background:var(--primary);color:#fff" target="_blank">
              <i class="fa-solid fa-eye"></i> Preview
            </a>
            <a href="#contact" class="project-overlay-btn" style="background:rgba(255,255,255,0.1);color:#fff;border:1px solid rgba(255,255,255,0.2)">
              <i class="fa-solid fa-info-circle"></i> Details
            </a>
          </div>
        </div>
      </div>
      <div class="project-body">
        <span class="project-tag">${p.tag}</span>
        <h3>${p.title}</h3>
        <p>${p.desc}</p>
      </div>
    </div>
  `).join('');

  // Certifications
  const cg = document.getElementById('certs-grid');
  cg.innerHTML = d.certifications.map((c,i) => `
    <div class="cert-card reveal reveal-delay-${(i%5)+1}" onclick="openModal('${c.img}')">
      <img src="${c.img}" alt="${c.label}" loading="lazy">
      <div class="cert-badge-icon"><i class="fa-solid fa-certificate"></i></div>
      <div class="cert-label">${c.label}</div>
    </div>
  `).join('');

  // Map
  document.getElementById('map-iframe').src = d.googleMapSrc;

  // Footer
  document.getElementById('footer-copy').innerHTML =
    `&copy; ${new Date().getFullYear()} ${d.name}. All rights reserved. Built with <i class="fa-solid fa-heart" style="color:#ff6b6b"></i> in Dhaka, Bangladesh.`;
}

/* ============================================================
   TYPING EFFECT
   ============================================================ */
function initTyping() {
  const roles = SITE_DATA.roles;
  const el = document.getElementById('typing-text');
  let ri = 0, ci = 0, deleting = false;

  function type() {
    const current = roles[ri];
    if (deleting) {
      el.textContent = current.substring(0, ci--);
      if (ci < 0) { deleting = false; ri = (ri + 1) % roles.length; setTimeout(type, 500); return; }
    } else {
      el.textContent = current.substring(0, ci++);
      if (ci > current.length) { deleting = true; setTimeout(type, 1800); return; }
    }
    setTimeout(type, deleting ? 60 : 90);
  }
  type();
}

/* ============================================================
   HERO PARTICLES
   ============================================================ */
function createParticles() {
  const container = document.getElementById('hero-particles');
  for (let i = 0; i < 18; i++) {
    const s = document.createElement('span');
    const size = Math.random() * 6 + 3;
    s.style.cssText = `
      width:${size}px; height:${size}px;
      left:${Math.random()*100}%;
      animation-duration:${Math.random()*15+10}s;
      animation-delay:${Math.random()*10}s;
    `;
    container.appendChild(s);
  }
}

/* ============================================================
   SCROLL REVEAL
   ============================================================ */
function initScrollReveal() {
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(e => { if (e.isIntersecting) { e.target.classList.add('visible'); observer.unobserve(e.target); } });
  }, { threshold: 0.12 });
  document.querySelectorAll('.reveal').forEach(el => observer.observe(el));
}

/* ============================================================
   NAVBAR SCROLL
   ============================================================ */
window.addEventListener('scroll', () => {
  const nav = document.getElementById('navbar');
  const bt = document.getElementById('back-top');
  if (window.scrollY > 80) { nav.classList.add('scrolled'); } else { nav.classList.remove('scrolled'); }
  if (window.scrollY > 400) { bt.classList.add('show'); } else { bt.classList.remove('show'); }

  // Active nav link
  const sections = ['about','skills','portfolio','certifications','experience','contact'];
  let current = '';
  sections.forEach(id => {
    const s = document.getElementById(id);
    if (s && window.scrollY >= s.offsetTop - 120) current = id;
  });
  document.querySelectorAll('.nav-links a').forEach(a => {
    a.classList.toggle('active', a.getAttribute('href') === '#' + current);
  });
});

/* ============================================================
   MOBILE MENU
   ============================================================ */
function openMobile() { document.getElementById('mobile-menu').classList.add('open'); document.body.style.overflow='hidden'; }
function closeMobile() { document.getElementById('mobile-menu').classList.remove('open'); document.body.style.overflow=''; }

/* ============================================================
   MODAL
   ============================================================ */
function openModal(src) {
  document.getElementById('modal-img').src = src;
  document.getElementById('modal-overlay').classList.add('open');
  document.body.style.overflow = 'hidden';
}
function closeModal() {
  document.getElementById('modal-overlay').classList.remove('open');
  document.body.style.overflow = '';
}

/* ============================================================
   CONTACT FORM
   ============================================================ */
async function submitForm() {
  const name = document.getElementById('f-name').value.trim();
  const phone = document.getElementById('f-phone').value.trim();
  const email = document.getElementById('f-email').value.trim();
  const msg = document.getElementById('f-msg').value.trim();
  const status = document.getElementById('form-status');

  if (!name || !email || !msg) {
    showStatus('error', '<i class="fa-solid fa-circle-exclamation"></i> Please fill in all required fields.');
    return;
  }

  const btn = document.querySelector('#contact-form button');
  btn.innerHTML = '<i class="fa-solid fa-spinner fa-spin"></i> Sending...';
  btn.disabled = true;

  const payload = { name, phone, email, message: msg, timestamp: new Date().toLocaleString() };

  // 1. Google Sheet via Apps Script
  const gsFetch = fetch(SITE_DATA.googleScriptURL, {
    method: 'POST',
    mode: 'no-cors',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(payload)
  }).catch(() => {});

  // 2. Telegram Bot
  const tgText = `📬 *New Contact Message*\n\n👤 *Name:* ${name}\n📞 *Phone:* ${phone || 'N/A'}\n📧 *Email:* ${email}\n💬 *Message:* ${msg}\n🕐 *Time:* ${payload.timestamp}`;
  const tgFetch = fetch(`https://api.telegram.org/bot${SITE_DATA.telegramBotToken}/sendMessage`, {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ chat_id: SITE_DATA.telegramChatId, text: tgText, parse_mode: 'Markdown' })
  }).catch(() => {});

  await Promise.allSettled([gsFetch, tgFetch]);

  showStatus('success', '<i class="fa-solid fa-circle-check"></i> Message sent successfully! I\'ll respond within 24 hours.');
  document.getElementById('f-name').value = '';
  document.getElementById('f-phone').value = '';
  document.getElementById('f-email').value = '';
  document.getElementById('f-msg').value = '';
  btn.innerHTML = '<i class="fa-solid fa-paper-plane"></i> Send Message';
  btn.disabled = false;
}

function showStatus(type, html) {
  const el = document.getElementById('form-status');
  el.className = type; el.innerHTML = html; el.style.display = 'block';
  setTimeout(() => { el.style.display = 'none'; }, 5000);
}

/* ============================================================
   INIT
   ============================================================ */
document.addEventListener('DOMContentLoaded', () => {
  buildPage();
  initTyping();
  createParticles();
  setTimeout(initScrollReveal, 100);
});
</script>
</body>
</html>
