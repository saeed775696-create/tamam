<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description"
        content="تمام ميديا – وكالة إعلامية وتسويقية رقمية متكاملة في تعز، اليمن. هوية بصرية، إنتاج مرئي، تسويق رقمي، تطوير مواقع.">
    <meta name="keywords" content="تمام ميديا, تسويق رقمي, هوية بصرية, إنتاج مرئي, تطوير مواقع, تعز, اليمن">
    <meta name="author" content="Tamam Media">
    <meta property="og:title" content="تمام ميديا | Tamam Media">
    <meta property="og:description" content="نحو حضور أقوى… ونمو أذكى — حلول إعلامية رقمية متكاملة">
    <meta property="og:type" content="website">
    <title>تمام ميديا | Tamam Media — نحو حضور أقوى</title>

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link
        href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;500;600;700;800&family=Poppins:wght@300;400;500;600;700&display=swap"
        rel="stylesheet">

    <!-- Lucide Icons CDN -->
    <script src="https://unpkg.com/lucide@latest"></script>

    <style>
        /* ── Tamam Media Brand Design System ── */
        :root {
            --primary: #1A8F9D;
            --primary-light: #22b0c1;
            --primary-dark: #136e7a;
            --secondary: #F39C12;
            --secondary-light: #f5b942;
            --secondary-dark: #d68910;
            --background: #ffffff;
            --foreground: #0f1923;
            --card: #ffffff;
            --card-foreground: #0f1923;
            --muted: #f4f7f8;
            --muted-foreground: #6b7c85;
            --border: #e2ecee;
            --input: #e2ecee;
            --ring: #1A8F9D;
            --popover: #ffffff;
            --popover-foreground: #0f1923;
            --accent: #F39C12;
            --accent-foreground: #ffffff;
            --destructive: oklch(0.58 0.22 25);
            --destructive-foreground: #ffffff;
            --radius: 0.75rem;
            --font-sans: 'Cairo', 'Poppins', sans-serif;
        }

        [dir="rtl"] body {
            font-family: 'Cairo', sans-serif;
        }

        [dir="ltr"] body {
            font-family: 'Poppins', sans-serif;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
        }

        html[dir="rtl"] body {
            font-family: 'Cairo', sans-serif;
        }

        html[dir="ltr"] body {
            font-family: 'Poppins', sans-serif;
        }

        body {
            background: var(--background);
            color: var(--foreground);
            min-height: 100vh;
            line-height: 1.75;
        }

        h1,
        h2,
        h3,
        h4,
        h5,
        h6 {
            font-weight: 700;
            letter-spacing: -0.02em;
            line-height: 1.3;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        /* ── Utility Classes ── */
        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 1rem;
        }

        .section-pad {
            padding: 5rem 0;
        }

        /* Gradient text */
        .text-gradient {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        /* Section reveal animation */
        .reveal {
            opacity: 0;
            transform: translateY(32px);
            transition: opacity 0.7s ease-out, transform 0.7s ease-out;
        }

        .reveal.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .reveal-delay-1 {
            transition-delay: 0.1s;
        }

        .reveal-delay-2 {
            transition-delay: 0.2s;
        }

        .reveal-delay-3 {
            transition-delay: 0.3s;
        }

        .reveal-delay-4 {
            transition-delay: 0.4s;
        }

        /* Card hover lift */
        .card-hover {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card-hover:hover {
            transform: translateY(-6px);
            box-shadow: 0 20px 40px -10px rgba(26, 143, 157, 0.2);
        }

        /* Buttons */
        .btn-primary {
            background: var(--primary);
            color: white;
            padding: 0.75rem 2rem;
            border-radius: var(--radius);
            font-weight: 700;
            font-size: 0.95rem;
            transition: all 0.25s ease;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            border: none;
            cursor: pointer;
        }

        .btn-primary:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: 0 8px 20px -4px rgba(26, 143, 157, 0.5);
        }

        .btn-secondary {
            background: var(--secondary);
            color: white;
            padding: 0.75rem 2rem;
            border-radius: var(--radius);
            font-weight: 700;
            font-size: 0.95rem;
            transition: all 0.25s ease;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            border: none;
            cursor: pointer;
        }

        .btn-secondary:hover {
            background: var(--secondary-dark);
            transform: translateY(-2px);
            box-shadow: 0 8px 20px -4px rgba(243, 156, 18, 0.5);
        }

        .btn-outline {
            background: transparent;
            color: var(--primary);
            border: 2px solid var(--primary);
            padding: 0.7rem 2rem;
            border-radius: var(--radius);
            font-weight: 700;
            font-size: 0.95rem;
            transition: all 0.25s ease;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            cursor: pointer;
        }

        .btn-outline:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-2px);
        }

        /* Section tag */
        .section-tag {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.4rem 1rem;
            border-radius: 9999px;
            background: rgba(26, 143, 157, 0.1);
            border: 1px solid rgba(26, 143, 157, 0.2);
            color: var(--primary);
            font-size: 0.75rem;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            margin-bottom: 0.75rem;
        }

        /* Glass card */
        .glass-card {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(26, 143, 157, 0.15);
        }

        /* ── Navbar Styles ── */
        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 50;
            transition: all 0.4s ease;
        }

        .navbar.scrolled {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(12px);
            box-shadow: 0 4px 20px -4px rgba(26, 143, 157, 0.08);
            border-bottom: 1px solid var(--border);
        }

        .navbar-inner {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 1rem 0;
            height: 4.5rem;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 0.625rem;
        }

        .logo-icon {
            width: 2.5rem;
            height: 2.5rem;
            border-radius: 0.75rem;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 900;
            font-size: 1.125rem;
            background: linear-gradient(135deg, #1A8F9D, #136e7a);
            box-shadow: 0 4px 14px -4px rgba(26, 143, 157, 0.4);
        }

        .logo-text {
            line-height: 1.2;
        }

        .logo-name {
            display: block;
            font-weight: 900;
            color: var(--foreground);
            font-size: 1.125rem;
            letter-spacing: -0.02em;
        }

        .logo-name span {
            color: var(--secondary);
        }

        .logo-sub {
            display: block;
            font-size: 0.625rem;
            font-weight: 500;
            color: var(--muted-foreground);
            text-transform: uppercase;
            letter-spacing: 0.15em;
        }

        .nav-links {
            display: none;
            align-items: center;
            gap: 1.5rem;
        }

        @media (min-width: 768px) {
            .nav-links {
                display: flex;
            }
        }

        .nav-link {
            font-size: 0.875rem;
            font-weight: 600;
            color: rgba(15, 25, 35, 0.8);
            transition: color 0.2s;
            position: relative;
            padding-bottom: 0.125rem;
        }

        .nav-link:hover,
        .nav-link.active {
            color: var(--primary);
        }

        .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 2px;
            background: var(--primary);
            border-radius: 1px;
            transform: scaleX(0);
            transition: transform 0.3s;
        }

        [dir="ltr"] .nav-link::after {
            transform-origin: left;
        }

        [dir="rtl"] .nav-link::after {
            transform-origin: right;
        }

        .nav-link:hover::after,
        .nav-link.active::after {
            transform: scaleX(1);
        }

        .nav-actions {
            display: flex;
            align-items: center;
            gap: 0.75rem;
        }

        .lang-toggle {
            display: flex;
            align-items: center;
            gap: 0.375rem;
            padding: 0.375rem 0.75rem;
            border-radius: 0.5rem;
            border: 1px solid var(--border);
            font-size: 0.875rem;
            font-weight: 600;
            color: var(--muted-foreground);
            background: transparent;
            cursor: pointer;
            transition: all 0.2s;
        }

        .lang-toggle:hover {
            color: var(--primary);
            border-color: rgba(26, 143, 157, 0.4);
        }

        .nav-cta {
            display: none;
            align-items: center;
            gap: 0.5rem;
            padding: 0.5rem 1.25rem;
            border-radius: 0.75rem;
            font-size: 0.875rem;
            font-weight: 700;
            color: white;
            background: linear-gradient(135deg, #1A8F9D, #136e7a);
            box-shadow: 0 4px 14px -4px rgba(26, 143, 157, 0.4);
            transition: all 0.2s;
        }

        @media (min-width: 768px) {
            .nav-cta {
                display: inline-flex;
            }
        }

        .nav-cta:hover {
            transform: translateY(-1px);
            box-shadow: 0 8px 20px -4px rgba(26, 143, 157, 0.5);
        }

        .mobile-toggle {
            display: flex;
            padding: 0.5rem;
            border-radius: 0.5rem;
            background: transparent;
            border: none;
            cursor: pointer;
            color: var(--foreground);
            transition: background 0.2s;
        }

        @media (min-width: 768px) {
            .mobile-toggle {
                display: none;
            }
        }

        .mobile-toggle:hover {
            background: var(--muted);
        }

        .mobile-menu {
            display: none;
            flex-direction: column;
            gap: 0.25rem;
            padding: 1rem;
            background: white;
            border-top: 1px solid var(--border);
            box-shadow: 0 20px 40px -10px rgba(0, 0, 0, 0.1);
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease;
        }

        .mobile-menu.open {
            display: flex;
            max-height: 500px;
        }

        .mobile-menu-link {
            padding: 0.75rem 1rem;
            border-radius: 0.75rem;
            font-weight: 600;
            font-size: 1rem;
            transition: all 0.2s;
            color: var(--foreground);
        }

        .mobile-menu-link:hover,
        .mobile-menu-link.active {
            background: rgba(26, 143, 157, 0.1);
            color: var(--primary);
        }

        /* ── Hero Section ── */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            overflow: hidden;
            background: linear-gradient(135deg, white 0%, rgba(34, 176, 193, 0.05) 50%, white 100%);
            padding-top: 5rem;
        }

        .hero-bg-decoration {
            position: absolute;
            inset: 0;
            pointer-events: none;
            overflow: hidden;
        }

        .hero-blob-1 {
            position: absolute;
            top: 25%;
            right: -5rem;
            width: 24rem;
            height: 24rem;
            border-radius: 50%;
            background: rgba(26, 143, 157, 0.06);
            filter: blur(3rem);
        }

        .hero-blob-2 {
            position: absolute;
            bottom: 25%;
            left: -5rem;
            width: 20rem;
            height: 20rem;
            border-radius: 50%;
            background: rgba(243, 156, 18, 0.08);
            filter: blur(3rem);
        }

        .hero-grid {
            position: absolute;
            top: 0;
            right: 0;
            width: 100%;
            height: 100%;
            opacity: 0.03;
            background-image: radial-gradient(circle, #1A8F9D 1px, transparent 1px);
            background-size: 40px 40px;
        }

        .hero-grid-pattern {
            width: 100%;
            height: 100%;
        }

        .hero-content {
            position: relative;
            z-index: 10;
            width: 100%;
        }

        .hero-grid-layout {
            display: grid;
            grid-template-columns: 1fr;
            gap: 4rem;
            align-items: center;
            padding: 4rem 0;
        }

        @media (min-width: 1024px) {
            .hero-grid-layout {
                grid-template-columns: 1fr 1fr;
            }
        }

        .hero-badge {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.5rem 1rem;
            border-radius: 9999px;
            background: rgba(243, 156, 18, 0.1);
            border: 1px solid rgba(243, 156, 18, 0.2);
            color: var(--secondary);
            font-size: 0.875rem;
            font-weight: 700;
        }

        .hero-badge-dot {
            width: 0.5rem;
            height: 0.5rem;
            border-radius: 50%;
            background: var(--secondary);
            animation: pulse 2s infinite;
        }

        @keyframes pulse {

            0%,
            100% {
                opacity: 1;
            }

            50% {
                opacity: 0.5;
            }
        }

        .hero-title {
            font-size: 3rem;
            font-weight: 900;
            line-height: 1.1;
            margin: 1.5rem 0;
        }

        @media (min-width: 768px) {
            .hero-title {
                font-size: 3.75rem;
            }
        }

        @media (min-width: 1024px) {
            .hero-title {
                font-size: 4.5rem;
            }
        }

        .hero-subtitle {
            font-size: 1.125rem;
            color: var(--muted-foreground);
            line-height: 1.75;
            max-width: 36rem;
            margin-bottom: 1.25rem;
        }

        .hero-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            margin-bottom: 0.5rem;
        }

        .hero-stats {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            padding-top: 0.5rem;
        }

        .hero-stat {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.5rem 1rem;
            border-radius: 0.75rem;
            background: white;
            border: 1px solid var(--border);
            box-shadow: 0 2px 8px -2px rgba(0, 0, 0, 0.05);
        }

        .hero-stat-value {
            font-size: 1.25rem;
            font-weight: 900;
            color: var(--primary);
        }

        .hero-stat-label {
            font-size: 0.75rem;
            color: var(--muted-foreground);
            font-weight: 500;
        }

        .hero-image-wrapper {
            position: relative;
        }

        .hero-image-glow {
            position: absolute;
            inset: -1.5rem;
            background: rgba(26, 143, 157, 0.05);
            border-radius: 1.5rem;
            filter: blur(2rem);
        }

        .hero-image-card {
            position: relative;
            border-radius: 1.5rem;
            overflow: hidden;
            border: 4px solid white;
            box-shadow: 0 25px 50px -12px rgba(26, 143, 157, 0.15);
        }

        .hero-image-card img {
            width: 100%;
            height: 500px;
            object-fit: cover;
            display: block;
        }

        .hero-image-overlay {
            position: absolute;
            inset: 0;
            background: linear-gradient(to top, rgba(15, 25, 35, 0.3), transparent 50%);
        }

        .hero-float-card {
            position: absolute;
            bottom: -1.5rem;
            left: -1.5rem;
            background: white;
            border-radius: 1.25rem;
            padding: 1rem;
            box-shadow: 0 20px 40px -10px rgba(0, 0, 0, 0.1);
            border: 1px solid var(--border);
        }

        .hero-float-card-inner {
            display: flex;
            align-items: center;
            gap: 0.75rem;
        }

        .hero-float-icon {
            width: 2.5rem;
            height: 2.5rem;
            border-radius: 0.75rem;
            background: rgba(243, 156, 18, 0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.25rem;
        }

        .hero-float-value {
            font-weight: 900;
            color: var(--foreground);
            font-size: 1.125rem;
        }

        .hero-float-label {
            font-size: 0.75rem;
            color: var(--muted-foreground);
            font-weight: 500;
        }

        .hero-badge-top {
            position: absolute;
            top: -1rem;
            right: -1rem;
            background: var(--primary);
            border-radius: 1.25rem;
            padding: 0.5rem 1rem;
            box-shadow: 0 10px 30px -6px rgba(26, 143, 157, 0.5);
        }

        .hero-badge-top-text {
            color: white;
            font-weight: 900;
            font-size: 0.875rem;
        }

        /* ── Services Section ── */
        .services-section {
            padding: 5rem 0;
            background: rgba(244, 247, 248, 0.4);
        }

        .section-header {
            text-align: center;
            margin-bottom: 3.5rem;
        }

        .section-title {
            font-size: 2rem;
            font-weight: 900;
            color: var(--foreground);
            margin-bottom: 1rem;
        }

        @media (min-width: 768px) {
            .section-title {
                font-size: 2.5rem;
            }
        }

        .section-desc {
            color: var(--muted-foreground);
            max-width: 36rem;
            margin: 0 auto;
        }

        .services-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
        }

        @media (min-width: 640px) {
            .services-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (min-width: 1024px) {
            .services-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        .service-card {
            padding: 1.75rem;
            border-radius: 1rem;
            background: white;
            border: 1px solid rgba(226, 236, 238, 0.6);
            cursor: default;
            position: relative;
            overflow: hidden;
            transition: all 0.3s;
        }

        .service-card::before {
            content: '';
            position: absolute;
            inset: 0;
            opacity: 0;
            transition: opacity 0.4s;
        }

        .service-card:hover {
            border-color: rgba(26, 143, 157, 0.3);
        }

        .service-card:hover::before {
            opacity: 1;
        }

        .service-card-inner {
            position: relative;
        }

        .service-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .service-title {
            font-size: 1.125rem;
            font-weight: 900;
            color: var(--foreground);
            margin-bottom: 0.5rem;
        }

        .service-desc {
            font-size: 0.875rem;
            color: var(--muted-foreground);
            line-height: 1.75;
            margin-bottom: 1rem;
        }

        .service-link {
            display: inline-flex;
            align-items: center;
            gap: 0.25rem;
            color: var(--primary);
            font-size: 0.875rem;
            font-weight: 700;
            transition: gap 0.2s;
        }

        .service-link:hover {
            gap: 0.5rem;
        }

        /* ── About Section ── */
        .about-section {
            padding: 5rem 0;
            background: white;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 4rem;
            align-items: center;
        }

        @media (min-width: 1024px) {
            .about-grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        .about-content {}

        .about-desc {
            color: var(--muted-foreground);
            line-height: 1.75;
            margin-bottom: 1.5rem;
        }

        .about-cards {
            display: grid;
            gap: 1rem;
            margin-bottom: 2rem;
        }

        .about-card {
            display: flex;
            gap: 1rem;
            padding: 1rem;
            border-radius: 0.75rem;
            background: rgba(244, 247, 248, 0.6);
            border: 1px solid rgba(226, 236, 238, 0.4);
        }

        .about-card-icon {
            font-size: 1.5rem;
        }

        .about-card-label {
            font-weight: 700;
            color: var(--foreground);
            font-size: 0.875rem;
            margin-bottom: 0.25rem;
        }

        .about-card-text {
            font-size: 0.875rem;
            color: var(--muted-foreground);
            line-height: 1.75;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1.25rem;
        }

        .stat-card {
            padding: 1.5rem;
            border-radius: 1rem;
            color: white;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .stat-card:hover {
            transform: translateY(-6px);
            box-shadow: 0 20px 40px -10px rgba(26, 143, 157, 0.3);
        }

        .stat-card-1 {
            background: var(--primary);
        }

        .stat-card-2 {
            background: var(--secondary);
        }

        .stat-card-3 {
            background: var(--foreground);
        }

        .stat-card-4 {
            background: rgba(26, 143, 157, 0.8);
        }

        .stat-icon {
            font-size: 1.875rem;
            margin-bottom: 0.5rem;
        }

        .stat-value {
            font-size: 2.25rem;
            font-weight: 900;
            margin-bottom: 0.25rem;
        }

        .stat-label {
            font-size: 0.875rem;
            opacity: 0.8;
            font-weight: 500;
        }

        /* ── Portfolio Section ── */
        .portfolio-section {
            padding: 5rem 0;
            background: rgba(244, 247, 248, 0.4);
        }

        .portfolio-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
        }

        @media (min-width: 768px) {
            .portfolio-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (min-width: 1024px) {
            .portfolio-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        .portfolio-card {
            position: relative;
            overflow: hidden;
            border-radius: 1rem;
            border: 1px solid rgba(226, 236, 238, 0.4);
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .portfolio-card:hover {
            transform: translateY(-6px);
            box-shadow: 0 20px 40px -10px rgba(26, 143, 157, 0.2);
        }

        .portfolio-card img {
            width: 100%;
            height: 256px;
            object-fit: cover;
            transition: transform 0.5s;
        }

        .portfolio-card:hover img {
            transform: scale(1.05);
        }

        .portfolio-overlay {
            position: absolute;
            inset: 0;
            background: linear-gradient(to top, rgba(15, 25, 35, 0.8), rgba(15, 25, 35, 0.2), transparent);
            transform: translateY(4px);
            transition: transform 0.3s;
        }

        .portfolio-card:hover .portfolio-overlay {
            transform: translateY(0);
        }

        .portfolio-content {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            padding: 1.25rem;
        }

        .portfolio-category {
            display: inline-block;
            padding: 0.25rem 0.625rem;
            border-radius: 9999px;
            background: var(--primary);
            color: white;
            font-size: 0.75rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
            text-transform: capitalize;
        }

        .portfolio-title {
            font-weight: 900;
            color: white;
        }

        .portfolio-center {
            text-align: center;
            margin-top: 2.5rem;
        }

        /* ── Testimonials Section ── */
        .testimonials-section {
            padding: 5rem 0;
            background: white;
        }

        .testimonials-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
        }

        @media (min-width: 768px) {
            .testimonials-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        .testimonial-card {
            padding: 1.75rem;
            border-radius: 1rem;
            border: 1px solid rgba(226, 236, 238, 0.5);
            background: white;
            box-shadow: 0 2px 8px -2px rgba(0, 0, 0, 0.05);
            display: flex;
            flex-direction: column;
            transition: all 0.3s;
        }

        .testimonial-card:hover {
            box-shadow: 0 8px 24px -6px rgba(26, 143, 157, 0.15);
            border-color: rgba(26, 143, 157, 0.3);
        }

        .testimonial-stars {
            display: flex;
            gap: 0.25rem;
            margin-bottom: 1rem;
        }

        .testimonial-star {
            color: var(--secondary);
        }

        .testimonial-text {
            font-size: 0.875rem;
            color: rgba(15, 25, 35, 0.8);
            line-height: 1.75;
            flex: 1;
            margin-bottom: 1.25rem;
            font-style: italic;
        }

        .testimonial-author {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            padding-top: 1rem;
            border-top: 1px solid var(--border);
        }

        .testimonial-avatar {
            width: 2.5rem;
            height: 2.5rem;
            border-radius: 0.75rem;
            background: var(--primary);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 900;
            font-size: 0.875rem;
        }

        .testimonial-name {
            font-weight: 700;
            color: var(--foreground);
            font-size: 0.875rem;
        }

        .testimonial-role {
            font-size: 0.75rem;
            color: var(--muted-foreground);
        }

        /* ── CTA Section ── */
        .cta-section {
            padding: 5rem 0;
            position: relative;
            overflow: hidden;
            background: linear-gradient(135deg, #0f1923 0%, #1A8F9D 100%);
        }

        .cta-pattern {
            position: absolute;
            inset: 0;
            opacity: 0.1;
            background-image: radial-gradient(circle, white 1px, transparent 1px);
            background-size: 30px 30px;
        }

        .cta-content {
            position: relative;
            max-width: 48rem;
            margin: 0 auto;
            text-align: center;
        }

        .cta-icon {
            font-size: 4rem;
            margin-bottom: 1.25rem;
        }

        .cta-title {
            font-size: 2rem;
            font-weight: 900;
            color: white;
            margin-bottom: 1.25rem;
        }

        @media (min-width: 768px) {
            .cta-title {
                font-size: 2.5rem;
            }
        }

        .cta-desc {
            font-size: 1.125rem;
            color: rgba(255, 255, 255, 0.7);
            line-height: 1.75;
            margin-bottom: 2rem;
        }

        /* ── About Page ── */
        .page-hero {
            padding: 8rem 0 4rem;
            background: linear-gradient(135deg, white 0%, rgba(34, 176, 193, 0.05) 100%);
        }

        .page-hero-title {
            font-size: 2.5rem;
            font-weight: 900;
            color: var(--foreground);
            margin-bottom: 1rem;
        }

        @media (min-width: 768px) {
            .page-hero-title {
                font-size: 3rem;
            }
        }

        .page-hero-desc {
            font-size: 1.125rem;
            color: var(--muted-foreground);
            max-width: 48rem;
            line-height: 1.75;
        }

        .values-section {
            padding: 5rem 0;
            background: rgba(244, 247, 248, 0.4);
        }

        .values-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
            margin-top: 3rem;
        }

        @media (min-width: 640px) {
            .values-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (min-width: 1024px) {
            .values-grid {
                grid-template-columns: repeat(4, 1fr);
            }
        }

        .value-card {
            padding: 1.5rem;
            border-radius: 1rem;
            background: white;
            border: 1px solid var(--border);
            text-align: center;
            transition: all 0.3s;
        }

        .value-card:hover {
            border-color: var(--primary);
            box-shadow: 0 10px 30px -8px rgba(26, 143, 157, 0.15);
        }

        .value-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .value-title {
            font-weight: 900;
            color: var(--foreground);
            margin-bottom: 0.5rem;
        }

        .method-section {
            padding: 5rem 0;
            background: white;
        }

        .method-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 2rem;
            margin-top: 3rem;
        }

        @media (min-width: 768px) {
            .method-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (min-width: 1024px) {
            .method-grid {
                grid-template-columns: repeat(4, 1fr);
            }
        }

        .method-card {
            position: relative;
            padding: 1.5rem;
        }

        .method-number {
            font-size: 3rem;
            font-weight: 900;
            color: rgba(26, 143, 157, 0.15);
            margin-bottom: 0.5rem;
        }

        .method-title {
            font-weight: 900;
            color: var(--foreground);
            margin-bottom: 0.5rem;
        }

        .method-desc {
            font-size: 0.875rem;
            color: var(--muted-foreground);
            line-height: 1.75;
        }

        /* ── Services Page ── */
        .service-detail-card {
            padding: 2rem;
            border-radius: 1rem;
            background: white;
            border: 1px solid var(--border);
            margin-bottom: 2rem;
        }

        .service-detail-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .service-detail-title {
            font-size: 1.5rem;
            font-weight: 900;
            color: var(--foreground);
            margin-bottom: 0.75rem;
        }

        .service-detail-desc {
            color: var(--muted-foreground);
            line-height: 1.75;
            margin-bottom: 1.5rem;
        }

        .benefits-list {
            list-style: none;
            margin-bottom: 1.5rem;
        }

        .benefits-list li {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.5rem 0;
            color: var(--muted-foreground);
        }

        .benefits-list li::before {
            content: '✓';
            color: var(--primary);
            font-weight: 700;
        }

        .audience-tag {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.5rem 1rem;
            border-radius: 0.5rem;
            background: var(--muted);
            font-size: 0.875rem;
            color: var(--muted-foreground);
        }

        /* ── Contact Page ── */
        .contact-section {
            padding: 5rem 0;
            background: rgba(244, 247, 248, 0.4);
        }

        .contact-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 3rem;
        }

        @media (min-width: 1024px) {
            .contact-grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        .contact-info {}

        .contact-info-title {
            font-size: 1.5rem;
            font-weight: 900;
            color: var(--foreground);
            margin-bottom: 1rem;
        }

        .contact-info-desc {
            color: var(--muted-foreground);
            line-height: 1.75;
            margin-bottom: 2rem;
        }

        .contact-list {
            list-style: none;
        }

        .contact-list li {
            display: flex;
            align-items: flex-start;
            gap: 0.75rem;
            padding: 0.75rem 0;
            color: var(--muted-foreground);
        }

        .contact-list-icon {
            color: var(--primary);
            margin-top: 0.125rem;
        }

        .contact-form {
            background: white;
            padding: 2rem;
            border-radius: 1rem;
            border: 1px solid var(--border);
            box-shadow: 0 4px 20px -4px rgba(0, 0, 0, 0.05);
        }

        .form-group {
            margin-bottom: 1.25rem;
        }

        .form-label {
            display: block;
            font-weight: 600;
            color: var(--foreground);
            margin-bottom: 0.5rem;
            font-size: 0.875rem;
        }

        .form-input {
            width: 100%;
            padding: 0.75rem 1rem;
            border: 1px solid var(--border);
            border-radius: 0.5rem;
            font-size: 1rem;
            transition: border-color 0.2s;
            font-family: inherit;
        }

        .form-input:focus {
            outline: none;
            border-color: var(--primary);
        }

        .form-textarea {
            width: 100%;
            padding: 0.75rem 1rem;
            border: 1px solid var(--border);
            border-radius: 0.5rem;
            font-size: 1rem;
            min-height: 120px;
            resize: vertical;
            font-family: inherit;
        }

        .form-textarea:focus {
            outline: none;
            border-color: var(--primary);
        }

        .form-select {
            width: 100%;
            padding: 0.75rem 1rem;
            border: 1px solid var(--border);
            border-radius: 0.5rem;
            font-size: 1rem;
            background: white;
            font-family: inherit;
        }

        .form-select:focus {
            outline: none;
            border-color: var(--primary);
        }

        .form-success {
            padding: 1rem;
            border-radius: 0.5rem;
            background: rgba(34, 197, 94, 0.1);
            border: 1px solid rgba(34, 197, 94, 0.3);
            color: #166534;
            text-align: center;
            margin-bottom: 1rem;
            display: none;
        }

        .form-success.show {
            display: block;
        }

        /* ── Footer ── */
        .footer {
            background: var(--foreground);
            color: white;
            padding: 4rem 0 2rem;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 2.5rem;
            padding-bottom: 3rem;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        @media (min-width: 768px) {
            .footer-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (min-width: 1024px) {
            .footer-grid {
                grid-template-columns: 2fr 1fr 1fr;
            }
        }

        .footer-brand {}

        .footer-desc {
            color: rgba(255, 255, 255, 0.6);
            font-size: 0.875rem;
            line-height: 1.75;
            max-width: 18rem;
            margin: 1rem 0 1.5rem;
        }

        .footer-social {
            display: flex;
            gap: 0.75rem;
        }

        .footer-social-link {
            width: 2.25rem;
            height: 2.25rem;
            border-radius: 0.5rem;
            background: rgba(255, 255, 255, 0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            color: rgba(255, 255, 255, 0.6);
            transition: all 0.2s;
        }

        .footer-social-link:hover {
            background: var(--primary);
            color: white;
        }

        .footer-title {
            font-weight: 700;
            color: white;
            font-size: 0.875rem;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            margin-bottom: 1rem;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 0.625rem;
        }

        .footer-link {
            color: rgba(255, 255, 255, 0.55);
            font-size: 0.875rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            transition: color 0.2s;
        }

        .footer-link:hover {
            color: var(--primary);
        }

        .footer-link::before {
            content: '';
            width: 4px;
            height: 4px;
            border-radius: 50%;
            background: rgba(26, 143, 157, 0.6);
        }

        .footer-contact-item {
            display: flex;
            align-items: flex-start;
            gap: 0.5rem;
            color: rgba(255, 255, 255, 0.55);
            font-size: 0.875rem;
            margin-bottom: 0.75rem;
        }

        .footer-contact-icon {
            color: var(--primary);
            margin-top: 0.125rem;
        }

        .footer-bottom {
            padding-top: 1.5rem;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 0.75rem;
        }

        @media (min-width: 768px) {
            .footer-bottom {
                flex-direction: row;
                justify-content: space-between;
            }
        }

        .footer-copyright {
            font-size: 0.875rem;
            color: rgba(255, 255, 255, 0.4);
        }

        .footer-made {
            font-size: 0.75rem;
            color: rgba(255, 255, 255, 0.3);
        }

        /* ── WhatsApp FAB ── */
        .whatsapp-fab {
            position: fixed;
            bottom: 1.5rem;
            left: 1.5rem;
            z-index: 50;
            width: 3.5rem;
            height: 3.5rem;
            border-radius: 50%;
            background: #22c55e;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            box-shadow: 0 10px 30px -6px rgba(34, 197, 94, 0.5);
            transition: all 0.3s;
        }

        .whatsapp-fab:hover {
            background: #16a34a;
            transform: scale(1.1);
        }

        /* ── Page wrapper ── */
        .page-wrapper {
            display: none;
        }

        .page-wrapper.active {
            display: block;
        }

        /* ── 404 ── */
        .not-found {
            min-height: 80vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 4rem 1rem;
        }

        .not-found-icon {
            font-size: 6rem;
            margin-bottom: 1rem;
        }

        .not-found-title {
            font-size: 2rem;
            font-weight: 900;
            color: var(--foreground);
            margin-bottom: 0.5rem;
        }

        .not-found-desc {
            color: var(--muted-foreground);
            margin-bottom: 2rem;
        }
    </style>
</head>

<body>
    <!-- Navbar -->
    <nav class="navbar" id="navbar">
        <div class="container">
            <div class="navbar-inner">
                <!-- Logo -->
                <a href="#/" class="logo" onclick="navigate('home')">
                    <div class="logo-icon">ت</div>
                    <div class="logo-text">
                        <span class="logo-name">تمام<span>.</span></span>
                        <span class="logo-sub">TAMAM MEDIA</span>
                    </div>
                </a>

                <!-- Desktop Nav -->
                <div class="nav-links" id="navLinks">
                    <a href="#/" class="nav-link" data-page="home" onclick="navigate('home')" id="nav_home"></a>
                    <a href="#/about" class="nav-link" data-page="about" onclick="navigate('about')" id="nav_about"></a>
                    <a href="#/services" class="nav-link" data-page="services" onclick="navigate('services')"
                        id="nav_services"></a>
                    <a href="#/portfolio" class="nav-link" data-page="portfolio" onclick="navigate('portfolio')"
                        id="nav_portfolio"></a>
                    <a href="#/contact" class="nav-link" data-page="contact" onclick="navigate('contact')"
                        id="nav_contact"></a>
                </div>

                <!-- Actions -->
                <div class="nav-actions">
                    <button class="lang-toggle" onclick="toggleLang()">
                        <i data-lucide="globe" style="width:14px;height:14px;"></i>
                        <span id="langBtn">EN</span>
                    </button>
                    <a href="#/contact" class="nav-cta" onclick="navigate('contact')" id="nav_cta"></a>
                    <button class="mobile-toggle" onclick="toggleMobile()">
                        <i data-lucide="menu" style="width:20px;height:20px;"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu -->
        <div class="mobile-menu" id="mobileMenu">
            <a href="#/" class="mobile-menu-link" data-page="home" onclick="navigate('home')" id="mobile_nav_home"></a>
            <a href="#/about" class="mobile-menu-link" data-page="about" onclick="navigate('about')"
                id="mobile_nav_about"></a>
            <a href="#/services" class="mobile-menu-link" data-page="services" onclick="navigate('services')"
                id="mobile_nav_services"></a>
            <a href="#/portfolio" class="mobile-menu-link" data-page="portfolio" onclick="navigate('portfolio')"
                id="mobile_nav_portfolio"></a>
            <a href="#/contact" class="mobile-menu-link" data-page="contact" onclick="navigate('contact')"
                id="mobile_nav_contact"></a>
        </div>
    </nav>

    <!-- Main Content -->
    <main>
        <!-- HOME PAGE -->
        <div class="page-wrapper active" id="page-home">
            <!-- Hero -->
            <section class="hero">
                <div class="hero-bg-decoration">
                    <div class="hero-blob-1"></div>
                    <div class="hero-blob-2"></div>
                    <div class="hero-grid">
                        <div class="hero-grid-pattern"></div>
                    </div>
                </div>
                <div class="container hero-content">
                    <div class="hero-grid-layout">
                        <div class="hero-text">
                            <div class="hero-badge">
                                <div class="hero-badge-dot"></div>
                                <span id="hero_badge2"></span>
                            </div>
                            <h1 class="hero-title">
                                <span id="hero_headline"></span><br>
                                <span class="text-gradient" id="hero_headline2"></span>
                            </h1>
                            <p class="hero-subtitle" id="hero_sub"></p>
                            <div class="hero-buttons">
                                <a href="#/contact" class="btn-secondary" onclick="navigate('contact')">
                                    <span id="hero_cta1"></span>
                                    <i data-lucide="arrow-right" style="width:16px;height:16px;"></i>
                                </a>
                                <a href="#/about" class="btn-outline" onclick="navigate('about')">
                                    <span id="hero_cta2"></span>
                                </a>
                            </div>
                            <div class="hero-stats">
                                <div class="hero-stat">
                                    <span class="hero-stat-value">150+</span>
                                    <span class="hero-stat-label" id="stat_projects_l"></span>
                                </div>
                                <div class="hero-stat">
                                    <span class="hero-stat-value">80+</span>
                                    <span class="hero-stat-label" id="stat_clients_l"></span>
                                </div>
                                <div class="hero-stat">
                                    <span class="hero-stat-value">3+</span>
                                    <span class="hero-stat-label" id="stat_years_l"></span>
                                </div>
                            </div>
                        </div>
                        <div class="hero-image-wrapper">
                            <div class="hero-image-glow"></div>
                            <div class="hero-image-card">
                                <img src="https://images.unsplash.com/photo-1636647677481-f134fda3f408?w=900&q=80"
                                    alt="Tamam Media Team">
                                <div class="hero-image-overlay"></div>
                            </div>
                            <div class="hero-float-card">
                                <div class="hero-float-card-inner">
                                    <div class="hero-float-icon">🚀</div>
                                    <div>
                                        <div class="hero-float-value">+150</div>
                                        <div class="hero-float-label" id="stat_projects_l2"></div>
                                    </div>
                                </div>
                            </div>
                            <div class="hero-badge-top">
                                <div class="hero-badge-top-text">تعز → العالم</div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Services Overview -->
            <section class="services-section">
                <div class="container">
                    <div class="section-header reveal">
                        <span class="section-tag" id="services_tag"></span>
                        <h2 class="section-title" id="services_title"></h2>
                        <p class="section-desc" id="services_sub"></p>
                    </div>
                    <div class="services-grid" id="servicesGrid"></div>
                </div>
            </section>

            <!-- About Brief -->
            <section class="about-section">
                <div class="container">
                    <div class="about-grid">
                        <div class="about-content reveal">
                            <span class="section-tag" id="about_tag"></span>
                            <h2 class="section-title" id="about_title"></h2>
                            <p class="about-desc" id="about_desc"></p>
                            <div class="about-cards">
                                <div class="about-card">
                                    <span class="about-card-icon">🔭</span>
                                    <div>
                                        <div class="about-card-label" id="about_v_label"></div>
                                        <div class="about-card-text" id="about_v_text"></div>
                                    </div>
                                </div>
                                <div class="about-card">
                                    <span class="about-card-icon">🎯</span>
                                    <div>
                                        <div class="about-card-label" id="about_m_label"></div>
                                        <div class="about-card-text" id="about_m_text"></div>
                                    </div>
                                </div>
                            </div>
                            <a href="#/about" class="btn-primary" onclick="navigate('about')">
                                <span id="about_cta"></span> →
                            </a>
                        </div>
                        <div class="reveal reveal-delay-2">
                            <div class="stats-grid">
                                <div class="stat-card stat-card-1 card-hover">
                                    <div class="stat-icon">🏆</div>
                                    <div class="stat-value">150+</div>
                                    <div class="stat-label" id="stat_projects_l3"></div>
                                </div>
                                <div class="stat-card stat-card-2 card-hover">
                                    <div class="stat-icon">😊</div>
                                    <div class="stat-value">80+</div>
                                    <div class="stat-label" id="stat_clients_l2"></div>
                                </div>
                                <div class="stat-card stat-card-3 card-hover">
                                    <div class="stat-icon">📅</div>
                                    <div class="stat-value">3+</div>
                                    <div class="stat-label" id="stat_years_l2"></div>
                                </div>
                                <div class="stat-card stat-card-4 card-hover">
                                    <div class="stat-icon">📊</div>
                                    <div class="stat-value">100%</div>
                                    <div class="stat-label" id="hero_badge3"></div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Portfolio Preview -->
            <section class="portfolio-section">
                <div class="container">
                    <div class="section-header reveal">
                        <span class="section-tag" id="port_tag"></span>
                        <h2 class="section-title" id="port_title"></h2>
                        <p class="section-desc" id="port_sub"></p>
                    </div>
                    <div class="portfolio-grid" id="portfolioGrid"></div>
                    <div class="portfolio-center reveal reveal-delay-4">
                        <a href="#/portfolio" class="btn-outline" onclick="navigate('portfolio')">
                            <span id="view_all_work"></span> →
                        </a>
                    </div>
                </div>
            </section>

            <!-- Testimonials -->
            <section class="testimonials-section">
                <div class="container">
                    <div class="section-header reveal">
                        <span class="section-tag" id="testi_tag"></span>
                        <h2 class="section-title" id="testi_title"></h2>
                    </div>
                    <div class="testimonials-grid" id="testimonialsGrid"></div>
                </div>
            </section>

            <!-- CTA -->
            <section class="cta-section">
                <div class="cta-pattern"></div>
                <div class="cta-content">
                    <div class="cta-icon">🚀</div>
                    <h2 class="cta-title" id="cta_title"></h2>
                    <p class="cta-desc" id="cta_sub"></p>
                    <a href="#/contact" class="btn-secondary" style="font-size:1.125rem;padding:1rem 2rem;"
                        onclick="navigate('contact')">
                        <span id="cta_btn"></span> →
                    </a>
                </div>
            </section>
        </div>

        <!-- ABOUT PAGE -->
        <div class="page-wrapper" id="page-about">
            <section class="page-hero">
                <div class="container">
                    <span class="section-tag" id="about_tag_p"></span>
                    <h1 class="page-hero-title" id="about_title_p"></h1>
                    <p class="page-hero-desc" id="about_desc_p"></p>
                </div>
            </section>

            <section class="values-section">
                <div class="container">
                    <div class="section-header">
                        <span class="section-tag" id="aboutp_why_title_p"></span>
                    </div>
                    <div class="values-grid" id="valuesGrid"></div>
                </div>
            </section>

            <section class="method-section">
                <div class="container">
                    <div class="section-header">
                        <span class="section-tag" id="method_title_p"></span>
                    </div>
                    <div class="method-grid" id="methodGrid"></div>
                </div>
            </section>

            <section class="cta-section">
                <div class="cta-pattern"></div>
                <div class="cta-content">
                    <div class="cta-icon">🚀</div>
                    <h2 class="cta-title" id="cta_title_about"></h2>
                    <p class="cta-desc" id="cta_sub_about"></p>
                    <a href="#/contact" class="btn-secondary" style="font-size:1.125rem;padding:1rem 2rem;"
                        onclick="navigate('contact')">
                        <span id="cta_btn_about"></span> →
                    </a>
                </div>
            </section>
        </div>

        <!-- SERVICES PAGE -->
        <div class="page-wrapper" id="page-services">
            <section class="page-hero">
                <div class="container">
                    <span class="section-tag" id="servp_tag_p"></span>
                    <h1 class="page-hero-title" id="servp_title_p"></h1>
                </div>
            </section>

            <section class="services-section" style="padding-top:3rem;">
                <div class="container">
                    <div id="servicesDetailGrid"></div>
                </div>
            </section>
        </div>

        <!-- PORTFOLIO PAGE -->
        <div class="page-wrapper" id="page-portfolio">
            <section class="page-hero">
                <div class="container">
                    <span class="section-tag" id="portp_tag_p"></span>
                    <h1 class="page-hero-title" id="portp_title_p"></h1>
                </div>
            </section>

            <section class="portfolio-section" style="padding-top:3rem;">
                <div class="container">
                    <div class="portfolio-grid" id="portfolioFullGrid"></div>
                </div>
            </section>
        </div>

        <!-- CONTACT PAGE -->
        <div class="page-wrapper" id="page-contact">
            <section class="page-hero">
                <div class="container">
                    <span class="section-tag" id="cont_tag_p"></span>
                    <h1 class="page-hero-title" id="cont_title_p"></h1>
                    <p class="page-hero-desc" id="cont_desc_p"></p>
                </div>
            </section>

            <section class="contact-section">
                <div class="container">
                    <div class="contact-grid">
                        <div class="contact-info">
                            <h2 class="contact-info-title" id="contact_info_title"></h2>
                            <p class="contact-info-desc" id="contact_info_desc"></p>
                            <ul class="contact-list">
                                <li>
                                    <span class="contact-list-icon">📍</span>
                                    <span id="location_p"></span>
                                </li>
                                <li>
                                    <span class="contact-list-icon">📧</span>
                                    <span><a href="/cdn-cgi/l/email-protection" class="__cf_email__"
                                            data-cfemail="3950575f56794d58545854545c5d5058175a5654">[email&#160;protected]</a></span>
                                </li>
                                <li>
                                    <span class="contact-list-icon">📞</span>
                                    <span dir="ltr">+967 700 123 456</span>
                                </li>
                            </ul>
                            <a href="https://wa.me/967700123456" target="_blank" class="btn-primary"
                                style="margin-top:1.5rem;background:#22c55e;">
                                <span id="whatsapp_btn_p"></span>
                                <i data-lucide="message-circle" style="width:16px;height:16px;"></i>
                            </a>
                        </div>
                        <div class="contact-form">
                            <div class="form-success" id="formSuccess">
                                <span id="form_success_p"></span>
                            </div>
                            <form onsubmit="handleSubmit(event)">
                                <div class="form-group">
                                    <label class="form-label" id="form_name_p"></label>
                                    <input type="text" class="form-input" required>
                                </div>
                                <div class="form-group">
                                    <label class="form-label" id="form_phone_p"></label>
                                    <input type="tel" class="form-input" required>
                                </div>
                                <div class="form-group">
                                    <label class="form-label" id="form_service_p"></label>
                                    <select class="form-select" id="serviceSelect"></select>
                                </div>
                                <div class="form-group">
                                    <label class="form-label" id="form_message_p"></label>
                                    <textarea class="form-textarea" required></textarea>
                                </div>
                                <button type="submit" class="btn-primary" style="width:100%;justify-content:center;">
                                    <span id="form_submit_p"></span>
                                </button>
                            </form>
                        </div>
                    </div>
                </div>
            </section>
        </div>

        <!-- NOT FOUND -->
        <div class="page-wrapper" id="page-404">
            <div class="not-found">
                <div>
                    <div class="not-found-icon">🔍</div>
                    <h1 class="not-found-title" id="not_found_title">الصفحة غير موجودة</h1>
                    <p class="not-found-desc" id="not_found_desc">عذراً، الصفحة التي تبحث عنها غير موجودة</p>
                    <a href="#/" class="btn-primary" onclick="navigate('home')">
                        <span id="not_found_btn">العودة للرئيسية</span>
                    </a>
                </div>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-grid">
                <div class="footer-brand">
                    <div class="logo">
                        <div class="logo-icon">ت</div>
                        <div class="logo-text">
                            <span class="logo-name" style="color:white;">تمام<span>.</span></span>
                            <span class="logo-sub">TAMAM MEDIA</span>
                        </div>
                    </div>
                    <p class="footer-desc" id="footer_tagline_p"></p>
                    <div class="footer-social">
                        <a href="#" class="footer-social-link" aria-label="Facebook">
                            <i data-lucide="facebook" style="width:16px;height:16px;"></i>
                        </a>
                        <a href="#" class="footer-social-link" aria-label="Instagram">
                            <i data-lucide="instagram" style="width:16px;height:16px;"></i>
                        </a>
                        <a href="https://wa.me/967700123456" class="footer-social-link" aria-label="WhatsApp"
                            target="_blank">
                            <i data-lucide="message-circle" style="width:16px;height:16px;"></i>
                        </a>
                    </div>
                </div>
                <div>
                    <h4 class="footer-title" id="footer_quick_p"></h4>
                    <ul class="footer-links">
                        <li><a href="#/" class="footer-link" onclick="navigate('home')" id="footer_home"></a></li>
                        <li><a href="#/about" class="footer-link" onclick="navigate('about')" id="footer_about"></a>
                        </li>
                        <li><a href="#/services" class="footer-link" onclick="navigate('services')"
                                id="footer_services"></a></li>
                        <li><a href="#/portfolio" class="footer-link" onclick="navigate('portfolio')"
                                id="footer_portfolio"></a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="footer-title" id="footer_contact_col_p"></h4>
                    <div class="footer-contact-item">
                        <span class="footer-contact-icon">📍</span>
                        <span id="footer_location"></span>
                    </div>
                    <div class="footer-contact-item">
                        <span class="footer-contact-icon">📧</span>
                        <span><a href="/cdn-cgi/l/email-protection" class="__cf_email__"
                                data-cfemail="d2bbbcb4bd92a6b3bfb3bfbfb7b6bbb3fcb1bdbf">[email&#160;protected]</a></span>
                    </div>
                    <div class="footer-contact-item">
                        <span class="footer-contact-icon">📞</span>
                        <span dir="ltr">+967 700 123 456</span>
                    </div>
                </div>
            </div>
            <div class="footer-bottom">
                <p class="footer-copyright">© 2025 تمام ميديا | Tamam Media — <span id="footer_rights_p"></span></p>
                <p class="footer-made">Made with ❤️ in Taiz, Yemen</p>
            </div>
        </div>
    </footer>

    <!-- WhatsApp FAB -->
    <a href="https://wa.me/967700123456" target="_blank" class="whatsapp-fab" aria-label="WhatsApp">
        <i data-lucide="message-circle" style="width:28px;height:28px;"></i>
    </a>

    <script data-cfasync="false" src="/cdn-cgi/scripts/5c5dd728/cloudflare-static/email-decode.min.js" defer></script>
    <script>
        // ── Translations Data ──
        const translations = {
            ar: {
                nav_home: "الرئيسية",
                nav_about: "من نحن",
                nav_services: "خدماتنا",
                nav_portfolio: "أعمالنا",
                nav_contact: "اتصل بنا",
                hero_headline: "نحو حضور أقوى…",
                hero_headline2: "ونمو أذكى",
                hero_sub: "حلول إعلامية وتسويقية رقمية متكاملة تصل بك إلى جمهورك بثقة وفعالية، انطلاقاً من تعز نحو كل اليمن والعالم.",
                hero_cta1: "ابدأ مشروعك",
                hero_cta2: "تعرف علينا",
                hero_badge2: "خبرة محلية",
                hero_badge3: "نتائج قابلة للقياس",
                services_tag: "خدماتنا",
                services_title: "خدمات متكاملة تحت سقف واحد",
                services_sub: "نقدم حلولاً شاملة تحول علامتك التجارية إلى قوة رقمية فاعلة",
                s1_title: "الهوية البصرية",
                s1_desc: "نصمم هوية بصرية متكاملة تعكس قيم علامتك وتترك أثراً لا يُنسى لدى جمهورك.",
                s2_title: "إدارة السوشيال ميديا",
                s2_desc: "إدارة احترافية للمنصات الاجتماعية مع إنتاج محتوى إبداعي وحملات مدروسة لزيادة التفاعل.",
                s3_title: "الإنتاج الإعلامي",
                s3_desc: "تصوير فوتوغرافي، إنتاج فيديو، موشن جرافيك وتصميم إعلانات بجودة عالية تنافس العالمية.",
                s4_title: "تطوير المواقع",
                s4_desc: "بناء مواقع ومتاجر إلكترونية سريعة ومتجاوبة وآمنة تدعم نمو أعمالك تقنياً.",
                s5_title: "الحملات التسويقية",
                s5_desc: "تخطيط وتنفيذ حملات إعلانية مدفوعة (ميتا، جوجل) بأعلى عائد على الاستثمار.",
                s6_title: "حلول النمو",
                s6_desc: "استشارات استراتيجية وخطط نمو مخصصة لتوسيع أعمالك وزيادة حصتك السوقية.",
                learn_more: "اعرف أكثر",
                about_tag: "من نحن",
                about_title: "قصة تمام ميديا",
                about_desc: "انطلقت تمام ميديا من تعز – اليمن، بهدف تقديم بديل محلي متكامل يليق بطموح الشركات والأفراد. نجمع بين الخبرة الإعلامية والتقنية لنصنع حلولاً ذكية ومؤثرة.",
                about_v_label: "رؤيتنا",
                about_v_text: "ريادة الإعلام الرقمي المتكامل في اليمن وأن نكون الشريك الأول لكل من يبني حضوراً مؤثراً.",
                about_m_label: "رسالتنا",
                about_m_text: "تقديم حلول إعلامية وتسويقية عالية الجودة بأسعار مناسبة مع مراعاة خصوصية السوق المحلي.",
                about_cta: "اقرأ قصتنا كاملة",
                stat_projects_l: "مشروع ناجح",
                stat_clients_l: "عميل سعيد",
                stat_years_l: "سنوات خبرة",
                port_tag: "أعمالنا",
                port_title: "مشاريع نفخر بها",
                port_sub: "نماذج من أعمالنا الناجحة في مجالات متعددة",
                view_all_work: "استعراض كل الأعمال",
                testi_tag: "آراء العملاء",
                testi_title: "ماذا يقول عملاؤنا؟",
                cta_title: "هل أنت مستعد لتعزيز حضورك الرقمي؟",
                cta_sub: "تواصل مع فريقنا اليوم واحصل على استشارة مجانية لمشروعك",
                cta_btn: "طلب استشارة مجانية",
                footer_tagline: "نحو حضور أقوى، ونمو أذكى",
                footer_rights: "جميع الحقوق محفوظة",
                footer_quick: "روابط سريعة",
                footer_services_col: "خدماتنا",
                footer_contact_col: "تواصل معنا",
                location: "تعز، اليمن",
                aboutp_story_title: "قصتنا",
                aboutp_why_title: "لماذا تمام ميديا؟",
                val1: "تمام الإتقان",
                val2: "الواقعية والمرونة",
                val3: "الشفافية والشراكة",
                val4: "التأثير المحلي",
                method_title: "منهجية عملنا",
                step1_title: "تحليل وفهم",
                step1_desc: "ندرس السوق والجمهور والمنافسين بعمق لوضع أساس متين للاستراتيجية.",
                step2_title: "استراتيجية مخصصة",
                step2_desc: "نضع خطة عمل مخصصة تماماً لأهدافك وميزانيتك وجمهورك المستهدف.",
                step3_title: "تنفيذ إبداعي",
                step3_desc: "إنتاج احترافي بأحدث الأدوات وأفضل المواهب لضمان أعلى جودة.",
                step4_title: "قياس وتحسين",
                step4_desc: "متابعة مستمرة للنتائج وتحسين مستمر لضمان أفضل عائد على استثمارك.",
                servp_tag: "خدماتنا التفصيلية",
                servp_title: "حلول مصممة لنجاحك",
                benefits: "الفوائد",
                audience: "الجمهور المستهدف",
                portp_tag: "معرض الأعمال",
                portp_title: "أعمالنا المميزة",
                cont_tag: "تواصل معنا",
                cont_title: "نحن هنا لمساعدتك",
                cont_desc: "سواء كنت تريد تطوير هويتك، إطلاق حملة تسويقية، أو بناء موقع جديد — فريقنا جاهز للحديث معك.",
                form_name: "الاسم الكامل",
                form_phone: "رقم الهاتف",
                form_service: "الخدمة المطلوبة",
                form_message: "تفاصيل مشروعك",
                form_submit: "إرسال الرسالة",
                form_success: "تم إرسال رسالتك بنجاح! سنتواصل معك قريباً.",
                whatsapp_btn: "راسلنا على واتساب",
                langLabel: "EN",
                not_found_title: "الصفحة غير موجودة",
                not_found_desc: "عذراً، الصفحة التي تبحث عنها غير موجودة",
                not_found_btn: "العودة للرئيسية",
                contact_info_title: "معلومات التواصل",
                contact_info_desc: "نحن هنا للإجابة على استفساراتك ومساعدتك في تحقيق أهدافك الرقمية."
            },
            en: {
                nav_home: "Home",
                nav_about: "About",
                nav_services: "Services",
                nav_portfolio: "Portfolio",
                nav_contact: "Contact",
                hero_headline: "Towards a Stronger Presence…",
                hero_headline2: "And Smarter Growth",
                hero_sub: "Integrated media and digital marketing solutions that connect you with your audience confidently, launching from Taiz to all of Yemen and beyond.",
                hero_cta1: "Start Your Project",
                hero_cta2: "Learn About Us",
                hero_badge2: "Local Expertise",
                hero_badge3: "Measurable Results",
                services_tag: "Our Services",
                services_title: "Integrated Services Under One Roof",
                services_sub: "We deliver comprehensive solutions that transform your brand into a powerful digital force",
                s1_title: "Branding & Identity",
                s1_desc: "We craft complete visual identities that reflect your brand values and leave a lasting impression on your audience.",
                s2_title: "Social Media Management",
                s2_desc: "Professional social platform management with creative content production and strategic campaigns to boost engagement.",
                s3_title: "Media Production",
                s3_desc: "Photography, video production, motion graphics and ad design with world-class quality.",
                s4_title: "Web Development",
                s4_desc: "Building fast, responsive, and secure websites and e-commerce stores to support your business growth.",
                s5_title: "Marketing Campaigns",
                s5_desc: "Planning and executing paid ad campaigns (Meta, Google) with maximum return on investment.",
                s6_title: "Growth Solutions",
                s6_desc: "Strategic consulting and custom growth plans to expand your business and increase market share.",
                learn_more: "Learn More",
                about_tag: "Who We Are",
                about_title: "The Tamam Media Story",
                about_desc: "Tamam Media launched from Taiz, Yemen, aiming to provide a comprehensive local alternative worthy of businesses' and individuals' ambitions. We combine media and technical expertise to create smart, impactful solutions.",
                about_v_label: "Our Vision",
                about_v_text: "To lead integrated digital media in Yemen and be the first partner for everyone building an impactful presence.",
                about_m_label: "Our Mission",
                about_m_text: "Delivering high-quality media and marketing solutions at affordable prices while respecting local market needs.",
                about_cta: "Read Our Full Story",
                stat_projects_l: "Projects Completed",
                stat_clients_l: "Happy Clients",
                stat_years_l: "Years Experience",
                port_tag: "Our Work",
                port_title: "Projects We're Proud Of",
                port_sub: "Samples from our successful projects across multiple fields",
                view_all_work: "View All Works",
                testi_tag: "Client Testimonials",
                testi_title: "What Do Our Clients Say?",
                cta_title: "Ready to Boost Your Digital Presence?",
                cta_sub: "Connect with our team today and get a free consultation for your project",
                cta_btn: "Request Free Consultation",
                footer_tagline: "Towards stronger presence, smarter growth",
                footer_rights: "All Rights Reserved",
                footer_quick: "Quick Links",
                footer_services_col: "Services",
                footer_contact_col: "Contact Us",
                location: "Taiz, Yemen",
                aboutp_story_title: "Our Story",
                aboutp_why_title: "Why Tamam Media?",
                val1: "Total Excellence",
                val2: "Realism & Flexibility",
                val3: "Transparency & Partnership",
                val4: "Local Impact",
                method_title: "Our Work Methodology",
                step1_title: "Analysis & Discovery",
                step1_desc: "We deeply study the market, audience and competitors to build a solid strategic foundation.",
                step2_title: "Custom Strategy",
                step2_desc: "We create a work plan fully customized to your goals, budget and target audience.",
                step3_title: "Creative Execution",
                step3_desc: "Professional production with the latest tools and best talents to ensure the highest quality.",
                step4_title: "Measure & Improve",
                step4_desc: "Continuous monitoring of results and ongoing improvement to ensure the best return on your investment.",
                servp_tag: "Our Detailed Services",
                servp_title: "Solutions Designed for Your Success",
                benefits: "Benefits",
                audience: "Target Audience",
                portp_tag: "Work Portfolio",
                portp_title: "Our Featured Work",
                cont_tag: "Get in Touch",
                cont_title: "We're Here to Help You",
                cont_desc: "Whether you want to develop your identity, launch a marketing campaign, or build a new website — our team is ready to talk with you.",
                form_name: "Full Name",
                form_phone: "Phone Number",
                form_service: "Service Requested",
                form_message: "Project Details",
                form_submit: "Send Message",
                form_success: "Your message was sent successfully! We'll contact you soon.",
                whatsapp_btn: "Chat on WhatsApp",
                langLabel: "عربي",
                not_found_title: "Page Not Found",
                not_found_desc: "Sorry, the page you're looking for doesn't exist",
                not_found_btn: "Back to Home",
                contact_info_title: "Contact Information",
                contact_info_desc: "We're here to answer your questions and help you achieve your digital goals."
            }
        };

        // ── Data ──
        const services = [
            { id: "branding", icon: "🎨", titleKey: "s1_title", descKey: "s1_desc", color: "rgba(20, 184, 166, 0.1)" },
            { id: "social", icon: "📱", titleKey: "s2_title", descKey: "s2_desc", color: "rgba(249, 115, 22, 0.1)" },
            { id: "media", icon: "🎬", titleKey: "s3_title", descKey: "s3_desc", color: "rgba(139, 92, 246, 0.1)" },
            { id: "web", icon: "💻", titleKey: "s4_title", descKey: "s4_desc", color: "rgba(59, 130, 246, 0.1)" },
            { id: "campaigns", icon: "📢", titleKey: "s5_title", descKey: "s5_desc", color: "rgba(244, 63, 94, 0.1)" },
            { id: "growth", icon: "📈", titleKey: "s6_title", descKey: "s6_desc", color: "rgba(34, 197, 94, 0.1)" }
        ];

        const portfolioItems = [
            { id: "p1", titleAr: "هوية مطعم السعادة", titleEn: "Al-Saada Restaurant Branding", category: "branding", image: "https://images.unsplash.com/photo-1597979732130-9d2ad18df38b?w=600&q=80", descAr: "هوية بصرية متكاملة لمطعم فاخر", descEn: "Complete visual identity for a luxury restaurant" },
            { id: "p2", titleAr: "فيديو تعريفي لشركة أوج", titleEn: "Awj Corp Intro Video", category: "video", image: "https://images.unsplash.com/photo-1492724441997-5dc865305da7?w=600&q=80", descAr: "فيلم تعريفي احترافي لشركة استثمارية", descEn: "Professional intro video for an investment company" },
            { id: "p3", titleAr: "حملة رمضان التجارية", titleEn: "Ramadan Social Campaign", category: "social", image: "https://images.unsplash.com/photo-1611162617474-5b21e879e113?w=600&q=80", descAr: "حملة سوشيال ميديا رمضانية متكاملة", descEn: "Integrated Ramadan social media campaign" },
            { id: "p4", titleAr: "متجر أزياء العراقة", titleEn: "Al-Iraqa Fashion Store", category: "web", image: "https://images.unsplash.com/photo-1636647677481-f134fda3f408?w=600&q=80", descAr: "متجر إلكتروني متكامل للأزياء", descEn: "Full e-commerce fashion store" },
            { id: "p5", titleAr: "شعار وهوية نخبة للتعليم", titleEn: "Nukhba Education Logo & Identity", category: "branding", image: "https://images.unsplash.com/photo-1649000809102-61d0fe6759b9?w=600&q=80", descAr: "هوية بصرية لمركز تعليمي متميز", descEn: "Visual identity for a prestigious educational center" },
            { id: "p6", titleAr: "فيديو ترويجي لمنتج", titleEn: "Product Promotional Video", category: "video", image: "https://images.unsplash.com/photo-1582005450386-52b25f82d9bb?w=600&q=80", descAr: "فيديو ترويجي احترافي لإطلاق منتج جديد", descEn: "Professional promotional video for a new product launch" }
        ];

        const testimonials = [
            { nameAr: "أحمد المقبلي", nameEn: "Ahmed Al-Maqbali", roleAr: "مدير مطعم السعادة", roleEn: "Manager, Al-Saada Restaurant", textAr: "تمام ميديا غيّرت حضورنا الرقمي بشكل جذري. الهوية التي صمموها لنا زادت من ثقة عملائنا بنا ورفعت من مستوى مطعمنا.", textEn: "Tamam Media radically changed our digital presence. The identity they designed for us increased our clients' trust and elevated our restaurant's level.", rating: 5, avatar: "أ" },
            { nameAr: "أروى الجابري", nameEn: "Arwa Al-Jabri", roleAr: "مالكة متجر إلكتروني", roleEn: "E-commerce Store Owner", textAr: "الموقع الذي بنوه لمتخري فاق توقعاتي، سريع، جميل، وزاد مبيعاتي بنسبة ٧٠٪ في أول شهرين.", textEn: "The website they built for my store exceeded my expectations — fast, beautiful, and increased my sales by 70% in the first two months.", rating: 5, avatar: "أ" },
            { nameAr: "خالد العنسي", nameEn: "Khaled Al-Ansi", roleAr: "مؤسس شركة ناشئة", roleEn: "Startup Founder", textAr: "فريق محترف ومبدع يعمل بروح الفريق الواحد. الحملة الإعلانية التي نفذوها جلبت لنا عملاء جدد بتكلفة منخفضة جداً.", textEn: "A professional and creative team working with a unified team spirit. The ad campaign they executed brought us new clients at a very low cost.", rating: 5, avatar: "خ" }
        ];

        const values = [
            { icon: "✨", key: "val1" },
            { icon: "🔄", key: "val2" },
            { icon: "🤝", key: "val3" },
            { icon: "🌍", key: "val4" }
        ];

        const methodSteps = [
            { num: "01", titleKey: "step1_title", descKey: "step1_desc" },
            { num: "02", titleKey: "step2_title", descKey: "step2_desc" },
            { num: "03", titleKey: "step3_title", descKey: "step3_desc" },
            { num: "04", titleKey: "step4_title", descKey: "step4_desc" }
        ];

        // ── State ──
        let currentLang = 'ar';
        let mobileMenuOpen = false;

        // ── Translation Function ──
        function t(key) {
            return translations[currentLang][key] || key;
        }

        // ── Update All Translations ──
        function updateTranslations() {
            // Navbar
            document.getElementById('nav_home').textContent = t('nav_home');
            document.getElementById('nav_about').textContent = t('nav_about');
            document.getElementById('nav_services').textContent = t('nav_services');
            document.getElementById('nav_portfolio').textContent = t('nav_portfolio');
            document.getElementById('nav_contact').textContent = t('nav_contact');
            document.getElementById('nav_cta').textContent = t('nav_contact');
            document.getElementById('langBtn').textContent = t('langLabel');
            // Mobile
            document.getElementById('mobile_nav_home').textContent = t('nav_home');
            document.getElementById('mobile_nav_about').textContent = t('nav_about');
            document.getElementById('mobile_nav_services').textContent = t('nav_services');
            document.getElementById('mobile_nav_portfolio').textContent = t('nav_portfolio');
            document.getElementById('mobile_nav_contact').textContent = t('nav_contact');

            // Hero
            document.getElementById('hero_badge2').textContent = t('hero_badge2');
            document.getElementById('hero_headline').textContent = t('hero_headline');
            document.getElementById('hero_headline2').textContent = t('hero_headline2');
            document.getElementById('hero_sub').textContent = t('hero_sub');
            document.getElementById('hero_cta1').textContent = t('hero_cta1');
            document.getElementById('hero_cta2').textContent = t('hero_cta2');
            document.getElementById('hero_badge3').textContent = t('hero_badge3');

            // Stats
            document.getElementById('stat_projects_l').textContent = t('stat_projects_l');
            document.getElementById('stat_projects_l2').textContent = t('stat_projects_l');
            document.getElementById('stat_projects_l3').textContent = t('stat_projects_l');
            document.getElementById('stat_clients_l').textContent = t('stat_clients_l');
            document.getElementById('stat_clients_l2').textContent = t('stat_clients_l');
            document.getElementById('stat_years_l').textContent = t('stat_years_l');
            document.getElementById('stat_years_l2').textContent = t('stat_years_l');

            // Services
            document.getElementById('services_tag').textContent = t('services_tag');
            document.getElementById('services_title').textContent = t('services_title');
            document.getElementById('services_sub').textContent = t('services_sub');

            // About
            document.getElementById('about_tag').textContent = t('about_tag');
            document.getElementById('about_title').textContent = t('about_title');
            document.getElementById('about_desc').textContent = t('about_desc');
            document.getElementById('about_v_label').textContent = t('about_v_label');
            document.getElementById('about_v_text').textContent = t('about_v_text');
            document.getElementById('about_m_label').textContent = t('about_m_label');
            document.getElementById('about_m_text').textContent = t('about_m_text');
            document.getElementById('about_cta').textContent = t('about_cta');

            // Portfolio
            document.getElementById('port_tag').textContent = t('port_tag');
            document.getElementById('port_title').textContent = t('port_title');
            document.getElementById('port_sub').textContent = t('port_sub');
            document.getElementById('view_all_work').textContent = t('view_all_work');

            // Testimonials
            document.getElementById('testi_tag').textContent = t('testi_tag');
            document.getElementById('testi_title').textContent = t('testi_title');

            // CTA
            document.getElementById('cta_title').textContent = t('cta_title');
            document.getElementById('cta_sub').textContent = t('cta_sub');
            document.getElementById('cta_btn').textContent = t('cta_btn');

            // Footer
            document.getElementById('footer_tagline_p').textContent = t('footer_tagline');
            document.getElementById('footer_rights_p').textContent = t('footer_rights');
            document.getElementById('footer_quick_p').textContent = t('footer_quick');
            document.getElementById('footer_contact_col_p').textContent = t('footer_contact_col');
            document.getElementById('footer_home').textContent = t('nav_home');
            document.getElementById('footer_about').textContent = t('nav_about');
            document.getElementById('footer_services').textContent = t('nav_services');
            document.getElementById('footer_portfolio').textContent = t('nav_portfolio');
            document.getElementById('footer_location').textContent = t('location');

            // About Page
            document.getElementById('about_tag_p').textContent = t('about_tag');
            document.getElementById('about_title_p').textContent = t('about_title');
            document.getElementById('about_desc_p').textContent = t('about_desc');
            document.getElementById('aboutp_why_title_p').textContent = t('aboutp_why_title');
            document.getElementById('method_title_p').textContent = t('method_title');
            document.getElementById('cta_title_about').textContent = t('cta_title');
            document.getElementById('cta_sub_about').textContent = t('cta_sub');
            document.getElementById('cta_btn_about').textContent = t('cta_btn');

            // Services Page
            document.getElementById('servp_tag_p').textContent = t('servp_tag');
            document.getElementById('servp_title_p').textContent = t('servp_title');

            // Portfolio Page
            document.getElementById('portp_tag_p').textContent = t('portp_tag');
            document.getElementById('portp_title_p').textContent = t('portp_title');

            // Contact Page
            document.getElementById('cont_tag_p').textContent = t('cont_tag');
            document.getElementById('cont_title_p').textContent = t('cont_title');
            document.getElementById('cont_desc_p').textContent = t('cont_desc');
            document.getElementById('location_p').textContent = t('location');
            document.getElementById('whatsapp_btn_p').textContent = t('whatsapp_btn');
            document.getElementById('form_name_p').textContent = t('form_name');
            document.getElementById('form_phone_p').textContent = t('form_phone');
            document.getElementById('form_service_p').textContent = t('form_service');
            document.getElementById('form_message_p').textContent = t('form_message');
            document.getElementById('form_submit_p').textContent = t('form_submit');
            document.getElementById('form_success_p').textContent = t('form_success');
            document.getElementById('contact_info_title').textContent = t('contact_info_title');
            document.getElementById('contact_info_desc').textContent = t('contact_info_desc');

            // 404
            document.getElementById('not_found_title').textContent = t('not_found_title');
            document.getElementById('not_found_desc').textContent = t('not_found_desc');
            document.getElementById('not_found_btn').textContent = t('not_found_btn');

            // Services Dropdown
            const select = document.getElementById('serviceSelect');
            if (select) {
                select.innerHTML = `<option value="">${t('form_service')}</option>` +
                    services.map(s => `<option value="${s.id}">${t(s.titleKey)}</option>`).join('');
            }

            // Update direction
            document.documentElement.dir = currentLang === 'ar' ? 'rtl' : 'ltr';
            document.documentElement.lang = currentLang;

            // Update arrow directions
            updateArrowDirections();
        }

        function updateArrowDirections() {
            const arrows = document.querySelectorAll('[data-arrow]');
            arrows.forEach(arrow => {
                arrow.innerHTML = currentLang === 'ar'
                    ? '<i data-lucide="arrow-left" style="width:16px;height:16px;"></i>'
                    : '<i data-lucide="arrow-right" style="width:16px;height:16px;"></i>';
            });
            lucide.createIcons();
        }

        // ── Render Components ──
        function renderServicesGrid() {
            const grid = document.getElementById('servicesGrid');
            grid.innerHTML = services.map((s, i) => `
        <div class="service-card card-hover reveal reveal-delay-${(i % 3) + 1}">
          <div class="service-card-inner" style="background:${s.color};">
            <div class="service-icon">${s.icon}</div>
            <h3 class="service-title">${t(s.titleKey)}</h3>
            <p class="service-desc">${t(s.descKey)}</p>
            <a href="#/services" class="service-link" onclick="navigate('services')">
              ${t('learn_more')} →
            </a>
          </div>
        </div>
      `).join('');
        }

        function renderPortfolioGrid(containerId, items) {
            const grid = document.getElementById(containerId);
            grid.innerHTML = items.map(item => `
        <div class="portfolio-card reveal">
          <img src="${item.image}" alt="${currentLang === 'ar' ? item.titleAr : item.titleEn}" loading="lazy">
          <div class="portfolio-overlay">
            <div class="portfolio-content">
              <span class="portfolio-category">${item.category}</span>
              <h3 class="portfolio-title">${currentLang === 'ar' ? item.titleAr : item.titleEn}</h3>
            </div>
          </div>
        </div>
      `).join('');
        }

        function renderTestimonials() {
            const grid = document.getElementById('testimonialsGrid');
            grid.innerHTML = testimonials.map((testimonial, i) => `
        <div class="testimonial-card reveal reveal-delay-${i + 1}">
          <div class="testimonial-stars">
            ${Array(testimonial.rating).fill('<i data-lucide="star" class="testimonial-star" style="width:16px;height:16px;fill:#F39C12;color:#F39C12;"></i>').join('')}
          </div>
          <p class="testimonial-text">"${currentLang === 'ar' ? testimonial.textAr : testimonial.textEn}"</p>
          <div class="testimonial-author">
            <div class="testimonial-avatar">${testimonial.avatar}</div>
            <div>
              <div class="testimonial-name">${currentLang === 'ar' ? testimonial.nameAr : testimonial.nameEn}</div>
              <div class="testimonial-role">${currentLang === 'ar' ? testimonial.roleAr : testimonial.roleEn}</div>
            </div>
          </div>
        </div>
      `).join('');
        }

        function renderValues() {
            const grid = document.getElementById('valuesGrid');
            grid.innerHTML = values.map(value => `
        <div class="value-card reveal">
          <div class="value-icon">${value.icon}</div>
          <h3 class="value-title">${t(value.key)}</h3>
        </div>
      `).join('');
        }

        function renderMethod() {
            const grid = document.getElementById('methodGrid');
            grid.innerHTML = methodSteps.map(step => `
        <div class="method-card reveal">
          <div class="method-number">${step.num}</div>
          <h3 class="method-title">${t(step.titleKey)}</h3>
          <p class="method-desc">${t(step.descKey)}</p>
        </div>
      `).join('');
        }

        function renderServicesDetail() {
            const grid = document.getElementById('servicesDetailGrid');
            grid.innerHTML = services.map(service => `
        <div class="service-detail-card reveal">
          <div class="service-detail-icon">${service.icon}</div>
          <h3 class="service-detail-title">${t(service.titleKey)}</h3>
          <p class="service-detail-desc">${t(service.descKey)}</p>
          <h4 style="font-weight:700;margin-bottom:0.5rem;">${t('benefits')}</h4>
          <ul class="benefits-list">
            ${service.benefits.map(b => `<li>${currentLang === 'ar' ? b.ar : b.en}</li>`).join('')}
          </ul>
          <div class="audience-tag">
            <strong>${t('audience')}:</strong>
            <span style="margin-right:0.25rem;">${service.audience}</span>
          </div>
        </div>
      `).join('');
        }

        // ── Navigation ──
        function navigate(page) {
            // Hide all pages
            document.querySelectorAll('.page-wrapper').forEach(p => p.classList.remove('active'));

            // Show target page
            const targetPage = document.getElementById(`page-${page}`);
            if (targetPage) {
                targetPage.classList.add('active');
            } else {
                document.getElementById('page-404').classList.add('active');
            }

            // Update active nav link
            document.querySelectorAll('.nav-link, .mobile-menu-link').forEach(link => {
                link.classList.remove('active');
                if (link.dataset.page === page) {
                    link.classList.add('active');
                }
            });

            // Close mobile menu
            mobileMenuOpen = false;
            document.getElementById('mobileMenu').classList.remove('open');

            // Scroll to top
            window.scrollTo({ top: 0, behavior: 'smooth' });

            // Update URL
            window.location.hash = page === 'home' ? '/' : `/${page}`;

            // Re-initialize icons
            lucide.createIcons();

            // Re-run reveal animations
            setTimeout(initReveal, 100);

            return false;
        }

        function handleHashChange() {
            const hash = window.location.hash.slice(2) || 'home';
            navigate(hash);
        }

        // ── Mobile Menu ──
        function toggleMobile() {
            mobileMenuOpen = !mobileMenuOpen;
            const menu = document.getElementById('mobileMenu');
            if (mobileMenuOpen) {
                menu.classList.add('open');
            } else {
                menu.classList.remove('open');
            }
        }

        // ── Language Toggle ──
        function toggleLang() {
            currentLang = currentLang === 'ar' ? 'en' : 'ar';
            updateTranslations();
            renderServicesGrid();
            renderPortfolioGrid('portfolioGrid', portfolioItems.slice(0, 3));
            renderPortfolioGrid('portfolioFullGrid', portfolioItems);
            renderTestimonials();
            renderValues();
            renderMethod();
            renderServicesDetail();
        }

        // ── Form Submit ──
        function handleSubmit(e) {
            e.preventDefault();
            document.getElementById('formSuccess').classList.add('show');
            setTimeout(() => {
                document.getElementById('formSuccess').classList.remove('show');
                e.target.reset();
            }, 3000);
        }

        // ── Scroll Handler ──
        function handleScroll() {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
        }

        // ── Reveal Animation ──
        function initReveal() {
            const reveals = document.querySelectorAll('.reveal');
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            }, { threshold: 0.1 });

            reveals.forEach(el => observer.observe(el));
        }

        // ── Initialize ──
        function init() {
            // Initialize icons
            lucide.createIcons();

            // Update translations
            updateTranslations();

            // Render components
            renderServicesGrid();
            renderPortfolioGrid('portfolioGrid', portfolioItems.slice(0, 3));
            renderPortfolioGrid('portfolioFullGrid', portfolioItems);
            renderTestimonials();
            renderValues();
            renderMethod();
            renderServicesDetail();

            // Event listeners
            window.addEventListener('scroll', handleScroll, { passive: true });
            window.addEventListener('hashchange', handleHashChange);

            // Handle initial route
            handleHashChange();

            // Init reveal animations
            initReveal();
        }

        // Run on DOM ready
        document.addEventListener('DOMContentLoaded', init);
    </script>
</body>

</html>
