<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shattuck-St. Mary's | Forest City International School</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --forest-deep: #0a2e1f;
            --leaf-green: #2d6a4f;
            --soft-lime: #95d5b2;
            --accent-gold: #d4af37;
            --ivory: #fcfaf1;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Playfair Display', serif; /* Elegant heading font */
        }

        body {
            background-color: var(--ivory);
            color: var(--forest-deep);
            overflow-x: hidden;
        }

        /* Foliage Background Elements */
        .leaf-decor {
            position: fixed;
            opacity: 0.1;
            z-index: -1;
            pointer-events: none;
        }

        /* Navigation */
        nav {
            background: rgba(255, 255, 255, 0.95);
            padding: 1.5rem 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 3px solid var(--leaf-green);
        }

        .logo-box { line-height: 1; }
        .logo-main { font-size: 1.4rem; font-weight: 900; color: var(--forest-deep); }
        .logo-sub { font-size: 0.8rem; letter-spacing: 2px; color: var(--accent-gold); }

        nav ul { display: flex; list-style: none; }
        nav ul li { margin-left: 30px; }
        nav ul li a { text-decoration: none; color: var(--forest-deep); font-weight: 600; font-family: sans-serif; transition: 0.3s; }
        nav ul li a:hover { color: var(--leaf-green); }

        /* Hero Video/Image Area */
        .hero {
            height: 90vh;
            background: linear-gradient(to bottom, rgba(10, 46, 31, 0.4), rgba(10, 46, 31, 0.8)), 
                        url('https://images.unsplash.com/photo-1590066305974-bc1997a3475b?auto=format&fit=crop&w=1600&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            clip-path: ellipse(150% 100% at 50% 0%); /* Curved bottom for organic feel */
        }

        .hero h1 { font-size: 4rem; margin-bottom: 10px; text-shadow: 2px 2px 10px rgba(0,0,0,0.5); }
        .hero p { font-size: 1.4rem; font-family: sans-serif; max-width: 800px; margin-bottom: 30px; }

        /* Info Sections */
        .section-padding { padding: 100px 10%; }
        
        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
            margin-top: 50px;
        }

        .info-card {
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            border-top: 5px solid var(--leaf-green);
            position: relative;
            overflow: hidden;
        }

        .info-card i { font-size: 2rem; color: var(--accent-gold); margin-bottom: 15px; }

        /* Plant Decorative Accents */
        .plant-divider {
            text-align: center;
            font-size: 2rem;
            color: var(--leaf-green);
            margin: 50px 0;
        }

        /* Boarding & Campus */
        .campus-highlight {
            background: var(--forest-deep);
            color: white;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            border-radius: 40px;
            margin: 0 5%;
            overflow: hidden;
        }

        .campus-text { flex: 1; padding: 60px; min-width: 300px; }
        .campus-img { flex: 1; min-width: 300px; height: 500px; background: url('https://images.unsplash.com/photo-1560448204-61dc36dc98c8?auto=format&fit=crop&w=800&q=80') center/cover; }

        /* Footer */
        footer {
            background: #051610;
            color: #d1d1d1;
            padding: 80px 10% 20px;
            margin-top: 100px;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: 2fr 1fr 1fr;
            gap: 50px;
            border-bottom: 1px solid #1a3a2e;
            padding-bottom: 50px;
        }

        .contact-pill {
            display: inline-block;
            background: var(--leaf-green);
            color: white;
            padding: 10px 20px;
            border-radius: 50px;
            text-decoration: none;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <i class="fas fa-leaf leaf-decor" style="top: 15%; left: 5%; font-size: 150px; transform: rotate(45deg);"></i>
    <i class="fas fa-seedling leaf-decor" style="bottom: 10%; right: 5%; font-size: 200px;"></i>

    <nav>
        <div class="logo-box">
            <div class="logo-main">SHATTUCK-ST. MARY'S</div>
            <div class="logo-sub">FOREST CITY MALAYSIA</div>
        </div>
        <ul>
            <li><a href="#about">Our School</a></li>
            <li><a href="#academics">Academics</a></li>
            <li><a href="#boarding">Boarding</a></li>
            <li><a href="#admission">Admissions</a></li>
        </ul>
    </nav>

    <header class="hero">
        <h1>Where Nature Meets Knowledge</h1>
        <p>An elite American boarding school experience nestled in Johor's most sustainable forest city.</p>
        <a href="#" class="btn" style="background: var(--accent-gold); color: white; padding: 15px 40px; border-radius: 50px; text-decoration: none; font-weight: bold;">BOOK A CAMPUS TOUR</a>
    </header>

    <section class="section-padding" id="about">
        <div class="plant-divider"><i class="fas fa-leaf"></i></div>
        <h2 style="text-align: center; font-size: 2.5rem;">Academic Excellence</h2>
        <div class="info-grid">
            <div class="info-card">
                <i class="fas fa-book-open"></i>
                <h3>American Curriculum</h3>
                <p>We offer a rigorous standards-based American curriculum, culminating in the prestigious High School Diploma, preparing students for top global universities.</p>
            </div>
            <div class="info-card">
                <i class="fas fa-microscope"></i>
                <h3>weCreate® Center</h3>
                <p>A unique space dedicated to creativity and innovation, where students explore robotics, digital media, fashion design, and music production.</p>
            </div>
            <div class="info-card">
                <i class="fas fa-users"></i>
                <h3>Expert Faculty</h3>
                <p>Our educators are world-class professionals committed to personalized learning and the holistic growth of every scholar.</p>
            </div>
        </div>
    </section>

    <div class="campus-highlight" id="boarding">
        <div class="campus-text">
            <h2 style="font-size: 2.2rem; margin-bottom: 20px;">World-Class Boarding</h2>
            <p>Our residential life program provides a safe, supportive "home away from home." Students live in modern, eco-friendly suites with 24/7 care and a vibrant community atmosphere.</p>
            <ul style="margin-top: 20px; list-style: circle; padding-left: 20px;">
                <li>Full & Weekly Boarding Options</li>
                <li>Healthy, Internationally Inspired Meals</li>
                <li>Evening Enrichment & Support</li>
            </ul>
        </div>
        <div class="campus-img"></div>
    </div>

    <section class="section-padding">
        <h2 style="text-align: center; margin-bottom: 50px;">Key Information</h2>
        <div class="info-grid">
            <div class="info-card">
                <h3><i class="fas fa-map-marker-alt"></i> Location</h3>
                <p>Forest City, Gelang Patah, Johor. Only 15 minutes from the Tuas Second Link to Singapore.</p>
            </div>
            <div class="info-card">
                <h3><i class="fas fa-child"></i> Grades</h3>
                <p>Serving students from Pre-K (3 years old) through Grade 12 (Graduation).</p>
            </div>
            <div class="info-card">
                <h3><i class="fas fa-swimmer"></i> Facilities</h3>
                <p>Olympic-sized pool, theater, indoor gym, and state-of-the-art science labs.</p>
            </div>
        </div>
    </section>

    <footer>
        <div class="footer-grid">
            <div>
                <h3 style="color: white; margin-bottom: 20px;">Contact Us</h3>
                <p>Jalan Forest City 8, Pulau Satu, Forest City</p>
                <p>81550 Gelang Patah, Johor, Malaysia</p>
                <a href="mailto:admissions@ssm-fc.org" class="contact-pill">Email Admissions</a>
            </div>
            <div>
                <h4 style="color: var(--accent-gold);">Quick Links</h4>
                <p>School Calendar</p>
                <p>Fee Structure</p>
                <p>Careers</p>
            </div>
            <div>
                <h4 style="color: var(--accent-gold);">Follow Us</h4>
                <div style="font-size: 1.5rem; margin-top: 15px;">
                    <i class="fab fa-facebook" style="margin-right: 15px;"></i>
                    <i class="fab fa-instagram" style="margin-right: 15px;"></i>
                    <i class="fab fa-linkedin"></i>
                </div>
            </div>
        </div>
        <p style="text-align: center; margin-top: 30px; font-size: 0.8rem;">&copy; 2026 Shattuck-St. Mary's Forest City International School. All Rights Reserved.</p>
    </footer>

</body>
</html>
