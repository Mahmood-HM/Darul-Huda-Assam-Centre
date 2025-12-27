<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Darul Huda Assam Centre</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Reset and Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --dark: #1a252f;
            --light: #f8f9fa;
            --gray: #6c757d;
        }

        body {
            line-height: 1.6;
            color: #333;
            background-color: #f5f7fa;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        /* Header Styles - UPDATED TO WHITISH COLOR */
        header {
            background-color: rgba(255, 255, 255, 0.95); /* Changed to white-ish semi-transparent */
            color: var(--primary); /* Changed text color to dark for contrast */
            padding: 1rem 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            transition: background-color 0.3s ease;
        }

        header.scrolled {
            background-color: rgba(255, 255, 255, 0.98); /* Slightly more opaque when scrolled */
            backdrop-filter: blur(10px);
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-icon {
            position: relative;
            width: 50px;
            height: 50px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        /* Updated logo to use the provided image */
        .logo-icon img {
            width: 100%;
            height: auto;
            object-fit: contain;
        }

        /* Removed the bird logo CSS since we're using an image */
        .logo-text h1 {
            font-size: 1.6rem;
            background: linear-gradient(45deg, var(--secondary), var(--accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .logo-text p {
            font-size: 0.75rem;
            color: var(--gray); /* Changed to gray for better contrast on white */
            margin-top: 2px;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 1.5rem;
        }

        nav a {
            color: var(--primary); /* Changed to dark color for white background */
            text-decoration: none;
            font-weight: 600;
            padding: 0.5rem 0;
            transition: color 0.3s;
            position: relative;
        }

        nav a:hover {
            color: var(--accent);
        }

        nav a.active {
            color: var(--accent);
        }

        nav a.active::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 3px;
            background-color: var(--accent);
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: var(--primary); /* Changed to dark color for white background */
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Hero Section - UPDATED: Changed background image */
        .hero {
            position: relative;
            background: 
                /* Transparent overlay with slight darkening */
                linear-gradient(rgba(44, 62, 80, 0.7), rgba(44, 62, 80, 0.8)),
                /* Updated school background image */
                url('https://dhiu.in/source/Files/images/DH%20Assam%201.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed; /* Creates parallax effect */
            color: white;
            padding: 10rem 0 5rem;
            text-align: center;
            margin-top: 0;
        }

        /* Removing the old hero::before background since we're using direct background image */
        .hero::before {
            content: none;
        }

        .hero-content {
            position: relative;
            z-index: 2;
        }

        .hero h2 {
            font-size: 2.8rem;
            margin-bottom: 1.5rem;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2.5rem;
            opacity: 0.95;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
        }

        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: white;
            padding: 0.9rem 2rem;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }

        .btn:hover {
            background-color: #c0392b;
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.25);
        }

        .btn-primary {
            background-color: var(--secondary);
        }

        .btn-primary:hover {
            background-color: #2980b9;
        }

        /* Sections */
        section {
            padding: 4rem 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            color: var(--dark);
        }

        .section-title h2 {
            font-size: 2.2rem;
            position: relative;
            display: inline-block;
            padding-bottom: 10px;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background-color: var(--secondary);
        }

        /* Features */
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .feature-card {
            background-color: white;
            border-radius: 10px;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: all 0.3s;
            border-top: 4px solid var(--secondary);
            position: relative;
            overflow: hidden;
        }

        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }

        .feature-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .feature-card h3 {
            margin-bottom: 1rem;
            color: var(--dark);
        }

        /* Content with Read More functionality */
        .content-preview {
            max-height: 200px;
            overflow: hidden;
            position: relative;
            transition: max-height 0.5s ease;
        }

        .content-preview.expanded {
            max-height: 2000px;
        }

        .content-preview::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 60px;
            background: linear-gradient(to bottom, transparent, white);
            transition: opacity 0.3s ease;
            pointer-events: none;
        }

        .content-preview.expanded::after {
            opacity: 0;
        }

        .read-more-btn {
            display: inline-block;
            margin-top: 1rem;
            color: var(--secondary);
            background: none;
            border: none;
            font-weight: 600;
            cursor: pointer;
            padding: 0.5rem 1rem;
            border-radius: 4px;
            transition: all 0.3s;
        }

        .read-more-btn:hover {
            background-color: rgba(52, 152, 219, 0.1);
        }

        .read-more-btn i {
            margin-left: 5px;
            transition: transform 0.3s;
        }

        .read-more-btn.expanded i {
            transform: rotate(180deg);
        }

        /* Highlight sections within content */
        .content-section {
            margin-bottom: 1.5rem;
        }

        .content-section h4 {
            color: var(--primary);
            margin-bottom: 0.5rem;
            font-size: 1.1rem;
        }

        /* News Section */
        .news-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .news-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
        }

        .news-card:hover {
            transform: translateY(-5px);
        }

        .news-img {
            height: 200px;
            background-color: var(--gray);
            background-size: cover;
            background-position: center;
            transition: transform 0.5s;
        }

        .news-card:hover .news-img {
            transform: scale(1.05);
        }

        .news-content {
            padding: 1.5rem;
        }

        .news-date {
            color: var(--accent);
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
        }

        .news-card h3 {
            margin-bottom: 0.8rem;
            color: var(--dark);
        }

        /* NEW: Students Section Styles */
        .students-stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-bottom: 3rem;
        }

        .class-card {
            background: white;
            border-radius: 10px;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            border-left: 4px solid var(--secondary);
            transition: transform 0.3s;
        }

        .class-card:hover {
            transform: translateY(-5px);
        }

        .class-card h3 {
            color: var(--primary);
            margin-bottom: 1rem;
            font-size: 1.2rem;
        }

        .student-count {
            font-size: 2.5rem;
            font-weight: bold;
            color: var(--secondary);
            margin-bottom: 0.5rem;
        }

        .total-students {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .total-students h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .total-count {
            font-size: 3.5rem;
            font-weight: bold;
            margin-bottom: 0.5rem;
        }

        /* NEW: Staff Section Styles */
        .staff-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .staff-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: all 0.3s;
        }

        .staff-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }

        .staff-img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            transition: transform 0.5s;
        }

        .staff-card:hover .staff-img {
            transform: scale(1.05);
        }

        .staff-info {
            padding: 1.5rem;
        }

        .staff-name {
            color: var(--primary);
            margin-bottom: 0.5rem;
            font-size: 1.3rem;
        }

        .staff-position {
            color: var(--secondary);
            font-weight: 600;
            margin-bottom: 1rem;
        }

        .staff-degree {
            color: var(--gray);
            font-size: 0.9rem;
            margin-bottom: 1rem;
            line-height: 1.4;
        }

        .staff-contact {
            margin-top: 1rem;
            padding-top: 1rem;
            border-top: 1px solid #eee;
        }

        .staff-contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 0.5rem;
            font-size: 0.9rem;
        }

        .staff-contact-item i {
            color: var(--secondary);
            width: 20px;
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 3rem 0 1rem;
        }

        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-logo h2 {
            color: white;
            margin-bottom: 1rem;
            font-size: 1.8rem;
        }

        .footer-logo span {
            color: var(--accent);
        }

        .footer-links h3, .footer-contact h3 {
            color: var(--accent);
            margin-bottom: 1.5rem;
            font-size: 1.2rem;
        }

        .footer-links ul {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 0.8rem;
        }

        .footer-links a {
            color: #ddd;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-links a:hover {
            color: var(--accent);
        }

        .footer-contact p {
            margin-bottom: 0.8rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .footer-contact i {
            color: var(--secondary);
            width: 20px;
        }

        .social-icons {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
        }

        .social-icons a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            text-decoration: none;
            transition: all 0.3s;
        }

        .social-icons a:hover {
            background-color: var(--accent);
            transform: translateY(-3px);
        }

        .copyright {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #aaa;
            font-size: 0.9rem;
        }

        /* Page Content */
        .page-content {
            min-height: 60vh;
            padding: 3rem 0;
        }

        /* About Page */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .about-img {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .about-img img {
            width: 100%;
            height: auto;
            display: block;
            transition: transform 0.5s;
        }

        .about-img:hover img {
            transform: scale(1.05);
        }

        .about-text h2 {
            color: var(--dark);
            margin-bottom: 1.5rem;
        }

        .about-text p {
            margin-bottom: 1.5rem;
        }

        /* Academics Page */
        .academics-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .academic-department {
            background-color: white;
            border-radius: 10px;
            padding: 2rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            border-left: 4px solid var(--secondary);
        }

        .academic-department h3 {
            color: var(--primary);
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        /* Contact Page - UPDATED WITH WORKING FORM */
        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
        }

        .contact-info {
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }

        .contact-form {
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
        }

        .form-control {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
            transition: border-color 0.3s;
        }

        .form-control:focus {
            outline: none;
            border-color: var(--secondary);
        }

        textarea.form-control {
            min-height: 150px;
            resize: vertical;
        }

        /* Form submission success message */
        .form-success {
            display: none;
            text-align: center;
            padding: 2rem;
            background-color: #d4edda;
            color: #155724;
            border-radius: 5px;
            margin-top: 1rem;
            border: 1px solid #c3e6cb;
        }

        .form-success i {
            font-size: 3rem;
            margin-bottom: 1rem;
            color: #28a745;
        }

        /* Responsive Styles */
        @media (max-width: 992px) {
            .about-content, .contact-container {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                align-items: flex-start;
            }

            .mobile-menu-btn {
                display: block;
                position: absolute;
                top: 1rem;
                right: 1rem;
            }

            nav {
                width: 100%;
                display: none;
                margin-top: 1rem;
            }

            nav.active {
                display: block;
            }

            nav ul {
                flex-direction: column;
                gap: 0;
            }

            nav li {
                width: 100%;
                border-bottom: 1px solid rgba(0, 0, 0, 0.1); /* Lighter border for white header */
            }

            nav a {
                display: block;
                padding: 1rem 0;
                color: var(--primary); /* Ensure dark color in mobile menu */
            }

            .hero {
                padding: 8rem 0 4rem;
                background-attachment: scroll;
            }

            .hero h2 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .students-stats {
                grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            }

            .student-count {
                font-size: 2rem;
            }

            .total-count {
                font-size: 2.5rem;
            }

            .staff-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header - Updated to whitish color -->
    <header id="mainHeader">
        <div class="container header-container">
            <div class="logo">
                <div class="logo-icon">
                    <!-- Updated logo to use the provided image -->
                    <img src="https://dhassam.in/img/logo.png" alt="Darul Huda Assam Centre Logo">
                </div>
                <div class="logo-text">
                    <!-- Updated school name -->
                    <h1>Darul Huda Assam Centre</h1>
                    <p>Soaring to Excellence Since 1990</p>
                </div>
            </div>
            
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            
            <nav id="mainNav">
                <ul>
                    <li><a href="#" class="active" data-page="home">Home</a></li>
                    <li><a href="#" data-page="about">About</a></li>
                    <li><a href="#" data-page="academics">Academics</a></li>
                    <!-- UPDATED NAVIGATION: Added Students and Staff -->
                    <li><a href="#" data-page="students">Students</a></li>
                    <li><a href="#" data-page="staff">Staff</a></li>
                    <li><a href="#" data-page="admissions">Admissions</a></li>
                    <li><a href="#" data-page="contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Main Content -->
    <main id="mainContent">
        <!-- Home Page Content -->
        <section id="homePage" class="page">
            <!-- Hero Section - Now transparent with school picture behind -->
            <div class="hero">
                <div class="container hero-content">
                    <!-- Updated hero heading to reflect new school name -->
                    <h2>Where Minds Take Flight</h2>
                    <p>At Darul Huda Assam Centre, we nurture curious minds and inspire lifelong learners. Our innovative approach to education prepares students not just for exams, but for life's challenges and opportunities.</p>
                    <!-- UPDATED: Changed to open Google Form link -->
                    <a href="https://forms.gle/gTjnW1gFAxHwbHnm8" target="_blank" class="btn">Begin Your Journey</a>
                    <a href="https://share.google/JGTO92OMcTmP2Srts" target="_blank" class="btn btn-primary" style="margin-left: 15px;">Discover More</a>
                </div>
            </div>

            <!-- Features Section -->
            <section class="container">
                <div class="section-title">
                    <h2>Why Darul Huda Assam Centre?</h2>
                </div>
                <div class="features">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-feather-alt"></i>
                        </div>
                        <h3>Innovative Learning</h3>
                        <p>Our project-based curriculum encourages creativity, critical thinking, and collaboration - skills for the 21st century.</p>
                    </div>
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-users"></i>
                        </div>
                        <h3>Nurturing Community</h3>
                        <p>Small class sizes and dedicated mentors ensure every student receives personalized attention and support.</p>
                    </div>
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-globe-americas"></i>
                        </div>
                        <h3>Global Perspective</h3>
                        <p>International exchange programs and diverse curriculum prepare students to be global citizens.</p>
                    </div>
                </div>
            </section>

            <!-- News Section -->
            <section style="background-color: #f0f7ff;">
                <div class="container">
                    <div class="section-title">
                        <h2>Latest News & Events</h2>
                    </div>
                    <div class="news-container">
                        <div class="news-card">
                            <div class="news-img" style="background-image: url('https://images.unsplash.com/photo-1546410531-bb4caa6b424d?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80');"></div>
                            <div class="news-content">
                                <div class="news-date">June 10, 2023</div>
                                <h3>Innovation Fair Winners</h3>
                                <p>Our students won three awards at the Regional Innovation Fair with projects on renewable energy and AI applications.</p>
                            </div>
                        </div>
                        <div class="news-card">
                            <div class="news-img" style="background-image: url('https://images.unsplash.com/photo-1543269865-cbf427effbad?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80');"></div>
                            <div class="news-content">
                                <div class="news-date">May 25, 2023</div>
                                <h3>New Arts Wing Opening</h3>
                                <p>State-of-the-art facilities for visual and performing arts to be inaugurated next month. Open house scheduled.</p>
                            </div>
                        </div>
                        <div class="news-card">
                            <div class="news-img" style="background-image: url('https://images.unsplash.com/photo-1511632765486-a01980e01a18?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80');"></div>
                            <div class="news-content">
                                <div class="news-date">May 5, 2023</div>
                                <h3>Darul Huda Assam Centre Robotics Team Advances</h3>
                                <p>Our robotics team qualified for the national championships after winning the regional tournament.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </section>

        <!-- About Page Content -->
        <section id="aboutPage" class="page" style="display: none;">
            <div class="container page-content">
                <div class="section-title">
                    <!-- Updated title -->
                    <h2>About Darul Huda Assam Centre</h2>
                </div>
                <div class="about-content">
                    <div class="about-img">
                        <img src="https://images.unsplash.com/photo-1562774053-701939374585?ixlib=rb-4.0.3&auto=format&fit=crop&w=1064&q=80" alt="Darul Huda Assam Centre Campus">
                    </div>
                    <div class="about-text">
                        <!-- Updated heading -->
                        <h2>Our Story</h2>
                        <p>Founded in 1990, Darul Huda Assam Centre began with a simple but powerful vision: to create an educational environment where students could truly take flight in their learning journey. Named after the skylark bird, known for its joyful flight and beautiful song, our centre embodies the spirit of reaching new heights while staying grounded in values.</p>
                        <p>What started as a small progressive school with 150 students has grown into a respected institution serving over 1,800 students from preschool through high school, all while maintaining our commitment to personalized education.</p>
                        <p>We believe education should be an adventure of discovery. Our approach combines academic rigor with creative exploration, encouraging students to find their unique passions and strengths.</p>
                        <a href="#" class="btn btn-primary" data-page="contact">Schedule a Visit</a>
                    </div>
                </div>
                
                <div style="margin-top: 4rem;">
                    <div class="section-title">
                        <h2>Our Mission & Values</h2>
                    </div>
                    <div class="features">
                        <div class="feature-card">
                            <div class="feature-icon">
                                <i class="fas fa-bullseye"></i>
                            </div>
                            <h3>Our Mission</h3>
                            <div class="content-preview" id="missionPreview">
                                <p><strong>Our mission can be viewed from four dimensions:</strong></p>
                                
                                <div class="content-section">
                                    <h4>Dynamic and Dutiful</h4>
                                    <p>To develop an Islamic educational framework in order to prepare religious scientists ('Ulama) who acquire, practice and propagate Islam, being alert of their ultimate responsibilities towards Almighty Allah and towards themselves, family, institution, society, surroundings and private and public resources and to make them capable of competing the shifting trends of modern education.</p>
                                </div>
                                
                                <div class="content-section">
                                    <h4>Holistic and Harmonious</h4>
                                    <p>To offer a holistic and comprehensive material education, harmonious with the Islamic principles in order to foster the personal, spiritual and intellectual developments of the students.</p>
                                </div>
                                
                                <div class="content-section">
                                    <h4>Integrated</h4>
                                    <p>To incorporate the Islamic doctrinal beliefs and value into the educational practices, so as to integrate educational theories with practices, and extend the class room activities with real-life situations and societal experiences.</p>
                                </div>
                                
                                <div class="content-section">
                                    <h4>Unified</h4>
                                    <p>To unify the purpose of seeking knowledge of various contents and nature in line with the Islamic legacy of hierarchy and unity of knowledge as proclaimed in the holy Quran and the tradition of holy prophet (pbuh).</p>
                                </div>
                                
                                <div class="content-section">
                                    <h4>Excellence and Innovative</h4>
                                    <p>To provide academic excellence of highest standards to develop new trends and ideas to keep with the modernization of knowledge.</p>
                                </div>
                                
                                <div class="content-section">
                                    <h4>Productive and Self Reliant</h4>
                                    <p>To offer the students evidence-based academic tools of wisdom to produce better material to build up the confidence of self reliant by which they can meet the academic challenges and find happiness through achievements.</p>
                                </div>
                            </div>
                            <button class="read-more-btn" id="missionBtn">
                                Read More <i class="fas fa-chevron-down"></i>
                            </button>
                        </div>
                        <div class="feature-card">
                            <div class="feature-icon">
                                <i class="fas fa-heart"></i>
                            </div>
                            <h3>Our Values</h3>
                            <p>Curiosity, Integrity, Compassion, Resilience, and Innovation - these values guide every aspect of life at Darul Huda Assam Centre.</p>
                        </div>
                        <div class="feature-card">
                            <div class="feature-icon">
                                <i class="fas fa-chart-line"></i>
                            </div>
                            <h3>Our Vision</h3>
                            <div class="content-preview" id="visionPreview">
                                <p>DHIU aims to be the bastion of expertise in Islamic education restoring the dynamic role and educational superiority of past Muslim society in all intellectual programs and that seeks to rekindle the spirit of scholarship in Islamic sciences in the era of ever-changing society due to the innovative growth of modern sciences.</p>
                                
                                <div class="content-section">
                                    <p>Its vision also includes Islamization of the knowledge and setting up of international research centers of educational excellence in various Islamic disciplines for the development of Muslim community in learning, teaching and research of highest standards and keeping intellectual tradition alive.</p>
                                </div>
                                
                                <div class="content-section">
                                    <p>It also aims to be an exemplary institution which can mould up a bunch of such religious scientists (Ulamas) who are the virtual heirs of the holy prophet Muhammed (pbuh).</p>
                                </div>
                            </div>
                            <button class="read-more-btn" id="visionBtn">
                                Read More <i class="fas fa-chevron-down"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Academics Page Content -->
        <section id="academicsPage" class="page" style="display: none;">
            <div class="container page-content">
                <div class="section-title">
                    <!-- Updated title -->
                    <h2>Academics at Darul Huda Assam Centre</h2>
                </div>
                <p style="text-align: center; max-width: 800px; margin: 0 auto 3rem; font-size: 1.1rem;">Our curriculum is designed to challenge minds, inspire creativity, and develop critical thinking skills. We offer a balanced education that prepares students for both academic success and personal fulfillment.</p>
                
                <div class="academics-grid">
                    <div class="academic-department">
                        <h3><i class="fas fa-rocket"></i> STEM Program</h3>
                        <p>Our Science, Technology, Engineering, and Mathematics program emphasizes hands-on experimentation, coding, robotics, and real-world problem-solving.</p>
                        <ul style="margin-top: 1rem; padding-left: 1.5rem;">
                            <li>Advanced Laboratory Facilities</li>
                            <li>Robotics & Coding Clubs</li>
                            <li>Science Research Opportunities</li>
                            <li>Math Olympiad Preparation</li>
                        </ul>
                    </div>
                    <div class="academic-department">
                        <h3><i class="fas fa-paint-brush"></i> Creative Arts</h3>
                        <p>Nurturing creative expression through comprehensive programs in visual arts, music, theater, dance, and digital media.</p>
                        <ul style="margin-top: 1rem; padding-left: 1.5rem;">
                            <li>Studio Arts & Ceramics</li>
                            <li>Digital Media & Film Production</li>
                            <li>Theater & Performance Arts</li>
                            <li>Music Ensembles & Choir</li>
                        </ul>
                    </div>
                    <div class="academic-department">
                        <h3><i class="fas fa-globe"></i> Global Studies</h3>
                        <p>Developing global citizenship through language acquisition, cultural studies, and international exchange programs.</p>
                        <ul style="margin-top: 1rem; padding-left: 1.5rem;">
                            <li>Spanish, French & Mandarin Programs</li>
                            <li>International Student Exchange</li>
                            <li>Model United Nations</li>
                            <li>Global Issues & Cultural Studies</li>
                        </ul>
                    </div>
                    <div class="academic-department">
                        <h3><i class="fas fa-leaf"></i> Wellness & Sustainability</h3>
                        <p>Promoting physical health, environmental stewardship, and emotional well-being through comprehensive programs.</p>
                        <ul style="margin-top: 1rem; padding-left: 1.5rem;">
                            <li>Outdoor Education & Ecology</li>
                            <li>Mindfulness & Wellness Programs</li>
                            <li>Competitive & Recreational Sports</li>
                            <li>Sustainability Initiatives</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- NEW: Students Page Content -->
        <section id="studentsPage" class="page" style="display: none;">
            <div class="container page-content">
                <div class="section-title">
                    <h2>Our Student Community</h2>
                </div>
                
                <p style="text-align: center; max-width: 800px; margin: 0 auto 3rem; font-size: 1.1rem;">
                    Darul Huda Assam Centre is home to a diverse and vibrant student community. We take pride in our growing family of learners who come from various backgrounds to pursue excellence in Islamic and modern education.
                </p>
                
                <div class="students-stats">
                    <!-- Class-wise Student Counts -->
                    <div class="class-card">
                        <h3>Preparatory Year</h3>
                        <div class="student-count">85</div>
                        <p>Students in foundation program</p>
                    </div>
                    
                    <div class="class-card">
                        <h3>First Year</h3>
                        <div class="student-count">92</div>
                        <p>Students in primary studies</p>
                    </div>
                    
                    <div class="class-card">
                        <h3>Second Year</h3>
                        <div class="student-count">78</div>
                        <p>Students in intermediate studies</p>
                    </div>
                    
                    <div class="class-card">
                        <h3>Third Year</h3>
                        <div class="student-count">65</div>
                        <p>Students in advanced studies</p>
                    </div>
                    
                    <div class="class-card">
                        <h3>Fourth Year</h3>
                        <div class="student-count">58</div>
                        <p>Students in specialized studies</p>
                    </div>
                    
                    <div class="class-card">
                        <h3>Fifth Year</h3>
                        <div class="student-count">45</div>
                        <p>Students in final year</p>
                    </div>
                </div>
                
                <!-- Total Students -->
                <div class="total-students">
                    <h3>Total Student Strength</h3>
                    <div class="total-count">423</div>
                    <p>Bright minds shaping their future at Darul Huda Assam Centre</p>
                    <p style="margin-top: 1rem; font-size: 0.9rem; opacity: 0.9;">
                        <i class="fas fa-info-circle"></i> Updated: December 2023 | Student-Teacher Ratio: 12:1
                    </p>
                </div>
                
                <!-- Additional Information -->
                <div style="margin-top: 4rem;">
                    <div class="section-title">
                        <h2>Student Life & Activities</h2>
                    </div>
                    <div class="features">
                        <div class="feature-card">
                            <div class="feature-icon">
                                <i class="fas fa-users"></i>
                            </div>
                            <h3>Student Organizations</h3>
                            <p>15+ active student clubs and organizations including Islamic Study Circle, Debate Club, Community Service Group, and Sports Committee.</p>
                        </div>
                        <div class="feature-card">
                            <div class="feature-icon">
                                <i class="fas fa-trophy"></i>
                            </div>
                            <h3>Achievements</h3>
                            <p>Our students have won 25+ awards in regional and national competitions in academics, sports, and cultural events in the past year.</p>
                        </div>
                        <div class="feature-card">
                            <div class="feature-icon">
                                <i class="fas fa-hands-helping"></i>
                            </div>
                            <h3>Community Outreach</h3>
                            <p>Students participate in regular community service projects, benefiting over 500 families annually through various outreach programs.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- NEW: Staff Page Content -->
        <section id="staffPage" class="page" style="display: none;">
            <div class="container page-content">
                <div class="section-title">
                    <h2>Our Dedicated Staff</h2>
                </div>
                
                <p style="text-align: center; max-width: 800px; margin: 0 auto 3rem; font-size: 1.1rem;">
                    Meet our team of experienced educators and administrative staff who are committed to providing quality Islamic and modern education. Our faculty members bring diverse expertise and passion to create a nurturing learning environment.
                </p>
                
                <div class="staff-grid">
                    <!-- Staff Member 1 -->
                    <div class="staff-card">
                        <img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Dr. Ahmed Khan" class="staff-img">
                        <div class="staff-info">
                            <h3 class="staff-name">Dr. Ahmed Khan</h3>
                            <p class="staff-position">Principal & Director</p>
                            <p class="staff-degree">PhD in Islamic Studies (Al-Azhar University), MA in Education (University of Cambridge)</p>
                            <p>With over 25 years of experience in Islamic education, Dr. Khan leads our institution with vision and dedication.</p>
                            <div class="staff-contact">
                                <div class="staff-contact-item">
                                    <i class="fas fa-envelope"></i>
                                    <span>ahmed.khan@darulhudaassam.edu</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-phone"></i>
                                    <span>+91 98765 43210</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-clock"></i>
                                    <span>Office Hours: Mon-Fri, 9 AM - 4 PM</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Staff Member 2 -->
                    <div class="staff-card">
                        <img src="https://images.unsplash.com/photo-1582750433449-648ed127bb54?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Prof. Fatima Ahmed" class="staff-img">
                        <div class="staff-info">
                            <h3 class="staff-name">Prof. Fatima Ahmed</h3>
                            <p class="staff-position">Head of Islamic Studies</p>
                            <p class="staff-degree">MA in Islamic Law (Darul Uloom Deoband), BA in Arabic Literature (Jamia Millia Islamia)</p>
                            <p>Specializes in Quranic Studies and Islamic Jurisprudence with 15+ years of teaching experience.</p>
                            <div class="staff-contact">
                                <div class="staff-contact-item">
                                    <i class="fas fa-envelope"></i>
                                    <span>fatima.ahmed@darulhudaassam.edu</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-phone"></i>
                                    <span>+91 98765 43211</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-book"></i>
                                    <span>Subjects: Quran, Hadith, Fiqh</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Staff Member 3 -->
                    <div class="staff-card">
                        <img src="https://images.unsplash.com/photo-1544725176-7c40e5a71c5e?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Mr. Rahimuddin Shah" class="staff-img">
                        <div class="staff-info">
                            <h3 class="staff-name">Mr. Rahimuddin Shah</h3>
                            <p class="staff-position">Head of Modern Sciences</p>
                            <p class="staff-degree">MSc in Physics (University of Delhi), BEd (Aligarh Muslim University)</p>
                            <p>Expert in integrating modern scientific knowledge with Islamic principles. 12 years of teaching experience.</p>
                            <div class="staff-contact">
                                <div class="staff-contact-item">
                                    <i class="fas fa-envelope"></i>
                                    <span>rahim.shah@darulhudaassam.edu</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-phone"></i>
                                    <span>+91 98765 43212</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-book"></i>
                                    <span>Subjects: Physics, Mathematics</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Staff Member 4 -->
                    <div class="staff-card">
                        <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&auto=format&fit=crop&w=688&q=80" alt="Ms. Ayesha Rahman" class="staff-img">
                        <div class="staff-info">
                            <h3 class="staff-name">Ms. Ayesha Rahman</h3>
                            <p class="staff-position">Arabic Language Department Head</p>
                            <p class="staff-degree">MA in Arabic Language (University of Jordan), Certificate in Teaching Arabic as Foreign Language</p>
                            <p>Native Arabic speaker with 10 years of experience teaching Arabic language and literature.</p>
                            <div class="staff-contact">
                                <div class="staff-contact-item">
                                    <i class="fas fa-envelope"></i>
                                    <span>ayesha.rahman@darulhudaassam.edu</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-phone"></i>
                                    <span>+91 98765 43213</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-book"></i>
                                    <span>Subjects: Arabic Grammar, Literature</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Staff Member 5 -->
                    <div class="staff-card">
                        <img src="https://images.unsplash.com/photo-1551836026-d5c2a2f0143a?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Mr. Imran Hussain" class="staff-img">
                        <div class="staff-info">
                            <h3 class="staff-name">Mr. Imran Hussain</h3>
                            <p class="staff-position">Computer Science & IT Coordinator</p>
                            <p class="staff-degree">MCA (IIT Delhi), Diploma in Islamic Studies (Darul Huda Islamic University)</p>
                            <p>Specializes in educational technology and digital literacy integration in Islamic education.</p>
                            <div class="staff-contact">
                                <div class="staff-contact-item">
                                    <i class="fas fa-envelope"></i>
                                    <span>imran.hussain@darulhudaassam.edu</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-phone"></i>
                                    <span>+91 98765 43214</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-laptop"></i>
                                    <span>Lab Hours: Mon-Thu, 2 PM - 5 PM</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Staff Member 6 -->
                    <div class="staff-card">
                        <img src="https://images.unsplash.com/photo-1562788869-4ed32648eb72?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Mr. Salman Ahmed" class="staff-img">
                        <div class="staff-info">
                            <h3 class="staff-name">Mr. Salman Ahmed</h3>
                            <p class="staff-position">Administrative Officer</p>
                            <p class="staff-degree">MBA (University of Assam), BA in Islamic Studies (Darul Huda)</p>
                            <p>Manages institutional operations, student services, and parent relations with 8 years of experience.</p>
                            <div class="staff-contact">
                                <div class="staff-contact-item">
                                    <i class="fas fa-envelope"></i>
                                    <span>salman.ahmed@darulhudaassam.edu</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-phone"></i>
                                    <span>+91 98765 43215</span>
                                </div>
                                <div class="staff-contact-item">
                                    <i class="fas fa-briefcase"></i>
                                    <span>For admissions and general inquiries</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Staff Statistics -->
                <div style="margin-top: 4rem;">
                    <div class="total-students">
                        <h3>Our Academic Team</h3>
                        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 2rem; margin-top: 2rem;">
                            <div style="text-align: center;">
                                <div class="total-count" style="font-size: 2.5rem;">35</div>
                                <p>Teaching Faculty</p>
                            </div>
                            <div style="text-align: center;">
                                <div class="total-count" style="font-size: 2.5rem;">12</div>
                                <p>Administrative Staff</p>
                            </div>
                            <div style="text-align: center;">
                                <div class="total-count" style="font-size: 2.5rem;">8</div>
                                <p>Support Staff</p>
                            </div>
                            <div style="text-align: center;">
                                <div class="total-count" style="font-size: 2.5rem;">55</div>
                                <p>Total Staff Members</p>
                            </div>
                        </div>
                        <p style="margin-top: 1rem; font-size: 0.9rem; opacity: 0.9;">
                            <i class="fas fa-chart-line"></i> Average Experience: 10+ years | Faculty with PhD: 8 members
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Admissions Page Content -->
        <section id="admissionsPage" class="page" style="display: none;">
            <div class="container page-content">
                <div class="section-title">
                    <h2>Admissions Process</h2>
                </div>
                
                <div class="about-content">
                    <div class="about-text">
                        <!-- Updated heading -->
                        <h2>Join Our Flock</h2>
                        <p>We welcome applications from curious, motivated students who are eager to learn and grow. Our admissions process seeks to identify students who will thrive in our collaborative, innovative learning environment.</p>
                        
                        <h3 style="margin-top: 2rem;">Admission Timeline</h3>
                        <ol style="margin-left: 1.5rem; margin-top: 1rem;">
                            <li><strong>Explore:</strong> Attend an open house or schedule a personal tour</li>
                            <li><strong>Apply:</strong> Submit online application with required documents</li>
                            <li><strong>Assess:</strong> Student assessment and family interview</li>
                            <li><strong>Decide:</strong> Admission decisions communicated</li>
                            <li><strong>Enroll:</strong> Complete enrollment and orientation</li>
                        </ol>
                        
                        <!-- UPDATED: Added Apply for Admission button with Google Form link -->
                        <div style="margin-top: 2rem; display: flex; gap: 1rem; flex-wrap: wrap;">
                            <a href="#" class="btn" id="downloadProspectus">Download Prospectus</a>
                            <a href="https://forms.gle/gTjnW1gFAxHwbHnm8" target="_blank" class="btn btn-primary">
                                Apply for Admission
                            </a>
                        </div>
                    </div>
                    
                    <div class="about-img">
                        <div style="background-color: white; padding: 2rem; border-radius: 10px; box-shadow: 0 5px 15px rgba(0,0,0,0.05); border-top: 4px solid var(--accent);">
                            <h3 style="color: var(--primary); margin-bottom: 1.5rem;">Important Dates 2024-2025</h3>
                            <div style="margin-bottom: 1.5rem;">
                                <p><strong>Application Opens:</strong> September 1, 2023</p>
                                <p><strong>Early Decision Deadline:</strong> November 15, 2023</p>
                                <p><strong>Regular Decision Deadline:</strong> January 31, 2024</p>
                                <p><strong>Admissions Decisions:</strong> March 15, 2024</p>
                                <p><strong>Academic Year Begins:</strong> August 26, 2024</p>
                            </div>
                            <h3 style="color: var(--primary); margin-bottom: 1rem;">Admissions Office</h3>
                            <p><i class="fas fa-phone"></i> (555) 789-1234</p>
                            <p><i class="fas fa-envelope"></i> admissions@darulhudaassam.edu</p>
                            <p><i class="fas fa-clock"></i> Mon-Fri: 9:00 AM - 4:00 PM</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Page Content - UPDATED WITH WORKING FORM -->
        <section id="contactPage" class="page" style="display: none;">
            <div class="container page-content">
                <div class="section-title">
                    <h2>Contact Us</h2>
                </div>
                
                <div class="contact-container">
                    <div class="contact-info">
                        <h3>Let's Connect</h3>
                        <p>We welcome your inquiries and would be delighted to show you our campus. Contact us to schedule a visit, learn more about our programs, or ask any questions you may have.</p>
                        
                        <div style="margin-top: 2rem;">
                            <h4 style="color: var(--primary); margin-bottom: 1rem;">Campus Location</h4>
                            <p><i class="fas fa-map-marker-alt"></i> <strong>Address:</strong> 456 Education Heights, Learning City, LC 67890</p>
                            <p><i class="fas fa-phone"></i> <strong>Main Office:</strong> (555) 789-1234</p>
                            <p><i class="fas fa-fax"></i> <strong>Fax:</strong> (555) 789-1235</p>
                            <p><i class="fas fa-envelope"></i> <strong>Email:</strong> info@darulhudaassam.edu</p>
                            <p><i class="fas fa-clock"></i> <strong>Office Hours:</strong> Monday-Friday, 8:00 AM - 5:00 PM</p>
                        </div>
                        
                        <div style="margin-top: 2rem;">
                            <h4 style="color: var(--primary); margin-bottom: 1rem;">Campus Tours</h4>
                            <p>Experience the Darul Huda Assam Centre difference firsthand. We offer personalized campus tours throughout the week.</p>
                            <a href="#" class="btn" style="margin-top: 1rem;" id="scheduleTour">Schedule a Tour</a>
                        </div>
                    </div>
                    
                    <!-- UPDATED: Working HTML Form with your email configured -->
                    <div class="contact-form">
                        <h3>Send a Message</h3>
                        <p style="text-align: center; margin-bottom: 1.5rem; color: var(--gray);">
                            Fill out the form below and we'll get back to you within 24 hours.
                        </p>
                        
                        <!-- FormSubmit.co form with your email -->
                        <form action="https://formsubmit.co/your.dear.mahmood@gmail.com" method="POST" id="contactForm">
                            <!-- Email configuration -->
                            <input type="hidden" name="_subject" value="New Contact Form Submission - Darul Huda Assam Centre">
                            <input type="hidden" name="_template" value="table">
                            <input type="hidden" name="_next" value="#" id="thankYouPage">
                            <input type="hidden" name="_captcha" value="false">
                            <input type="hidden" name="_autoresponse" value="Thank you for contacting Darul Huda Assam Centre! We have received your message and will get back to you within 24 hours.">
                            
                            <!-- Form fields -->
                            <div class="form-group">
                                <label for="name">Full Name *</label>
                                <input type="text" id="name" name="name" class="form-control" required placeholder="Your name">
                            </div>
                            
                            <div class="form-group">
                                <label for="email">Email Address *</label>
                                <input type="email" id="email" name="email" class="form-control" required placeholder="Your email address">
                            </div>
                            
                            <div class="form-group">
                                <label for="phone">Phone Number</label>
                                <input type="tel" id="phone" name="phone" class="form-control" placeholder="Your phone number">
                            </div>
                            
                            <div class="form-group">
                                <label for="subject">Inquiry Type *</label>
                                <select id="subject" name="subject" class="form-control" required>
                                    <option value="">Select inquiry type</option>
                                    <option value="admissions">Admissions Inquiry</option>
                                    <option value="general">General Information</option>
                                    <option value="tour">Schedule Campus Tour</option>
                                    <option value="employment">Employment Opportunities</option>
                                    <option value="other">Other</option>
                                </select>
                            </div>
                            
                            <div class="form-group">
                                <label for="message">Message *</label>
                                <textarea id="message" name="message" class="form-control" required placeholder="How can we help you?" rows="5"></textarea>
                            </div>
                            
                            <button type="submit" class="btn btn-primary">Send Message</button>
                        </form>
                        
                        <div class="form-success" id="formSuccess">
                            <i class="fas fa-check-circle"></i>
                            <h3>Thank You!</h3>
                            <p>Your message has been sent successfully. We'll get back to you within 24 hours.</p>
                            <p>You should receive a confirmation email shortly.</p>
                        </div>
                        
                        <p style="text-align: center; margin-top: 1rem; font-size: 0.9rem; color: var(--gray);">
                            <i class="fas fa-lock"></i> Your information is secure and will not be shared.
                        </p>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-logo">
                    <!-- Updated footer name -->
                    <h2>Darul Huda <span>Assam Centre</span></h2>
                    <p>Soaring to Excellence Since 1990</p>
                    <p>Inspiring curious minds to reach new heights through innovative education and compassionate community.</p>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-youtube"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
                
                <div class="footer-links">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#" data-page="home">Home</a></li>
                        <li><a href="#" data-page="about">About Us</a></li>
                        <li><a href="#" data-page="academics">Academics</a></li>
                        <!-- UPDATED FOOTER: Added Students and Staff links -->
                        <li><a href="#" data-page="students">Students</a></li>
                        <li><a href="#" data-page="staff">Staff</a></li>
                        <li><a href="#" data-page="admissions">Admissions</a></li>
                        <li><a href="#" data-page="contact">Contact</a></li>
                        <li><a href="#">Faculty Directory</a></li>
                        <li><a href="#">School Calendar</a></li>
                    </ul>
                </div>
                
                <div class="footer-contact">
                    <h3>Contact Information</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 456 Education Heights, Learning City, LC 67890</p>
                    <p><i class="fas fa-phone"></i> (555) 789-1234</p>
                    <!-- Updated email in footer -->
                    <p><i class="fas fa-envelope"></i> info@darulhudaassam.edu</p>
                    <p><i class="fas fa-clock"></i> Mon-Fri: 8:00 AM - 5:00 PM</p>
                </div>
            </div>
            
            <div class="copyright">
                <!-- Updated copyright notice -->
                <p>&copy; 2023 Darul Huda Assam Centre. All rights reserved. | <a href="#" style="color: var(--accent); text-decoration: none;">Privacy Policy</a> | <a href="#" style="color: var(--accent); text-decoration: none;">Terms of Use</a></p>
                <p style="margin-top: 0.5rem;">Designed with <i class="fas fa-heart" style="color: var(--accent);"></i> for the future of education</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mainNav = document.getElementById('mainNav');
        const mainHeader = document.getElementById('mainHeader');
        
        mobileMenuBtn.addEventListener('click', () => {
            mainNav.classList.toggle('active');
            const icon = mobileMenuBtn.querySelector('i');
            if (mainNav.classList.contains('active')) {
                icon.classList.remove('fa-bars');
                icon.classList.add('fa-times');
            } else {
                icon.classList.remove('fa-times');
                icon.classList.add('fa-bars');
            }
        });
        
        // Header scroll effect - becomes less transparent when scrolled
        window.addEventListener('scroll', () => {
            if (window.scrollY > 100) {
                mainHeader.classList.add('scrolled');
            } else {
                mainHeader.classList.remove('scrolled');
            }
        });
        
        // Page Navigation
        const navLinks = document.querySelectorAll('nav a, .footer-links a');
        const pages = document.querySelectorAll('.page');
        
        // Function to show a specific page
        function showPage(pageId) {
            // Hide all pages
            pages.forEach(page => {
                page.style.display = 'none';
            });
            
            // Show the selected page
            const activePage = document.getElementById(pageId + 'Page');
            if (activePage) {
                activePage.style.display = 'block';
            }
            
            // Update active nav link
            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('data-page') === pageId) {
                    link.classList.add('active');
                }
            });
            
            // Close mobile menu if open
            if (mainNav.classList.contains('active')) {
                mainNav.classList.remove('active');
                const icon = mobileMenuBtn.querySelector('i');
                icon.classList.remove('fa-times');
                icon.classList.add('fa-bars');
            }
            
            // Scroll to top
            window.scrollTo(0, 0);
        }
        
        // Add click event to all navigation links
        navLinks.forEach(link => {
            link.addEventListener('click', (e) => {
                e.preventDefault();
                const pageId = link.getAttribute('data-page');
                if (pageId) {
                    showPage(pageId);
                }
            });
        });
        
        // Contact Form Submission with FormSubmit.co
        const contactForm = document.getElementById('contactForm');
        const formSuccess = document.getElementById('formSuccess');
        
        if (contactForm) {
            contactForm.addEventListener('submit', async (e) => {
                e.preventDefault();
                
                // Show loading state
                const submitBtn = contactForm.querySelector('button[type="submit"]');
                const originalText = submitBtn.textContent;
                submitBtn.textContent = 'Sending...';
                submitBtn.disabled = true;
                
                try {
                    // Submit the form data to FormSubmit.co
                    const formData = new FormData(contactForm);
                    const response = await fetch(contactForm.action, {
                        method: 'POST',
                        body: formData,
                        headers: {
                            'Accept': 'application/json'
                        }
                    });
                    
                    if (response.ok) {
                        // Show success message
                        contactForm.style.display = 'none';
                        formSuccess.style.display = 'block';
                        
                        // Reset form
                        contactForm.reset();
                        
                        // Scroll to success message
                        formSuccess.scrollIntoView({ behavior: 'smooth', block: 'center' });
                    } else {
                        throw new Error('Form submission failed');
                    }
                } catch (error) {
                    // If fetch fails (CORS issues), let the form submit normally
                    console.log('Using standard form submission');
                    contactForm.submit();
                } finally {
                    // Reset button state
                    submitBtn.textContent = originalText;
                    submitBtn.disabled = false;
                }
            });
        }
        
        // Download Prospectus
        const downloadProspectus = document.getElementById('downloadProspectus');
        if (downloadProspectus) {
            downloadProspectus.addEventListener('click', (e) => {
                e.preventDefault();
                alert('Thank you for your interest in Darul Huda Assam Centre! Our prospectus download will begin shortly.');
            });
        }
        
        // Schedule Tour Button
        const scheduleTour = document.getElementById('scheduleTour');
        if (scheduleTour) {
            scheduleTour.addEventListener('click', (e) => {
                e.preventDefault();
                showPage('contact');
                // Auto-select "Schedule Campus Tour" in the form
                setTimeout(() => {
                    document.getElementById('subject').value = 'tour';
                    document.getElementById('message').value = "I'd like to schedule a campus tour. Please contact me to arrange a convenient time.";
                }, 100);
            });
        }
        
        // Read More functionality for Mission and Vision
        const missionBtn = document.getElementById('missionBtn');
        const visionBtn = document.getElementById('visionBtn');
        const missionPreview = document.getElementById('missionPreview');
        const visionPreview = document.getElementById('visionPreview');
        
        if (missionBtn && missionPreview) {
            missionBtn.addEventListener('click', () => {
                missionPreview.classList.toggle('expanded');
                missionBtn.classList.toggle('expanded');
                
                if (missionPreview.classList.contains('expanded')) {
                    missionBtn.innerHTML = 'Read Less <i class="fas fa-chevron-up"></i>';
                } else {
                    missionBtn.innerHTML = 'Read More <i class="fas fa-chevron-down"></i>';
                }
            });
        }
        
        if (visionBtn && visionPreview) {
            visionBtn.addEventListener('click', () => {
                visionPreview.classList.toggle('expanded');
                visionBtn.classList.toggle('expanded');
                
                if (visionPreview.classList.contains('expanded')) {
                    visionBtn.innerHTML = 'Read Less <i class="fas fa-chevron-up"></i>';
                } else {
                    visionBtn.innerHTML = 'Read More <i class="fas fa-chevron-down"></i>';
                }
            });
        }
        
        // Initialize with home page
        document.addEventListener('DOMContentLoaded', () => {
            showPage('home');
            // Add scroll class if page loads scrolled
            if (window.scrollY > 100) {
                mainHeader.classList.add('scrolled');
            }
        });
    </script>
</body>
</html>
