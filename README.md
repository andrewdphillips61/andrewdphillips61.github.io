<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Stratix Automation - Practical AI solutions for growing businesses">
    <title>Stratix Automation | AI Tools for SMBs</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
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
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background-color: rgba(255, 255, 255, 0.95);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            z-index: 100;
            transition: all 0.3s ease;
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
            height: 50px;
            width: auto;
            max-width: 180px;
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
        }
        .cta-btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
        }
        #menu-toggle {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--dark);
        }
        main {
            padding-top: 80px;
            max-width: 1400px;
            margin: 0 auto;
        }
        section {
            padding: 5rem 2rem;
            scroll-margin-top: 80px;
        }
        section:nth-child(even) {
            background-color: #f1f5f9;
        }
        h1, h2, h3 {
            line-height: 1.2;
            margin-bottom: 1.5rem;
        }
        h1 {
            font-size: 2.8rem;
            font-weight: 700;
        }
        h2 {
            font-size: 2.2rem;
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
        }
        h2:after {
            content: '';
            position: absolute;
            width: 80px;
            height: 4px;
            background-color: var(--primary);
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }
        h3 {
            font-size: 1.3rem;
            color: var(--primary);
        }
        p {
            margin-bottom: 1rem;
            color: var(--gray);
        }
        .hero {
            min-height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: linear-gradient(135deg, rgba(37, 99, 235, 0.1) 0%, rgba(255, 255, 255, 1) 100%);
        }
        .hero p {
            font-size: 1.3rem;
            max-width: 700px;
            margin-bottom: 2rem;
        }
        .hero button {
            background-color: var(--primary);
            color: white;
            border: none;
            padding: 1rem 2rem;
            font-size: 1.1rem;
            border-radius: 6px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        .hero button:hover {
            background-color: var(--primary-dark);
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(37, 99, 235, 0.2);
        }
        .services-list, .industries-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        .services-list li, .industries-list li {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            list-style: none;
        }
        .services-list li:hover, .industries-list li:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
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
        label {
            font-weight: 500;
            color: var(--dark);
        }
        input, textarea {
            padding: 0.8rem 1rem;
            border: 1px solid #ddd;
            border-radius: 6px;
            font-family: inherit;
            font-size: 1rem;
            transition: border-color 0.3s ease;
        }
        input:focus, textarea:focus {
            outline: none;
            border-color: var(--primary);
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
            border-radius: 6px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        form button:hover {
            background-color: var(--primary-dark);
        }
        footer {
            text-align: center;
            padding: 2rem;
            background-color: var(--dark);
            color: white;
        }
        footer p {
            color: white;
        }
        .fade-in {
            opacity: 0;
            animation: fadeIn 1s ease forwards;
        }
        @keyframes fadeIn {
            to { opacity: 1; }
        }
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 1rem;
            margin-top: 2rem;
            text-align: center;
        }
        .stats-grid h3 {
            font-size: 2rem;
            color: var(--primary);
        }
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
        }
        #back-to-top.visible {
            opacity: 1;
            visibility: visible;
        }
        #back-to-top:hover {
            background-color: var(--primary-dark);
            transform: translateY(-5px);
        }
        @media (max-width: 768px) {
            h1 {
                font-size: 2.2rem;
            }
            h2 {
                font-size: 1.8rem;
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
                padding: 3rem 1.5rem;
            }
            .hero {
                min-height: 70vh;
                padding: 0 1.5rem;
            }
            .services-list, .industries-list {
                grid-template-columns: 1fr;
            }
            .logo img {
                height: 40px;
            }
            .stats-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Splash Screen -->
    <div id="splash">
        <img src="https://res.cloudinary.com/dhpl09d00/image/upload/f_auto,q_auto,w_300/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png" 
             alt="Stratix Automation Logo">
    </div>
    <header>
        <nav>
            <div class="logo">
                <img src="https://res.cloudinary.com/dhpl09d00/image/upload/f_auto,q_auto,w_200/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png" 
                     alt="Stratix Automation">
            </div>
            <div class="nav-links">
                <a href="#about">About</a>
                <a href="#services">Solutions</a>
                <a href="#industries">Industries</a>
                <a href="#contact">Contact</a>
                <a class="cta-btn" href="#contact">Early Access</a>
            </div>
            <button id="menu-toggle" aria-label="Toggle Navigation">☰</button>
        </nav>
    </header>
    <main>
        <section class="hero fade-in" id="hero">
            <h1>Practical AI for Growing Businesses</h1>
            <p>We're building affordable automation tools to help businesses work smarter, not harder.</p>
            <button onclick="window.location.href='#contact'">Join Our Beta</button>
        </section>
        <section id="about" class="fade-in">
            <h2>Our Startup Story</h2>
            <div class="about-content">
                <p>Founded in 2025, Stratix Automation is bootstrapping its way to create genuinely useful AI tools.</p>
                <p>We're not another AI hype company - we're focused on delivering real value through simple, effective solutions.</p>
                <div class="stats-grid">
                    <div>
                        <h3>5+</h3>
                        <p>Pilot Clients</p>
                    </div>
                    <div>
                        <h3>3</h3>
                        <p>Core Features</p>
                    </div>
                    <div>
                        <h3>100%</h3>
                        <p>Founder-Led</p>
                    </div>
                </div>
            </div>
        </section>
        <section id="services" class="fade-in">
            <h2>Our Current Focus</h2>
            <div class="services-list">
                <div>
                    <h3><i class="fas fa-robot" style="margin-right: 10px;"></i> Smart CRM Assistant</h3>
                    <p>Basic AI tools to help manage customer relationships more effectively. Currently in beta testing with select clients.</p>
                </div>
                <div>
                    <h3><i class="fas fa-comment-dots" style="margin-right: 10px;"></i> Chat Automation</h3>
                    <p>Advanced chatbot solutions for instantly handling common customer inquiries. </p>
                </div>
                <div>
                    <h3><i class="fas fa-chart-line" style="margin-right: 10px;"></i> Data Reports</h3>
                    <p>Automated business insights from your existing data. Currently supports basic spreadsheet analysis.</p>
                </div>
            </div>
        </section>
        <section id="industries" class="fade-in">
            <h2>Who We're Building For</h2>
            <div class="industries-list">
                <div>
                    <h3><i class="fas fa-store" style="margin-right: 10px;"></i> Small Retail</h3>
                    <p>Tools to help local real estate companies manage customer interactions.</p>
                </div>
                <div>
                    <h3><i class="fas fa-briefcase" style="margin-right: 10px;"></i> Professional Services</h3>
                    <p>Basic automation for consultants, lawyers, and accountants.</p>
                </div>
                <div>
                    <h3><i class="fas fa-utensils" style="margin-right: 10px;"></i> Restaurants</h3>
                    <p>Simple solutions for reservations and customer feedback.</p>
                </div>
            </div>
        </section>
        <section id="contact" class="fade-in">
            <h2>Work With Us</h2>
            <div class="contact-form">
                <p>We're currently onboarding a limited number of beta testers. Let's chat about how we might help your business.</p>
                <form id="contactForm" action="#" method="POST">
                    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1rem;">
                        <div>
                            <label for="name">Name*</label>
                            <input type="text" id="name" name="name" required>
                        </div>
                        <div>
                            <label for="email">Email*</label>
                            <input type="email" id="email" name="email" required>
                        </div>
                    </div>
                    <div>
                        <label for="company">Business Name</label>
                        <input type="text" id="company" name="company">
                    </div>
                    <div>
                        <label for="service">Interest Area</label>
                        <select id="service" name="service">
                            <option value="">Select an option</option>
                            <option value="crm">CRM Assistant</option>
                            <option value="chat">Chat Automation</option>
                            <option value="data">Data Reports</option>
                            <option value="other">Just Exploring</option>
                        </select>
                    </div>
                    <div>
                        <label for="message">What challenges are you facing?*</label>
                        <textarea id="message" name="message" rows="5" required></textarea>
                    </div>
                    <button type="submit">Send Message <i class="fas fa-paper-plane" style="margin-left: 8px;"></i></button>
                </form>
            </div>
        </section>
    </main>
    <footer>
        <div style="max-width: 1200px; margin: 0 auto; display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 2rem; text-align: left; padding-bottom: 2rem;">
            <div>
                <img src="https://res.cloudinary.com/dhpl09d00/image/upload/f_auto,q_auto,w_200,e_colorize:100,co_white/v1744120867/Screenshot_2025-04-07_at_9.52.00_PM_vpj01g.png" 
                     alt="Stratix Automation Logo" 
                     style="height: 40px; margin-bottom: 1rem;">
                <p>Building practical AI tools for real businesses.</p>
            </div>
            <div>
                <h3 style="color: white; margin-bottom: 1rem;">Quick Links</h3>
                <ul style="list-style: none;">
                    <li style="margin-bottom: 0.5rem;"><a href="#about" style="color: white; text-decoration: none;">Our Story</a></li>
                    <li style="margin-bottom: 0.5rem;"><a href="#services" style="color: white; text-decoration: none;">Solutions</a></li>
                    <li style="margin-bottom: 0.5rem;"><a href="#industries" style="color: white; text-decoration: none;">Industries</a></li>
                    <li style="margin-bottom: 0.5rem;"><a href="#contact" style="color: white; text-decoration: none;">Beta Program</a></li>
                </ul>
            </div>
            <div>
                <h3 style="color: white; margin-bottom: 1rem;">Contact</h3>
                <p><i class="fas fa-user" style="margin-right: 10px;"></i> Andrew Phillips, Founder</p>
                <p><i class="fas fa-phone" style="margin-right: 10px;"></i> <a href="tel:6159559515" style="color: white; text-decoration: none;">(615) 955-9515</a></p>
                <p><i class="fas fa-envelope" style="margin-right: 10px;"></i> <a href="mailto:stratixautomation@gmail.com" style="color: white; text-decoration: none;">stratixautomation@gmail.com</a></p>
            </div>
        </div>
        <div style="border-top: 1px solid rgba(255, 255, 255, 0.1); padding-top: 1.5rem;">
            <p>&copy; 2025 Stratix Automation. A bootstrapped startup.</p>
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
                alert('Thanks for your interest! We\'ll be in touch soon about our beta program.');
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
        });
    </script>
</body>
</html>
