// ==================================
// PORTFOLIO - ADVANCED INTERACTIONS
// ==================================

document.addEventListener('DOMContentLoaded', () => {
  console.log('🚀 Portfolio Loading...');

  // ===== THEME TOGGLE =====
  const initTheme = () => {
    const themeBtn = document.getElementById('themeBtn');
    const htmlElement = document.documentElement;
    const icon = themeBtn.querySelector('i');

    // Controlla tema salvato o preferenza di sistema
    const savedTheme = localStorage.getItem('theme');
    const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
    const isDarkMode = savedTheme ? savedTheme === 'dark' : prefersDark;

    if (isDarkMode) {
      htmlElement.classList.add('dark-mode');
      icon.classList.remove('fa-moon');
      icon.classList.add('fa-sun');
    }

    // Toggle tema
    themeBtn.addEventListener('click', () => {
      const isNowDark = htmlElement.classList.toggle('dark-mode');
      localStorage.setItem('theme', isNowDark ? 'dark' : 'light');

      if (isNowDark) {
        icon.classList.remove('fa-moon');
        icon.classList.add('fa-sun');
      } else {
        icon.classList.remove('fa-sun');
        icon.classList.add('fa-moon');
      }

      icon.style.animation = 'spin 0.6s ease-in-out';
      setTimeout(() => {
        icon.style.animation = '';
      }, 600);
    });

    // Ascolta cambiamenti di sistema
    window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', (e) => {
      if (!localStorage.getItem('theme')) {
        if (e.matches) {
          htmlElement.classList.add('dark-mode');
          icon.classList.remove('fa-moon');
          icon.classList.add('fa-sun');
        } else {
          htmlElement.classList.remove('dark-mode');
          icon.classList.remove('fa-sun');
          icon.classList.add('fa-moon');
        }
      }
    });
  };

  // ===== MOBILE MENU =====
  const initMobileMenu = () => {
    const menuBtn = document.getElementById('menuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    const mobileLinks = document.querySelectorAll('.mobile-link');

    menuBtn.addEventListener('click', () => {
      menuBtn.classList.toggle('active');
      mobileMenu.classList.toggle('active');
    });

    mobileLinks.forEach((link) => {
      link.addEventListener('click', () => {
        menuBtn.classList.remove('active');
        mobileMenu.classList.remove('active');
      });
    });

    document.addEventListener('click', (e) => {
      if (!e.target.closest('.navbar') && mobileMenu.classList.contains('active')) {
        menuBtn.classList.remove('active');
        mobileMenu.classList.remove('active');
      }
    });
  };

  // ===== SMOOTH SCROLL =====
  const initSmoothScroll = () => {
    document.querySelectorAll('a[href^="#"]').forEach((anchor) => {
      anchor.addEventListener('click', (e) => {
        const href = anchor.getAttribute('href');
        if (href !== '#') {
          e.preventDefault();
          const target = document.querySelector(href);
          if (target) {
            target.scrollIntoView({ behavior: 'smooth', block: 'start' });
          }
        }
      });
    });
  };

  // ===== SCROLL ANIMATIONS =====
  const initScrollAnimations = () => {
    const observerOptions = {
      threshold: 0.1,
      rootMargin: '0px 0px -50px 0px',
    };

    const observer = new IntersectionObserver((entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.style.animation = 'fadeInUp 0.6s ease-out forwards';
          observer.unobserve(entry.target);
        }
      });
    }, observerOptions);

    document.querySelectorAll(
      '.skill-category, .project-card, .stat-card, .timeline-item, .contact-method'
    ).forEach((el) => {
      observer.observe(el);
    });
  };

  // ===== ACTIVE NAV LINK =====
  const initActiveNav = () => {
    const navLinks = document.querySelectorAll('.nav-link');
    const sections = document.querySelectorAll('section[id]');

    const updateActiveLink = () => {
      let current = '';
      sections.forEach((section) => {
        if (window.scrollY >= section.offsetTop - 200) {
          current = section.getAttribute('id');
        }
      });

      navLinks.forEach((link) => {
        link.classList.remove('active');
        const href = link.getAttribute('href').substring(1);
        if (href === current) {
          link.style.color = 'var(--primary)';
        } else {
          link.style.color = 'inherit';
        }
      });
    };

    window.addEventListener('scroll', updateActiveLink);
    updateActiveLink();
  };

  // ===== PAGE LOAD ANIMATION =====
  const initPageLoad = () => {
    document.body.style.opacity = '0';
    setTimeout(() => {
      document.body.style.transition = 'opacity 0.8s ease-out';
      document.body.style.opacity = '1';
    }, 100);
  };

  // ===== ADD CSS ANIMATIONS =====
  const addAnimations = () => {
    const style = document.createElement('style');
    style.textContent = `
      @keyframes fadeInUp {
        from {
          opacity: 0;
          transform: translateY(30px);
        }
        to {
          opacity: 1;
          transform: translateY(0);
        }
      }

      @keyframes spin {
        from { transform: rotate(0deg); }
        to { transform: rotate(360deg); }
      }

      @keyframes slideInDown {
        from {
          opacity: 0;
          transform: translateY(-20px);
        }
        to {
          opacity: 1;
          transform: translateY(0);
        }
      }

      .hero-content { animation: slideInDown 0.8s ease-out; }
      .hero-visual { animation: slideInDown 0.8s ease-out 0.2s both; }
    `;
    document.head.appendChild(style);
  };

  // ===== INITIALIZE ALL =====
  initTheme();
  addAnimations();
  initPageLoad();
  initMobileMenu();
  initSmoothScroll();
  initScrollAnimations();
  initActiveNav();

  console.log('✅ All interactions loaded!');
});
