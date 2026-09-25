# -student-hub
My first git repository 
AUTHOR-AIR
/* =========================================
   STUDENTS HUB - STEP 3 UI
========================================= */

:root {

    --primary: #4f46e5;
    --primary-dark: #3730a3;
    --primary-light: #eef2ff;

    --text: #172033;
    --text-light: #667085;
    --text-muted: #98a2b3;

    --bg: #f7f8fc;
    --white: #ffffff;

    --border: #e7e9f0;

    --blue: #3b82f6;
    --purple: #8b5cf6;
    --green: #10b981;
    --orange: #f59e0b;
    --red: #ef4444;
    --cyan: #06b6d4;

    --shadow-sm:
        0 2px 10px rgba(16, 24, 40, 0.04);

    --shadow:
        0 10px 30px rgba(16, 24, 40, 0.07);

    --shadow-lg:
        0 20px 60px rgba(16, 24, 40, 0.12);

    --radius-sm: 10px;
    --radius: 16px;
    --radius-lg: 24px;

    --sidebar-width: 260px;
}


/* =========================================
   RESET
========================================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: "Inter", sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.6;
}

h1,
h2,
h3,
h4 {
    font-family: "Poppins", sans-serif;
}

a {
    text-decoration: none;
    color: inherit;
}

button,
input,
select {
    font-family: inherit;
}

button {
    cursor: pointer;
}

img {
    max-width: 100%;
}

.container {
    width: min(1180px, calc(100% - 40px));
    margin: auto;
}


/* =========================================
   BRAND
========================================= */

.brand {
    display: inline-flex;
    align-items: center;
    gap: 10px;

    font-family: "Poppins", sans-serif;
    font-weight: 800;
    font-size: 21px;
    letter-spacing: -0.5px;
}

.brand > span:last-child > span {
    color: var(--primary);
}

.brand-icon {
    width: 40px;
    height: 40px;

    display: flex;
    align-items: center;
    justify-content: center;

    color: white;

    border-radius: 12px;

    background:
        linear-gradient(
            135deg,
            var(--primary),
            #7c3aed
        );

    box-shadow:
        0 8px 18px rgba(79, 70, 229, 0.25);
}


/* =========================================
   BUTTONS
========================================= */

.btn {
    min-height: 46px;

    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 9px;

    border: 0;
    border-radius: 11px;

    padding: 0 20px;

    font-size: 14px;
    font-weight: 700;

    transition:
        transform .2s ease,
        box-shadow .2s ease,
        background .2s ease;
}

.btn:hover {
    transform: translateY(-2px);
}

.btn-primary {
    color: white;

    background:
        linear-gradient(
            135deg,
            var(--primary),
            #6366f1
        );

    box-shadow:
        0 8px 18px rgba(79, 70, 229, .22);
}

.btn-primary:hover {
    box-shadow:
        0 12px 25px rgba(79, 70, 229, .3);
}

.btn-outline {
    color: var(--text);

    background: var(--white);

    border: 1px solid var(--border);
}

.btn-outline:hover {
    border-color: var(--primary);
    color: var(--primary);
}

.btn-white {
    color: var(--primary);
    background: white;
}

.btn-large {
    min-height: 54px;
    padding: 0 25px;
}


/* =========================================
   TOP NAVBAR
========================================= */

.topbar {
    position: sticky;
    top: 0;
    z-index: 100;

    background:
        rgba(255,255,255,.9);

    backdrop-filter: blur(18px);

    border-bottom:
        1px solid rgba(231,233,240,.8);
}

.nav-container {
    min-height: 76px;

    display: flex;
    align-items: center;
    justify-content: space-between;

    gap: 25px;
}

.desktop-nav {
    display: flex;
    align-items: center;
    gap: 32px;
}

.desktop-nav a {
    color: var(--text-light);

    font-size: 14px;
    font-weight: 600;

    transition: .2s;
}

.desktop-nav a:hover,
.desktop-nav a.active {
    color: var(--primary);
}

.nav-actions {
    display: flex;
    align-items: center;
    gap: 15px;
}

