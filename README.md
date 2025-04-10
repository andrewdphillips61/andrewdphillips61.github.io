<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Stratix AI - Cutting-edge AI solutions for businesses">
    <title>Stratix AI | AI Solutions for Business Growth</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://res.cloudinary.com/dhpl09d00/image/upload/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png">
    <style>
        :root {
            --primary: #2563eb;
            --primary-dark: #1d4ed8;
            --dark: #1e293b;
            --light: #f8fafc;
            --gray: #94a3b8;
            --success: #10b981;
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Space Grotesk', sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
            overflow-x: hidden;
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
            animation: pulse 2s infinite;
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
        .ai-chip:hover {
            background: rgba(37, 99, 235, 0.2);
            transform: translateY(-2px);
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
            animation: pulse 2s infinite;
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
        header.scrolled {
            background-color: rgba(255, 255, 255, 0.98);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
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
            cursor: pointer;
            color: var(--dark);
            transition: transform 0.3s ease;
        }
        #menu-toggle:hover {
            transform: scale(1.1);
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
            cursor: pointer;
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
            cursor: pointer;
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
            animation: fadeIn 1s ease forwards;
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
            cursor: pointer;
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
        }
    </style>
</head>

<body>
    <div id="splash">
        <img src="https://res.cloudinary.com/dhpl09d00/image/upload/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png" alt="Stratix AI Logo">
    </div>
    <div class="floating-shapes">
        <div class="shape shape-1"></div>
        <div class="shape shape-2"></div>
        <div class="shape shape-3"></div>
    </div>
    <header>
        <nav>
            <div class="logo">
                <img src="https://drive.google.com/uc?id=14n0I2p7w7cp83dr9zv6m9HT2rIcqdXNJ&export=view" alt="Stratix AI Logo">
            </div>
            <div class="nav-links">
                <a href="#about">About</a>
                <a href="#services">Services</a>
                <a href="#industries">Industries</a>
                <a href="#contact">Contact</a>
                <a class="cta-btn" href="#signup">Free Demo</a>
            </div>
            <button id="menu-toggle" aria-label="Toggle Navigation">☰</button>
        </nav>
    </header>
    <main>
        <section class="hero gradient-bg fade-in" id="hero">
            <div class="hero-content">
                <h1>Transform Your Business with <span class="gradient-text">AI</span></h1>
                <p>Innovative AI solutions designed to help startups and growing businesses compete in the digital age.</p>
                <button onclick="window.location.href='#contact'">Get Started Today</button>
            </div>    
            <div class="animated-illustration">
                <svg viewBox="0 0 500 300" xmlns="http://www.w3.org/2000/svg">
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
                    <line x1="250" y1="150" x2="150" y2="150" stroke="var(--primary)" stroke-width="2" stroke-opacity="0.3"/>
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
                    <h3><i class="fas fa-eye" style="margin-right: 10px;"></i> Computer Vision</h3>
                    <p>Image and video analysis solutions to automate visual inspection and recognition tasks.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Object Detection</span>
                        <span class="ai-chip">Quality Control</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-database" style="margin-right: 10px;"></i> Data Solutions</h3>
                    <p>Turn your raw data into actionable intelligence with our comprehensive data analysis pipelines.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Analytics</span>
                        <span class="ai-chip">Visualization</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-puzzle-piece" style="margin-right: 10px;"></i> AI Integration</h3>
                    <p>Seamless implementation of AI capabilities into your existing systems and workflows.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">APIs</span>
                        <span class="ai-chip">Microservices</span>
                    </div>
                </div>
            </div>
        </section>
        <section id="industries" class="fade-in">
            <h2>Industries We Serve</h2>
            <div class="industries-list">
                <div class="tech-card">
                    <h3><i class="fas fa-shopping-cart" style="margin-right: 10px;"></i> E-commerce</h3>
                    <p>Enhance customer experiences with personalized recommendations and intelligent search.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Recommendations</span>
                        <span class="ai-chip">Visual Search</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-heartbeat" style="margin-right: 10px;"></i> Healthcare</h3>
                    <p>Support medical professionals with diagnostic tools and patient management systems.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Diagnostics</span>
                        <span class="ai-chip">Patient Care</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-chart-line" style="margin-right: 10px;"></i> Finance</h3>
                    <p>Detect fraud, assess risk, and personalize financial services with AI-powered solutions.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Fraud Detection</span>
                        <span class="ai-chip">Risk Assessment</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-industry" style="margin-right: 10px;"></i> Manufacturing</h3>
                    <p>Optimize production lines and quality control with intelligent monitoring systems.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Predictive Maintenance</span>
                        <span class="ai-chip">Quality Control</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-bullseye" style="margin-right: 10px;"></i> Marketing</h3>
                    <p>Create more effective campaigns with AI-driven customer insights and content generation.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">Customer Insights</span>
                        <span class="ai-chip">Content Generation</span>
                    </div>
                </div>
                <div class="tech-card">
                    <h3><i class="fas fa-wifi" style="margin-right: 10px;"></i> Technology</h3>
                    <p>Enhance your tech products with cutting-edge AI capabilities and intelligent features.</p>
                    <div style="margin-top: 1rem;">
                        <span class="ai-chip">SaaS</span>
                        <span class="ai-chip">Developer Tools</span>
                    </div>
                </div>
            </div>
        </section>
        <section id="contact" class="fade-in" style="padding-bottom: 0;">
            <div class="contact-form">
                <h2>Let's Build Something Amazing</h2>
                <p>As a new startup, we're excited to work with innovative partners. Reach out to discuss how we can help bring your AI vision to life.</p>
                <form id="contactForm" action="#" method="POST">
                    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1rem;">
                        <div class="form-group">
                            <label for="name">Name*</label>
                            <input type="text" id="name" name="name" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email*</label>
                            <input type="email" id="email" name="email" required>
                        </div>
                    </div>
                    <div class="form-group">
                        <label for="company">Company</label>
                        <input type="text" id="company" name="company">
                    </div>
                    <div class="form-group">
                        <label for="service">Service of Interest</label>
                        <select id="service" name="service">
                            <option value="">Select a service</option>
                            <option value="consulting">AI Consulting</option>
                            <option value="ml">Machine Learning</option>
                            <option value="nlp">NLP Solutions</option>
                            <option value="vision">Computer Vision</option>
                            <option value="data">Data Solutions</option>
                            <option value="integration">AI Integration</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="message">How can we help you?*</label>
                        <textarea id="message" name="message" rows="5" required></textarea>
                    </div>
                    <button type="submit">Send Message <i class="fas fa-paper-plane" style="margin-left: 8px;"></i></button>
                </form>
            </div>   
            <div style="margin-top: 4rem; text-align: center;">
                <h3>Prefer to email us directly?</h3>
                <p style="font-size: 1.2rem; margin-top: 1rem;">
                    <a href="mailto:hello@stratixai.com" style="color: var(--primary); text-decoration: none; font-weight: 600;">hello@stratixai.com</a>
                </p>
            </div>
        </section>
    </main>
    <footer>
        <div class="footer-content">
            <div class="footer-logo">
                <img src="https://res.cloudinary.com/dhpl09d00/image/upload/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png" alt="Stratix AI Logo">
                <p>Building the future of business AI, one solution at a time.</p>
                <div class="social-links">
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-linkedin"></i></a>
                    <a href="#"><i class="fab fa-github"></i></a>
                </div>
            </div>
            <div class="footer-links">
                <h3>Quick Links</h3>
                <ul>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#industries">Industries</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </div>
            <div class="footer-links">
                <h3>Resources</h3>
                <ul>
                    <li><a href="#">Blog</a></li>
                    <li><a href="#">Documentation</a></li>
                    <li><a href="#">API Reference</a></li>
                    <li><a href="#">Case Studies</a></li>
                </ul>
            </div>
            <div class="footer-links">
                <h3>Legal</h3>
                <ul>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Terms of Service</a></li>
                    <li><a href="#">Cookie Policy</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2024 Stratix AI. All rights reserved.</p>
        </div>
    </footer>
    <button id="back-to-top" aria-label="Back to top">↑</button>
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // Splash screen
            const splash = document.getElementById('splash');
            setTimeout(() => {
                splash.style.opacity = '0';
                setTimeout(() => splash.style.display = 'none', 1000);
            }, 2000);
            // Mobile menu toggle
            const menuToggle = document.getElementById('menu-toggle');
            const navLinks = document.querySelector('.nav-links');
            menuToggle.addEventListener('click', () => {
                navLinks.classList.toggle('show');
                menuToggle.innerHTML = navLinks.classList.contains('show') ? '✕' : '☰';
            });
            // Close mobile menu when clicking a link
            document.querySelectorAll('.nav-links a').forEach(link => {
                link.addEventListener('click', () => {
                    navLinks.classList.remove('show');
                    menuToggle.innerHTML = '☰';
                });
            });
            // Header scroll effect
            const header = document.querySelector('header');
            window.addEventListener('scroll', () => {
                if (window.scrollY > 50) {
                    header.classList.add('scrolled');
                } else {
                    header.classList.remove('scrolled');
                }
            });
            // Back to top button
            const backToTop = document.getElementById('back-to-top');
            window.addEventListener('scroll', () => {
                if (window.scrollY > 300) {
                    backToTop.classList.add('visible');
                } else {
                    backToTop.classList.remove('visible');
                }
            });
            backToTop.addEventListener('click', () => {
                window.scrollTo({
                    top: 0,
                    behavior: 'smooth'
                });
            });
            // Form submission
            const contactForm = document.getElementById('contactForm');
            contactForm.addEventListener('submit', (e) => {
                e.preventDefault();
                // Here you would typically send the form data to your server
                alert('Thank you for your message! We will get back to you soon.');
                contactForm.reset();
            });
            // Animate elements when they come into view
            const fadeEls = document.querySelectorAll('.fade-in');
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.animation = `fadeIn 1s ease forwards`;
                        observer.unobserve(entry.target);
                    }
                });
            }, { threshold: 0.1 });
            fadeEls.forEach(el => observer.observe(el));
            // Tech card hover effects
            document.querySelectorAll('.tech-card').forEach(card => {
                card.addEventListener('mousemove', (e) => {
                    const x = e.pageX - card.offsetLeft;
                    const y = e.pageY - card.offsetTop;  
                    card.style.setProperty('--mouse-x', `${x}px`);
                    card.style.setProperty('--mouse-y', `${y}px`);
                });
            });
        });
    </script>
</body>
</html>
