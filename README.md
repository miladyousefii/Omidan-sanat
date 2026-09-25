<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Google Search Console Verification -->
    <meta name="google-site-verification" content="dGUUkB_gNbh0UmdzlG26A-icTRoczYw6CFBjdpbC48I" />

    <title>میلاد یوسفی | مهندس راه‌اندازی بیسیم و شبکه‌های رادیویی</title>

    <meta name="description" content="میلاد یوسفی - مهندس راه‌اندازی بیسیم موتورولا، شبکه‌های رادیویی و سایت‌های تکرارکننده در قائمشهر، مازندران و سراسر ایران. همکاری با شرکت امیدان صنعت.">

    <meta name="keywords" content="مهندس بیسیم, راه اندازی بیسیم, مهندس راه اندازی بیسیم, راه اندازی بیسیم موتورولا, راه اندازی سایت بیسیم, شرکت امیدان صنعت, بیسیم مازندران, بیسیم قائمشهر, 09048818508">

    <!-- فونت وزیرمتن -->
    <link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Vazirmatn-font-face.css" rel="stylesheet" type="text/css">

    <style>
        :root {
            --bg-dark: #070a14;
            --bg-card: rgba(15, 23, 42, 0.75);
            --blue-glow: #3b82f6;
            --gold-primary: #f59e0b;
            --gold-light: #fbbf24;
            --gold-gradient: linear-gradient(
                135deg,
                #d97706 0%,
                #f59e0b 50%,
                #fef08a 100%
            );
            --text-main: #f8fafc;
            --text-sub: #94a3b8;
        }

        *,
        *::before,
        *::after {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html,
        body {
            width: 100%;
            max-width: 100%;
            overflow-x: hidden !important;
            position: relative;
            background-color: var(--bg-dark);
            color: var(--text-main);
            line-height: 1.8;
            font-family: 'Vazirmatn', sans-serif;
            min-height: 100vh;
        }

        /* پس‌زمینه امواج رادیویی */
        .radio-waves-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: radial-gradient(
                circle at 50% 15%,
                #0f1c3f 0%,
                #070a14 75%
            );
            overflow: hidden;
            pointer-events: none;
        }

        .wave-line {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            background: repeating-radial-gradient(
                circle at 50% 30%,
                transparent 0,
                transparent 30px,
                rgba(59, 130, 246, 0.05) 31px,
                transparent 32px
            );
            animation: wavePulse 12s infinite linear;
            pointer-events: none;
        }

        @keyframes wavePulse {
            0% {
                transform: scale(0.95);
                opacity: 0.3;
            }

            50% {
                transform: scale(1.05);
                opacity: 0.7;
            }

            100% {
                transform: scale(0.95);
                opacity: 0.3;
            }
        }

        /* هیرو */
        .hero {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 50px 15px 25px;
            text-align: center;
            position: relative;
            width: 100%;
        }

        .antenna-container {
            position: relative;
            width: 120px;
            height: 120px;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(15, 23, 42, 0.8);
            border-radius: 50%;
            border: 3px solid var(--gold-primary);
            box-shadow:
                0 0 30px rgba(245, 158, 11, 0.3),
                inset 0 0 15px rgba(59, 130, 246, 0.4);
        }

        .pulse-ring {
            position: absolute;
            border: 2px solid var(--gold-primary);
            border-radius: 50%;
            animation: ringExpand 3s infinite
                cubic-bezier(0.215, 0.61, 0.355, 1);
            opacity: 0;
            pointer-events: none;
        }

        .pulse-ring:nth-child(1) {
            animation-delay: 0s;
        }

        .pulse-ring:nth-child(2) {
            animation-delay: 1s;
        }

        .pulse-ring:nth-child(3) {
            animation-delay: 2s;
        }

        @keyframes ringExpand {
            0% {
                width: 120px;
                height: 120px;
                opacity: 0.8;
                border-color: var(--gold-primary);
            }

            50% {
                border-color: var(--blue-glow);
            }

            100% {
                width: 220px;
                height: 220px;
                opacity: 0;
            }
        }

        .antenna-icon {
            width: 55px;
            height: 55px;
            fill: url(#goldGradient);
            z-index: 2;
        }

        .hero h1 {
            font-size: 2.1rem;
            font-weight: 900;
            background: var(--gold-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 8px;
            word-break: break-word;
        }

        .hero h2 {
            font-size: 1.1rem;
            color: #e2e8f0;
            font-weight: 500;
            margin-bottom: 18px;
            word-break: break-word;
        }

        .badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
            max-width: 100%;
        }

        .badge {
            background: rgba(30, 58, 138, 0.4);
            border: 1px solid rgba(59, 130, 246, 0.4);
            color: #f1f5f9;
            padding: 6px 14px;
            border-radius: 30px;
            font-size: 0.85rem;
            backdrop-filter: blur(8px);
            max-width: 100%;
        }

        .badge.gold-badge {
            background: rgba(245, 158, 11, 0.15);
            border-color: var(--gold-primary);
            color: var(--gold-light);
            font-weight: 600;
        }

        /* کانتینر */
        .container {
            max-width: 900px;
            width: 100%;
            margin: 0 auto;
            padding: 0 15px 30px;
        }

        .card {
            background: var(--bg-card);
            border: 1px solid rgba(245, 158, 11, 0.25);
            border-radius: 18px;
            padding: 24px 18px;
            margin-bottom: 20px;
            backdrop-filter: blur(16px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.4);
            word-wrap: break-word;
            overflow-wrap: break-word;
        }

        .card-title {
            font-size: 1.2rem;
            color: var(--gold-light);
            border-right: 4px solid var(--gold-primary);
            padding-right: 12px;
            margin-bottom: 16px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(
                auto-fit,
                minmax(240px, 1fr)
            );
            gap: 15px;
            width: 100%;
        }

        .service-box {
            background: rgba(10, 15, 30, 0.7);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 12px;
            padding: 16px;
            border-right: 3px solid var(--blue-glow);
        }

        .service-box h4 {
            color: #ffffff;
            font-size: 0.98rem;
            margin-bottom: 8px;
        }

        .service-box p {
            color: var(--text-sub);
            font-size: 0.88rem;
            line-height: 1.7;
        }

        /* دکمه تماس */
        .cta-wrapper {
            text-align: center;
            margin-top: 25px;
            width: 100%;
        }

        .btn-call {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            background: var(--gold-gradient);
            color: #0d1322;
            font-weight: 800;
            font-size: 1.05rem;
            padding: 14px 25px;
            border-radius: 50px;
            text-decoration: none;
            box-shadow: 0 0 25px rgba(245, 158, 11, 0.4);
            max-width: 100%;
            text-align: center;
        }

        /* فوتر */
        footer {
            text-align: center;
            padding: 25px 15px;
            color: var(--text-sub);
            font-size: 0.85rem;
            border-top: 1px solid rgba(255, 255, 255, 0.08);
            background: rgba(5, 8, 16, 0.9);
            width: 100%;
        }

        .seo-keywords {
            margin-top: 15px;
            font-size: 0.75rem;
            color: #64748b;
            line-height: 1.8;
            word-wrap: break-word;
        }

        /* موبایل */
        @media (max-width: 600px) {

            .hero {
                padding: 35px 10px 18px;
            }

            .hero h1 {
                font-size: 1.6rem;
            }

            .hero h2 {
                font-size: 0.95rem;
            }

            .card {
                padding: 18px 14px;
                border-radius: 14px;
            }

            .card-title {
                font-size: 1.08rem;
            }

            .btn-call {
                font-size: 0.92rem;
                padding: 12px 16px;
                width: 100%;
            }

            .badge {
                font-size: 0.78rem;
                padding: 5px 10px;
            }
        }
    </style>
</head>

<body>

    <!-- پس‌زمینه -->
    <div class="radio-waves-bg">
        <div class="wave-line"></div>
    </div>

    <!-- بخش اصلی -->
    <section class="hero">

        <div class="antenna-container">

            <div class="pulse-ring"></div>
            <div class="pulse-ring"></div>
            <div class="pulse-ring"></div>

            <svg
                class="antenna-icon"
                viewBox="0 0 64 64"
                xmlns="http://www.w3.org/2000/svg"
            >
                <defs>
                    <linearGradient
                        id="goldGradient"
                        x1="0%"
                        y1="0%"
                        x2="100%"
                        y2="100%"
                    >
                        <stop offset="0%" stop-color="#d97706"/>
                        <stop offset="50%" stop-color="#f59e0b"/>
                        <stop offset="100%" stop-color="#fef08a"/>
                    </linearGradient>
                </defs>

                <path d="M31 5h2v28h-2z"/>
                <path d="M27 31h10v4H27z"/>
                <path d="M30 34h4v22h-4z"/>
                <path d="M20 57h24v3H20z"/>

                <path d="M16 15c-4 4-6 9-6 15s2 11 6 15l3-3c-3-3-4-7-4-12s1-9 4-12z"/>
                <path d="M48 15l-3 3c3 3 4 7 4 12s-1 9-4 12l3 3c4-4 6-9 6-15s-2-11-6-15z"/>

                <path d="M9 8C3 14 0 22 0 30s3 16 9 22l3-3c-5-5-7-12-7-19s2-14 7-19z"/>
                <path d="M55 8l-3 3c5 5 7 12 7 19s-2 14-7 19l3 3c6-6 9-14 9-22s-3-16-9-22z"/>
            </svg>

        </div>

        <h1>میلاد یوسفی</h1>

        <h2>
            مهندس راه‌اندازی بیسیم و شبکه‌های رادیویی
        </h2>

        <div class="badges">
            <span class="badge gold-badge">Motorola</span>
            <span class="badge">VHF / UHF</span>
            <span class="badge">DMR</span>
            <span class="badge">Radio Network</span>
        </div>

    </section>

    <!-- محتوای سایت -->
    <main class="container">

        <section class="card">

            <h3 class="card-title">
                📡 تخصص و فعالیت
            </h3>

            <p>
                طراحی، راه‌اندازی، تنظیم و پشتیبانی شبکه‌های بیسیم و رادیویی
                حرفه‌ای با تمرکز بر سیستم‌های Motorola و شبکه‌های VHF، UHF و DMR.
            </p>

        </section>

        <section class="card">

            <h3 class="card-title">
                🛠 خدمات تخصصی
            </h3>

            <div class="services-grid">

                <div class="service-box">
                    <h4>راه‌اندازی بیسیم</h4>
                    <p>
                        نصب، برنامه‌ریزی و تنظیم بیسیم‌های حرفه‌ای و خودرویی.
                    </p>
                </div>

                <div class="service-box">
                    <h4>شبکه‌های رادیویی</h4>
                    <p>
                        طراحی و راه‌اندازی شبکه‌های رادیویی و سایت‌های تکرارکننده.
                    </p>
                </div>

                <div class="service-box">
                    <h4>Motorola</h4>
                    <p>
                        تنظیم و راه‌اندازی تجهیزات و سیستم‌های رادیویی موتورولا.
                    </p>
                </div>

                <div class="service-box">
                    <h4>VHF / UHF / DMR</h4>
                    <p>
                        طراحی لینک‌ها، تنظیم فرکانس‌ها و بهینه‌سازی پوشش رادیویی.
                    </p>
                </div>

            </div>

        </section>

        <section class="card">

            <h3 class="card-title">
                📍 محدوده فعالیت
            </h3>

            <p>
                قائمشهر، مازندران و سراسر ایران
            </p>

            <p style="margin-top: 10px;">
                همکاری با شرکت امیدان صنعت
            </p>

        </section>

        <div class="cta-wrapper">

            <a
                class="btn-call"
                href="tel:09048818508"
            >
                📞 تماس با مهندس یوسفی
            </a>

        </div>

        <div class="seo-keywords">
            مهندس بیسیم، راه‌اندازی بیسیم، مهندس راه‌اندازی بیسیم،
            راه‌اندازی بیسیم موتورولا، راه‌اندازی سایت بیسیم،
            شبکه رادیویی، VHF، UHF، DMR، بیسیم مازندران،
            بیسیم قائمشهر
        </div>

    </main>

    <!-- فوتر -->
    <footer>

        <p>
            © تمامی حقوق محفوظ است.
        </p>

        <p style="margin-top: 5px;">
            میلاد یوسفی | مهندس راه‌اندازی بیسیم و شبکه‌های رادیویی
        </p>

    </footer>

</body>
</html>