.login-link {
    font-size: 14px;
    font-weight: 700;
}

.icon-btn {
    width: 40px;
    height: 40px;

    display: inline-flex;
    align-items: center;
    justify-content: center;

    border: 1px solid var(--border);
    border-radius: 10px;

    color: var(--text-light);
    background: var(--white);

    transition: .2s;
}

.icon-btn:hover {
    color: var(--primary);
    border-color: var(--primary);
}

.mobile-menu-btn {
    display: none;

    width: 42px;
    height: 42px;

    border: 0;
    border-radius: 10px;

    background: var(--primary);
    color: white;

    font-size: 18px;
}

.mobile-nav {
    display: none;
}


/* =========================================
   HERO
========================================= */

.hero {
    overflow: hidden;

    padding:
        90px 0 100px;

    background:
        radial-gradient(
            circle at 80% 20%,
            #e9e7ff 0,
            transparent 35%
        ),
        radial-gradient(
            circle at 10% 70%,
            #e8f3ff 0,
            transparent 30%
        ),
        #fbfbff;
}

.hero-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;

    align-items: center;

    gap: 80px;
}

.hero-content {
    max-width: 600px;
}

.hero-badge {
    display: inline-flex;
    align-items: center;
    gap: 8px;

    padding: 8px 13px;

    border-radius: 50px;

    color: var(--primary);

    background: var(--primary-light);

    font-size: 12px;
    font-weight: 800;

    margin-bottom: 24px;
}

.hero-content h1 {
    font-size: clamp(42px, 5vw, 70px);
    line-height: 1.05;

    letter-spacing: -3px;

    margin-bottom: 25px;
}

.hero-content h1 span {
    display: block;
    color: var(--primary);
}

.hero-content > p {
    max-width: 560px;

    color: var(--text-light);

    font-size: 17px;
    line-height: 1.8;

    margin-bottom: 32px;
}

.hero-buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 13px;
}

.hero-trust {
    display: flex;
    align-items: center;
    gap: 14px;

    margin-top: 35px;
}

.avatar-stack {
    display: flex;
}

.avatar-stack span {
    width: 34px;
    height: 34px;

    display: flex;
    align-items: center;
    justify-content: center;

    margin-left: -7px;

    border: 3px solid white;
    border-radius: 50%;

    background: #dbeafe;

    color: var(--primary);

    font-size: 10px;
    font-weight: 800;
}

.avatar-stack span:first-child {
    margin-left: 0;
}

.hero-trust strong,
.hero-trust small {
    display: block;
}

.hero-trust strong {
    font-size: 13px;
}

.hero-trust small {
    color: var(--text-muted);
    font-size: 11px;
}


/* =========================================
   HERO VISUAL
========================================= */

.hero-visual {
    position: relative;
    min-height: 550px;

    display: flex;
    align-items: center;
    justify-content: center;
}

.dashboard-preview {
    width: min(470px, 100%);

    padding: 25px;

    border:
        1px solid rgba(255,255,255,.8);

    border-radius: 25px;

    background:
        rgba(255,255,255,.85);

    box-shadow:
        0 35px 80px rgba(50, 50, 100, .14);

    backdrop-filter: blur(20px);
}

.preview-top {
    display: flex;
    align-items: center;
    justify-content: space-between;

    margin-bottom: 25px;
}

.small-label {
    display: block;

    color: var(--text-muted);

    font-size: 10px;
    font-weight: 700;

    text-transform: uppercase;
}

.preview-top h3 {
    font-size: 20px;
    margin-top: 4px;
}

.preview-avatar {
    width: 44px;
    height: 44px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 13px;

    color: white;

    background:
        linear-gradient(
            135deg,
            var(--primary),
            #8b5cf6
        );
}

.progress-card-mini {
    padding: 17px;

    border-radius: 15px;

    background: #f5f6ff;

    margin-bottom: 17px;
}

.mini-progress-info {
    display: flex;
    align-items: center;
    justify-content: space-between;

    margin-bottom: 12px;
}

