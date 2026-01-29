/* ===========================
   VARIABILI E RESET GLOBALI
   =========================== */

:root {
  /* Colori */
  --primary: #3b82f6;
  --secondary: #1e40af;
  --accent: #06b6d4;
  --dark: #0f172a;
  --darker: #050f1f;
  --light: #f8fafc;
  --lighter: #e2e8f0;
  --text: #1e293b;
  --text-light: #64748b;
  --border: #e2e8f0;
  --success: #10b981;
  --danger: #ef4444;

  /* Spacing */
  --space-xs: 0.5rem;
  --space-sm: 1rem;
  --space-md: 1.5rem;
  --space-lg: 2rem;
  --space-xl: 3rem;
  --space-2xl: 4rem;

  /* Border Radius */
  --radius-sm: 0.375rem;
  --radius-md: 0.5rem;
  --radius-lg: 1rem;
  --radius-xl: 1.5rem;
  --radius-full: 9999px;

  /* Typography */
  --font-sans: 'Poppins', sans-serif;
  --font-mono: 'JetBrains Mono', monospace;

  /* Shadows */
  --shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
  --shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
  --shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1);

  /* Transitions */
  --transition: 300ms cubic-bezier(0.4, 0, 0.2, 1);
}

/* Dark Mode */
html.dark-mode {
  --primary: #60a5fa;
  --secondary: #3b82f6;
  --accent: #22d3ee;
  --dark: #030712;
  --darker: #0a0f1e;
  --light: #1e293b;
  --lighter: #334155;
  --text: #f1f5f9;
  --text-light: #cbd5e1;
  --border: #334155;
}

/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: var(--font-sans);
  color: var(--text);
  background-color: var(--light);
  line-height: 1.6;
  transition: background-color var(--transition), color var(--transition);
}

/* ===========================
   TIPOGRAFIA
   =========================== */

h1, h2, h3, h4, h5, h6 {
  font-weight: 700;
  line-height: 1.2;
}

h1 { font-size: 3.5rem; }
h2 { font-size: 2.5rem; }
h3 { font-size: 1.75rem; }
h4 { font-size: 1.25rem; }

p {
  margin-bottom: 1rem;
  color: var(--text-light);
}

a {
  color: var(--primary);
  text-decoration: none;
  transition: color var(--transition);
}

a:hover {
  color: var(--secondary);
}

/* ===========================
   CONTAINER E LAYOUT
   =========================== */

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 var(--space-lg);
}

main {
  overflow: hidden;
}

/* ===========================
   NAVBAR
   =========================== */

.navbar {
  position: fixed;
  top: 0;
  width: 100%;
  background: rgba(248, 250, 252, 0.8);
  backdrop-filter: blur(10px);
  border-bottom: 1px solid var(--border);
  z-index: 1000;
  transition: all var(--transition);
}

html.dark-mode .navbar {
  background: rgba(15, 23, 42, 0.8);
}

.navbar:hover {
  background: rgba(248, 250, 252, 0.95);
  border-bottom-color: var(--primary);
}

html.dark-mode .navbar:hover {
  background: rgba(15, 23, 42, 0.95);
}

.nav-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 1rem var(--space-lg);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5rem;
  font-weight: 800;
  display: flex;
  gap: 0.25rem;
  color: var(--text);
  transition: transform var(--transition);
}

.logo-bracket {
  color: var(--primary);
}

.logo:hover {
  transform: scale(1.05);
}

.nav-links {
  display: flex;
  gap: var(--space-lg);
  list-style: none;
}

.nav-link {
  color: var(--text);
  font-weight: 500;
  position: relative;
  transition: color var(--transition);
}

.nav-link::after {
  content: '';
  position: absolute;
  bottom: -0.5rem;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--primary);
  transition: width var(--transition);
}

.nav-link:hover {
  color: var(--primary);
}

.nav-link:hover::after {
  width: 100%;
}

.nav-actions {
  display: flex;
  gap: var(--space-md);
  align-items: center;
}

.theme-btn {
  background: var(--primary);
  color: white;
  border: none;
  padding: 0.5rem 1rem;
  border-radius: var(--radius-lg);
  font-size: 1rem;
  cursor: pointer;
  transition: all var(--transition);
  display: flex;
  align-items: center;
  justify-content: center;
}

.theme-btn:hover {
  transform: scale(1.1) rotate(20deg);
  background: var(--secondary);
}

.menu-btn {
  display: none;
  background: none;
  border: none;
  flex-direction: column;
  gap: 0.35rem;
  cursor: pointer;
}

