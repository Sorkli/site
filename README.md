<!DOCTYPE html>
<html lang="ru">
<head>
        <!-- Google tag (gtag.js) -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=G-BETR1B8E28"></script>
    <script>
        window.dataLayer = window.dataLayer || [];
        function gtag(){dataLayer.push(arguments);}
        gtag('js', new Date());
        gtag('config', 'G-BETR1B8E28');
    </script>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Маникюрный салон | Титановые ногти</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="icon" href="https://cdn-icons-png.flaticon.com/512/436/436469.png" sizes="any">
    <style>
        :root {
            --primary: #ff6b8b;
            --secondary: #a78bfa;
            --accent: #fbbf24;
            --light: #f8fafc;
            --dark: #1e293b;
            --text: #334155;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--text);
            line-height: 1.6;
            scroll-behavior: smooth;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }
        
        .header-scrolled {
            padding: 0.7rem 0;
            background: rgba(255, 107, 139, 0.95);
            backdrop-filter: blur(10px);
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            display: flex;
            align-items: center;
        }
        
        .logo i {
            margin-right: 10px;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 2rem;
            position: relative;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 5px 0;
        }
        
        nav ul li a:hover {
            color: var(--accent);
        }
        
        nav ul li a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background-color: var(--accent);
            transition: width 0.3s ease;
        }
        
        nav ul li a:hover::after {
            width: 100%;
        }
        
        .mobile-menu {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
            background: none;
            border: none;
            color: white;
        }
        
        /* Mobile Navigation */
        .mobile-nav {
            position: fixed;
            top: 0;
            right: -100%;
            width: 80%;
            max-width: 300px;
            height: 100vh;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            z-index: 1000;
            padding: 2rem;
            transition: right 0.4s ease;
            box-shadow: -5px 0 15px rgba(0, 0, 0, 0.1);
        }
        
        .mobile-nav.active {
            right: 0;
        }
        
        .mobile-nav-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 2rem;
        }
        
        .mobile-nav-logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: white;
        }
        
        .close-mobile-nav {
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        .mobile-nav-links {
            list-style: none;
        }
        
        .mobile-nav-links li {
            margin-bottom: 1.5rem;
        }
        
        .mobile-nav-links a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: 500;
            display: block;
            padding: 0.5rem 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }
        
        .mobile-nav-links a:hover {
            color: var(--accent);
            padding-left: 10px;
        }
        
        .mobile-nav-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            z-index: 999;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }
        
        .mobile-nav-overlay.active {
            opacity: 1;
            visibility: visible;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 100px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000" preserveAspectRatio="none"><path fill="rgba(255,255,255,0.05)" d="M0,0 L1000,0 L1000,1000 L0,1000 Z M0,0 C250,150 750,150 1000,0 L1000,1000 L0,1000 Z"></path></svg>');
            background-size: cover;
            background-position: center;
        }

        .hero .container {
            max-width: 800px;
            position: relative;
            z-index: 1;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            font-weight: 700;
            animation: fadeInUp 0.8s ease;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0.9;
            line-height: 1.6;
            animation: fadeInUp 0.8s ease 0.2s both;
        }

        .hero-buttons {
            display: flex;
            gap: 20px;
            justify-content: center;
            flex-wrap: wrap;
            animation: fadeInUp 0.8s ease 0.4s both;
        }

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

        .btn {
            display: inline-block;
            background: #2ecc71;
            color: white;
            padding: 15px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(46, 204, 113, 0.3);
        }

        .btn:hover {
            background: #27ae60;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .btn-secondary {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: rgba(255, 255, 255, 0.2);
            color: white;
            padding: 15px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            border: 2px solid rgba(255, 255, 255, 0.3);
            cursor: pointer;
            backdrop-filter: blur(10px);
        }

        .btn-secondary:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            z-index: 1000;
            overflow-y: auto;
            padding: 20px;
        }

        .modal-content {
            background-color: white;
            margin: 50px auto;
            padding: 0;
            border-radius: 15px;
            width: 90%;
            max-width: 700px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            animation: modalAppear 0.3s ease;
        }

        @keyframes modalAppear {
            from {
                opacity: 0;
                transform: translateY(-50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .modal-header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 20px;
            border-radius: 15px 15px 0 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: relative;
        }

        .modal-header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 100" preserveAspectRatio="none"><path fill="rgba(255,255,255,0.1)" d="M0,0 L1000,0 L1000,100 L0,100 Z M0,0 C250,50 750,50 1000,0 L1000,100 L0,100 Z"></path></svg>');
            background-size: cover;
        }

        .modal-header h3 {
            font-size: 24px;
            margin: 0;
            display: flex;
            align-items: center;
            gap: 10px;
            position: relative;
            z-index: 1;
        }

        .close-button {
            background: none;
            border: none;
            color: white;
            font-size: 24px;
            cursor: pointer;
            width: 30px;
            height: 30px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            transition: background 0.3s;
            position: relative;
            z-index: 1;
        }

        .close-button:hover {
            background: rgba(255, 255, 255, 0.2);
        }

        .modal-body {
            padding: 25px;
            color: #333;
            line-height: 1.6;
        }

        .modal-body p {
            margin-bottom: 15px;
            font-size: 16px;
        }

        .feature-list {
            list-style: none;
            margin: 20px 0;
        }

        .feature-list li {
            padding: 10px 0;
            border-bottom: 1px solid #eee;
            display: flex;
            align-items: flex-start;
            gap: 10px;
        }

        .feature-list li:last-child {
            border-bottom: none;
        }

        .feature-icon {
            color: #667eea;
            font-size: 18px;
            margin-top: 3px;
            flex-shrink: 0;
        }

        .benefit-card {
            background: #f8f9ff;
            border-radius: 10px;
            padding: 20px;
            margin: 20px 0;
            border-left: 4px solid #667eea;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
        }

        .benefit-card h4 {
            color: #2c3e50;
            margin-bottom: 10px;
            font-size: 18px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .highlight {
            background: linear-gradient(120deg, #f093fb 0%, #f5576c 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }

        .emoji {
            font-size: 20px;
            margin-right: 5px;
        }

        .advantages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin: 20px 0;
        }

        .advantage-item {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s ease;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
        }

        .advantage-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
        }

        .advantage-item i {
            font-size: 24px;
            color: #667eea;
            margin-bottom: 10px;
        }

        /* About Section */
        .section {
            padding: 5rem 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--dark);
            margin-bottom: 1rem;
            position: relative;
            display: inline-block;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background: linear-gradient(to right, var(--primary), var(--secondary));
            border-radius: 3px;
        }
        
        .section-title p {
            color: var(--text);
            max-width: 600px;
            margin: 0 auto;
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 3rem;
        }
        
        .about-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            position: relative;
        }
        
        .about-image::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, rgba(255,107,139,0.1), rgba(167,139,250,0.1));
            z-index: 1;
        }
        
        .about-image img {
            width: 100%;
            height: auto;
            display: block;
            transition: transform 0.5s ease;
        }
        
        .about-image:hover img {
            transform: scale(1.05);
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h3 {
            font-size: 1.8rem;
            margin-bottom: 1.5rem;
            color: var(--dark);
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1.5rem;
            margin-top: 2rem;
        }
        
        .feature {
            display: flex;
            align-items: flex-start;
            padding: 15px;
            border-radius: 8px;
            transition: all 0.3s ease;
        }
        
        .feature:hover {
            background: rgba(255,107,139,0.05);
            transform: translateY(-3px);
        }
        
        .feature i {
            color: var(--primary);
            font-size: 1.5rem;
            margin-right: 1rem;
            margin-top: 5px;
        }
        
        /* Services Section */
        .services {
            background-color: #f1f5f9;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .service-card {
            background-color: white;
            border-radius: 10px;
            padding: 2rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(to right, var(--primary), var(--secondary));
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .service-card i {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
        }
        
        .service-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--dark);
        }
        
        .price {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
            margin: 1rem 0;
        }
        
        /* Booking Section */
        .booking-container {
            display: flex;
            gap: 3rem;
            background-color: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .calendar-container {
            flex: 1;
            padding: 2rem;
            background-color: #f8fafc;
        }
        
        .calendar-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1.5rem;
        }
        
        .calendar-header button {
            background: var(--primary);
            color: white;
            border: none;
            width: 35px;
            height: 35px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .calendar-header button:hover {
            background: var(--secondary);
            transform: scale(1.1);
        }
        
        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 10px;
        }
        
        .calendar-day {
            text-align: center;
            font-weight: 600;
            padding: 10px 0;
            color: var(--dark);
        }
        
        .calendar-date {
            text-align: center;
            padding: 12px 0;
            border-radius: 50%;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 500;
        }
        
        .calendar-date:hover {
            background-color: #e2e8f0;
        }
        
        .calendar-date.selected {
            background-color: var(--primary);
            color: white;
        }
        
        .calendar-date.disabled {
            color: #cbd5e1;
            cursor: not-allowed;
        }
        
        .calendar-date.today {
            background-color: rgba(255,107,139,0.1);
            color: var(--primary);
            font-weight: 700;
        }
        
        .time-slots {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
            margin-top: 1.5rem;
        }
        
        .time-slot {
            padding: 10px;
            text-align: center;
            background-color: white;
            border: 1px solid #e2e8f0;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 500;
        }
        
        .time-slot:hover {
            background-color: #f1f5f9;
        }
        
        .time-slot.selected {
            background-color: var(--primary);
            color: white;
            border-color: var(--primary);
        }
        
        .booking-form {
            flex: 1;
            padding: 2rem;
        }
        
        .form-group {
            margin-bottom: 1.5rem;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
            color: var(--dark);
        }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #e2e8f0;
            border-radius: 5px;
            font-size: 1rem;
            transition: border 0.3s ease, box-shadow 0.3s ease;
        }
        
        .form-control:focus {
            border-color: var(--primary);
            outline: none;
            box-shadow: 0 0 0 3px rgba(255,107,139,0.1);
        }
        
        /* Gallery Section */
        .gallery {
            background-color: #f1f5f9;
        }
        
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }
        
        .gallery-item {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
            position: relative;
            cursor: pointer;
        }
        
        .gallery-item:hover {
            transform: scale(1.05);
        }
        
        .gallery-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            display: block;
            transition: transform 0.5s ease;
        }
        
        .gallery-item:hover img {
            transform: scale(1.1);
        }
        
        /* Contact Section */
        .contact-container {
            display: flex;
            gap: 3rem;
        }
        
        .contact-info {
            flex: 1;
        }
        
        .contact-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 2rem;
            padding: 15px;
            border-radius: 8px;
            transition: all 0.3s ease;
        }
        
        .contact-item:hover {
            background: rgba(255,107,139,0.05);
            transform: translateX(5px);
        }
        
        .contact-item i {
            color: var(--primary);
            font-size: 1.5rem;
            margin-right: 1rem;
            margin-top: 5px;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 3rem 0 1.5rem;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-between;
            margin-bottom: 2rem;
        }
        
        .footer-logo {
            font-size: 1.8rem;
            font-weight: 700;
            margin-bottom: 1rem;
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
        }
        
        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s ease, transform 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255,255,255,0.1);
        }
        
        .social-links a:hover {
            color: var(--primary);
            transform: translateY(-3px);
            background: rgba(255,255,255,0.2);
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: 1.5rem;
            border-top: 1px solid #334155;
        }
        
        /* Back to top button */
        .back-to-top {
            position: fixed;
            bottom: 20px;
            right: 20px;
            width: 50px;
            height: 50px;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            cursor: pointer;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
            z-index: 99;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }
        
        .back-to-top.visible {
            opacity: 1;
            visibility: visible;
        }
        
        .back-to-top:hover {
            background: var(--secondary);
            transform: translateY(-3px);
        }
        
        /* Loading animation */
        .loading {
            display: inline-block;
            width: 20px;
            height: 20px;
            border: 3px solid rgba(255,255,255,.3);
            border-radius: 50%;
            border-top-color: #fff;
            animation: spin 1s ease-in-out infinite;
            margin-right: 10px;
        }
        
        @keyframes spin {
            to { transform: rotate(360deg); }
        }
        
        /* Success message */
        .success-message {
            background: #2ecc71;
            color: white;
            padding: 15px 20px;
            border-radius: 8px;
            margin-bottom: 20px;
            display: none;
            animation: fadeIn 0.5s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        /* Responsive */
        @media (max-width: 992px) {
            .about-content, .booking-container, .contact-container {
                flex-direction: column;
            }
            
            .calendar-container, .booking-form {
                width: 100%;
            }
        }
        
        @media (max-width: 768px) {
            nav ul {
                display: none;
            }
            
            .mobile-menu {
                display: block;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .features {
                grid-template-columns: 1fr;
            }
            
            .time-slots {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .footer-content {
                flex-direction: column;
                gap: 2rem;
            }
            
            .hero-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .btn, .btn-secondary {
                width: 100%;
                max-width: 280px;
                justify-content: center;
            }

            .modal-content {
                margin: 20px auto;
                width: 95%;
            }

            .advantages-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header id="main-header">
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-spa"></i>
                    ANNAILS
                </div>
                <nav>
                    <ul>
                        <li><a href="#home">Главная</a></li>
                        <li><a href="#about">Обо мне</a></li>
                        <li><a href="#services">Услуги</a></li>
                        <li><a href="#gallery">Галерея</a></li>
                        <li><a href="#booking">Запись</a></li>
                        <li><a href="#contact">Контакты</a></li>
                    </ul>
                </nav>
                <button class="mobile-menu">
                    <i class="fas fa-bars"></i>
                </button>
            </div>
        </div>
    </header>

    <!-- Mobile Navigation -->
    <div class="mobile-nav-overlay"></div>
    <div class="mobile-nav">
        <div class="mobile-nav-header">
            <div class="mobile-nav-logo">
                <i class="fas fa-spa"></i>
                ANNAILS
            </div>
            <button class="close-mobile-nav">
                <i class="fas fa-times"></i>
            </button>
        </div>
        <ul class="mobile-nav-links">
            <li><a href="#home">Главная</a></li>
            <li><a href="#about">Обо мне</a></li>
            <li><a href="#services">Услуги</a></li>
            <li><a href="#booking">Запись</a></li>
            <li><a href="#gallery">Галерея</a></li>
            <li><a href="#contact">Контакты</a></li>
        </ul>
    </div>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Профессиональный маникюр с любовью к деталям</h1>
            <p>Создам идеальный маникюр, который подчеркнет вашу индивидуальность и дополнит ваш образ. Уникальная техника Титановые ногти - подходит для тех, у кого аллергия на гель-лак.</p>
            <div class="hero-buttons">
                <a href="#booking" class="btn">Записаться онлайн</a>
                <button class="btn-secondary" id="hero-titanium-btn">
                    <i class="fas fa-gem"></i>
                    Что такое титановые ногти
                </button>
            </div>
        </div>
    </section>

    <!-- Modal Window -->
    <div class="modal" id="titanium-modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3><i class="fas fa-gem"></i> Что же такое Титановые ногти?</h3>
                <button class="close-button" id="close-modal">&times;</button>
            </div>
            <div class="modal-body">
                <p>Давайте поговорим о титановых ногтях <span class="emoji">🌟</span></p>
                
                <p>Это название звучит довольно внушительно, верно? Многие из вас удивляются, услышав его <span class="emoji">)</span></p>
                
                <div class="benefit-card">
                    <h4><i class="fas fa-info-circle"></i> Откуда появилось название?</h4>
                    <p>Название «titanium nails» пришло к нам из Европы. Это особый порошок, используемый для создания маникюра, основанный на <span class="highlight">диоксиде титана</span>. Именно поэтому ногти получаются титановыми <span class="emoji">🤗</span></p>
                </div>
                
                <div class="advantages-grid">
                    <div class="advantage-item">
                        <i class="fas fa-sync-alt"></i>
                        <p><strong>Другие названия</strong><br>dip-система, порошковый маникюр, гель-пудра</p>
                    </div>
                    <div class="advantage-item">
                        <i class="fas fa-shield-alt"></i>
                        <p><strong>Для хрупких ногтей</strong><br>Идеально для длинных и хрупких ногтей</p>
                    </div>
                    <div class="advantage-item">
                        <i class="fas fa-allergies"></i>
                        <p><strong>Гипоаллергенно</strong><br>99% гипоаллергенно</p>
                    </div>
                    <div class="advantage-item">
                        <i class="fas fa-sun"></i>
                        <p><strong>Без УФ-лампы</strong><br>Не требует УФ-сушки</p>
                    </div>
                </div>
                
                <ul class="feature-list">
                    <li>
                        <i class="fas fa-check-circle feature-icon"></i>
                        <div>
                            <strong>Тонкое и прочное покрытие</strong> – идеально подходящее для длинных и хрупких ногтей.
                        </div>
                    </li>
                    <li>
                        <i class="fas fa-check-circle feature-icon"></i>
                        <div>
                            <strong>Гипоаллергенно на 99%</strong> и не требует использования ультрафиолетовой лампы <span class="emoji">🔥</span>
                        </div>
                    </li>
                </ul>
                
                <div class="benefit-card">
                    <h4><i class="fas fa-heart"></i> Решение для аллергии</h4>
                    <p>Так что, если вы столкнулись с проблемой аллергии на гель-лак, не отчаивайтесь! У меня есть решение для вас.</p>
                </div>
                
                <p>Большинство моих клиенток, которые уже опробовали этот метод, остались в восторге. Конечно, есть те, кто предпочитает гель-лак. И хорошо, что у нас есть такой широкий выбор!</p>
            </div>
        </div>
    </div>

    <!-- About Section -->
    <section class="section" id="about">
        <div class="container">
            <div class="section-title">
                <h2>Обо мне</h2>
            </div>
            <div class="about-content">
                <div class="about-image">
                    <img src="https://niidpo.ru/uplfile/news_image/kak-stat-masterom-manikyura-s-nulya.jpeg" alt="Мастер маникюра">
                </div>
                <div class="about-text">
                    <h3>Привет, я Семёнова Анна - мастер маникюра из г. Гатчины</h3>
                    <p>Я специализируюсь на современных техниках маникюра, включая гель-лак, титановые ногти, гелевое наращивание и художественную роспись. Моя цель - не просто сделать красивый маникюр, а создать произведение искусства, которое будет радовать вас каждый день.</p>
                    <p>Я постоянно совершенствую свои навыки, посещая мастер-классы, конкурсы и слежу за последними тенденциями в индустрии ногтевого сервиса.</p>
                    
                    <div class="features">
                        <div class="feature">
                            <i class="fas fa-award"></i>
                            <div>
                                <h4>Высокое качество</h4>
                                <p>Использую только профессиональные материалы</p>
                            </div>
                        </div>
                        <div class="feature">
                            <i class="fas fa-clock"></i>
                            <div>
                                <h4>Экономия времени</h4>
                                <p>Быстрое и качественное выполнение работы</p>
                            </div>
                        </div>
                        <div class="feature">
                            <i class="fas fa-heart"></i>
                            <div>
                                <h4>Индивидуальный подход</h4>
                                <p>Учитываю все ваши пожелания</p>
                            </div>
                        </div>
                        <div class="feature">
                            <i class="fas fa-shield-alt"></i>
                            <div>
                                <h4>Безопасность</h4>
                                <p>Строгое соблюдение норм гигиены</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="section services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Мои услуги</h2>
                <p>Широкий спектр услуг для ухода за вашими ногтями</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <i class="fas fa-paint-brush"></i>
                    <h3>Классический маникюр</h3>
                    <p>Обрезной маникюр с покрытием обычным лаком</p>
                    <div class="price">1000 ₽</div>
                </div>
                <div class="service-card">
                    <i class="fas fa-gem"></i>
                    <h3>Гель-лак</h3>
                    <p>Маникюр с покрытием гель-лаком</p>
                    <div class="price">1900 ₽</div>
                </div>
                <div class="service-card">
                    <i class="fas fa-magic"></i>
                    <h3>Наращивание ногтей</h3>
                    <p>Наращивание ногтей акрилом или гелем</p>
                    <div class="price">от 2000 ₽</div>
                </div>
                <div class="service-card">
                    <i class="fa-solid fa-wand-magic-sparkles"></i>
                    <h3>Титановые ногти</h3>
                    <p>Стойкое покрытие без УФ лампы</p>
                    <div class="price">2200 ₽</div>
                </div>
                <div class="service-card">
                    <i class="fas fa-palette"></i>
                    <h3>Дизайн ногтей</h3>
                    <p>Художественная роспись, стемпинг, фольга и другие техники</p>
                    <div class="price">от 500 ₽</div>
                </div>
                <div class="service-card">
                    <i class="fa-solid fa-shoe-prints"></i>
                    <h3>Педикюр</h3>
                    <p>Педикюр с покрытием гель-лаком</p>
                    <div class="price">2500 ₽</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="section gallery" id="gallery">
        <div class="container">
            <div class="section-title">
                <h2>Мои работы</h2>
            </div>
            <div class="gallery-grid">
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/736x/18/ac/b4/18acb42a1f403b160b72c16b86ce9ad0.jpg" alt="Маникюр 1">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/736x/01/87/98/018798c98465fed5ec90a23d470c9521.jpg" alt="Маникюр 2">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/1200x/df/90/e4/df90e44ec03866c075a16854c7d436f7.jpg" alt="Маникюр 3">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/1200x/c6/3b/d4/c63bd43d433bb5358ff91d8c378bbc89.jpg" alt="Маникюр 4">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/736x/1f/8d/71/1f8d7149f7b9d5076a09248e3449f193.jpg" alt="Маникюр 5">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/1200x/05/ee/e1/05eee1b443efa40eee81d4f34b7f8c73.jpg" alt="Маникюр 6">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/736x/43/aa/88/43aa889156503079625d1ab966162fa0.jpg" alt="Маникюр 7">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/736x/17/22/e3/1722e39780b53aa61d672ccda4ce635e.jpg" alt="Маникюр 8">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/736x/0c/14/26/0c1426e3d43ed7bbeebfd6b8d308a4dd.jpg" alt="Маникюр 9">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/736x/78/91/8a/78918a0ab9076cb23160025165b0ac9e.jpg" alt="Маникюр 10">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/736x/1d/4c/aa/1d4caa5e323591055e7a3c9510b4b53d.jpg" alt="Маникюр 11">
                </div>
                <div class="gallery-item">
                    <img src="https://i.pinimg.com/736x/80/89/c2/8089c2be92f9782b658768eaff32460f.jpg" alt="Маникюр 12">
                </div>
            </div>
        </div>
    </section>

    <!-- Booking Section -->
    <section class="section" id="booking">
        <div class="container">
            <div class="section-title">
                <h2>Онлайн запись</h2>
                <p>Выберите удобную дату и время для визита</p>
            </div>
            <div class="success-message" id="success-message">
                <i class="fas fa-check-circle"></i> Спасибо за запись! Мы свяжемся с вами для подтверждения.
            </div>
            <div class="booking-container">
                <div class="calendar-container">
                    <div class="calendar-header">
                        <button id="prev-month"><i class="fas fa-chevron-left"></i></button>
                        <h3 id="current-month">Ноябрь 2025</h3>
                        <button id="next-month"><i class="fas fa-chevron-right"></i></button>
                    </div>
                    <div class="calendar-grid" id="calendar-days">
                        <!-- Days of week -->
                        <div class="calendar-day">Пн</div>
                        <div class="calendar-day">Вт</div>
                        <div class="calendar-day">Ср</div>
                        <div class="calendar-day">Чт</div>
                        <div class="calendar-day">Пт</div>
                        <div class="calendar-day">Сб</div>
                        <div class="calendar-day">Вс</div>
                        <!-- Dates will be generated by JavaScript -->
                    </div>
                    
                    <h4 style="margin-top: 2rem;">Выберите время:</h4>
                    <div class="time-slots" id="time-slots">
                        <!-- Time slots will be generated by JavaScript -->
                    </div>
                </div>
                
                <div class="booking-form">
                    <h3>Заполните данные для записи</h3>
                    <form id="appointment-form">
                        <input type="hidden" id="selected-date" name="selected-date">
                        <input type="hidden" id="selected-time" name="selected-time">
                        <div class="form-group">
                            <label for="name">Ваше имя</label>
                            <input type="text" id="name" name="name" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="phone">Телефон</label>
                            <input type="tel" id="phone" name="phone" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" name="email" class="form-control">
                        </div>
                        <div class="form-group">
                            <label for="service">Услуга</label>
                            <select id="service" name="service" class="form-control" required>
                                <option value="">Выберите услугу</option>
                                <option value="Классический маникюр">Классический маникюр - 1000 ₽</option>
                                <option value="Титановые ногти">Титановые ногти - 2200 ₽</option>
                                <option value="Гель-лак">Гель-лак - 1900₽</option>
                                <option value="Наращивание ногтей">Наращивание ногтей - от 2000 ₽</option>
                                <option value="Педикюр">Педикюр + гель-лак - 2500 ₽</option>
                                <option value="Дизайн ногтей">Дизайн ногтей - от 300 ₽</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="notes">Дополнительные пожелания</label>
                            <textarea id="notes" name="notes" class="form-control" rows="4"></textarea>
                        </div>
                        <button type="submit" class="btn" style="width: 100%;" id="submit-btn">
                            <span id="submit-text">Записаться</span>
                            <span id="submit-loading" class="loading" style="display: none;"></span>
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="section" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Контакты</h2>
                <p>Свяжитесь со мной для консультации</p>
            </div>
            
            <div class="contact-container">
                <div class="contact-info">
                    <div class="contact-item">
                        <i class="fas fa-map-marker-alt"></i>
                        <div>
                            <h3>Адрес</h3>
                            <p>г. Гатчина, ул. Филиппова, д. 4</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-phone"></i>
                        <div>
                            <h3>Телефон</h3>
                            <p>+7 (921) 111-11-11</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-envelope"></i>
                        <div>
                            <h3>Email</h3>
                            <p>sorklielza@yandex.ru</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-clock"></i>
                        <div>
                            <h3>Время работы</h3>
                            <p>Пн-Пт: 9:00 - 20:00</p>
                            <p>Сб-Вс: 10:00 - 18:00</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div>
                    <div class="footer-logo">
                        <i class="fas fa-spa"></i>
                        ANNAILS
                    </div>
                    <p>Профессиональный маникюр с любовью к деталям</p>
                </div>
                <div>
                    <h4>Быстрые ссылки</h4>
                    <ul style="list-style: none; padding: 0;">
                        <li><a href="#home" style="color: white; text-decoration: none;">Главная</a></li>
                        <li><a href="#about" style="color: white; text-decoration: none;">Обо мне</a></li>
                        <li><a href="#services" style="color: white; text-decoration: none;">Услуги</a></li>
                        <li><a href="#booking" style="color: white; text-decoration: none;">Запись</a></li>
                    </ul>
                </div>
                <div>
                    <h4>Социальные сети</h4>
                    <div class="social-links">
                        <a href="https://t.me/annails_gatchina"><i class="fab fa-telegram"></i></a>
                        <a href="https://api.whatsapp.com/send/?phone=79817684278&text&type=phone_number&app_absent=0"><i class="fab fa-whatsapp"></i></a>
                        <a href="https://vk.com/annailsss"><i class="fab fa-vk"></i></a>
                    </div>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2025 ANNAILS. Все права защищены.</p>
            </div>
        </div>
    </footer>

    <!-- Back to top button -->
    <button class="back-to-top" id="back-to-top">
        <i class="fas fa-chevron-up"></i>
    </button>

    <script>
        // Calendar functionality with Formspree integration
        document.addEventListener('DOMContentLoaded', function() {
            let currentDate = new Date();
            let selectedDate = null;
            let selectedTime = null;
            
            const monthNames = ["Январь", "Февраль", "Март", "Апрель", "Май", "Июнь",
                "Июль", "Август", "Сентябрь", "Октябрь", "Ноябрь", "Декабрь"
            ];
            
            const timeSlots = [
                "09:00", "10:00", "11:00", "12:00", "13:00", "14:00", 
                "15:00", "16:00", "17:00", "18:00", "19:00"
            ];
            
            // Initialize calendar
            function initCalendar() {
                renderCalendar(currentDate);
                renderTimeSlots();
                
                // Add event listeners
                document.getElementById('prev-month').addEventListener('click', prevMonth);
                document.getElementById('next-month').addEventListener('click', nextMonth);
                
                // Form submission
                document.getElementById('appointment-form').addEventListener('submit', handleAppointmentSubmit);
                
                // Mobile navigation
                document.querySelector('.mobile-menu').addEventListener('click', openMobileNav);
                document.querySelector('.close-mobile-nav').addEventListener('click', closeMobileNav);
                document.querySelector('.mobile-nav-overlay').addEventListener('click', closeMobileNav);
                
                // Mobile nav links
                document.querySelectorAll('.mobile-nav-links a').forEach(link => {
                    link.addEventListener('click', closeMobileNav);
                });
                
                // Back to top button
                document.getElementById('back-to-top').addEventListener('click', scrollToTop);
                window.addEventListener('scroll', toggleBackToTop);
                
                // Header scroll effect
                window.addEventListener('scroll', toggleHeaderScroll);
            }
            
            function renderCalendar(date) {
                const calendarDays = document.getElementById('calendar-days');
                const currentMonth = document.getElementById('current-month');
                
                // Clear existing dates (keep days of week)
                while (calendarDays.children.length > 7) {
                    calendarDays.removeChild(calendarDays.lastChild);
                }
                
                // Set current month
                currentMonth.textContent = `${monthNames[date.getMonth()]} ${date.getFullYear()}`;
                
                // Get first day of month and number of days
                const firstDay = new Date(date.getFullYear(), date.getMonth(), 1);
                const lastDay = new Date(date.getFullYear(), date.getMonth() + 1, 0);
                const daysInMonth = lastDay.getDate();
                
                // Calculate the day of week for the first day (0=Sunday, 1=Monday, etc.)
                // Adjust for our calendar where Monday is the first day
                let firstDayOfWeek = firstDay.getDay();
                // Convert to our system where Monday=0, Tuesday=1, ..., Sunday=6
                firstDayOfWeek = firstDayOfWeek === 0 ? 6 : firstDayOfWeek - 1;
                
                // Add empty cells for days before the first day of the month
                for (let i = 0; i < firstDayOfWeek; i++) {
                    const emptyCell = document.createElement('div');
                    emptyCell.className = 'calendar-date disabled';
                    calendarDays.appendChild(emptyCell);
                }
                
                // Add cells for each day of the month
                const today = new Date();
                today.setHours(0, 0, 0, 0);
                
                for (let i = 1; i <= daysInMonth; i++) {
                    const dateCell = document.createElement('div');
                    dateCell.className = 'calendar-date';
                    dateCell.textContent = i;
                    
                    const cellDate = new Date(date.getFullYear(), date.getMonth(), i);
                    
                    // Highlight today
                    if (cellDate.toDateString() === today.toDateString()) {
                        dateCell.classList.add('today');
                    }
                    
                    // Disable past dates
                    if (cellDate < today) {
                        dateCell.classList.add('disabled');
                    } else {
                        dateCell.addEventListener('click', function() {
                            selectedDate = cellDate;
                            updateSelected();
                        });
                    }
                    
                    // Highlight selected date
                    if (selectedDate && 
                        selectedDate.getDate() === i && 
                        selectedDate.getMonth() === date.getMonth() && 
                        selectedDate.getFullYear() === date.getFullYear()) {
                        dateCell.classList.add('selected');
                    }
                    
                    calendarDays.appendChild(dateCell);
                }
            }
            
            function renderTimeSlots() {
                const timeSlotsContainer = document.getElementById('time-slots');
                timeSlotsContainer.innerHTML = '';
                
                timeSlots.forEach(time => {
                    const timeSlot = document.createElement('div');
                    timeSlot.className = 'time-slot';
                    timeSlot.textContent = time;
                    
                    timeSlot.addEventListener('click', function() {
                        selectedTime = time;
                        updateSelected();
                    });
                    
                    if (selectedTime === time) {
                        timeSlot.classList.add('selected');
                    }
                    
                    timeSlotsContainer.appendChild(timeSlot);
                });
            }
            
            function updateSelected() {
                // Update calendar
                const dates = document.querySelectorAll('.calendar-date');
                dates.forEach(date => {
                    date.classList.remove('selected');
                });
                
                if (selectedDate) {
                    const selectedDateElement = Array.from(dates).find(date => {
                        return !date.classList.contains('disabled') && 
                               parseInt(date.textContent) === selectedDate.getDate();
                    });
                    
                    if (selectedDateElement) {
                        selectedDateElement.classList.add('selected');
                    }
                }
                
                // Update time slots
                const times = document.querySelectorAll('.time-slot');
                times.forEach(time => {
                    time.classList.remove('selected');
                    if (time.textContent === selectedTime) {
                        time.classList.add('selected');
                    }
                });
                
                // Update hidden fields
                document.getElementById('selected-date').value = selectedDate ? selectedDate.toLocaleDateString('ru-RU') : '';
                document.getElementById('selected-time').value = selectedTime || '';
            }
            
            function prevMonth() {
                currentDate.setMonth(currentDate.getMonth() - 1);
                renderCalendar(currentDate);
            }
            
            function nextMonth() {
                currentDate.setMonth(currentDate.getMonth() + 1);
                renderCalendar(currentDate);
            }
            
            // Form submission handlers
            function handleAppointmentSubmit(e) {
                e.preventDefault();
                
                // Validate date and time selection
                if (!selectedDate || !selectedTime) {
                    alert('Пожалуйста, выберите дату и время для записи');
                    return;
                }
                
                const submitBtn = document.getElementById('submit-btn');
                const submitText = document.getElementById('submit-text');
                const submitLoading = document.getElementById('submit-loading');
                
                // Show loading state
                submitText.textContent = 'Отправка...';
                submitLoading.style.display = 'inline-block';
                submitBtn.disabled = true;
                
                // Prepare form data
                const formData = new FormData(document.getElementById('appointment-form'));
                
                // Send to Formspree
                fetch('https://formspree.io/f/xrbonwnv', {
                    method: 'POST',
                    body: formData,
                    headers: {
                        'Accept': 'application/json'
                    }
                })
                .then(response => {
                    if (response.ok) {
                        // Show success message
                        document.getElementById('success-message').style.display = 'block';
                        // Reset form
                        document.getElementById('appointment-form').reset();
                        // Reset date and time selection
                        selectedDate = null;
                        selectedTime = null;
                        updateSelected();
                        renderCalendar(currentDate);
                        
                        // Hide success message after 5 seconds
                        setTimeout(() => {
                            document.getElementById('success-message').style.display = 'none';
                        }, 5000);
                    } else {
                        throw new Error('Ошибка отправки формы');
                    }
                })
                .catch(error => {
                    alert('Произошла ошибка при отправке формы. Пожалуйста, попробуйте позже или свяжитесь с нами по телефону.');
                    console.error('Form submission error:', error);
                })
                .finally(() => {
                    // Reset button state
                    submitText.textContent = 'Записаться';
                    submitLoading.style.display = 'none';
                    submitBtn.disabled = false;
                });
            }
            
            // Mobile navigation functions
            function openMobileNav() {
                document.querySelector('.mobile-nav').classList.add('active');
                document.querySelector('.mobile-nav-overlay').classList.add('active');
                document.body.style.overflow = 'hidden';
            }
            
            function closeMobileNav() {
                document.querySelector('.mobile-nav').classList.remove('active');
                document.querySelector('.mobile-nav-overlay').classList.remove('active');
                document.body.style.overflow = 'auto';
            }
            
            // Back to top functionality
            function scrollToTop() {
                window.scrollTo({
                    top: 0,
                    behavior: 'smooth'
                });
            }
            
            function toggleBackToTop() {
                const backToTopBtn = document.getElementById('back-to-top');
                if (window.pageYOffset > 300) {
                    backToTopBtn.classList.add('visible');
                } else {
                    backToTopBtn.classList.remove('visible');
                }
            }
            
            // Header scroll effect
            function toggleHeaderScroll() {
                const header = document.getElementById('main-header');
                if (window.pageYOffset > 50) {
                    header.classList.add('header-scrolled');
                } else {
                    header.classList.remove('header-scrolled');
                }
            }
            
            // Initialize the calendar
            initCalendar();
        });

        // Modal functionality for titanium nails
        document.addEventListener('DOMContentLoaded', function() {
            const modal = document.getElementById('titanium-modal');
            const heroBtn = document.getElementById('hero-titanium-btn');
            const closeBtn = document.getElementById('close-modal');
            
            // Open modal when button is clicked
            if (heroBtn) {
                heroBtn.addEventListener('click', function() {
                    if (modal) {
                        modal.style.display = 'block';
                        document.body.style.overflow = 'hidden';
                    }
                });
            }
            
            // Close modal when X button is clicked
            if (closeBtn) {
                closeBtn.addEventListener('click', function() {
                    if (modal) {
                        modal.style.display = 'none';
                        document.body.style.overflow = 'auto';
                    }
                });
            }
            
            // Close modal when clicking outside the content
            if (modal) {
                modal.addEventListener('click', function(e) {
                    if (e.target === modal) {
                        modal.style.display = 'none';
                        document.body.style.overflow = 'auto';
                    }
                });
            }
            
            // Close modal with Escape key
            document.addEventListener('keydown', function(e) {
                if (e.key === 'Escape' && modal && modal.style.display === 'block') {
                    modal.style.display = 'none';
                    document.body.style.overflow = 'auto';
                }
            });
        });
    </script>
</body>
</html>