.mini-progress-info div span,
.mini-progress-info div strong {
    display: block;
}

.mini-progress-info span {
    color: var(--text-light);
    font-size: 11px;
}

.mini-progress-info strong {
    font-size: 22px;
}

.mini-progress-info > i {
    color: var(--primary);
}

.progress-bar {
    height: 7px;

    border-radius: 20px;

    background: #dfe2f5;

    overflow: hidden;
}

.progress-bar span {
    display: block;
    height: 100%;

    border-radius: inherit;

    background:
        linear-gradient(
            90deg,
            var(--primary),
            #8b5cf6
        );
}

.preview-stats {
    display: grid;
    grid-template-columns: repeat(3, 1fr);

    gap: 10px;

    margin-bottom: 25px;
}

.preview-stats div {
    padding: 15px 10px;

    text-align: center;

    border:
        1px solid var(--border);

    border-radius: 13px;
}

.preview-stats i {
    display: block;

    color: var(--primary);

    margin-bottom: 5px;
}

.preview-stats strong,
.preview-stats span {
    display: block;
}

.preview-stats strong {
    font-size: 17px;
}

.preview-stats span {
    color: var(--text-muted);
    font-size: 9px;
}

.preview-list-title {
    display: flex;
    justify-content: space-between;

    margin-bottom: 12px;

    font-size: 12px;
}

.preview-list-title span {
    color: var(--primary);
}

.preview-item {
    display: flex;
    align-items: center;
    gap: 11px;

    padding: 12px;

    border-radius: 12px;

    background: #fafafa;

    margin-top: 8px;
}

.preview-item-icon {
    width: 38px;
    height: 38px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 10px;
}

.preview-item > div:nth-child(2) {
    flex: 1;
}

.preview-item strong,
.preview-item span {
    display: block;
}

.preview-item strong {
    font-size: 11px;
}

.preview-item span {
    color: var(--text-muted);
    font-size: 9px;
}

.preview-item > b {
    font-size: 11px;
    color: var(--primary);
}

.floating-card {
    position: absolute;

    display: flex;
    align-items: center;
    gap: 10px;

    padding: 13px 16px;

    border-radius: 15px;

    background: white;

    box-shadow:
        0 15px 40px rgba(0,0,0,.12);

    animation: floatCard 4s ease-in-out infinite;
}

.floating-card > i {
    width: 35px;
    height: 35px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 10px;

    color: var(--green);

    background: #ecfdf5;
}

.floating-card strong,
.floating-card small {
    display: block;
}

.floating-card strong {
    font-size: 11px;
}

.floating-card small {
    color: var(--text-muted);
    font-size: 9px;
}

.floating-card-one {
    left: -25px;
    top: 100px;
}

.floating-card-two {
    right: -20px;
    bottom: 100px;
}

.floating-card-two > i {
    color: var(--orange);
    background: #fffbeb;
}

@keyframes floatCard {
    0%,100% {
        transform: translateY(0);
    }

    50% {
        transform: translateY(-9px);
    }
}


/* =========================================
   STATS STRIP
========================================= */

.stats-strip {
    background: white;

    border-top: 1px solid var(--border);
    border-bottom: 1px solid var(--border);
}

.stats-grid {
    display: grid;
    grid-template-columns: repeat(4,1fr);
}

.stat-item {
    display: flex;
    align-items: center;
    gap: 14px;

    padding: 25px;

    border-right: 1px solid var(--border);
}

.stat-item:last-child {
    border-right: 0;
}

.stat-icon {
    width: 43px;
    height: 43px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 12px;

    color: var(--primary);

    background: var(--primary-light);
}

.stat-item strong,
.stat-item span {
    display: block;
}

.stat-item strong {
    font-size: 20px;
}

.stat-item span {
    color: var(--text-muted);
    font-size: 11px;
}


/* =========================================
   SECTIONS
========================================= */

.section {
    padding: 100px 0;
}

.section-heading {
    margin-bottom: 50px;
}

.centered {
    text-align: center;
}

