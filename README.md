<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <meta name="description" content="Stratix AI - Cutting-edge AI solutions for businesses">
    <!-- OpenGraph / Social Media Meta Tags -->
    <meta property="og:title" content="Stratix AI | AI Solutions for Business Growth">
    <meta property="og:description" content="Innovative AI solutions designed to help startups and growing businesses compete in the digital age.">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://stratixai.com">
    <meta property="og:image" content="https://res.cloudinary.com/dhpl09d00/image/upload/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png">
    <!-- Favicon -->
    <link rel="icon" href="https://res.cloudinary.com/dhpl09d00/image/upload/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png" type="image/png">
    <title>Stratix AI | AI Solutions for Business Growth</title>
    <!-- Preconnect to external resources -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="preload" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
    <noscript><link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"></noscript>
    <link rel="preload" href="https://cdn.jsdelivr.net/npm/locomotive-scroll@4.1.4/dist/locomotive-scroll.min.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
    <noscript><link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/locomotive-scroll@4.1.4/dist/locomotive-scroll.min.css"></noscript>
    <!-- Structured Data -->
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Organization",
      "name": "Stratix AI",
      "url": "https://stratixai.com",
      "logo": "https://res.cloudinary.com/dhpl09d00/image/upload/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png",
      "description": "Innovative AI solutions for the modern business",
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "San Francisco",
        "addressRegion": "CA",
        "postalCode": "94107",
        "addressCountry": "US"
      },
      "contactPoint": {
        "@type": "ContactPoint",
        "contactType": "customer support",
        "email": "contact@stratixai.com"
      }
    }
    </script>
    <style>
        :root {
            --primary: #2563eb;
            --primary-dark: #1d4ed8;
            --dark: #1e293b;
            --light: #f8fafc;
            --gray: #94a3b8;
            --success: #10b981;
            --cursor-x: 0px;
            --cursor-y: 0px;
        }
       body {
    cursor: default; /* Set cursor visibility for better accessibility */
}
        body {
            font-family: 'Space Grotesk', sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
            overflow-x: hidden;
            transition: background 0.5s ease;
        }
        /* Dark Mode */
        body.dark-mode {
            background-color: #0f172a;
            color: #f8fafc;
        }
        body.dark-mode section:nth-child(even) {
            background-color: #1e293b;
        }
        body.dark-mode .tech-card,
        body.dark-mode .network-node,
        body.dark-mode .contact-form {
            background-color: #1e293b;
            border-color: #334155;
            color: #f8fafc;
        }
        body.dark-mode p {
            color: #cbd5e1;
        }
        body.dark-mode input,
        body.dark-mode textarea,
        body.dark-mode select {
            background: #1e293b;
            border-color: #334155;
            color: #f8fafc;
        }
        /* Splash Screen */
        #splash {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: var(--light);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 9999;
            transition: opacity 1s ease;
        }
        #splash img {
            width: 150px;
            height: auto;
            animation: pulse 2s;
        }
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
        /* Floating Shapes Background */
        .floating-shapes {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: -1;
            top: 0;
            left: 0;
        }
        .shape {
            position: absolute;
            opacity: 0.15;
            filter: blur(60px);
            border-radius: 50%;
        }
        .shape-1 {
            width: 400px;
            height: 400px;
            background: var(--primary);
            top: 10%;
            left: 5%;
            animation: float 15s infinite ease-in-out;
        }
        .shape-2 {
            width: 300px;
            height: 300px;
            background: #10b981;
            bottom: 15%;
            right: 10%;
            animation: float 12s infinite ease-in-out reverse;
        }
        .shape-3 {
            width: 250px;
            height: 250px;
            background: #7c3aed;
            top: 40%;
            right: 20%;
            animation: float 18s infinite ease-in-out;
            animation-delay: 2s;
        }
        @keyframes float {
            0%, 100% { transform: translate(0, 0) rotate(0deg); }
            50% { transform: translate(30px, 40px) rotate(5deg); }
        }
        /* Gradient Backgrounds */
        .gradient-bg {
            background: radial-gradient(circle at 70% 30%, rgba(37, 99, 235, 0.08) 0%, rgba(255,255,255,1) 60%);
        }
        body.dark-mode .gradient-bg {
            background: radial-gradient(circle at 70% 30%, rgba(37, 99, 235, 0.1) 0%, rgba(15, 23, 42, 1) 60%);
        }
        .gradient-text {
            background: linear-gradient(90deg, var(--primary), #7c3aed);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: inline;
        }
        /* Tech Cards */
        .tech-card {
            background: white;
            border-radius: 16px;
            padding: 2rem;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            position: relative;
            overflow: hidden;
            transition: transform 0.4s ease, box-shadow 0.4s ease;
            border: 1px solid rgba(0, 0, 0, 0.03);
            will-change: transform;
        }
        body.dark-mode .tech-card {
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }
        .tech-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(37, 99, 235, 0.03), transparent);
            transform: rotate(45deg);
            z-index: 0;
            transition: all 0.6s ease;
        }
        .tech-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
        }
        body.dark-mode .tech-card:hover {
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
        }
        .tech-card:hover::before {
            transform: rotate(45deg) translate(10%, 10%);
        }
        /* AI Chips */
        .ai-chip {
            display: inline-block;
            background: rgba(37, 99, 235, 0.1);
            color: var(--primary);
            padding: 0.5rem 1rem;
            border-radius: 100px;
            font-size: 0.9rem;
            margin-right: 0.5rem;
            margin-bottom: 0.5rem;
            transition: all 0.3s ease;
        }
        body.dark-mode .ai-chip {
            background: rgba(37, 99, 235, 0.2);
        }
        .ai-chip:hover {
            background: rgba(37, 99, 235, 0.2);
            transform: translateY(-2px);
        }
        body.dark-mode .ai-chip:hover {
            background: rgba(37, 99, 235, 0.3);
        }
        /* Animated Illustrations */
        .animated-illustration {
            width: 100%;
            max-width: 500px;
            height: auto;
            margin: 2rem auto;
            position: relative;
        }
        .pulse-dot {
            position: absolute;
            width: 12px;
            height: 12px;
            background: var(--primary);
            border-radius: 50%;
            animation: pulse 2s ;
        }
        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.3); opacity: 0.7; }
        }
        /* Network Grid */
        .network-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 1rem;
            margin: 3rem 0;
        }
        .network-node {
            background: white;
            border-radius: 12px;
            padding: 1.5rem;
            text-align: center;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            will-change: transform;
        }
        .network-node::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), #7c3aed);
        }
        .network-node:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.08);
        }
        body.dark-mode .network-node:hover {
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        /* Header */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background-color: rgba(255, 255, 255, 0.95);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            z-index: 100;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }
        body.dark-mode header {
            background-color: rgba(15, 23, 42, 0.95);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
        }
        header.scrolled {
            background-color: rgba(255, 255, 255, 0.98);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }
        body.dark-mode header.scrolled {
            background-color: rgba(15, 23, 42, 0.98);
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
            max-width: 1400px;
            margin: 0 auto;
        }
        .logo img {
            height: 40px;
            width: auto;
            transition: transform 0.3s ease;
        }
        .logo:hover img {
            transform: scale(1.05);
        }
        .nav-links {
            display: flex;
            gap: 2rem;
            align-items: center;
        }
        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: color 0.3s ease;
            position: relative;
        }
        body.dark-mode .nav-links a {
            color: #f8fafc;
        }
        .nav-links a:hover {
            color: var(--primary);
        }
        .nav-links a:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -5px;
            left: 0;
            background-color: var(--primary);
            transition: width 0.3s ease;
        }
        .nav-links a:hover:after {
            width: 100%;
        }
        .cta-btn {
            background-color: var(--primary);
            color: white;
            padding: 0.6rem 1.2rem;
            border-radius: 6px;
            font-weight: 600;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        .cta-btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(37, 99, 235, 0.3);
        }
        .cta-btn::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(transparent, rgba(255,255,255,0.3), transparent);
            transform: rotate(45deg);
            transition: all 0.6s ease;
        }
        .cta-btn:hover::after {
            left: 100%;
        }
        #menu-toggle {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: none;
            color: var(--dark);
            transition: transform 0.3s ease;
        }
        body.dark-mode #menu-toggle {
            color: #f8fafc;
        }
        #menu-toggle:hover {
            transform: scale(1.1);
        }
        /* Dark Mode Toggle */
        .dark-mode-toggle {
            position: relative;
            width: 50px;
            height: 24px;
            background: #e2e8f0;
            border-radius: 12px;
            cursor: none;
            transition: background 0.3s ease;
            margin-left: 1rem;
        }
        body.dark-mode .dark-mode-toggle {
            background: #334155;
        }
        .toggle-thumb {
            position: absolute;
            top: 2px;
            left: 2px;
            width: 20px;
            height: 20px;
            background: var(--primary);
            border-radius: 50%;
            transition: transform 0.3s ease;
        }
        body.dark-mode .toggle-thumb {
            transform: translateX(26px);
        }
        /* Main Content */
        main {
            padding-top: 80px;
            max-width: 1400px;
            margin: 0 auto;
            position: relative;
        }
        section {
            padding: 6rem 2rem;
            scroll-margin-top: 80px;
            position: relative;
        }
        section:nth-child(even) {
            background-color: #f1f5f9;
        }
        body.dark-mode section:nth-child(even) {
            background-color: #1e293b;
        }
        h1, h2, h3 {
            line-height: 1.2;
            margin-bottom: 1.5rem;
        }
        h1 {
            font-size: 3.5rem;
            font-weight: 700;
        }
        h2 {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
        }
        h2:after {
            content: '';
            position: absolute;
            width: 80px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), #7c3aed);
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }
        h3 {
            font-size: 1.5rem;
            color: var(--primary);
        }
        p {
            margin-bottom: 1rem;
            color: var(--gray);
        }
        body.dark-mode p {
            color: #94a3b8;
        }
        /* Hero Section */
        .hero {
            min-height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        .hero-content {
            position: relative;
            z-index: 2;
            max-width: 800px;
        }
        .hero p {
            font-size: 1.5rem;
            max-width: 700px;
            margin: 2rem auto;
        }
        .hero button {
            background-color: var(--primary);
            color: white;
            border: none;
            padding: 1rem 2rem;
            font-size: 1.1rem;
            border-radius: 8px;
            cursor: none;
            font-weight: 600;
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(37, 99, 235, 0.2);
        }
        .hero button:hover {
            background-color: var(--primary-dark);
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(37, 99, 235, 0.3);
        }
        .hero button::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(transparent, rgba(255,255,255,0.4), transparent);
            transform: rotate(45deg);
            transition: all 0.6s ease;
        }
        .hero button:hover::after {
            left: 100%;
        }
        /* Typing Animation */
        .typing-text {
            display: inline-block;
            position: relative;
        }
        .typing-text::after {
            content: '|';
            position: absolute;
            right: -8px;
            animation: blink 0.7s infinite;
        }
        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }
        /* Grid Layouts */
        .services-list, .industries-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        /* Contact Form */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: white;
            padding: 2.5rem;
            border-radius: 16px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
            position: relative;
            overflow: hidden;
        }
        body.dark-mode .contact-form {
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }
        .contact-form::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--primary), #7c3aed);
        }
        .contact-form p {
            text-align: center;
            margin-bottom: 2rem;
        }
        form {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }
        .form-group {
            position: relative;
        }
        label {
            font-weight: 500;
            color: var(--dark);
            margin-bottom: 0.5rem;
            display: block;
        }
        body.dark-mode label {
            color: #f8fafc;
        }
        input, textarea, select {
            padding: 0.8rem 1rem;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
            font-family: inherit;
            font-size: 1rem;
            transition: all 0.3s ease;
            width: 100%;
            background: #f8fafc;
        }
        input:focus, textarea:focus, select:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.1);
            background: white;
        }
        body.dark-mode input:focus,
        body.dark-mode textarea:focus,
        body.dark-mode select:focus {
            background: #1e293b;
            box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.2);
        }
        textarea {
            resize: vertical;
            min-height: 150px;
        }
        form button {
            background-color: var(--primary);
            color: white;
            border: none;
            padding: 1rem;
            font-size: 1rem;
            border-radius: 8px;
            cursor: none;
            font-weight: 600;
            transition: all 0.3s ease;
            margin-top: 1rem;
        }
        form button:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(37, 99, 235, 0.2);
        }
        /* Footer */
        footer {
            text-align: center;
            padding: 3rem 2rem;
            background-color: var(--dark);
            color: white;
            position: relative;
            overflow: hidden;
        }
        footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--primary), #7c3aed);
        }
        footer p {
            color: rgba(255,255,255,0.8);
        }
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            text-align: left;
            padding-bottom: 2rem;
        }
        .footer-logo img {
            height: 40px;
            margin-bottom: 1rem;
            filter: brightness(0) invert(1);
        }
        .footer-links h3 {
            color: white;
            margin-bottom: 1rem;
            font-size: 1.2rem;
        }
        .footer-links ul {
            list-style: none;
        }
        .footer-links li {
            margin-bottom: 0.5rem;
        }
        .footer-links a {
            color: rgba(255,255,255,0.8);
            text-decoration: none;
            transition: color 0.3s ease;
        }
        .footer-links a:hover {
            color: white;
        }
        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
        }
        .social-links a {
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255,255,255,0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }
        .social-links a:hover {
            background: var(--primary);
            transform: translateY(-3px);
        }
        .footer-bottom {
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding-top: 1.5rem;
            margin-top: 2rem;
        }
        /* Animations */
        .fade-in {
            opacity: 0;
        }
        @keyframes fadeIn {
            to { opacity: 1; }
        }
        /* Back to Top Button */
        #back-to-top {
            position: fixed;
            bottom: 2rem;
            right: 2rem;
            width: 50px;
            height: 50px;
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: none;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
            z-index: 99;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        #back-to-top.visible {
            opacity: 1;
            visibility: visible;
        }
        #back-to-top:hover {
            background-color: var(--primary-dark);
            transform: translateY(-5px);
        }
        /* Loading Bar */
        .loading-bar {
            position: fixed;
            top: 0;
            left: 0;
            height: 3px;
            background: linear-gradient(90deg, var(--primary), #7c3aed);
            z-index: 1000;
            transition: width 0.4s ease;
        }
        /* Mobile Styles */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            h2 {
                font-size: 2rem;
            }
            .nav-links {
                position: fixed;
                top: 80px;
                left: 0;
                width: 100%;
                background-color: white;
                flex-direction: column;
                gap: 1rem;
                padding: 2rem;
                box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
                transform: translateY(-150%);
                transition: transform 0.3s ease;
            }
            body.dark-mode .nav-links {
                background-color: #1e293b;
                box-shadow: 0 10px 15px rgba(0, 0, 0, 0.3);
            }
            .nav-links.show {
                transform: translateY(0);
            }
            .nav-links a {
                padding: 0.5rem 0;
            }
            #menu-toggle {
                display: block;
            }
            section {
                padding: 4rem 1.5rem;
            }
            .hero {
                min-height: 70vh;
                padding: 0 1.5rem;
            }
            .services-list, .industries-list {
                grid-template-columns: 1fr;
            }
            .footer-content {
                grid-template-columns: 1fr;
                text-align: center;
            }
            .footer-links {
                text-align: center;
            }
            .social-links {
                justify-content: center;
            }
            .network-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>