.menu-btn span {
  width: 1.5rem;
  height: 3px;
  background: var(--text);
  border-radius: var(--radius-sm);
  transition: all var(--transition);
}

.menu-btn.active span:nth-child(1) {
  transform: rotate(45deg) translate(0.5rem, 0.8rem);
}

.menu-btn.active span:nth-child(2) {
  opacity: 0;
}

.menu-btn.active span:nth-child(3) {
  transform: rotate(-45deg) translate(0.3rem, -0.8rem);
}

.mobile-menu {
  display: none;
  position: fixed;
  top: 70px;
  left: 0;
  right: 0;
  background: var(--light);
  border-bottom: 1px solid var(--border);
  padding: var(--space-lg);
  z-index: 999;
}

.mobile-menu.active {
  display: flex;
  flex-direction: column;
  gap: var(--space-md);
}

.mobile-link {
  color: var(--text);
  font-weight: 500;
  transition: color var(--transition);
}

.mobile-link:hover {
  color: var(--primary);
}

/* ===========================
   HERO SECTION
   =========================== */

.hero {
  min-height: 100vh;
  padding-top: 100px;
  background: linear-gradient(135deg, var(--light) 0%, rgba(59, 130, 246, 0.05) 100%);
  position: relative;
  overflow: hidden;
  display: flex;
  align-items: center;
}

html.dark-mode .hero {
  background: linear-gradient(135deg, var(--dark) 0%, rgba(96, 165, 250, 0.05) 100%);
}

.stars {
  position: absolute;
  width: 100%;
  height: 100%;
  pointer-events: none;
}

.stars::before,
.stars::after {
  content: '';
  position: absolute;
  border-radius: 50%;
  background: var(--primary);
  opacity: 0.1;
}

.stars::before {
  width: 300px;
  height: 300px;
  top: -50px;
  right: -50px;
  animation: float 6s ease-in-out infinite;
}

.stars::after {
  width: 200px;
  height: 200px;
  bottom: -30px;
  left: -30px;
  animation: float 8s ease-in-out infinite reverse;
}

@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-30px); }
}

.hero .container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: var(--space-2xl);
  align-items: center;
  position: relative;
  z-index: 1;
}

.hero-content {
  animation: slideInLeft 0.8s ease-out;
}

.hero-badge {
  display: inline-block;
  background: rgba(59, 130, 246, 0.1);
  color: var(--primary);
  padding: 0.5rem 1rem;
  border-radius: var(--radius-full);
  font-size: 0.875rem;
  font-weight: 600;
  margin-bottom: var(--space-md);
}

.hero-title {
  font-size: 3.5rem;
  font-weight: 800;
  line-height: 1.1;
  margin-bottom: var(--space-lg);
  color: var(--text);
}

.gradient-text {
  background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.hero-subtitle {
  font-size: 1.25rem;
  color: var(--text-light);
  margin-bottom: var(--space-lg);
  line-height: 1.8;
}

.hero-cta {
  display: flex;
  gap: var(--space-md);
  margin-bottom: var(--space-xl);
  flex-wrap: wrap;
}

.hero-socials {
  display: flex;
  gap: var(--space-md);
}

.social-link {
  width: 3rem;
  height: 3rem;
  border-radius: var(--radius-lg);
  background: rgba(59, 130, 246, 0.1);
  color: var(--primary);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.25rem;
  transition: all var(--transition);
}

.social-link:hover {
  background: var(--primary);
  color: white;
  transform: translateY(-5px);
}

.hero-visual {
  position: relative;
  animation: slideInRight 0.8s ease-out;
}

.code-window {
  background: var(--text);
  border-radius: var(--radius-lg);
  overflow: hidden;
  box-shadow: var(--shadow-xl);
}

.window-header {
  display: flex;
  gap: 0.5rem;
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
}

.window-header span {
  width: 0.75rem;
  height: 0.75rem;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.3);
}

.window-content {
  padding: var(--space-lg);
  font-family: var(--font-mono);
  font-size: 0.875rem;
  color: #4ade80;
  background: #1a1a1a;
  overflow-x: auto;
}