.section-label {
    display: block;

    color: var(--primary);

    font-size: 10px;
    font-weight: 800;

    letter-spacing: 1.5px;
}

.section-heading h2 {
    font-size: clamp(30px, 4vw, 44px);

    line-height: 1.15;

    letter-spacing: -1.5px;

    margin: 8px 0 13px;
}

.section-heading h2 span {
    color: var(--primary);
}

.section-heading p {
    color: var(--text-light);
}


/* =========================================
   FEATURES
========================================= */

.feature-grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 20px;
}

.feature-card {
    position: relative;

    padding: 30px;

    border:
        1px solid var(--border);

    border-radius: var(--radius-lg);

    background: white;

    overflow: hidden;

    transition:
        transform .25s,
        box-shadow .25s,
        border .25s;
}

.feature-card:hover {
    transform: translateY(-6px);

    border-color:
        rgba(79,70,229,.25);

    box-shadow: var(--shadow-lg);
}

.feature-icon {
    width: 55px;
    height: 55px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 15px;

    font-size: 20px;

    margin-bottom: 28px;
}

.feature-number {
    position: absolute;
    top: 25px;
    right: 25px;

    color: #e8eaf0;

    font-size: 32px;
    font-weight: 800;
}

.feature-card h3 {
    font-size: 21px;
    margin-bottom: 9px;
}

.feature-card p {
    color: var(--text-light);
    font-size: 13px;
    line-height: 1.7;

    margin-bottom: 25px;
}

.feature-link {
    display: inline-flex;
    align-items: center;
    gap: 8px;

    color: var(--primary);

    font-size: 12px;
    font-weight: 800;
}

.feature-link i {
    transition: .2s;
}

.feature-card:hover .feature-link i {
    transform: translateX(5px);
}


/* =========================================
   COLOR BACKGROUNDS
========================================= */

.blue-bg {
    color: #2563eb !important;
    background: #eff6ff !important;
}

.purple-bg {
    color: #7c3aed !important;
    background: #f5f3ff !important;
}

.green-bg {
    color: #059669 !important;
    background: #ecfdf5 !important;
}

.orange-bg {
    color: #d97706 !important;
    background: #fffbeb !important;
}

.red-bg {
    color: #dc2626 !important;
    background: #fef2f2 !important;
}

.cyan-bg {
    color: #0891b2 !important;
    background: #ecfeff !important;
}


/* =========================================
   CTA
========================================= */

.cta-section {
    padding: 20px 0 100px;
}

.cta-box {
    position: relative;

    display: flex;
    align-items: center;
    justify-content: space-between;

    gap: 30px;

    padding: 50px;

    border-radius: 28px;

    color: white;

    overflow: hidden;

    background:
        linear-gradient(
            120deg,
            #3730a3,
            #6366f1,
            #7c3aed
        );

    box-shadow:
        0 25px 60px rgba(79,70,229,.25);
}

.cta-box:after {
    content: "";

    position: absolute;

    width: 300px;
    height: 300px;

    right: -100px;
    top: -130px;

    border-radius: 50%;

    background:
        rgba(255,255,255,.08);
}

.light-label {
    color: #c7d2fe;
}

.cta-box h2 {
    max-width: 600px;

    font-size: 35px;
    line-height: 1.2;

    margin: 8px 0 12px;
}

.cta-box h2 span {
    color: #c7d2fe;
}

.cta-box p {
    color: #e0e7ff;
}


/* =========================================
   FOOTER
========================================= */

.footer {
    color: #cbd5e1;
    background: #101322;
}

.footer-grid {
    display: grid;
    grid-template-columns: 2fr 1fr 1fr 1fr;

    gap: 50px;

    padding: 70px 0;
}

.footer .brand {
    color: white;
}

.footer .brand > span:last-child > span {
    color: #818cf8;
}

.footer-brand p {
    max-width: 320px;

    margin: 18px 0;

    color: #94a3b8;

    font-size: 13px;
}

.footer-grid h4 {
    color: white;
    margin-bottom: 18px;
}