<body>
    <div class="loading-bar"></div>
    <div id="splash">
        <img src="https://res.cloudinary.com/dhpl09d00/image/upload/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png" alt="Stratix AI Logo">
    </div>
    <div class="cursor"></div>
    <div class="cursor-follower"></div>
    <div class="floating-shapes">
        <div class="shape shape-1"></div>
        <div class="shape shape-2"></div>
        <div class="shape shape-3"></div>
    </div>
    <header>
        <nav>
            <div class="logo">
                <img src="https://res.cloudinary.com/dhpl09d00/image/upload/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png" alt="Stratix AI Logo" loading="lazy">
            </div>
            <div class="nav-links">
                <a href="#about" aria-label="About Section">About</a>
                <a href="#services" aria-label="Services Section">Services</a>
                <a href="#industries" aria-label="Industries Section">Industries</a>
                <a href="#contact" aria-label="Contact Section">Contact</a>
                <a class="cta-btn" href="#signup" aria-label="Free Demo">Free Demo</a>
               <button class="dark-mode-toggle" aria-label="Toggle Dark Mode">
    <span class="toggle-thumb" aria-hidden="true"></span>
</button>
            <button id="menu-toggle" aria-label="Toggle Navigation" aria-expanded="false">☰</button>
        </nav>
    </header>
    <main>
        <section class="hero gradient-bg fade-in" id="hero">
            <div class="hero-content">
                <h1>Transform Your Business with <span class="gradient-text typing-text">AI</span></h1>
                <p>Innovative AI solutions designed to help startups and growing businesses compete in the digital age.</p>
                <button onclick="window.location.href='#contact'" aria-label="Get Started">Get Started Today</button>
            </div>    
            <div class="animated-illustration">
               <svg viewBox="0 0 500 300" xmlns="http://www.w3.org/2000/svg" role="img" aria-labelledby="svgDesc">
    <title id="svgDesc">AI network illustration showing nodes and connections</title>
                    <!-- AI network illustration -->
                    <circle cx="250" cy="150" r="100" fill="none" stroke="var(--primary)" stroke-width="2" stroke-dasharray="5,5"/>
                    <circle cx="250" cy="150" r="70" fill="none" stroke="var(--primary)" stroke-width="2" stroke-dasharray="3,3"/>  
                    <!-- Nodes -->
                    <circle cx="250" cy="150" r="10" fill="var(--primary)"/>
                    <circle cx="150" cy="150" r="8" fill="var(--primary)" class="pulse-dot" style="top: 140px; left: 140px;"/>
                    <circle cx="350" cy="150" r="8" fill="var(--primary)" class="pulse-dot" style="top: 140px; left: 340px; animation-delay: 0.5s;"/>
                    <circle cx="250" cy="50" r="8" fill="var(--primary)" class="pulse-dot" style="top: 40px; left: 240px; animation-delay: 1s;"/>
                    <circle cx="250" cy="250" r="8" fill="var(--primary)" class="pulse-dot" style="top: 240px; left: 240px; animation-delay: 1.5s;"/>
                    <!-- Connecting lines -->
                    <line x1="250" y1="150" x2="350" y2="150" stroke="var(--primary)" stroke-width="2" stroke-opacity="0.3"/>
                    <line x1="250" y1="150" x2="250" y2="50" stroke="var(--primary)" stroke-width="2" stroke-opacity="0.3"/>
                    <line x1="250" y1="150" x2="250" y2="250" stroke="var(--primary)" stroke-width="2" stroke-opacity="0.3"/>
                </svg>
            </div>
        </section>
        <section id="about" class="fade-in">
            <h2>About Us</h2>
            <div class="about-content">
                <div class="tech-card" style="max-width: 1000px; margin: 0 auto;">
                    <h3 style="color: var(--primary); margin-bottom: 1rem;">The Future of Business AI Starts Here</h3>
                    <p>Stratix AI is a forward-thinking startup dedicated to bringing powerful AI solutions to businesses at all stages. Founded in 2024, we're building the tools that will help shape the future of intelligent business operations.</p>
                    <p>Our team combines cutting-edge technical expertise with a deep understanding of business challenges. We're passionate about creating AI solutions that are both powerful and accessible.</p>
                    <div style="margin-top: 2rem; display: flex; flex-wrap: wrap;">
                        <span class="ai-chip"><i class="fas fa-bolt" style="margin-right: 5px;"></i> Fast Implementation</span>
                        <span class="ai-chip"><i class="fas fa-lock" style="margin-right: 5px;"></i> Secure By Design</span>
                        <span class="ai-chip"><i class="fas fa-sync-alt" style="margin-right: 5px;"></i> Continuous Learning</span>
    <span class="ai-chip"><i class="fas fa-expand" style="margin-right: 5px;"></i> Scalable Solutions</span>
                    </div>
                </div>
                <div class="network-grid">
                    <div class="network-node">
                        <i class="fas fa-rocket" style="font-size: 2rem; color: var(--primary); margin-bottom: 1rem;"></i>
                        <h3>Innovation</h3>
                        <p>Pushing boundaries with cutting-edge AI research</p>
                    </div>
                    <div class="network-node">
                        <i class="fas fa-handshake" style="font-size: 2rem; color: var(--primary); margin-bottom: 1rem;"></i>
                        <h3>Partnership</h3>
                        <p>Collaborative approach to solving problems</p>
                    </div>
                    <div class="network-node">
                        <i class="fas fa-lightbulb" style="font-size: 2rem; color: var(--primary); margin-bottom: 1rem;"></i>
                        <h3>Creativity</h3>
                        <p>Unique solutions tailored to your needs</p>
                    </div>
                </div>
            </div>
        </section>
        <section id="services" class="fade-in gradient-bg">
            <h2>Our Services</h2>
            <div class="services-list">
                <div class="tech-card">
                    <h3><i class="fas fa-robot" style="margin-right: 10px;"></i> AI Consulting</h3>
                    <p>Strategic guidance to help you identify the best AI opportunities for your specific business needs and goals.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Strategy</span>
                        <span class="ai-chip">Roadmapping</span>
                        <span class="ai-chip">Implementation</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-brain" style="margin-right: 10px;"></i> Machine Learning</h3>
                    <p>Custom ML models designed to extract insights from your data and automate complex processes.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Predictive Analytics</span>
                        <span class="ai-chip">Automation</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-comment-dots" style="margin-right: 10px;"></i> NLP Solutions</h3>
                    <p>Natural language processing to help you understand and interact with customers more effectively.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Chatbots</span>
                        <span class="ai-chip">Sentiment Analysis</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-chart-line" style="margin-right: 10px;"></i> Data Analytics</h3>
                    <p>Transform your raw data into actionable insights with our advanced analytics platforms.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Visualization</span>
                        <span class="ai-chip">Real-time</span>
                        <span class="ai-chip">Dashboards</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-cogs" style="margin-right: 10px;"></i> Process Automation</h3>
                    <p>Streamline operations and reduce costs with intelligent automation solutions.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">RPA</span>
                        <span class="ai-chip">Workflows</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-shield-alt" style="margin-right: 10px;"></i> AI Security</h3>
                    <p>Protect your business with AI-powered threat detection and prevention systems.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Anomaly Detection</span>
                        <span class="ai-chip">Fraud Prevention</span>
                    </div>
                </div>
            </div>
        </section>
        <section id="industries" class="fade-in">
            <h2>Industries We Serve</h2>
            <div class="industries-list">
                <div class="tech-card">
                    <h3><i class="fas fa-heartbeat" style="margin-right: 10px;"></i> Healthcare</h3>
                    <p>AI solutions for diagnostics, patient care optimization, and medical research acceleration.</p>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-money-bill-wave" style="margin-right: 10px;"></i> Finance</h3>
                    <p>Fraud detection, risk assessment, algorithmic trading, and personalized banking.</p>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-shopping-cart" style="margin-right: 10px;"></i> Retail</h3>
                    <p>Personalized recommendations, inventory optimization, and customer experience enhancement.</p>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-industry" style="margin-right: 10px;"></i> Manufacturing</h3>
                    <p>Predictive maintenance, quality control, and supply chain optimization.</p>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-graduation-cap" style="margin-right: 10px;"></i> Education</h3>
                    <p>Adaptive learning platforms, automated grading, and student performance analytics.</p>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-truck" style="margin-right: 10px;"></i> Logistics</h3>
                    <p>Route optimization, demand forecasting, and autonomous delivery systems.</p>
                </div>
            </div>
        </section>
        <section id="contact" class="fade-in gradient-bg">
            <h2>Get In Touch</h2>
            <div class="contact-form">
                <p>Ready to transform your business with AI? Contact us for a free consultation.</p>
                <form id="contactForm">
                    <input type="hidden" name="_csrf" value="csrf-token-placeholder">
                    <div class="form-group">
                        <label for="name">Name</label>
                        <input type="text" id="name" name="name" required aria-required="true">
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="email" required aria-required="true">
                    </div>
                    <div class="form-group">
                        <label for="company">Company</label>
                        <input type="text" id="company" name="company">
                    </div>
                    <div class="form-group">
                        <label for="service">Service of Interest</label>
                        <select id="service" name="service" aria-label="Select a service">
                            <option value="">Select a service</option>
                            <option value="consulting">AI Consulting</option>
                            <option value="ml">Machine Learning</option>
                            <option value="nlp">NLP Solutions</option>
                            <option value="analytics">Data Analytics</option>
                            <option value="automation">Process Automation</option>
                            <option value="security">AI Security</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" name="message" required aria-required="true"></textarea>
                    </div>
                    <div class="form-group" aria-live="polite" id="formStatus"></div>
                    <button type="submit" aria-label="Send Message">Send Message</button>
                </form>
            </div>
        </section>
    </main>
    <footer>
        <div class="footer-content">
            <div class="footer-logo">
                <img src="https://res.cloudinary.com/dhpl09d00/image/upload/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png" alt="Stratix AI Logo" loading="lazy">
                <p>Innovative AI solutions for the modern business.</p>
                <div class="social-links">
                    <a href="#" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
                    <a href="#" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
                    <a href="#" aria-label="GitHub"><i class="fab fa-github"></i></a>
                    <a href="#" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
                </div>
            </div>
            <div class="footer-links">
                <h3>Company</h3>
                <ul>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#industries">Industries</a></li>
                    <li><a href="#">Careers</a></li>
                    <li><a href="#">Blog</a></li>
                </ul>
            </div>
            <div class="footer-links">
                <h3>Resources</h3>
                <ul>
                    <li><a href="#">Documentation</a></li>
                    <li><a href="#">API Reference</a></li>
                    <li><a href="#">Case Studies</a></li>
                    <li><a href="#">Whitepapers</a></li>
                    <li><a href="#">FAQ</a></li>
                </ul>
            </div>
            <div class="footer-links">
                <h3>Legal</h3>
                <ul>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Terms of Service</a></li>
                    <li><a href="#">Security</a></li>
                    <li><a href="#">Cookie Policy</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2024 Stratix AI. All rights reserved.</p>
        </div>
    </footer>
    <button id="back-to-top" aria-label="Back to Top">
        <i class="fas fa-arrow-up"></i>
    </button>
    <script src="https://cdn.jsdelivr.net/npm/locomotive-scroll@4.1.4/dist/locomotive-scroll.min.js"></script>
    <script>
        // Feature detection
        const supportsSmoothScroll = 'scrollBehavior' in document.documentElement.style;
        // Wait for the DOM to be fully loaded
        document.addEventListener('DOMContentLoaded', function() {
            // Splash screen animation
            setTimeout(function() {
                const splash = document.getElementById('splash');
                if (splash) {
                    splash.style.opacity = '0';
                    setTimeout(function() {
                        splash.style.display = 'none';
                    }, 1000);
                }
            }, 1500);
            // Initialize Locomotive Scroll with fallback
           try {
    const mainElement = document.querySelector('main');
    if (mainElement) {
        const scroll = new LocomotiveScroll({
            el: mainElement,
            smooth: true,
            smartphone: { smooth: true },
            tablet: { smooth: true }
        });
    }
}
                // Update scroll when content changes
                if (scroll && typeof scroll.update === 'function') {
                    scroll.update();
                }
            } catch (e) {
                console.error('Locomotive Scroll initialization failed:', e);
                if (supportsSmoothScroll) {
                    document.documentElement.style.scrollBehavior = 'smooth';
                }
            }
            // Custom cursor with fallback for touch devices
            if (!('ontouchstart' in window || navigator.maxTouchPoints)) {
                const cursor = document.querySelector('.cursor');
                const cursorFollower = document.querySelector('.cursor-follower');
                const links = document.querySelectorAll('a, button, .ai-chip, input, textarea, select');
                document.addEventListener('mousemove', (e) => {
                    if (cursor) {
                        cursor.style.left = e.clientX + 'px';
                        cursor.style.top = e.clientY + 'px';
                    }
                    // Follower with delay
                    setTimeout(() => {
                        if (cursorFollower) {
                            cursorFollower.style.left = e.clientX + 'px';
                            cursorFollower.style.top = e.clientY + 'px';
                        }
                    }, 100);
                });
                // Cursor hover effects
                if (links.length && cursor && cursorFollower) {
                    links.forEach(link => {
                        link.addEventListener('mouseenter', () => {
                            cursor.style.transform = 'translate(-50%, -50%) scale(1.5)';
                            cursorFollower.style.transform = 'translate(-50%, -50%) scale(1.2)';
                        });  
                        link.addEventListener('mouseleave', () => {
                            cursor.style.transform = 'translate(-50%, -50%) scale(1)';
                            cursorFollower.style.transform = 'translate(-50%, -50%) scale(1)';
                        });
                    });
                }
            } else {
                // Remove custom cursor elements on touch devices
                const cursor = document.querySelector('.cursor');
                const cursorFollower = document.querySelector('.cursor-follower');
                if (cursor) cursor.remove();
                if (cursorFollower) cursorFollower.remove();
                document.body.style.cursor = 'default';
            }
            // Mobile menu toggle with ARIA attributes
            const menuToggle = document.getElementById('menu-toggle');
            const navLinks = document.querySelector('.nav-links');
            if (menuToggle && navLinks) {
                menuToggle.addEventListener('click', () => {
                    const isExpanded = navLinks.classList.toggle('show');
                    menuToggle.setAttribute('aria-expanded', isExpanded);
                    menuToggle.textContent = isExpanded ? '✕' : '☰';
                });
            }
            // Close mobile menu when clicking a link
            document.querySelectorAll('.nav-links a').forEach(link => {
                link.addEventListener('click', () => {
                    if (window.innerWidth <= 768 && navLinks && menuToggle) {
                        navLinks.classList.remove('show');
                        menuToggle.setAttribute('aria-expanded', 'false');
                        menuToggle.textContent = '☰';
                    }
                });
            });
            // Dark mode toggle with localStorage
            const darkModeToggle = document.querySelector('.dark-mode-toggle');
            if (darkModeToggle) {
                darkModeToggle.addEventListener('click', toggleDarkMode);
                darkModeToggle.addEventListener('keydown', (e) => {
                    if (e.key === 'Enter' || e.key === ' ') {
                        e.preventDefault();
                        toggleDarkMode();
                    }
                });
            }
            function toggleDarkMode() {
                document.body.classList.toggle('dark-mode');
                const isDarkMode = document.body.classList.contains('dark-mode');
                localStorage.setItem('darkMode', isDarkMode);
            }
            // Check for saved dark mode preference
            if (localStorage.getItem('darkMode') === 'true') {
                document.body.classList.add('dark-mode');
            }
            // Back to top button with smooth scroll polyfill if needed
            const backToTopButton = document.getElementById('back-to-top');
            if (backToTopButton) {
                window.addEventListener('scroll', () => {
                    if (window.pageYOffset > 300) {
                        backToTopButton.classList.add('visible');
                    } else {
                        backToTopButton.classList.remove('visible');
                    }
                });
                backToTopButton.addEventListener('click', () => {
                    if (supportsSmoothScroll) {
                        window.scrollTo({ top: 0, behavior: 'smooth' });
                    } else {
                        // Fallback for browsers without smooth scroll
                        const scrollStep = -window.scrollY / (500 / 15);
                        const scrollInterval = setInterval(() => {
                            if (window.scrollY !== 0) {
                                window.scrollBy(0, scrollStep);
                            } else {
                                clearInterval(scrollInterval);
                            }
                        }, 15);
                    }
                });
            }
            // Form submission with fetch API
            const contactForm = document.getElementById('contactForm');
            const formStatus = document.getElementById('formStatus');
            if (contactForm) {
                contactForm.addEventListener('submit', async (e) => {
                    e.preventDefault();
                    const submitButton = contactForm.querySelector('button[type="submit"]');  
                    try {
                        // Disable submit button during submission
                        submitButton.disabled = true;
                        submitButton.textContent = 'Sending...';    
                        // Get form values
                        const formData = new FormData(contactForm);
                        const data = Object.fromEntries(formData);   
                        // In a real implementation, you would send this to your server
                        console.log('Form submitted:', data);
                        // Simulate API call delay
                        await new Promise(resolve => setTimeout(resolve, 1500));
                        // Show success message
                        if (formStatus) {
                            formStatus.textContent = 'Thank you for your message! We will get back to you soon.';
                            formStatus.style.color = 'var(--success)';
                        }
                        contactForm.reset();
                    } catch (error) {
                        console.error('Form submission error:', error);
                        if (formStatus) {
                            formStatus.textContent = 'There was an error submitting your message. Please try again.';
                            formStatus.style.color = 'red';
                        }
                    } finally {
                        // Re-enable submit button
                        if (submitButton) {
                            submitButton.disabled = false;
                            submitButton.textContent = 'Send Message';
                        } 
                        // Clear status message after 5 seconds
                        if (formStatus) {
                            setTimeout(() => {
                                formStatus.textContent = '';
                            }, 5000);
                        }
                    }
                });
            }
            // Loading bar animation
            const loadingBar = document.querySelector('.loading-bar');
            if (loadingBar) {
                window.addEventListener('scroll', () => {
                    const scrollHeight = document.documentElement.scrollHeight - window.innerHeight;
                    const scrolled = (window.scrollY / scrollHeight) * 100;
                    loadingBar.style.width = scrolled + '%';
                });
            }
            // Typing animation with error handling
            const typingText = document.querySelector('.typing-text');
            if (typingText) {
                const words = ['AI', 'Machine Learning', 'Automation', 'Innovation'];
                let wordIndex = 0;
                let charIndex = 0;
                let isDeleting = false;
                let isEnd = false;
                function type() {
                    if (!typingText) return;      
                    const currentWord = words[wordIndex];
                    const currentChar = currentWord.substring(0, charIndex);
                    typingText.textContent = currentChar;   
                    if (!isDeleting && charIndex < currentWord.length) {
                        // Typing
                        charIndex++;
                        setTimeout(type, 100);
                    } else if (isDeleting && charIndex > 0) {
                        // Deleting
                        charIndex--;
                        setTimeout(type, 50);
                    } else {
                        // Change word
                        isDeleting = !isDeleting;
                        if (!isDeleting) {
                            wordIndex = (wordIndex + 1) % words.length;
                        }
                        setTimeout(type, 1000);
                    }
                }
                // Start typing animation
                setTimeout(type, 1000);
            }
            // Fade-in animation for sections with intersection observer
            const fadeElements = document.querySelectorAll('.fade-in');
            if (fadeElements.length) {
                if ('IntersectionObserver' in window) {
                    const observer = new IntersectionObserver((entries) => {
                        entries.forEach(entry => {
                            if (entry.isIntersecting) {
                                entry.target.style.animation = 'fadeIn 1s forwards';
                                observer.unobserve(entry.target);
                            }
                        });
                    }, { threshold: 0.1 });
                    fadeElements.forEach(element => {
                        observer.observe(element);
                    });
                } else {
                    // Fallback for browsers without IntersectionObserver
                    function checkFade() {
                        fadeElements.forEach(element => {
                            const elementTop = element.getBoundingClientRect().top;
                            const windowHeight = window.innerHeight; 
                            if (elementTop < windowHeight - 100) {
                                element.style.animation = 'fadeIn 1s forwards';
                            }
                        });
                    } 
                    // Initial check
                    checkFade(); 
                    // Check on scroll
                    window.addEventListener('scroll', checkFade);
                }
            }
            // Header scroll effect
            const header = document.querySelector('header');
            if (header) {
                window.addEventListener('scroll', () => {
                    if (window.scrollY > 50) {
                        header.classList.add('scrolled');
                    } else {
                        header.classList.remove('scrolled');
                    }
                });
            }
            // Add focus styles for keyboard navigation
            document.addEventListener('keyup', function(e) {
                if (e.key === 'Tab') {
                    document.documentElement.classList.add('keyboard-navigation');
                }
            });
            document.addEventListener('mousedown', function() {
                document.documentElement.classList.remove('keyboard-navigation');
            });
        });
        </main>
  <footer>
    </footer>
  <script>
    document.addEventListener('DOMContentLoaded', function() {
      setTimeout(function() {
        const splash = document.getElementById('splash');
        if (splash) {
          splash.style.opacity = '0';
          setTimeout(function() {
            splash.style.display = 'none';
          }, 1000); // Wait for the fade-out transition
        }
      }, 2000); // Adjust the delay (in milliseconds) as needed
    });
  </script>
</body>
        // Add keyboard focus styles
        const style = document.createElement('style');
        style.textContent = `
            .keyboard-navigation a:focus,
            .keyboard-navigation button:focus,
            .keyboard-navigation input:focus,
            .keyboard-navigation textarea:focus,
            .keyboard-navigation select:focus {
                outline: 2px solid var(--primary);
                outline-offset: 2px;
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
