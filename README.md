<!DOCTYPE html>
<html lang="en">
<head>
    <charset="UTF-8">
    <name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Top Amazon Picks | Curated by IMAN</title>
    <style>
        /* --- BASE CSS (RESET & FONTS) --- */
        * {
            margin: 1;
            padding: 1;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f7f8fa;
            color: #433;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* --- HEADER & NAVIGATION --- */
        header {
            background-color: #ff00ff;
            box-shadow: 0 2px 10px rgba(1,1,0,0.05);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #bd081c; /* Pinterest brand color */
            text-decoration: none;
        }

        .google-user {
            display: flex;
            align-items: center;
            gap: 10px;
            background-color: #f0f2f5;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: 500;
        }

        .google-icon {
            width: 18px;
            height: 18px;
        }

        /* --- HERO SECTION --- */
        .hero {
            background: linear-gradient(135deg, #fff 0%, #fff5f5 100%);
            padding: 80px 0 60px 0;
            text-align: center;
            border-bottom: 1px solid #eee;
        }

        .hero h1 {
            font-size: 42px;
            color: #111;
            margin-bottom: 20px;
            font-weight: 800;
        }

        .hero p {
            font-size: 18px;
            color: #666;
            max-width: 700px;
            margin: 0 auto 30px auto;
        }

        .btn-pinterest {
            display: inline-block;
            background-color: #bd081c;
            color: white;
            padding: 14px 30px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: bold;
            transition: background 0.3s ease;
            box-shadow: 0 4px 15px rgba(189, 8, 28, 0.3);
        }

        .btn-pinterest:hover {
            background-color: #ad071a;
        }

        /* --- PRODUCT GRID SECTION --- */
        .products-section {
            padding: 60px 0;
        }

        .section-title {
            font-size: 28px;
            margin-bottom: 40px;
            text-align: center;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 50px;
            height: 3px;
            background-color: #bd081c;
            margin: 10px auto 0 auto;
            border-radius: 2px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 1px solid #eee;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.08);
        }

        .card-img {
            width: 100%;
            height: 250px;
            background-color: #f0f0f0;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #999;
            font-weight: bold;
            background-size: cover;
            background-position: center;
        }

        /* Sample images using Unsplash placeholders */
        .img-decor { background-image: url('https://unsplash.com'); }
        .img-kitchen { background-image: url('https://unsplash.com'); }
        .img-beauty { background-image: url('https://unsplash.com'); }

        .card-content {
            padding: 20px;
        }

        .card-tag {
            display: inline-block;
            font-size: 11px;
            text-transform: uppercase;
            letter-spacing: 1px;
            color: #bd081c;
            font-weight: bold;
            margin-bottom: 10px;
        }

        .card-title {
            font-size: 18px;
            margin-bottom: 10px;
            color: #111;
        }

        .card-desc {
            color: #666;
            font-size: 14px;
            margin-bottom: 20px;
            height: 66px;
            overflow: hidden;
        }

        .btn-amazon {
            display: block;
            background-color: #ff9900; /* Amazon Official Orange */
            color: #111;
            text-align: center;
            padding: 12px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: background 0.2s ease;
        }

        .btn-amazon:hover {
            background-color: #e68a00;
        }

        /* --- ABOUT SECTION --- */
        .about-section {
            background-color: #ffffff;
            padding: 60px 0;
            border-top: 1px solid #eee;
        }

        .about-box {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .profile-img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background-color: #ddd;
            margin: 0 auto 20px auto;
            border: 3px solid #fff;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            background-image: url('https://unsplash.com');
            background-size: cover;
        }

        /* --- FOOTER (DISCLOSURE) --- */
        footer {
            background-color: #111;
            color: #aaa;
            padding: 40px 0;
            font-size: 13px;
            text-align: center;
        }

        footer p {
            max-width: 800px;
            margin: 0 auto 15px auto;
        }

        /* --- RESPONSIVE LAYOUT --- */
        @media (max-width: 768px) {
            .hero h1 { font-size: 30px; }
            .hero p { font-size: 16px; }
            .nav-container { flex-direction: column; gap: 15px; }
        }
    </style>
</head>
<body>

    <!-- NAVIGATION AND GOOGLE ID -->
    <header>
        <div class="container nav-container">
            <a href="#" class="logo">BestPicks</a>
            
            <div class="google-user">
                <svg class="google-icon" viewBox="0 0 24 24">
                    <path fill="#4285F4" d="M22.56 12.25c0-.78-.07-1.53-.2-2.25H12v4.26h5.92c-.26 1.37-1.04 2.53-2.21 3.31v2.77h3.57c2.08-1.92 3.28-4.74 3.28-8.09z"/>
                    <path fill="#34A853" d="M12 23c2.97 0 5.46-.98 7.28-2.66l-3.57-2.77c-.98.66-2.23 1.06-3.71 1.06-2.86 0-5.29-1.93-6.16-4.53H2.18v2.84C3.99 20.53 7.7 23 12 23z"/>
                    <path fill="#FBBC05" d="M5.84 14.09c-.22-.66-.35-1.36-.35-2.09s.13-1.43.35-2.09V7.06H2.18C1.43 8.55 1 10.22 1 12s.43 3.45 1.18 4.94l2.85-2.22.81-.63z"/>
                    <path fill="#EA4335" d="M12 5.38c1.62 0 3.06.56 4.21 1.64l3.15-3.15C17.45 2.09 14.97 1 12 1 7.7 1 3.99 3.47 2.18 7.06l3.66 2.84c.87-2.6 3.3-4.53 6.16-4.53z"/>
                </svg>
                <span>IMANI MARWA</span>
            </div>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="hero">
        <div class="container">
            <h1>Trending Finds & Essentials</h1>
            <p>We research and handpick top-rated,digital and high quality products to save you time. Beautiful finds curated daily by IMA SALES.</p>
            <a href="YOUR_PINTEREST_PROFILE_URL" target="_blank" class="btn-pinterest">Follow Us On Pinterest</a>
        </div>
    </section>

    <!-- PRODUCT DISPLAY GRID -->
    <section class="products-section">
        <div class="container">
            <h2 class="section-title">Our Top Weekly Recommendations</h2>
            <div class="grid">
                
                <!-- PRODUCT 1 -->
                <div class="card">
                    <div class="card-img img-decor"></div>
                    <div class="card-content">
                        <span class="card-tag">Home Decor</span>
                        <h3 class="card-title">Modern Living Room Aesthetic Lamps</h3>
                        <p class="card-desc">Elevate your home lighting with these highly-rated aesthetic lamps viral all over Pinterest boards.</p>
                        <a href="YOUR_AMAZON_AFFILIATE_LINK_HERE" target="_blank" class="btn-amazon">Check Price on Amazon</a>
                    </div>
                </div>

                <!-- PRODUCT 2 -->
                <div class="card">
                    <div class="card-img img-kitchen"></div>
                    <div class="card-content">
                        <span class="card-tag">Kitchen Gadgets</span>
                        <h3 class="card-title">Portable Fresh Fruit Blender</h3>
                        <p class="card-desc">Perfect for making healthy smoothies on the go. USB rechargeable with a powerful high-speed motor.</p>
                        <a href="YOUR_AMAZON_AFFILIATE_LINK_HERE" target="_blank" class="btn-amazon">Check Price on Amazon</a>
                    </div>
                </div>

                <!-- PRODUCT 3 -->