.footer-grid > div:not(.footer-brand) > a {
    display: block;

    color: #94a3b8;

    font-size: 12px;

    margin-bottom: 11px;
}

.footer-grid > div:not(.footer-brand) > a:hover {
    color: white;
}

.social-links {
    display: flex;
    gap: 8px;
}

.social-links a {
    width: 36px;
    height: 36px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 9px;

    color: #cbd5e1;
    background: #1b2133;
}

.footer-bottom {
    padding: 18px 0;

    border-top: 1px solid #242a3c;

    color: #64748b;

    font-size: 11px;
}


/* =========================================
   AUTH PAGES
========================================= */

.auth-body {
    min-height: 100vh;
    background: white;
}

.auth-layout {
    min-height: 100vh;

    display: grid;
    grid-template-columns: 48% 52%;
}

.auth-visual {
    position: relative;

    display: flex;
    flex-direction: column;

    padding: 45px;

    color: white;

    overflow: hidden;

    background:
        radial-gradient(
            circle at 20% 20%,
            rgba(129,140,248,.5),
            transparent 30%
        ),
        linear-gradient(
            145deg,
            #111827,
            #312e81
        );
}

.signup-visual {
    background:
        radial-gradient(
            circle at 80% 20%,
            rgba(16,185,129,.25),
            transparent 30%
        ),
        linear-gradient(
            145deg,
            #111827,
            #064e3b
        );
}

.auth-brand {
    color: white;
}

.auth-brand > span:last-child > span {
    color: #a5b4fc;
}

.auth-visual-content {
    max-width: 570px;

    margin: auto 0;
}

.auth-visual-content h1 {
    font-size: clamp(38px, 5vw, 65px);

    line-height: 1.08;

    letter-spacing: -2px;

    margin: 12px 0 25px;
}

.auth-visual-content h1 span {
    display: block;
    color: #a5b4fc;
}

.auth-visual-content > p {
    max-width: 480px;

    color: #cbd5e1;

    line-height: 1.8;

    margin-bottom: 30px;
}

.auth-benefits > div {
    display: flex;
    align-items: center;
    gap: 10px;

    margin-top: 13px;

    color: #e2e8f0;

    font-size: 13px;
}

.auth-benefits i {
    color: #818cf8;
}

.auth-bottom {
    color: #94a3b8;
    font-size: 11px;
}

.auth-feature-box {
    display: flex;
    align-items: center;
    gap: 15px;

    max-width: 400px;

    padding: 18px;

    border:
        1px solid rgba(255,255,255,.1);

    border-radius: 17px;

    background:
        rgba(255,255,255,.07);

    backdrop-filter: blur(15px);
}

.auth-feature-icon {
    width: 45px;
    height: 45px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 12px;

    color: white;

    background:
        rgba(255,255,255,.1);
}

.auth-feature-box strong,
.auth-feature-box p {
    display: block;
}

.auth-feature-box strong {
    font-size: 13px;
}

.auth-feature-box p {
    margin: 2px 0 0;

    color: #94a3b8;

    font-size: 11px;
}

.auth-form-area {
    display: flex;
    align-items: center;
    justify-content: center;

    padding: 50px;
}

.auth-form-box {
    width: min(430px, 100%);
}

.mobile-auth-logo {
    display: none;
}

.auth-heading {
    margin-bottom: 30px;
}

.auth-heading h2 {
    font-size: 34px;
    letter-spacing: -1px;

    margin: 6px 0;
}

.auth-heading p {
    color: var(--text-light);
    font-size: 13px;
}

.input-group {
    margin-bottom: 18px;
}

.input-group label {
    display: block;

    margin-bottom: 7px;

    color: var(--text);

    font-size: 12px;
    font-weight: 700;
}

.label-row {
    display: flex;
    justify-content: space-between;
}

.label-row a {
    color: var(--primary);
    font-size: 11px;
    font-weight: 600;
}

.input-wrapper {
    position: relative;
}

.input-wrapper > i:first-child {
    position: absolute;

    left: 15px;
    top: