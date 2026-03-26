<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>القافلة الطبية - كلية الصيدلة جامعة عين شمس | Medical Caravan</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;500;600;700;800;900&family=Poppins:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;500;600;700;800;900&family=Poppins:wght@300;400;500;600;700;800;900&display=swap');
        
        :root {
            --primary: #1e40af;
            --primary-light: #3b82f6;
            --primary-dark: #1e3a8a;
            --secondary: #059669;
            --secondary-light: #10b981;
            --accent: #f59e0b;
            --accent-light: #fbbf24;
            --dark: #1f2937;
            --light: #f9fafb;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html {
            scroll-behavior: smooth;
        }
        
        body {
            font-family: 'Cairo', 'Poppins', sans-serif;
            background: var(--light);
            overflow-x: hidden;
        }
        
        body.en {
            direction: ltr;
        }
        
        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 10px;
        }
        
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        
        ::-webkit-scrollbar-thumb {
            background: var(--primary);
            border-radius: 5px;
        }
        
        ::-webkit-scrollbar-thumb:hover {
            background: var(--primary-dark);
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #1e40af 0%, #3b82f6 50%, #059669 100%);
        }
        
        .gradient-bg-2 {
            background: linear-gradient(135deg, #059669 0%, #10b981 100%);
        }
        
        .gradient-text {
            background: linear-gradient(135deg, #1e40af 0%, #3b82f6 50%, #059669 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .card-hover {
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .card-hover:hover {
            transform: translateY(-12px) scale(1.02);
            box-shadow: 0 25px 50px rgba(0,0,0,0.2);
        }
        
        /* Timeline Styles - Mobile First */
        .timeline-container {
            position: relative;
            max-width: 100%;
            margin: 0 auto;
            padding: 0 1rem;
        }
        
        .timeline-line {
            position: absolute;
            width: 4px;
            background: linear-gradient(180deg, #1e40af 0%, #3b82f6 50%, #059669 100%);
            top: 0;
            bottom: 0;
            right: 20px;
            border-radius: 2px;
            z-index: 1;
        }
        
        body.en .timeline-line {
            right: auto;
            left: 20px;
        }
        
        @media (min-width: 768px) {
            .timeline-line {
                right: 50%;
                transform: translateX(50%);
            }
            
            body.en .timeline-line {
                left: 50%;
                transform: translateX(-50%);
            }
        }
        
        .timeline-item {
            position: relative;
            padding: 1.5rem;
            margin: 1.5rem 0;
            background: white;
            border-radius: 1.5rem;
            box-shadow: 0 10px 40px rgba(0,0,0,0.1);
            transition: all 0.4s ease;
            width: 100%;
            margin-right: 50px;
            z-index: 2;
        }
        
        body.en .timeline-item {
            margin-right: 0;
            margin-left: 50px;
        }
        
        @media (min-width: 768px) {
            .timeline-item {
                width: calc(50% - 40px);
            }
            
            .timeline-item:nth-child(odd) {
                margin-right: auto;
                margin-left: 0;
            }
            
            body.en .timeline-item:nth-child(odd) {
                margin-right: 0;
                margin-left: auto;
            }
            
            .timeline-item:nth-child(even) {
                margin-left: auto;
                margin-right: 0;
            }
            
            body.en .timeline-item:nth-child(even) {
                margin-left: 0;
                margin-right: auto;
            }
        }
        
        .timeline-item:hover {
            transform: translateX(-8px);
            box-shadow: 0 20px 60px rgba(0,0,0,0.15);
        }
        
        body.en .timeline-item:hover {
            transform: translateX(8px);
        }
        
        .timeline-dot {
            position: absolute;
            width: 20px;
            height: 20px;
            background: linear-gradient(135deg, #1e40af, #3b82f6);
            border-radius: 50%;
            top: 2rem;
            right: -30px;
            border: 4px solid white;
            box-shadow: 0 0 0 4px rgba(30, 64, 175, 0.2);
            z-index: 10;
        }
        
        body.en .timeline-dot {
            right: auto;
            left: -30px;
        }
        
        @media (min-width: 768px) {
            .timeline-item:nth-child(even) .timeline-dot {
                right: auto;
                left: -30px;
            }
            
            body.en .timeline-item:nth-child(even) .timeline-dot {
                left: auto;
                right: -30px;
            }
        }
        
        .year-badge {
            background: linear-gradient(135deg, #1e40af, #3b82f6);
            color: white;
            padding: 0.5rem 1.5rem;
            border-radius: 2rem;
            font-weight: 700;
            display: inline-block;
            margin-bottom: 1rem;
            box-shadow: 0 4px 15px rgba(30, 64, 175, 0.3);
            font-size: 0.9rem;
        }
        
        .impact-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 0.75rem;
            margin-top: 1rem;
        }
        
        @media (min-width: 640px) {
            .impact-grid {
                grid-template-columns: repeat(4, 1fr);
            }
        }
        
        .impact-card {
            background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
            padding: 1rem;
            border-radius: 1rem;
            text-align: center;
            border-right: 4px solid var(--primary);
        }
        
        body.en .impact-card {
            border-right: none;
            border-left: 4px solid var(--primary);
        }
        
        .impact-number {
            font-size: 1.25rem;
            font-weight: 800;
            color: var(--primary);
        }
        
        .impact-label {
            font-size: 0.75rem;
            color: #6b7280;
            margin-top: 0.25rem;
        }
        
        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.85);
            z-index: 1000;
            overflow-y: auto;
            backdrop-filter: blur(5px);
        }
        
        .modal.active {
            display: flex;
            justify-content: center;
            align-items: flex-start;
            padding: 1rem;
            animation: fadeIn 0.3s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .modal-content {
            background: white;
            border-radius: 2rem;
            max-width: 1000px;
            width: 100%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
            animation: modalSlide 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            margin: 2rem auto;
        }
        
        @keyframes modalSlide {
            from {
                opacity: 0;
                transform: translateY(-50px) scale(0.9);
            }
            to {
                opacity: 1;
                transform: translateY(0) scale(1);
            }
        }
        
        .close-modal {
            position: sticky;
            top: 1rem;
            float: left;
            width: 48px;
            height: 48px;
            background: linear-gradient(135deg, #1e40af, #3b82f6);
            color: white;
            border: none;
            border-radius: 50%;
            cursor: pointer;
            font-size: 1.8rem;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
            z-index: 10;
            box-shadow: 0 4px 15px rgba(30, 64, 175, 0.4);
            margin: 1rem;
        }
        
        body.en .close-modal {
            float: right;
        }
        
        .close-modal:hover {
            transform: rotate(90deg) scale(1.1);
            box-shadow: 0 8px 25px rgba(30, 64, 175, 0.5);
        }
        
        /* Navigation */
        .nav-link {
            position: relative;
            padding: 0.5rem 1rem;
            transition: all 0.3s ease;
            font-weight: 500;
            font-size: 0.9rem;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            right: 0;
            width: 0;
            height: 3px;
            background: linear-gradient(90deg, #1e40af, #3b82f6);
            transition: width 0.3s ease;
            border-radius: 2px;
        }
        
        body.en .nav-link::after {
            right: auto;
            left: 0;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        /* Committee Cards */
        .committee-card {
            background: white;
            border-radius: 1.5rem;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 10px 40px rgba(0,0,0,0.08);
            cursor: pointer;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            border: 2px solid transparent;
            position: relative;
            overflow: hidden;
        }
        
        .committee-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, #1e40af, #3b82f6);
            transform: scaleX(0);
            transition: transform 0.4s ease;
        }
        
        .committee-card:hover::before {
            transform: scaleX(1);
        }
        
        .committee-card:hover {
            border-color: var(--primary-light);
            transform: translateY(-12px) scale(1.02);
            box-shadow: 0 25px 50px rgba(0,0,0,0.15);
        }
        
        .committee-icon {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 1rem;
            font-size: 2rem;
            background: linear-gradient(135deg, #1e40af, #3b82f6);
            color: white;
            box-shadow: 0 8px 25px rgba(30, 64, 175, 0.3);
            transition: all 0.4s ease;
        }
        
        .committee-card:hover .committee-icon {
            transform: scale(1.1) rotate(5deg);
            box-shadow: 0 12px 35px rgba(30, 64, 175, 0.4);
        }
        
        /* Stats Cards */
        .stat-card {
            background: linear-gradient(135deg, #1e40af 0%, #3b82f6 50%, #059669 100%);
            color: white;
            border-radius: 1.5rem;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 10px 40px rgba(30, 64, 175, 0.3);
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
        }
        
        .stat-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            animation: pulse 3s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 0.5; }
            50% { transform: scale(1.1); opacity: 0.8; }
        }
        
        .stat-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 60px rgba(30, 64, 175, 0.4);
        }
        
        .stat-number {
            font-size: 2.5rem;
            font-weight: 900;
            margin-bottom: 0.5rem;
            position: relative;
            z-index: 1;
        }
        
        .stat-label {
            font-size: 0.9rem;
            opacity: 0.9;
            position: relative;
            z-index: 1;
        }
        
        /* Section Title */
        .section-title {
            position: relative;
            display: inline-block;
            margin-bottom: 3rem;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -15px;
            right: 0;
            width: 70%;
            height: 5px;
            background: linear-gradient(90deg, #1e40af, #f59e0b);
            border-radius: 3px;
        }
        
        body.en .section-title::after {
            right: auto;
            left: 0;
        }
        
        /* Language Switch */
        .language-switch {
            display: flex;
            gap: 0.25rem;
            background: #f3f4f6;
            padding: 0.25rem;
            border-radius: 2rem;
        }
        
        .lang-btn {
            padding: 0.5rem 1rem;
            border: none;
            background: transparent;
            color: #6b7280;
            border-radius: 2rem;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            font-family: inherit;
            font-size: 0.85rem;
        }
        
        .lang-btn.active {
            background: linear-gradient(135deg, #1e40af, #3b82f6);
            color: white;
            box-shadow: 0 4px 15px rgba(30, 64, 175, 0.3);
        }
        
        .lang-btn:hover:not(.active) {
            color: var(--primary);
        }
        
        /* Hero Section */
        .hero-overlay {
            background: linear-gradient(135deg, rgba(30, 64, 175, 0.95) 0%, rgba(59, 130, 246, 0.85) 50%, rgba(5, 150, 105, 0.9) 100%);
        }
        
        .hero-pattern {
            background-image: url("image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.05'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
        }
        
        /* Buttons */
        .btn-primary {
            background: linear-gradient(135deg, #1e40af, #3b82f6);
            color: white;
            padding: 0.875rem 2rem;
            border-radius: 3rem;
            font-weight: 700;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            border: none;
            cursor: pointer;
            box-shadow: 0 8px 25px rgba(30, 64, 175, 0.4);
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 0.95rem;
        }
        
        .btn-primary:hover {
            transform: translateY(-4px);
            box-shadow: 0 15px 40px rgba(30, 64, 175, 0.5);
        }
        
        .btn-secondary {
            background: white;
            color: var(--primary);
            padding: 0.875rem 2rem;
            border-radius: 3rem;
            font-weight: 700;
            transition: all 0.4s ease;
            border: 3px solid white;
            cursor: pointer;
            box-shadow: 0 8px 25px rgba(0,0,0,0.2);
            font-size: 0.95rem;
        }
        
        .btn-secondary:hover {
            background: transparent;
            color: white;
            transform: translateY(-4px);
        }
        
        /* Animations */
        .fade-in {
            animation: fadeInUp 0.8s cubic-bezier(0.4, 0, 0.2, 1) forwards;
            opacity: 0;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(40px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .stagger-1 { animation-delay: 0.1s; }
        .stagger-2 { animation-delay: 0.2s; }
        .stagger-3 { animation-delay: 0.3s; }
        .stagger-4 { animation-delay: 0.4s; }
        
        /* Committee Detail */
        .detail-image {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 1.5rem;
            margin-bottom: 1.5rem;
            box-shadow: 0 10px 40px rgba(0,0,0,0.15);
        }
        
        @media (min-width: 768px) {
            .detail-image {
                height: 350px;
            }
        }
        
        .info-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1rem;
            margin: 1.5rem 0;
        }
        
        @media (min-width: 768px) {
            .info-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        
        .info-box {
            background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
            padding: 1.25rem;
            border-radius: 1.25rem;
            border-right: 5px solid var(--primary);
            transition: all 0.3s ease;
        }
        
        body.en .info-box {
            border-right: none;
            border-left: 5px solid var(--primary);
        }
        
        .info-box:hover {
            transform: translateX(-5px);
            box-shadow: 0 8px 25px rgba(30, 64, 175, 0.15);
        }
        
        body.en .info-box:hover {
            transform: translateX(5px);
        }
        
        /* Location Tags */
        .location-tag {
            background: linear-gradient(135deg, #059669, #10b981);
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 2rem;
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            margin: 0.25rem;
            font-size: 0.8rem;
        }
        
        /* Mobile Menu */
        .mobile-menu {
            display: block;
        }
        
        .desktop-menu {
            display: none;
        }
        
        @media (min-width: 768px) {
            .mobile-menu {
                display: none;
            }
            
            .desktop-menu {
                display: flex;
            }
        }
        
        /* Floating Animation */
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        
        @keyframes floating {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        /* Impact Badge */
        .impact-badge {
            background: linear-gradient(135deg, #059669, #10b981);
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 2rem;
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            margin: 0.25rem;
            box-shadow: 0 4px 15px rgba(5, 150, 105, 0.3);
            font-size: 0.8rem;
        }
        
        /* Mobile Navigation */
        .mobile-nav {
            display: none;
            position: fixed;
            top: 70px;
            left: 0;
            right: 0;
            background: white;
            padding: 1rem;
            box-shadow: 0 10px 40px rgba(0,0,0,0.1);
            z-index: 40;
        }
        
        .mobile-nav.active {
            display: block;
            animation: slideDown 0.3s ease;
        }
        
        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .mobile-nav a {
            display: block;
            padding: 0.75rem 1rem;
            color: #374151;
            text-decoration: none;
            border-radius: 0.5rem;
            margin: 0.25rem 0;
            transition: all 0.3s ease;
        }
        
        .mobile-nav a:hover {
            background: #eff6ff;
            color: var(--primary);
        }
        
        /* Timeline Content Visibility Fix */
        .timeline-content {
            display: block !important;
            visibility: visible !important;
            opacity: 1 !important;
        }
        
        /* Ensure all text is visible */
        h1, h2, h3, h4, h5, h6, p, span, div, li, a {
            visibility: visible !important;
            opacity: 1 !important;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="bg-white shadow-xl sticky top-0 z-50">
        <div class="container mx-auto px-4 py-3">
            <div class="flex justify-between items-center">
                <div class="flex items-center gap-2">
                    <div class="w-12 h-12 gradient-bg rounded-xl flex items-center justify-center text-white text-xl font-bold shadow-lg">
                        🏥
                    </div>
                    <div>
                        <h1 class="text-lg font-bold text-gray-800">القافلة الطبية</h1>
                        <p class="text-xs text-gray-500">كلية الصيدلة - جامعة عين شمس</p>
                    </div>
                </div>
                
                <div class="desktop-menu flex items-center gap-3">
                    <a href="#home" class="nav-link text-gray-700 hover:text-primary" data-en="Home" data-ar="الرئيسية">الرئيسية</a>
                    <a href="#about" class="nav-link text-gray-700 hover:text-primary" data-en="About" data-ar="عن القافلة">عن القافلة</a>
                    <a href="#committees" class="nav-link text-gray-700 hover:text-primary" data-en="Committees" data-ar="اللجان">اللجان</a>
                    <a href="#history" class="nav-link text-gray-700 hover:text-primary" data-en="History" data-ar="التاريخ">التاريخ</a>
                    <a href="#contact" class="nav-link text-gray-700 hover:text-primary" data-en="Contact" data-ar="تواصل معنا">تواصل معنا</a>
                    
                    <div class="language-switch">
                        <button class="lang-btn active" onclick="switchLang('ar')">عربي</button>
                        <button class="lang-btn" onclick="switchLang('en')">EN</button>
                    </div>
                </div>
                
                <button class="mobile-menu text-gray-700 p-2" onclick="toggleMobileMenu()">
                    <svg class="w-7 h-7" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
                    </svg>
                </button>
            </div>
        </div>
    </nav>

    <!-- Mobile Navigation -->
    <div class="mobile-nav" id="mobileNav">
        <a href="#home" onclick="toggleMobileMenu()" data-en="Home" data-ar="الرئيسية">الرئيسية</a>
        <a href="#about" onclick="toggleMobileMenu()" data-en="About" data-ar="عن القافلة">عن القافلة</a>
        <a href="#committees" onclick="toggleMobileMenu()" data-en="Committees" data-ar="اللجان">اللجان</a>
        <a href="#history" onclick="toggleMobileMenu()" data-en="History" data-ar="التاريخ">التاريخ</a>
        <a href="#contact" onclick="toggleMobileMenu()" data-en="Contact" data-ar="تواصل معنا">تواصل معنا</a>
        <div class="flex gap-2 mt-3 pt-3 border-t">
            <button class="lang-btn flex-1 active" onclick="switchLang('ar')">عربي</button>
            <button class="lang-btn flex-1" onclick="switchLang('en')">EN</button>
        </div>
    </div>

    <!-- Hero Section -->
    <section id="home" class="gradient-bg text-white py-16 md:py-24 relative overflow-hidden hero-pattern">
        <div class="absolute inset-0 hero-overlay"></div>
        <div class="container mx-auto px-4 relative z-10">
            <div class="grid lg:grid-cols-2 gap-8 md:gap-12 items-center">
                <div class="fade-in">
                    <div class="inline-block bg-white/20 backdrop-blur-sm px-4 py-2 rounded-full mb-4">
                        <span class="text-yellow-300 font-bold">✨</span>
                        <span class="mr-2 text-sm md:text-base" data-en="20 Years of Excellence" data-ar="20 عاماً من التميز">20 عاماً من التميز</span>
                    </div>
                    <h1 class="text-3xl md:text-4xl lg:text-5xl font-black mb-4 md:mb-6 leading-tight">
                        <span class="block">القافلة الطبية</span>
                        <span class="block text-yellow-300">كلية الصيدلة</span>
                        <span class="block text-xl md:text-2xl lg:text-3xl font-bold mt-3 md:mt-4 opacity-90">جامعة عين شمس</span>
                    </h1>
                    <p class="text-base md:text-lg mb-6 md:mb-8 opacity-95 leading-relaxed" data-en="Delivering healthcare services to underserved communities since 2005. Over 50,000 patients served through 8 specialized committees." data-ar="نقدم خدمات الرعاية الصحية للمجتمعات المحرومة منذ عام 2005. أكثر من 50,000 مريض تم خدمتهم من خلال 8 لجان متخصصة">
                        نقدم خدمات الرعاية الصحية للمجتمعات المحرومة منذ عام 2005. أكثر من 50,000 مريض تم خدمتهم من خلال 8 لجان متخصصة
                    </p>
                    <div class="flex flex-wrap gap-3">
                        <a href="#committees" class="btn-primary">
                            <span data-en="Explore Committees" data-ar="استكشف اللجان">استكشف اللجان</span>
                            <span>→</span>
                        </a>
                        <a href="#history" class="btn-secondary">
                            <span data-en="View History" data-ar="عرض التاريخ">عرض التاريخ</span>
                        </a>
                    </div>
                </div>
                <div class="fade-in stagger-2">
                    <img src="https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/1f6d5e4fd-8952-409f-ac86-5ee6c136a234.png" alt="Medical Caravan Team" class="rounded-2xl md:rounded-3xl shadow-2xl w-full floating">
                </div>
            </div>
            
            <!-- Stats -->
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4 md:gap-6 mt-12 md:mt-20">
                <div class="stat-card fade-in stagger-1">
                    <div class="stat-number">20+</div>
                    <div class="stat-label" data-en="Years of Service" data-ar="سنة من الخدمة">سنة من الخدمة</div>
                </div>
                <div class="stat-card fade-in stagger-2">
                    <div class="stat-number">50K+</div>
                    <div class="stat-label" data-en="Patients Served" data-ar="مريض تم خدمتهم">مريض تم خدمتهم</div>
                </div>
                <div class="stat-card fade-in stagger-3">
                    <div class="stat-number">8</div>
                    <div class="stat-label" data-en="Specialized Committees" data-ar="لجان متخصصة">لجان متخصصة</div>
                </div>
                <div class="stat-card fade-in stagger-4">
                    <div class="stat-number">100K+</div>
                    <div class="stat-label" data-en="Awareness Interactions" data-ar="تفاعل توعوي">تفاعل توعوي</div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 md:py-24 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12 md:mb-16">
                <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-800 section-title" data-en="About Medical Caravan" data-ar="عن القافلة الطبية">عن القافلة الطبية</h2>
            </div>
            
            <div class="grid lg:grid-cols-2 gap-8 md:gap-16 items-center">
                <div class="fade-in">
                    <img src="https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/1f6d5e4fd-8952-409f-ac86-5ee6c136a234.png" alt="About Caravan" class="rounded-2xl md:rounded-3xl shadow-2xl w-full">
                </div>
                <div class="fade-in stagger-2">
                    <h3 class="text-2xl md:text-3xl font-bold text-gray-800 mb-4 md:mb-6" data-en="Our Vision & Mission" data-ar="رؤيتنا ورسالتنا">رؤيتنا ورسالتنا</h3>
                    <p class="text-gray-600 mb-4 md:mb-6 leading-relaxed text-base md:text-lg" data-en="Medical Caravan was founded in 2005 as a student-led initiative built on core committees. From the very beginning, the Caravan was designed to reach underserved communities, delivering accessible healthcare services while building practical experience for its members." data-ar="تأسست القافلة الطبية عام 2005 كمبادرة طلابية مبنية على لجان أساسية. منذ البداية، صُممت القافلة للوصول إلى المجتمعات المحرومة، وتقديم خدمات الرعاية الصحية مع بناء خبرة عملية لأعضائها.">
                        تأسست القافلة الطبية عام 2005 كمبادرة طلابية مبنية على لجان أساسية. منذ البداية، صُممت القافلة للوصول إلى المجتمعات المحرومة، وتقديم خدمات الرعاية الصحية مع بناء خبرة عملية لأعضائها.
                    </p>
                    
                    <div class="space-y-3 md:space-y-4">
                        <div class="info-box">
                            <h4 class="font-bold text-primary mb-2 flex items-center gap-2 text-base md:text-lg">
                                <span>🎯</span>
                                <span data-en="Vision" data-ar="الرؤية">الرؤية</span>
                            </h4>
                            <p class="text-gray-600 text-sm md:text-base" data-en="To be a leading student organization providing sustainable healthcare services to underserved communities in Egypt." data-ar="أن نكون منظمة طلابية رائدة تقدم خدمات رعاية صحية مستدامة للمجتمعات المحرومة في مصر.">
                                أن نكون منظمة طلابية رائدة تقدم خدمات رعاية صحية مستدامة للمجتمعات المحرومة في مصر.
                            </p>
                        </div>
                        <div class="info-box">
                            <h4 class="font-bold text-primary mb-2 flex items-center gap-2 text-base md:text-lg">
                                <span>📋</span>
                                <span data-en="Mission" data-ar="الرسالة">الرسالة</span>
                            </h4>
                            <p class="text-gray-600 text-sm md:text-base" data-en="Delivering quality healthcare services, raising health awareness, and developing practical skills for pharmacy students through community service." data-ar="تقديم خدمات رعاية صحية عالية الجودة، ورفع الوعي الصحي، وتطوير المهارات العملية لطلاب الصيدلة من خلال خدمة المجتمع.">
                                تقديم خدمات رعاية صحية عالية الجودة، ورفع الوعي الصحي، وتطوير المهارات العملية لطلاب الصيدلة من خلال خدمة المجتمع.
                            </p>
                        </div>
                        <div class="info-box">
                            <h4 class="font-bold text-primary mb-2 flex items-center gap-2 text-base md:text-lg">
                                <span>💡</span>
                                <span data-en="Core Values" data-ar="القيم الأساسية">القيم الأساسية</span>
                            </h4>
                            <p class="text-gray-600 text-sm md:text-base" data-en="Excellence, Sustainability, Community Impact, Student Development, Healthcare Accessibility" data-ar="التميز، الاستدامة، التأثير المجتمعي، تطوير الطلاب، إمكانية الوصول للرعاية الصحية">
                                التميز، الاستدامة، التأثير المجتمعي، تطوير الطلاب، إمكانية الوصول للرعاية الصحية
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Committees Section -->
    <section id="committees" class="py-16 md:py-24 bg-gradient-to-b from-gray-50 to-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12 md:mb-16">
                <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-800 section-title" data-en="Our Committees" data-ar="لجاننا">لجاننا</h2>
                <p class="text-gray-600 mt-3 md:mt-4 text-base md:text-lg" data-en="Eight specialized committees working together to deliver comprehensive healthcare services" data-ar="ثماني لجان متخصصة تعمل معًا لتقديم خدمات رعاية صحية شاملة">
                    ثماني لجان متخصصة تعمل معًا لتقديم خدمات رعاية صحية شاملة
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-4 md:gap-6">
                <!-- Pharmacy Committee -->
                <div class="committee-card" onclick="openCommitteeModal('pharmacy')">
                    <div class="committee-icon">💊</div>
                    <h3 class="text-lg md:text-xl font-bold text-gray-800 mb-2" data-en="Pharmacy" data-ar="الصيدلة">الصيدلة</h3>
                    <p class="text-gray-600 text-sm" data-en="Medication dispensing & management" data-ar="صرف وإدارة الأدوية">صرف وإدارة الأدوية</p>
                </div>
                
                <!-- Lab Committee -->
                <div class="committee-card" onclick="openCommitteeModal('lab')">
                    <div class="committee-icon">🔬</div>
                    <h3 class="text-lg md:text-xl font-bold text-gray-800 mb-2" data-en="Laboratory" data-ar="المعمل">المعمل</h3>
                    <p class="text-gray-600 text-sm" data-en="Diagnostic tests & analysis" data-ar="الفحوصات والتحاليل">الفحوصات والتحاليل</p>
                </div>
                
                <!-- Preclinic Committee -->
                <div class="committee-card" onclick="openCommitteeModal('preclinic')">
                    <div class="committee-icon">📋</div>
                    <h3 class="text-lg md:text-xl font-bold text-gray-800 mb-2" data-en="Pre-Clinic" data-ar="ما قبل العيادة">ما قبل العيادة</h3>
                    <p class="text-gray-600 text-sm" data-en="Patient triage & assessment" data-ar="فرز وتقييم المرضى">فرز وتقييم المرضى</p>
                </div>
                
                <!-- Awareness Committee -->
                <div class="committee-card" onclick="openCommitteeModal('awareness')">
                    <div class="committee-icon">📢</div>
                    <h3 class="text-lg md:text-xl font-bold text-gray-800 mb-2" data-en="Awareness" data-ar="التوعية">التوعية</h3>
                    <p class="text-gray-600 text-sm" data-en="Health education campaigns" data-ar="حملات التوعية الصحية">حملات التوعية الصحية</p>
                </div>
                
                <!-- HR Committee -->
                <div class="committee-card" onclick="openCommitteeModal('hr')">
                    <div class="committee-icon">👥</div>
                    <h3 class="text-lg md:text-xl font-bold text-gray-800 mb-2" data-en="Human Resources" data-ar="الموارد البشرية">الموارد البشرية</h3>
                    <p class="text-gray-600 text-sm" data-en="Team management & development" data-ar="إدارة وتطوير الفريق">إدارة وتطوير الفريق</p>
                </div>
                
                <!-- FR Committee -->
                <div class="committee-card" onclick="openCommitteeModal('fr')">
                    <div class="committee-icon">💰</div>
                    <h3 class="text-lg md:text-xl font-bold text-gray-800 mb-2" data-en="Fundraising" data-ar="جمع التبرعات">جمع التبرعات</h3>
                    <p class="text-gray-600 text-sm" data-en="Sponsorships & partnerships" data-ar="الرعايات والشراكات">الرعايات والشراكات</p>
                </div>
                
                <!-- Operations Committee -->
                <div class="committee-card" onclick="openCommitteeModal('operations')">
                    <div class="committee-icon">🚚</div>
                    <h3 class="text-lg md:text-xl font-bold text-gray-800 mb-2" data-en="Operations & Logistics" data-ar="العمليات واللوجستيات">العمليات واللوجستيات</h3>
                    <p class="text-gray-600 text-sm" data-en="Supply chain & coordination" data-ar="سلسلة التوريد والتنسيق">سلسلة التوريد والتنسيق</p>
                </div>
                
                <!-- Media Committee -->
                <div class="committee-card" onclick="openCommitteeModal('media')">
                    <div class="committee-icon">📱</div>
                    <h3 class="text-lg md:text-xl font-bold text-gray-800 mb-2" data-en="Media & Marketing" data-ar="الإعلام والتسويق">الإعلام والتسويق</h3>
                    <p class="text-gray-600 text-sm" data-en="Brand & digital presence" data-ar="العلامة والتواجد الرقمي">العلامة والتواجد الرقمي</p>
                </div>
            </div>
        </div>
    </section>

    <!-- History Section -->
    <section id="history" class="py-16 md:py-24 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12 md:mb-16">
                <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-800 section-title" data-en="History & Timeline" data-ar="تاريخ القافلة">تاريخ القافلة</h2>
                <p class="text-gray-600 mt-3 md:mt-4 text-base md:text-lg" data-en="From 2005 to 2025 - Two decades of growth and impact" data-ar="من 2005 إلى 2025 - عقدين من النمو والتأثير">
                    من 2005 إلى 2025 - عقدين من النمو والتأثير
                </p>
            </div>
            
            <div class="max-w-6xl mx-auto">
                <!-- Timeline -->
                <div class="timeline-container">
                    <div class="timeline-line"></div>
                    
                    <!-- 2005-2010 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2005 - 2010</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Foundation & Field Identity" data-ar="التأسيس والهوية الميدانية">التأسيس والهوية الميدانية</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Medical Caravan was founded in 2005 (MC1) as a student-led initiative built on four core committees: Pharmacy, Laboratory, Awareness, and Project Management. The Caravan operated mainly in rural and underserved areas outside Cairo." data-ar="تأسست القافلة الطبية عام 2005 (MC1) كمبادرة طلابية مبنية على أربع لجان أساسية: الصيدلة، المعمل، التوعية، وإدارة المشاريع. عملت القافلة بشكل رئيسي في المناطق الريفية والمحرومة خارج القاهرة.">
                            تأسست القافلة الطبية عام 2005 (MC1) كمبادرة طلابية مبنية على أربع لجان أساسية: الصيدلة، المعمل، التوعية، وإدارة المشاريع. عملت القافلة بشكل رئيسي في المناطق الريفية والمحرومة خارج القاهرة.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 النصر - الإسماعيلية 2007</span>
                            <span class="location-tag">📍 جلبانة - الإسماعيلية 2009</span>
                            <span class="location-tag">📍 دفنو - الفيوم 2010</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">800-1,200</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">200-400</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">1,500-3,000</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2011 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2011</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Preparation & System Readiness" data-ar="التجهيز وجاهزية النظام">التجهيز وجاهزية النظام</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Although the Caravan did not deploy in the field this year, it was far from inactive. The focus shifted toward training, preparation, and internal system development — ensuring that future operations would be more efficient and scalable." data-ar="على الرغم من أن القافلة لم تنشر في الميدان هذا العام، إلا أنها لم تكن خاملة. تحول التركيز نحو التدريب والتجهيز وتطوير النظام الداخلي — لضمان أن العمليات المستقبلية ستكون أكثر كفاءة وقابلية للتوسع.">
                            على الرغم من أن القافلة لم تنشر في الميدان هذا العام، إلا أنها لم تكن خاملة. تحول التركيز نحو التدريب والتجهيز وتطوير النظام الداخلي — لضمان أن العمليات المستقبلية ستكون أكثر كفاءة وقابلية للتوسع.
                        </p>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">1,000+</div>
                                <div class="impact-label" data-en="Training Cases" data-ar="حالة تدريبية">حالة تدريبية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2012 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2012</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Expansion into Cairo" data-ar="التوسع إلى القاهرة">التوسع إلى القاهرة</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="First major step toward higher patient volume. Locations: Al-Waily & Abbassia. The Caravan expanded into densely populated urban areas, marking the beginning of larger-scale operations." data-ar="الخطوة الأولى الكبرى نحو حجم مرضى أعلى. المواقع: الوايلي والعباسية. توسعت القافلة إلى المناطق الحضرية ذات الكثافة السكانية العالية، مما يمثل بداية العمليات على نطاق أوسع.">
                            الخطوة الأولى الكبرى نحو حجم مرضى أعلى. المواقع: الوايلي والعباسية. توسعت القافلة إلى المناطق الحضرية ذات الكثافة السكانية العالية، مما يمثل بداية العمليات على نطاق أوسع.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 الوايلي</span>
                            <span class="location-tag">📍 العباسية</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">1,200-1,500</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">300-500</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">2,500-4,000</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2013 MC9 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2013 (MC9)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="First High-Impact Milestone" data-ar="أول معلم عالي التأثير">أول معلم عالي التأثير</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: Ezbet El-Hagana. This year marked a breakthrough in scale and performance. The workflow between committees became more efficient, allowing smoother patient handling and improved service delivery." data-ar="الموقع: عزبة الهجانة. هذا العام شهد اختراقًا في الحجم والأداء. أصبح سير العمل بين اللجان أكثر كفاءة، مما سمح بالتعامل السلس مع المرضى وتحسين تقديم الخدمات.">
                            الموقع: عزبة الهجانة. هذا العام شهد اختراقًا في الحجم والأداء. أصبح سير العمل بين اللجان أكثر كفاءة، مما سمح بالتعامل السلس مع المرضى وتحسين تقديم الخدمات.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 عزبة الهجانة</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">2,850</div>
                                <div class="impact-label" data-en="Patients" data-ar="مريض">مريض</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">2,170</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">550</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">3,000</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2014 MC10 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2014 (MC10)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="System Stability & Consistency" data-ar="استقرار النظام والاتساق">استقرار النظام والاتساق</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: Ezbet El-Hagana. After rapid growth, the focus shifted to stabilizing operations and maintaining consistent performance. Efforts were directed toward improving coordination and ensuring services were delivered efficiently without compromising quality." data-ar="الموقع: عزبة الهجانة. بعد النمو السريع، تحول التركيز نحو استقرار العمليات والحفاظ على أداء متسق. تم توجيه الجهود نحو تحسين التنسيق وضمان تقديم الخدمات بكفاءة دون المساس بالجودة.">
                            الموقع: عزبة الهجانة. بعد النمو السريع، تحول التركيز نحو استقرار العمليات والحفاظ على أداء متسق. تم توجيه الجهود نحو تحسين التنسيق وضمان تقديم الخدمات بكفاءة دون المساس بالجودة.
                        </p>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">2,200-2,600</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">500-700</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">3,000-4,000</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2015 MC11 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2015 (MC11)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Marketing Emergence & Brand Visibility" data-ar="ظهور التسويق ووضوح العلامة">ظهور التسويق ووضوح العلامة</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="2015 marked the introduction of the Marketing Committee, which changed how the Caravan communicated with its audience. Marketing was not only about promotion — it played a key role in increasing visibility, attracting volunteers, and strengthening the Caravan's identity." data-ar="شهد عام 2015 إدخال لجنة التسويق، التي غيرت طريقة تواصل القافلة مع جمهورها. لم يكن التسويق فقط عن الترويج — بل لعب دورًا رئيسيًا في زيادة الوضوح، وجذب المتطوعين، وتعزيز هوية القافلة.">
                            شهد عام 2015 إدخال لجنة التسويق، التي غيرت طريقة تواصل القافلة مع جمهورها. لم يكن التسويق فقط عن الترويج — بل لعب دورًا رئيسيًا في زيادة الوضوح، وجذب المتطوعين، وتعزيز هوية القافلة.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="impact-badge">✨ بداية بناء العلامة التجارية</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">2,300-2,700</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">600-800</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">3,500-4,500</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2016 MC12 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2016 (MC12)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Organizational Expansion & Internal Structuring" data-ar="التوسع التنظيمي والهيكل الداخلي">التوسع التنظيمي والهيكل الداخلي</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: El-Marg. 2016 marked a major shift — for the first time, the Human Resources (HR) Committee was introduced, transforming the Caravan into a more structured organization. Advanced lab services were introduced including Lipid profile and H. pylori testing." data-ar="الموقع: المرج. شهد عام 2016 تحولاً كبيرًا — لأول مرة، تم إدخال لجنة الموارد البشرية، مما حول القافلة إلى منظمة أكثر هيكلة. تم إدخال خدمات معملية متقدمة بما في ذلك تحليل الدهون وجرثومة المعدة.">
                            الموقع: المرج. شهد عام 2016 تحولاً كبيرًا — لأول مرة، تم إدخال لجنة الموارد البشرية، مما حول القافلة إلى منظمة أكثر هيكلة. تم إدخال خدمات معملية متقدمة بما في ذلك تحليل الدهون وجرثومة المعدة.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 المرج</span>
                            <span class="impact-badge">🔬 تحليل الدهون</span>
                            <span class="impact-badge">🦠 جرثومة المعدة</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">2,500-3,000</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">700-1,000</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">4,000-5,500</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2017 MC13 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2017 (MC13)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Fundraising & Sustainability" data-ar="جمع التبرعات والاستدامة">جمع التبرعات والاستدامة</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: Manshiet Naser. This year marked the beginning of Fundraising efforts, introducing a new layer of sustainability. Fundraising helped in securing financial support, expanding service capacity, and building external partnerships." data-ar="الموقع: منشية ناصر. هذا العام شهد بداية جهود جمع التبرعات، وإدخال طبقة جديدة من الاستدامة. ساعد جمع التبرعات في تأمين الدعم المالي، وتوسيع قدرة الخدمة، وبناء شراكات خارجية.">
                            الموقع: منشية ناصر. هذا العام شهد بداية جهود جمع التبرعات، وإدخال طبقة جديدة من الاستدامة. ساعد جمع التبرعات في تأمين الدعم المالي، وتوسيع قدرة الخدمة، وبناء شراكات خارجية.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 منشية ناصر</span>
                            <span class="impact-badge">💰 بداية جمع التبرعات</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">2,850</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">550</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">3,000</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2018 MC14 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2018 (MC14)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Community Reach Expansion" data-ar="توسيع الوصول المجتمعي">توسيع الوصول المجتمعي</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: Arab El-Tawila – El-Mataria. The Caravan reached a new level of community engagement, especially in awareness campaigns. This year represented a major leap in outreach and engagement." data-ar="الموقع: عرب الطويلة - المطرية. وصلت القافلة إلى مستوى جديد من المشاركة المجتمعية، خاصة في حملات التوعية. هذا العام يمثل قفزة كبيرة في الوصول والمشاركة.">
                            الموقع: عرب الطويلة - المطرية. وصلت القافلة إلى مستوى جديد من المشاركة المجتمعية، خاصة في حملات التوعية. هذا العام يمثل قفزة كبيرة في الوصول والمشاركة.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 عرب الطويلة - المطرية</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">3,262</div>
                                <div class="impact-label" data-en="Patients" data-ar="مريض">مريض</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">1,810</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">1,097</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">6,742</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2019 MC15 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2019 (MC15)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Identity Development & First Sponsorship" data-ar="تطوير الهوية وأول رعاية">تطوير الهوية وأول رعاية</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: El-Nahda – El Salam. The Caravan began shaping a stronger identity and secured its first sponsorship, marking an important step toward long-term sustainability." data-ar="الموقع: النهضة - السلام. بدأت القافلة في تشكيل هوية أقوى وحصلت على أول رعاية لها، مما يمثل خطوة مهمة نحو الاستدامة طويلة الأجل.">
                            الموقع: النهضة - السلام. بدأت القافلة في تشكيل هوية أقوى وحصلت على أول رعاية لها، مما يمثل خطوة مهمة نحو الاستدامة طويلة الأجل.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 النهضة - السلام</span>
                            <span class="impact-badge">🤝 أول رعاية</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">2,414</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">559</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">5,535</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2020 MC16 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2020 (MC16)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Digital Transformation" data-ar="التحول الرقمي">التحول الرقمي</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Due to global circumstances, the Caravan transitioned fully into a digital model with online awareness campaigns and virtual engagement activities. Sponsor: Supremo Pharmaceuticals. This year proved the Caravan's adaptability and resilience." data-ar="بسبب الظروف العالمية، تحولت القافلة بالكامل إلى نموذج رقمي مع حملات توعية عبر الإنترنت وأنشطة تفاعل افتراضية. الراعي: سوبرمو للأدوية. هذا العام أثبت قابلية القافلة للتكيف والمرونة.">
                            بسبب الظروف العالمية، تحولت القافلة بالكامل إلى نموذج رقمي مع حملات توعية عبر الإنترنت وأنشطة تفاعل افتراضية. الراعي: سوبرمو للأدوية. هذا العام أثبت قابلية القافلة للتكيف والمرونة.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="impact-badge">💻 تحول رقمي كامل</span>
                            <span class="impact-badge">🏥 سوبرمو للأدوية</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">1,000-1,500</div>
                                <div class="impact-label" data-en="Online Awareness" data-ar="توعية أونلاين">توعية أونلاين</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2021 MC17 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2021 (MC17)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Gradual Return & Recovery" data-ar="العودة التدريجية والتعافي">العودة التدريجية والتعافي</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: El-Mataria. The Caravan returned with partial on-ground operations, focusing on safe and controlled deployment. Although the scale was smaller, the Caravan successfully resumed its role within the community." data-ar="الموقع: المطرية. عادت القافلة بعمليات جزئية على الأرض، مع التركيز على النشر الآمن والمتحكم به. على الرغم من أن الحجم كان أصغر، إلا أن القافلة نجحت في استئناف دورها داخل المجتمع.">
                            الموقع: المطرية. عادت القافلة بعمليات جزئية على الأرض، مع التركيز على النشر الآمن والمتحكم به. على الرغم من أن الحجم كان أصغر، إلا أن القافلة نجحت في استئناف دورها داخل المجتمع.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 المطرية</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">1,200-1,800</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">200-400</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">2,000-3,500</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2022 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2022</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Multi-Day Operations Comeback" data-ar="عودة العمليات متعددة الأيام">عودة العمليات متعددة الأيام</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: El-Zawya El-Hamra. Operations regained full stability, and the Caravan returned to running more organized and extended multi-day campaigns. The team was able to handle larger numbers again." data-ar="الموقع: الزاوية الحمراء. استعادت العمليات استقرارها الكامل، وعادت القافلة إلى تشغيل حملات منظمة وممتدة متعددة الأيام. تمكن الفريق من التعامل مع أعداد أكبر مرة أخرى.">
                            الموقع: الزاوية الحمراء. استعادت العمليات استقرارها الكامل، وعادت القافلة إلى تشغيل حملات منظمة وممتدة متعددة الأيام. تمكن الفريق من التعامل مع أعداد أكبر مرة أخرى.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 الزاوية الحمراء</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">1,979</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">660</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">3,220</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2023 MC18 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2023 (MC18)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Campaign Expansion & Awareness Peak" data-ar="توسع الحملة وذروة التوعية">توسع الحملة وذروة التوعية</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: Mohamed Farid School. Campaign: Face & Hope. The Caravan focused heavily on awareness campaigns, achieving one of its highest engagement levels." data-ar="الموقع: مدرسة محمد فريد. الحملة: وجه وأمل. ركزت القافلة بشكل كبير على حملات التوعية، محققة أحد أعلى مستويات المشاركة.">
                            الموقع: مدرسة محمد فريد. الحملة: وجه وأمل. ركزت القافلة بشكل كبير على حملات التوعية، محققة أحد أعلى مستويات المشاركة.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 مدرسة محمد فريد</span>
                            <span class="impact-badge">🎭 حملة وجه وأمل</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">1,987</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">436</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">6,245</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2024 MC19 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2024 (MC19)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Smart Flow System & Pre-Clinic Implementation" data-ar="نظام التدفق الذكي وتنفيذ ما قبل العيادة">نظام التدفق الذكي وتنفيذ ما قبل العيادة</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="Location: Ain Shams. 2024 introduced one of the most impactful operational upgrades: the Pre-Clinic System. This system optimizes patient flow and ensures each case is properly assessed before reaching the physician." data-ar="الموقع: عين شمس. قدم عام 2024 أحد أكثر الترقيات التشغيلية تأثيرًا: نظام ما قبل العيادة. هذا النظام يحسن تدفق المرضى ويضمن تقييم كل حالة بشكل صحيح قبل الوصول إلى الطبيب.">
                            الموقع: عين شمس. قدم عام 2024 أحد أكثر الترقيات التشغيلية تأثيرًا: نظام ما قبل العيادة. هذا النظام يحسن تدفق المرضى ويضمن تقييم كل حالة بشكل صحيح قبل الوصول إلى الطبيب.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="location-tag">📍 عين شمس</span>
                            <span class="impact-badge">🔄 نظام ما قبل العيادة</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">~1,500</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">~550</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">~1,200</div>
                                <div class="impact-label" data-en="Awareness" data-ar="توعية">توعية</div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 2025 MC20 -->
                    <div class="timeline-item timeline-content">
                        <div class="timeline-dot"></div>
                        <span class="year-badge">2025 (MC20)</span>
                        <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-3 md:mb-4" data-en="Institutional Growth & Expansion" data-ar="النمو المؤسسي والتوسع">النمو المؤسسي والتوسع</h3>
                        <p class="text-gray-600 mb-3 md:mb-4 text-sm md:text-base" data-en="The Caravan continued evolving as a more mature organization. Key developments: LinkedIn presence, Sponsorship by Sato Pharma, Dentistry participation introduced." data-ar="واصلت القافلة التطور كمنظمة أكثر نضجًا. التطورات الرئيسية: وجود على LinkedIn، رعاية من ساتو فارما، إدخال مشاركة طب الأسنان.">
                            واصلت القافلة التطور كمنظمة أكثر نضجًا. التطورات الرئيسية: وجود على LinkedIn، رعاية من ساتو فارما، إدخال مشاركة طب الأسنان.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-3 md:mb-4">
                            <span class="impact-badge">💼 LinkedIn</span>
                            <span class="impact-badge">🏥 ساتو فارما</span>
                            <span class="impact-badge">🦷 طب الأسنان</span>
                        </div>
                        <div class="impact-grid">
                            <div class="impact-card">
                                <div class="impact-number">1,324</div>
                                <div class="impact-label" data-en="Prescriptions" data-ar="روشتات">روشتات</div>
                            </div>
                            <div class="impact-card">
                                <div class="impact-number">~1,150</div>
                                <div class="impact-label" data-en="Lab Tests" data-ar="تحاليل">تحاليل</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Final Insight -->
                <div class="mt-12 md:mt-16 p-6 md:p-10 gradient-bg text-white rounded-2xl md:rounded-3xl text-center shadow-2xl">
                    <h3 class="text-2xl md:text-3xl font-bold mb-4 md:mb-6" data-en="Final Insight" data-ar="الرؤية النهائية">الرؤية النهائية</h3>
                    <p class="text-base md:text-xl opacity-95 leading-relaxed mb-4 md:mb-6" data-en="From a small initiative built on four committees to a structured, scalable, and impact-driven organization. Medical Caravan has evolved into a model that combines Healthcare delivery, Community awareness, and Organizational excellence." data-ar="من مبادرة صغيرة مبنية على أربع لجان إلى منظمة منظمة وقابلة للتوسع وموجهة نحو التأثير. تطورت القافلة الطبية إلى نموذج يجمع بين تقديم الرعاية الصحية، والتوعية المجتمعية، والتميز التنظيمي.">
                        من مبادرة صغيرة مبنية على أربع لجان إلى منظمة منظمة وقابلة للتوسع وموجهة نحو التأثير. تطورت القافلة الطبية إلى نموذج يجمع بين تقديم الرعاية الصحية، والتوعية المجتمعية، والتميز التنظيمي.
                    </p>
                    <div class="flex flex-wrap justify-center gap-3 md:gap-4 mt-4 md:mt-6">
                        <span class="bg-white/20 backdrop-blur-sm px-4 md:px-6 py-2 md:py-3 rounded-full text-sm md:text-base">🏥 Healthcare Delivery</span>
                        <span class="bg-white/20 backdrop-blur-sm px-4 md:px-6 py-2 md:py-3 rounded-full text-sm md:text-base">📢 Community Awareness</span>
                        <span class="bg-white/20 backdrop-blur-sm px-4 md:px-6 py-2 md:py-3 rounded-full text-sm md:text-base">⭐ Organizational Excellence</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 md:py-24 bg-gradient-to-b from-gray-50 to-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12 md:mb-16">
                <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-800 section-title" data-en="Contact Us" data-ar="تواصل معنا">تواصل معنا</h2>
            </div>
            
            <div class="max-w-5xl mx-auto grid md:grid-cols-2 gap-6 md:gap-8">
                <div class="bg-white p-6 md:p-8 rounded-2xl md:rounded-3xl shadow-xl">
                    <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-4 md:mb-6" data-en="Get In Touch" data-ar="تواصل معنا">تواصل معنا</h3>
                    <div class="space-y-4 md:space-y-6">
                        <div class="flex items-center gap-3 md:gap-4">
                            <div class="w-12 h-12 md:w-14 md:h-14 gradient-bg rounded-xl md:rounded-2xl flex items-center justify-center text-white text-lg md:text-xl shadow-lg flex-shrink-0">📍</div>
                            <div>
                                <h4 class="font-bold text-gray-800 text-sm md:text-base" data-en="Address" data-ar="العنوان">العنوان</h4>
                                <p class="text-gray-600 text-xs md:text-sm" data-en="Faculty of Pharmacy, Ain Shams University, Cairo, Egypt" data-ar="كلية الصيدلة، جامعة عين شمس، القاهرة، مصر">كلية الصيدلة، جامعة عين شمس، القاهرة، مصر</p>
                            </div>
                        </div>
                        <div class="flex items-center gap-3 md:gap-4">
                            <div class="w-12 h-12 md:w-14 md:h-14 gradient-bg rounded-xl md:rounded-2xl flex items-center justify-center text-white text-lg md:text-xl shadow-lg flex-shrink-0">📧</div>
                            <div>
                                <h4 class="font-bold text-gray-800 text-sm md:text-base" data-en="Email" data-ar="البريد الإلكتروني">البريد الإلكتروني</h4>
                                <p class="text-gray-600 text-xs md:text-sm">medicalcaravan@pharm.asu.edu.eg</p>
                            </div>
                        </div>
                        <div class="flex items-center gap-3 md:gap-4">
                            <div class="w-12 h-12 md:w-14 md:h-14 gradient-bg rounded-xl md:rounded-2xl flex items-center justify-center text-white text-lg md:text-xl shadow-lg flex-shrink-0">📱</div>
                            <div>
                                <h4 class="font-bold text-gray-800 text-sm md:text-base" data-en="Social Media" data-ar="وسائل التواصل">وسائل التواصل</h4>
                                <p class="text-gray-600 text-xs md:text-sm" data-en="Follow us on LinkedIn, Facebook & Instagram" data-ar="تابعنا على LinkedIn و Facebook و Instagram">تابعنا على LinkedIn و Facebook و Instagram</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white p-6 md:p-8 rounded-2xl md:rounded-3xl shadow-xl">
                    <h3 class="text-xl md:text-2xl font-bold text-gray-800 mb-4 md:mb-6" data-en="Send Message" data-ar="أرسل رسالة">أرسل رسالة</h3>
                    <form class="space-y-3 md:space-y-4">
                        <input type="text" placeholder="الاسم / Name" class="w-full px-4 py-3 border border-gray-300 rounded-xl focus:outline-none focus:ring-2 focus:ring-primary transition text-sm md:text-base">
                        <input type="email" placeholder="البريد الإلكتروني / Email" class="w-full px-4 py-3 border border-gray-300 rounded-xl focus:outline-none focus:ring-2 focus:ring-primary transition text-sm md:text-base">
                        <textarea rows="4" placeholder="الرسالة / Message" class="w-full px-4 py-3 border border-gray-300 rounded-xl focus:outline-none focus:ring-2 focus:ring-primary transition text-sm md:text-base"></textarea>
                        <button type="submit" class="btn-primary w-full justify-center text-sm md:text-base" data-en="Send Message" data-ar="إرسال الرسالة">إرسال الرسالة</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark text-white py-12 md:py-16">
        <div class="container mx-auto px-4">
            <div class="grid md:grid-cols-3 gap-8 md:gap-12">
                <div>
                    <div class="flex items-center gap-3 mb-4 md:mb-6">
                        <div class="w-10 h-10 md:w-12 md:h-12 gradient-bg rounded-xl md:rounded-2xl flex items-center justify-center text-white text-lg md:text-xl shadow-lg">🏥</div>
                        <h3 class="text-xl md:text-2xl font-bold">القافلة الطبية</h3>
                    </div>
                    <p class="text-gray-400 leading-relaxed text-sm md:text-base" data-en="Delivering healthcare to underserved communities since 2005" data-ar="نقدم الرعاية الصحية للمجتمعات المحرومة منذ 2005">
                        نقدم الرعاية الصحية للمجتمعات المحرومة منذ 2005
                    </p>
                </div>
                <div>
                    <h4 class="font-bold mb-4 md:mb-6 text-base md:text-lg" data-en="Quick Links" data-ar="روابط سريعة">روابط سريعة</h4>
                    <ul class="space-y-2 md:space-y-3 text-gray-400 text-sm md:text-base">
                        <li><a href="#home" class="hover:text-white transition flex items-center gap-2"><span>▸</span> <span data-en="Home" data-ar="الرئيسية">الرئيسية</span></a></li>
                        <li><a href="#about" class="hover:text-white transition flex items-center gap-2"><span>▸</span> <span data-en="About" data-ar="عن القافلة">عن القافلة</span></a></li>
                        <li><a href="#committees" class="hover:text-white transition flex items-center gap-2"><span>▸</span> <span data-en="Committees" data-ar="اللجان">اللجان</span></a></li>
                        <li><a href="#history" class="hover:text-white transition flex items-center gap-2"><span>▸</span> <span data-en="History" data-ar="التاريخ">التاريخ</span></a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4 md:mb-6 text-base md:text-lg" data-en="Follow Us" data-ar="تابعنا">تابعنا</h4>
                    <div class="flex gap-3 md:gap-4">
                        <a href="#" class="w-10 h-10 md:w-12 md:h-12 bg-gray-700 rounded-xl flex items-center justify-center hover:gradient-bg transition shadow-lg">in</a>
                        <a href="#" class="w-10 h-10 md:w-12 md:h-12 bg-gray-700 rounded-xl flex items-center justify-center hover:gradient-bg transition shadow-lg">f</a>
                        <a href="#" class="w-10 h-10 md:w-12 md:h-12 bg-gray-700 rounded-xl flex items-center justify-center hover:gradient-bg transition shadow-lg">📷</a>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 md:mt-12 pt-6 md:pt-8 text-center text-gray-400 text-sm md:text-base">
                <p>&copy; 2025 Medical Caravan - Faculty of Pharmacy, Ain Shams University. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Committee Modal -->
    <div id="committeeModal" class="modal">
        <div class="modal-content">
            <button class="close-modal" onclick="closeCommitteeModal()">×</button>
            <div id="modalBody" class="p-6 md:p-8">
                <!-- Content will be injected here -->
            </div>
        </div>
    </div>

    <script>
        // Committee Data
        const committeeData = {
            pharmacy: {
                ar: {
                    title: "لجنة الصيدلة",
                    description: "لجنة الصيدلة هي العمود الفقري للقافلة الطبية، مسؤولة عن صرف الأدوية وإدارة المخزون الدوائي. تعمل اللجنة على ضمان توفير الأدوية المناسبة للمرضى وفقًا للوصفات الطبية، مع الحفاظ على أعلى معايير الجودة والسلامة.",
                    responsibilities: [
                        "صرف الأدوية للمرضى حسب الوصفات الطبية المعتمدة",
                        "إدارة المخزون الدوائي وتتبع تواريخ الصلاحية",
                        "التأكد من التخزين الصحيح للأدوية حسب متطلبات كل دواء",
                        "تقديم الاستشارات الدوائية للمرضى حول الاستخدام الصحيح",
                        "التنسيق مع اللجان الأخرى لضمان سير العمل بسلاسة",
                        "مراقبة التفاعلات الدوائية المحتملة",
                        "تصنيف الأدوية حسب الفئات العلاجية"
                    ],
                    achievements: "تم صرف أكثر من 50,000 وصفة طبية منذ تأسيس القافلة عام 2005، مع الحفاظ على أعلى معايير الجودة والسلامة الدوائية.",
                    history: "تأسست لجنة الصيدلة عام 2005 كواحدة من اللجان الأربع الأساسية للقافلة. كانت دائمًا في صميم عمليات القافلة، حيث نمت من صرف 800-1,200 روشتة سنويًا إلى آلاف الروشتات في الحملات الحديثة."
                },
                en: {
                    title: "Pharmacy Committee",
                    description: "The Pharmacy Committee is the backbone of the Medical Caravan, responsible for dispensing medications and managing pharmaceutical inventory. The committee ensures that patients receive appropriate medications according to medical prescriptions, maintaining the highest standards of quality and safety.",
                    responsibilities: [
                        "Dispensing medications to patients according to approved prescriptions",
                        "Managing pharmaceutical inventory and tracking expiry dates",
                        "Ensuring proper storage of medications according to requirements",
                        "Providing pharmaceutical consultations on proper usage",
                        "Coordinating with other committees to ensure smooth operations",
                        "Monitoring potential drug interactions",
                        "Classifying medications by therapeutic categories"
                    ],
                    achievements: "Over 50,000 prescriptions dispensed since the Caravan's foundation in 2005, maintaining the highest standards of pharmaceutical quality and safety.",
                    history: "The Pharmacy Committee was founded in 2005 as one of the four core committees of the Caravan. It has always been at the heart of Caravan operations, growing from dispensing 800-1,200 prescriptions annually to thousands in modern campaigns."
                },
                image: "https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/14b1043dc-9f47-4c95-9650-470f66cb1be0.png"
            },
            lab: {
                ar: {
                    title: "لجنة المعمل",
                    description: "لجنة المعمل تقوم بإجراء الفحوصات والتحاليل الطبية الأساسية للمرضى. توفر اللجنة خدمات تشخيصية متقدمة تساعد الأطباء في تحديد الحالات الطبية المناسبة واتخاذ القرارات العلاجية الصحيحة.",
                    responsibilities: [
                        "إجراء تحاليل الدم الأساسية (CBC)",
                        "قياس مستوى السكر في الدم",
                        "تحليل الكوليسترول والدهون",
                        "تحليل جرثومة المعدة (H. pylori)",
                        "تحليل وظائف الكبد والكلى",
                        "تسجيل النتائج وإرسالها للأطباء بدقة",
                        "صيانة وتجهيز الأجهزة المعملية"
                    ],
                    achievements: "تم إجراء أكثر من 10,000 تحليل طبي، مع إدخال تقنيات متقدمة مثل تحليل الدهون وجرثومة المعدة عام 2016.",
                    history: "بدأت لجنة المعمل كواحدة من اللجان الأساسية عام 2005، وتطورت لتشمل تحليلات متقدمة. من 200-400 تحليل سنويًا في البداية، وصلت إلى أكثر من 1,000 تحليل في الحملات الحديثة."
                },
                en: {
                    title: "Laboratory Committee",
                    description: "The Laboratory Committee conducts basic and advanced medical tests and analyses for patients. The committee provides diagnostic services that help physicians identify appropriate medical conditions and make correct treatment decisions.",
                    responsibilities: [
                        "Conducting basic blood tests (CBC)",
                        "Measuring blood sugar levels",
                        "Cholesterol and lipid profile analysis",
                        "H. pylori testing",
                        "Liver and kidney function tests",
                        "Recording results and sending them to physicians accurately",
                        "Maintaining and preparing laboratory equipment"
                    ],
                    achievements: "Over 10,000 medical tests conducted, with introduction of advanced techniques like lipid profile and H. pylori testing in 2016.",
                    history: "The Laboratory Committee started as one of the core committees in 2005, and evolved to include advanced analyses. From 200-400 tests annually in the beginning, it reached over 1,000 tests in modern campaigns."
                },
                image: "https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/1e19d5f1c-8cb7-4da6-8fd3-c31d5e140ad8.png"
            },
            preclinic: {
                ar: {
                    title: "لجنة ما قبل العيادة",
                    description: "لجنة ما قبل العيادة هي خط الدفاع الأول في نظام القافلة، مسؤولة عن فرز المرضى وتقييم الحالات الأولية قبل الوصول إلى الطبيب. تم إدخال هذا النظام عام 2024 كأحد أهم التطورات التشغيلية.",
                    responsibilities: [
                        "تسجيل بيانات المرضى الأساسية",
                        "قياس العلامات الحيوية (ضغط، حرارة، نبض، سكر)",
                        "تصنيف الحالات حسب الأولوية والخطورة",
                        "توجيه المرضى للعيادة المناسبة",
                        "تقليل وقت الانتظار وتحسين تجربة المريض",
                        "إجراء التقييم الأولي للأعراض",
                        "تنظيم تدفق المرضى بشكل منظم"
                    ],
                    achievements: "تم تطبيق نظام ما قبل العيادة عام 2024، مما حسن كفاءة التشغيل بنسبة 40% وقلل وقت الانتظار بشكل ملحوظ.",
                    history: "أُدخل نظام ما قبل العيادة عام 2024 (MC19) كأحد أكثر الترقيات التشغيلية تأثيرًا في تاريخ القافلة. هذا النظام يحسن تدفق المرضى ويضمن تقييم كل حالة بشكل صحيح."
                },
                en: {
                    title: "Pre-Clinic Committee",
                    description: "The Pre-Clinic Committee is the first line of defense in the Caravan system, responsible for triaging patients and assessing initial conditions before reaching the physician. This system was introduced in 2024 as one of the most important operational developments.",
                    responsibilities: [
                        "Recording basic patient data",
                        "Measuring vital signs (blood pressure, temperature, pulse, sugar)",
                        "Categorizing cases by priority and severity",
                        "Directing patients to appropriate clinics",
                        "Reducing waiting time and improving patient experience",
                        "Conducting initial symptom assessment",
                        "Organizing patient flow systematically"
                    ],
                    achievements: "Pre-Clinic System implemented in 2024, improving operational efficiency by 40% and significantly reducing waiting time.",
                    history: "The Pre-Clinic System was introduced in 2024 (MC19) as one of the most impactful operational upgrades in the Caravan's history. This system optimizes patient flow and ensures proper assessment of each case."
                },
                image: "https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/1ce3d8483-de25-4dab-9185-ec54a272e83e.png"
            },
            awareness: {
                ar: {
                    title: "لجنة التوعية",
                    description: "لجنة التوعية مسؤولة عن نشر الوعي الصحي في المجتمعات المستهدفة. تقوم اللجنة بحملات توعوية تفاعلية لتعليم المرضى عن الصحة والوقاية من الأمراض المزمنة.",
                    responsibilities: [
                        "تنظيم حملات التوعية الصحية التفاعلية",
                        "توزيع المنشورات والمواد التعليمية",
                        "إجراء جلسات توعوية جماعية وفردية",
                        "تثقيف المرضى عن الأمراض المزمنة (السكري، الضغط)",
                        "تعزيز نمط الحياة الصحي والتغذية السليمة",
                        "استخدام الوسائل البصرية والنماذج التشريحية",
                        "قياس تأثير الحملات التوعوية"
                    ],
                    achievements: "تم الوصول إلى أكثر من 100,000 تفاعل توعوي، مع حملات بارزة مثل 'وجه وأمل' عام 2023 التي حققت 6,245 تفاعل.",
                    history: "بدأت لجنة التوعية كلجنة أساسية عام 2005، وشهدت نموًا كبيرًا. من 1,500-3,000 تفاعل سنويًا في البداية، وصلت إلى أكثر من 6,000 تفاعل في الحملات الحديثة."
                },
                en: {
                    title: "Awareness Committee",
                    description: "The Awareness Committee is responsible for spreading health awareness in target communities. The committee conducts interactive awareness campaigns to educate patients about health and disease prevention.",
                    responsibilities: [
                        "Organizing interactive health awareness campaigns",
                        "Distributing brochures and educational materials",
                        "Conducting group and individual awareness sessions",
                        "Educating patients about chronic diseases (diabetes, hypertension)",
                        "Promoting healthy lifestyle and proper nutrition",
                        "Using visual aids and anatomical models",
                        "Measuring the impact of awareness campaigns"
                    ],
                    achievements: "Over 100,000 awareness interactions reached, with notable campaigns like 'Face & Hope' in 2023 achieving 6,245 interactions.",
                    history: "The Awareness Committee started as a core committee in 2005, and witnessed significant growth. From 1,500-3,000 interactions annually in the beginning, it reached over 6,000 interactions in modern campaigns."
                },
                image: "https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/1e70355bb-732b-4458-b3c3-0f45b09c3902.png"
            },
            hr: {
                ar: {
                    title: "لجنة الموارد البشرية",
                    description: "لجنة الموارد البشرية مسؤولة عن إدارة وتطوير أعضاء القافلة. تأسست اللجنة عام 2016 لتحويل القافلة إلى منظمة أكثر هيكلة واحترافية.",
                    responsibilities: [
                        "تنظيم الأعضاء في فرق وظيفية متخصصة",
                        "إدارة التواصل الداخلي وحل النزاعات",
                        "تعزيز إنتاجية الفريق والمساءلة",
                        "دعم التوظيف والتقييم وتطوير الأعضاء",
                        "تنظيم الفعاليات الداخلية وبناء الفريق",
                        "إدارة التدريب والتأهيل",
                        "تطوير الهيكل التنظيمي"
                    ],
                    achievements: "تم إدخال اللجنة عام 2016، مما ضمن تنسيق داخلي أقوى واستدامة للنمو المتزايد للقافلة.",
                    history: "تأسست لجنة الموارد البشرية عام 2016 (MC12) في المرج، مما مثل تحولاً كبيرًا في كيفية إدارة القافلة داخليًا. هذا حول القافلة من نشاط تشغيلي بحت إلى منظمة أكثر هيكلة."
                },
                en: {
                    title: "Human Resources Committee",
                    description: "The Human Resources Committee is responsible for managing and developing Caravan members. The committee was established in 2016 to transform the Caravan into a more structured and professional organization.",
                    responsibilities: [
                        "Organizing members into specialized functional teams",
                        "Managing internal communication and conflict resolution",
                        "Enhancing team productivity and accountability",
                        "Supporting recruitment, evaluation, and member development",
                        "Organizing internal events and team building",
                        "Managing training and qualification",
                        "Developing organizational structure"
                    ],
                    achievements: "Committee introduced in 2016, ensuring stronger internal coordination and sustainability for the Caravan's growing scale.",
                    history: "The HR Committee was established in 2016 (MC12) in El-Marg, marking a major shift in how the Caravan was managed internally. This transformed the Caravan from a purely operational activity into a more structured organization."
                },
                image: "https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/176793966-bed5-4003-828f-de2d84b75349.png"
            },
            fr: {
                ar: {
                    title: "لجنة جمع التبرعات",
                    description: "لجنة جمع التبرعات مسؤولة عن تأمين الدعم المالي وبناء الشراكات الخارجية. تأسست اللجنة عام 2017 لإضافة طبقة جديدة من الاستدامة المالية.",
                    responsibilities: [
                        "تأمين الدعم المالي من الرعاة",
                        "توسيع قدرة الخدمة من خلال التمويل",
                        "تحسين اللوجستيات والإمدادات الطبية",
                        "بناء الشراكات الخارجية مع الشركات",
                        "التواصل مع الرعاة الحاليين والمحتملين",
                        "إعداد مقترحات الرعاية",
                        "إدارة العلاقات مع الشركاء"
                    ],
                    achievements: "تم الحصول على رعايات من شركات مثل سوبرمو للأدوية (2020) وساتو فارما (2025)، مما ساهم في استمرارية القافلة.",
                    history: "بدأت جهود جمع التبرعات عام 2017 (MC13) في منشية ناصر، مما يمثل بداية بناء علاقات خارجية تساهم في استمرارية القافلة واستدامتها."
                },
                en: {
                    title: "Fundraising Committee",
                    description: "The Fundraising Committee is responsible for securing financial support and building external partnerships. The committee was established in 2017 to add a new layer of financial sustainability.",
                    responsibilities: [
                        "Securing financial support from sponsors",
                        "Expanding service capacity through funding",
                        "Improving logistics and medical supplies",
                        "Building external partnerships with companies",
                        "Communicating with current and potential sponsors",
                        "Preparing sponsorship proposals",
                        "Managing partner relationships"
                    ],
                    achievements: "Secured sponsorships from companies like Supremo Pharmaceuticals (2020) and Sato Pharma (2025), contributing to the Caravan's continuity.",
                    history: "Fundraising efforts began in 2017 (MC13) in Manshiet Naser, marking the beginning of building external relationships that contribute to the Caravan's continuity and sustainability."
                },
                image: "https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/13feda40d-2ac5-4533-8905-51fb4a0e6a5d.png"
            },
            operations: {
                ar: {
                    title: "لجنة العمليات واللوجستيات",
                    description: "لجنة العمليات واللوجستيات مسؤولة عن تنسيق جميع العمليات الميدانية وإدارة سلسلة التوريد. تضمن اللجنة سير الحملات بسلاسة وكفاءة.",
                    responsibilities: [
                        "نقل المعدات الطبية إلى مواقع القافلة",
                        "إدارة سلسلة التوريد والمخزون",
                        "تنظيم الإمدادات الطبية وتوزيعها",
                        "تنسيق اللوجستيات للقافلة",
                        "إدارة المستودعات والتوزيع",
                        "التخطيط للعمليات الميدانية",
                        "ضمان جاهزية المعدات"
                    ],
                    achievements: "تم تنفيذ نظام تدفق ذكي عام 2024، مما حسن الكفاءة التشغيلية وقلل الازدحام بشكل كبير.",
                    history: "تطورت لجنة العمليات على مر السنين لتصبح أكثر تعقيدًا واحترافية. من العمليات البسيطة في 2005 إلى نظام لوجستي متكامل في 2025."
                },
                en: {
                    title: "Operations & Logistics Committee",
                    description: "The Operations & Logistics Committee is responsible for coordinating all field operations and managing the supply chain. The committee ensures campaigns run smoothly and efficiently.",
                    responsibilities: [
                        "Medical equipment transport to Caravan locations",
                        "Supply chain and inventory management",
                        "Medical supplies organization and distribution",
                        "Logistics coordination for Caravan",
                        "Warehouse and distribution management",
                        "Field operations planning",
                        "Ensuring equipment readiness"
                    ],
                    achievements: "Smart Flow System implemented in 2024, improving operational efficiency and significantly reducing overcrowding.",
                    history: "The Operations Committee evolved over the years to become more complex and professional. From simple operations in 2005 to an integrated logistics system in 2025."
                },
                image: "https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/1745e1fa4-a3ca-445b-98d6-8bb6b290ac6a.png"
            },
            media: {
                ar: {
                    title: "لجنة الإعلام والتسويق",
                    description: "لجنة الإعلام والتسويق مسؤولة عن بناء العلامة التجارية والتواجد الرقمي للقافلة. تأسست اللجنة عام 2015 لتعزيز التواصل مع الجمهور.",
                    responsibilities: [
                        "إدارة وسائل التواصل الاجتماعي",
                        "إنشاء المحتوى المرئي والمكتوب",
                        "التصوير والتسجيل للحملات",
                        "تعزيز العلامة التجارية للقافلة",
                        "التسويق الرقمي والإعلانات",
                        "تغطية الأحداث والفعاليات",
                        "إدارة العلاقات العامة"
                    ],
                    achievements: "تم بناء علامة تجارية معروفة، مع وجود على LinkedIn وإنستجرام وفيسبوك، وزيادة كبيرة في الوصول والمشاركة.",
                    history: "تأسست لجنة التسويق عام 2015 (MC11)، مما غير طريقة تواصل القافلة مع جمهورها. هذا يمثل بداية بناء علامة تجارية معروفة وزيادة الوضوح."
                },
                en: {
                    title: "Media & Marketing Committee",
                    description: "The Media & Marketing Committee is responsible for building the Caravan's brand and digital presence. The committee was established in 2015 to enhance communication with the audience.",
                    responsibilities: [
                        "Social media management",
                        "Creating visual and written content",
                        "Photography and videography for campaigns",
                        "Promoting the Caravan's brand",
                        "Digital marketing and advertising",
                        "Event and activity coverage",
                        "Public relations management"
                    ],
                    achievements: "Built a recognizable brand with presence on LinkedIn, Instagram, and Facebook, with significant increase in reach and engagement.",
                    history: "The Marketing Committee was established in 2015 (MC11), changing how the Caravan communicated with its audience. This marked the beginning of building a recognizable brand and increasing visibility."
                },
                image: "https://image.qwenlm.ai/public_source/6aa70519-577d-4c7e-b511-b7d2992b909a/1335c2472-1a7d-46e4-94d9-575f7fd51237.png"
            }
        };

        // Language State
        let currentLang = 'ar';

        // Switch Language
        function switchLang(lang) {
            currentLang = lang;
            document.body.classList.toggle('en', lang === 'en');
            document.documentElement.lang = lang;
            document.documentElement.dir = lang === 'ar' ? 'rtl' : 'ltr';
            
            // Update language buttons
            document.querySelectorAll('.lang-btn').forEach(btn => {
                btn.classList.toggle('active', btn.textContent.toLowerCase().includes(lang === 'ar' ? 'عربي' : 'en'));
            });
            
            // Update all translatable elements
            document.querySelectorAll('[data-ar][data-en]').forEach(el => {
                el.textContent = el.getAttribute(`data-${lang}`);
            });
            
            // Update modal if open
            if (document.getElementById('committeeModal').classList.contains('active')) {
                const currentCommittee = document.getElementById('modalBody').dataset.committee;
                if (currentCommittee) {
                    openCommitteeModal(currentCommittee);
                }
            }
        }

        // Toggle Mobile Menu
        function toggleMobileMenu() {
            const nav = document.getElementById('mobileNav');
            nav.classList.toggle('active');
        }

        // Open Committee Modal
        function openCommitteeModal(committee) {
            const data = committeeData[committee];
            const content = data[currentLang];
            
            const modalBody = document.getElementById('modalBody');
            modalBody.dataset.committee = committee;
            modalBody.innerHTML = `
                <img src="${data.image}" alt="${content.title}" class="detail-image">
                <h2 class="text-2xl md:text-3xl lg:text-4xl font-bold text-gray-800 mb-3 md:mb-4">${content.title}</h2>
                <p class="text-gray-600 text-base md:text-lg mb-4 md:mb-6 leading-relaxed">${content.description}</p>
                
                <div class="info-grid">
                    <div class="info-box">
                        <h3 class="text-lg md:text-xl font-bold text-primary mb-3 flex items-center gap-2">
                            <span>📋</span>
                            <span>${currentLang === 'ar' ? 'المسؤوليات' : 'Responsibilities'}</span>
                        </h3>
                        <ul class="space-y-2">
                            ${content.responsibilities.map(item => `
                                <li class="flex items-start gap-3">
                                    <span class="text-primary mt-1 text-lg">✓</span>
                                    <span class="text-gray-600 text-sm md:text-base">${item}</span>
                                </li>
                            `).join('')}
                        </ul>
                    </div>
                </div>
                
                <div class="grid md:grid-cols-2 gap-4 md:gap-6 mt-4 md:mt-6">
                    <div class="bg-gradient-to-br from-blue-50 to-indigo-50 p-4 md:p-6 rounded-2xl">
                        <h3 class="text-lg md:text-xl font-bold text-primary mb-2 md:mb-3 flex items-center gap-2">
                            <span>🏆</span>
                            <span>${currentLang === 'ar' ? 'الإنجازات' : 'Achievements'}</span>
                        </h3>
                        <p class="text-gray-600 text-sm md:text-base">${content.achievements}</p>
                    </div>
                    <div class="bg-gradient-to-br from-green-50 to-emerald-50 p-4 md:p-6 rounded-2xl">
                        <h3 class="text-lg md:text-xl font-bold text-secondary mb-2 md:mb-3 flex items-center gap-2">
                            <span>📜</span>
                            <span>${currentLang === 'ar' ? 'التاريخ' : 'History'}</span>
                        </h3>
                        <p class="text-gray-600 text-sm md:text-base">${content.history}</p>
                    </div>
                </div>
            `;
            
            document.getElementById('committeeModal').classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        // Close Committee Modal
        function closeCommitteeModal() {
            document.getElementById('committeeModal').classList.remove('active');
            document.body.style.overflow = 'auto';
        }

        // Close modal on outside click
        document.getElementById('committeeModal').addEventListener('click', function(e) {
            if (e.target === this) {
                closeCommitteeModal();
            }
        });

        // Close modal on escape key
        document.addEventListener('keydown', function(e) {
            if (e.key === 'Escape') {
                closeCommitteeModal();
            }
        });

        // Smooth scroll for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });

        // Ensure all content is visible on load
        window.addEventListener('load', function() {
            document.querySelectorAll('.timeline-content').forEach(el => {
                el.style.display = 'block';
                el.style.visibility = 'visible';
                el.style.opacity = '1';
            });
        });
    </script>
</body>
</html>