.code-tag { color: #60a5fa; }
.code-attr { color: #f59e0b; }
.code-string { color: #34d399; }

@keyframes slideInLeft {
  from {
    opacity: 0;
    transform: translateX(-50px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slideInRight {
  from {
    opacity: 0;
    transform: translateX(50px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

/* ===========================
   BUTTONS
   =========================== */

.btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 1rem 2rem;
  border-radius: var(--radius-lg);
  font-weight: 600;
  border: none;
  cursor: pointer;
  transition: all var(--transition);
  font-size: 1rem;
}

.btn-primary {
  background: var(--primary);
  color: white;
}

.btn-primary:hover {
  background: var(--secondary);
  transform: translateY(-3px);
  box-shadow: var(--shadow-lg);
}

.btn-secondary {
  background: transparent;
  color: var(--primary);
  border: 2px solid var(--primary);
}

.btn-secondary:hover {
  background: var(--primary);
  color: white;
}

.btn-large {
  padding: 1.5rem 3rem;
  font-size: 1.125rem;
}

/* ===========================
   SEZIONI GENERICHE
   =========================== */

section {
  padding: 100px 0;
}

.section-title {
  text-align: center;
  margin-bottom: 4rem;
  position: relative;
  font-size: 2.5rem;
  font-weight: 800;
}

.section-title::after {
  content: '';
  position: absolute;
  bottom: -1rem;
  left: 50%;
  transform: translateX(-50%);
  width: 60px;
  height: 4px;
  background: linear-gradient(90deg, var(--primary), var(--accent));
  border-radius: var(--radius-full);
}

/* ===========================
   ABOUT SECTION
   =========================== */

.about {
  background: var(--light);
}

html.dark-mode .about {
  background: var(--dark);
}

.about-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: var(--space-2xl);
  align-items: center;
}

.about-text p {
  margin-bottom: var(--space-lg);
  font-size: 1.0625rem;
  line-height: 1.8;
}

.about-highlights {
  display: flex;
  flex-direction: column;
  gap: var(--space-md);
  margin-top: var(--space-xl);
}

.highlight-item {
  display: flex;
  align-items: center;
  gap: var(--space-md);
  font-weight: 500;
}

.highlight-item i {
  color: var(--success);
  font-size: 1.25rem;
}

.about-stats {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: var(--space-lg);
}

.stat-card {
  padding: var(--space-lg);
  background: white;
  border-radius: var(--radius-lg);
  text-align: center;
  transition: all var(--transition);
  border: 1px solid var(--border);
}

html.dark-mode .stat-card {
  background: var(--darker);
  border-color: var(--lighter);
}

.stat-card:hover {
  transform: translateY(-10px);
  box-shadow: var(--shadow-lg);
  border-color: var(--primary);
}

.stat-card h3 {
  font-size: 2.5rem;
  color: var(--primary);
  margin-bottom: 0.5rem;
}

.stat-card p {
  color: var(--text-light);
  font-size: 0.875rem;
  margin: 0;
}

/* ===========================
   SKILLS SECTION
   =========================== */

.skills {
  background: var(--light);
}

html.dark-mode .skills {
  background: var(--dark);
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: var(--space-xl);
}

.skill-category {
  padding: var(--space-lg);
  background: white;
  border-radius: var(--radius-lg);
  border: 1px solid var(--border);
  transition: all var(--transition);
}

html.dark-mode .skill-category {
  background: var(--darker);
  border-color: var(--lighter);
}

.skill-category:hover {
  transform: translateY(-10px);
  box-shadow: var(--shadow-lg);
  border-color: var(--primary);
}

.skill-category h3 {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  margin-bottom: var(--space-md);
  color: var(--primary);
}

.skill-category i {
  font-size: 1.5rem;
}

.skill-tags {
  display: flex;
  flex-wrap: wrap;
  gap: var(--space-sm);
}

.skill-tag {
  background: rgba(59, 130, 246, 0.1);
  color: var(--primary);
  padding: 0.5rem 1rem;
  border-radius: var(--radius-full);
  font-size: 0.875rem;
  font-weight: 500;
  transition: all var(--transition);
}

.skill-tag:hover {
  background: var(--primary);
  color: white;
}

/* ===========================
   PROJECTS SECTION
   =========================== */

.projects {
  background: var(--light);
}

html.dark-mode .projects {
  background: var(--dark);
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: var(--space-xl);
}

.project-card {
  background: white;
  border-radius: var(--radius-lg);
  overflow: hidden;
  border: 1px solid var(--border);
  transition: all var(--transition);
}

html.dark-mode .project-card {
  background: var(--darker);
  border-color: var(--lighter);
}

.project-card:hover {
  transform: translateY(-10px);
  box-shadow: var(--shadow-lg);
  border-color: var(--primary);
}

.project-image {
  height: 200px;
  background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 3rem;
  color: rgba(255, 255, 255, 0.3);
}

.project-content {
  padding: var(--space-lg);
}

.project-content h3 {
  margin-bottom: var(--space-md);
}

.project-content p {
  margin-bottom: var(--space-md);
  font-size: 0.9375rem;
}

.project-tech {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: var(--space-md);
}

.project-tech span {
  background: rgba(59, 130, 246, 0.1);
  color: var(--primary);
  padding: 0.25rem 0.75rem;
  border-radius: var(--radius-full);
  font-size: 0.8125rem;
  font-weight: 500;
}

.project-link {
  color: var(--primary);
  font-weight: 600;
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  transition: all var(--transition);
}

.project-link:hover {
  gap: 1rem;
}

/* ===========================
   EXPERIENCE SECTION
   =========================== */

.experience {
  background: var(--light);
}

html.dark-mode .experience {
  background: var(--dark);
}

.timeline {
  max-width: 800px;
  margin: 0 auto;
}

.timeline-item {
  display: grid;
  grid-template-columns: 200px 1fr;
  gap: var(--space-lg);
  margin-bottom: var(--space-2xl);
  padding-bottom: var(--space-2xl);
  border-bottom: 1px solid var(--border);
}

.timeline-item:last-child {
  border-bottom: none;
}

.timeline-date {
  font-weight: 700;
  color: var(--primary);
  font-size: 1rem;
}

.timeline-content h3 {
  margin-bottom: 0.5rem;
}

.location {
  color: var(--accent);
  font-size: 0.9375rem;
  font-weight: 600;
  margin-bottom: 0.75rem;
}

/* ===========================
   CONTACT SECTION
   =========================== */

.contact {
  background: var(--light);
}

html.dark-mode .contact {
  background: var(--dark);
}

.contact-content {
  max-width: 600px;
  margin: 0 auto;
  text-align: center;
}

.contact-info h3 {
  margin-bottom: var(--space-md);
}

.contact-info > p {
  font-size: 1.1rem;
  margin-bottom: var(--space-xl);
}

.contact-methods {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: var(--space-lg);
  margin-bottom: var(--space-2xl);
}

.contact-method {
  padding: var(--space-lg);
  background: white;
  border-radius: var(--radius-lg);
  border: 1px solid var(--border);
  transition: all var(--transition);
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

html.dark-mode .contact-method {
  background: var(--darker);
  border-color: var(--lighter);
}

.contact-method:hover {
  transform: translateY(-5px);
  border-color: var(--primary);
}

.contact-method i {
  font-size: 2rem;
  color: var(--primary);
  margin-bottom: 0.75rem;
}

.contact-method span {
  color: var(--text-light);
  font-size: 0.9375rem;
}

.contact-cta {
  margin-top: var(--space-xl);
}

/* ===========================
   FOOTER
   =========================== */

.footer {
  background: var(--text);
  color: white;
  padding: var(--space-2xl) 0;
  text-align: center;
}

html.dark-mode .footer {
  background: var(--darker);
}

.footer p {
  color: inherit;
  margin: 0;
}

.footer i {
  color: var(--danger);
}

/* ===========================
   RESPONSIVE
   =========================== */

@media (max-width: 768px) {
  .nav-links {
    display: none;
  }

  .menu-btn {
    display: flex;
  }

  .hero .container {
    grid-template-columns: 1fr;
  }

  .hero-title {
    font-size: 2.5rem;
  }

  .about-grid,
  .about-stats {
    grid-template-columns: 1fr;
  }

  .timeline-item {
    grid-template-columns: 1fr;
  }

  .contact-methods {
    grid-template-columns: 1fr;
  }

  .projects-grid {
    grid-template-columns: 1fr;
  }

  .hero-visual {
    margin-top: var(--space-xl);
  }

  .hero-cta {
    flex-direction: column;
  }

  .btn {
    width: 100%;
    justify-content: center;
  }
}

@media (max-width: 480px) {
  .hero-title {
    font-size: 2rem;
  }

  .section-title {
    font-size: 1.75rem;
  }

  h1 { font-size: 2rem; }
  h2 { font-size: 1.5rem; }
  h3 { font-size: 1.25rem; }

  section {
    padding: 60px 0;
  }

  .container {
    padding: 0 var(--space-md);
  }

  .stat-card h3 {
    font-size: 2rem;
  }

  .nav-container {
    padding: 1rem var(--space-md);
  }

  .mobile-menu {
    padding: var(--space-md);
  }
}
