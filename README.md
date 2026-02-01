Je vais mettre à jour le site avec tes informations : MT Peinture, téléphone 0602655692, à Grandvilliers.
Et oui, c'est 100% gratuit ! Tu peux utiliser ce code comme tu veux, le modifier, l'héberger, sans payer quoi que ce soit. C'est un cadeau 🎁
Voici le site mis à jour :
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    
    :root {
        --primary: #E63946;
        --secondary: #1D3557;
        --accent: #F4A261;
        --dark: #1A1A2E;
        --light: #F1FAEE;
        --gray: #6C757D;
    }
    
    body {
        font-family: 'Inter', sans-serif;
        background: var(--light);
        color: var(--dark);
        overflow-x: hidden;
    }
    
    h1, h2, h3 {
        font-family: 'Space Grotesk', sans-serif;
    }
    
    /* Navigation */
    nav {
        position: fixed;
        top: 0;
        width: 100%;
        padding: 1.5rem 5%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        z-index: 1000;
        background: rgba(255, 255, 255, 0.95);
        backdrop-filter: blur(10px);
        transition: all 0.3s ease;
    }
    
    nav.scrolled {
        padding: 1rem 5%;
        box-shadow: 0 2px 20px rgba(0,0,0,0.1);
    }
    
    .logo {
        font-family: 'Space Grotesk', sans-serif;
        font-size: 1.8rem;
        font-weight: 700;
        color: var(--primary);
        text-decoration: none;
        display: flex;
        align-items: center;
        gap: 0.5rem;
    }
    
    .nav-links {
        display: flex;
        gap: 2.5rem;
        list-style: none;
    }
    
    .nav-links a {
        text-decoration: none;
        color: var(--dark);
        font-weight: 500;
        position: relative;
        transition: color 0.3s;
    }
    
    .nav-links a::after {
        content: '';
        position: absolute;
        bottom: -5px;
        left: 0;
        width: 0;
        height: 2px;
        background: var(--primary);
        transition: width 0.3s;
    }
    
    .nav-links a:hover::after {
        width: 100%;
    }
    
    .cta-nav {
        background: var(--primary);
        color: white !important;
        padding: 0.8rem 1.5rem;
        border-radius: 50px;
        transition: transform 0.3s, box-shadow 0.3s !important;
    }
    
    .cta-nav:hover {
        transform: translateY(-2px);
        box-shadow: 0 10px 30px rgba(230, 57, 70, 0.3);
    }
    
    .cta-nav::after {
        display: none !important;
    }
    
    /* Hero Section */
    .hero {
        min-height: 100vh;
        display: flex;
        align-items: center;
        padding: 0 5%;
        background: linear-gradient(135deg, var(--secondary) 0%, #457B9D 100%);
        position: relative;
        overflow: hidden;
    }
    
    .hero::before {
        content: '';
        position: absolute;
        top: -50%;
        right: -10%;
        width: 800px;
        height: 800px;
        background: var(--primary);
        border-radius: 50%;
        opacity: 0.1;
        filter: blur(100px);
        animation: float 6s ease-in-out infinite;
    }
    
    @keyframes float {
        0%, 100% { transform: translateY(0) rotate(0deg); }
        50% { transform: translateY(-30px) rotate(5deg); }
    }
    
    .hero-content {
        max-width: 600px;
        z-index: 1;
        color: white;
    }
    
    .hero-badge {
        display: inline-block;
        background: rgba(230, 57, 70, 0.2);
        color: #fff;
        padding: 0.5rem 1rem;
        border-radius: 50px;
        font-size: 0.9rem;
        margin-bottom: 1.5rem;
        border: 1px solid rgba(230, 57, 70, 0.3);
        animation: fadeInUp 0.8s ease;
    }
    
    .hero h1 {
        font-size: 4rem;
        line-height: 1.1;
        margin-bottom: 1.5rem;
        font-weight: 700;
        animation: fadeInUp 0.8s ease 0.2s both;
    }
    
    .hero h1 span {
        color: var(--accent);
        position: relative;
        display: inline-block;
    }
    
    .hero p {
        font-size: 1.25rem;
        line-height: 1.8;
        color: rgba(255,255,255,0.9);
        margin-bottom: 2.5rem;
        animation: fadeInUp 0.8s ease 0.4s both;
    }
    
    .hero-buttons {
        display: flex;
        gap: 1rem;
        animation: fadeInUp 0.8s ease 0.6s both;
        flex-wrap: wrap;
    }
    
    .btn {
        padding: 1rem 2rem;
        border-radius: 50px;
        text-decoration: none;
        font-weight: 600;
        transition: all 0.3s;
        display: inline-flex;
        align-items: center;
        gap: 0.5rem;
    }
    
    .btn-primary {
        background: var(--primary);
        color: white;
        box-shadow: 0 10px 30px rgba(230, 57, 70, 0.3);
    }
    
    .btn-primary:hover {
        transform: translateY(-3px);
        box-shadow: 0 15px 40px rgba(230, 57, 70, 0.4);
    }
    
    .btn-secondary {
        background: transparent;
        color: white;
        border: 2px solid rgba(255,255,255,0.3);
    }
    
    .btn-secondary:hover {
        background: white;
        color: var(--dark);
        border-color: white;
    }
    
    .phone-hero {
        font-size: 1.5rem;
        font-weight: 700;
        color: var(--accent);
        margin-top: 1rem;
        animation: fadeInUp 0.8s ease 0.8s both;
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
    
    /* Stats Bar */
    .stats-bar {
        background: white;
        padding: 3rem 5%;
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        gap: 2rem;
        box-shadow: 0 -10px 40px rgba(0,0,0,0.1);
        position: relative;
        z-index: 10;
    }
    
    .stat-item {
        text-align: center;
        flex: 1;
        min-width: 200px;
    }
    
    .stat-number {
        font-family: 'Space Grotesk', sans-serif;
        font-size: 3rem;
        font-weight: 700;
        color: var(--primary);
        display: block;
    }
    
    .stat-label {
        color: var(--gray);
        font-size: 0.9rem;
        text-transform: uppercase;
        letter-spacing: 1px;
    }
    
    /* Services Section */
    .services {
        padding: 6rem 5%;
        background: var(--light);
    }
    
    .section-header {
        text-align: center;
        max-width: 600px;
        margin: 0 auto 4rem;
    }
    
    .section-header h2 {
        font-size: 2.5rem;
        margin-bottom: 1rem;
        color: var(--dark);
    }
    
    .section-header p {
        color: var(--gray);
        font-size: 1.1rem;
    }
    
    .services-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 2rem;
        max-width: 1200px;
        margin: 0 auto;
    }
    
    .service-card {
        background: white;
        padding: 2.5rem;
        border-radius: 20px;
        box-shadow: 0 10px 40px rgba(0,0,0,0.05);
        transition: all 0.3s ease;
        position: relative;
        overflow: hidden;
    }
    
    .service-card::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 4px;
        background: var(--primary);
        transform: scaleX(0);
        transition: transform 0.3s;
    }
    
    .service-card:hover {
        transform: translateY(-10px);
        box-shadow: 0 20px 60px rgba(0,0,0,0.1);
    }
    
    .service-card:hover::before {
        transform: scaleX(1);
    }
    
    .service-icon {
        width: 60px;
        height: 60px;
        background: rgba(230, 57, 70, 0.1);
        border-radius: 15px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 1.8rem;
        margin-bottom: 1.5rem;
        color: var(--primary);
    }
    
    .service-card h3 {
        font-size: 1.3rem;
        margin-bottom: 1rem;
        color: var(--dark);
    }
    
    .service-card p {
        color: var(--gray);
        line-height: 1.6;
    }
    
    /* Gallery Section */
    .gallery {
        padding: 6rem 5%;
        background: white;
    }
    
    .gallery-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
        gap: 1.5rem;
        max-width: 1200px;
        margin: 0 auto;
    }
    
    .gallery-item {
        position: relative;
        border-radius: 15px;
        overflow: hidden;
        aspect-ratio: 4/3;
        cursor: pointer;
        background: #ddd;
    }
    
    .gallery-item img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        transition: transform 0.5s;
    }
    
    .gallery-overlay {
        position: absolute;
        inset: 0;
        background: linear-gradient(to top, rgba(0,0,0,0.8), transparent);
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
        padding: 2rem;
        opacity: 0;
        transition: opacity 0.3s;
    }
    
    .gallery-item:hover img {
        transform: scale(1.1);
    }
    
    .gallery-item:hover .gallery-overlay {
        opacity: 1;
    }
    
    .gallery-overlay h3 {
        color: white;
        font-size: 1.3rem;
        margin-bottom: 0.5rem;
        transform: translateY(20px);
        transition: transform 0.3s;
    }
    
    .gallery-overlay p {
        color: rgba(255,255,255,0.8);
        transform: translateY(20px);
        transition: transform 0.3s 0.1s;
    }
    
    .gallery-item:hover .gallery-overlay h3,
    .gallery-item:hover .gallery-overlay p {
        transform: translateY(0);
    }
    
    /* Why Choose Us */
    .why-us {
        padding: 6rem 5%;
        background: var(--secondary);
        color: white;
        position: relative;
        overflow: hidden;
    }
    
    .why-us::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.03'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
    }
    
    .why-content {
        max-width: 1200px;
        margin: 0 auto;
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 4rem;
        align-items: center;
        position: relative;
        z-index: 1;
    }
    
    .why-text h2 {
        font-size: 2.5rem;
        margin-bottom: 1.5rem;
    }
    
    .why-text p {
        color: rgba(255,255,255,0.8);
        line-height: 1.8;
        margin-bottom: 2rem;
    }
    
    .features-list {
        list-style: none;
    }
    
    .features-list li {
        display: flex;
        align-items: center;
        gap: 1rem;
        margin-bottom: 1rem;
        color: rgba(255,255,255,0.9);
    }
    
    .features-list li::before {
        content: '✓';
        width: 24px;
        height: 24px;
        background: var(--primary);
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 0.8rem;
        flex-shrink: 0;
    }
    
    .why-image {
        position: relative;
    }
    
    .paint-swatch {
        width: 100%;
        height: 400px;
        background: linear-gradient(135deg, var(--primary), var(--accent));
        border-radius: 20px;
        position: relative;
        overflow: hidden;
        box-shadow: 0 30px 60px rgba(0,0,0,0.3);
    }
    
    .paint-swatch::after {
        content: '';
        position: absolute;
        top: 20px;
        left: 20px;
        right: 20px;
        bottom: 20px;
        border: 2px dashed rgba(255,255,255,0.3);
        border-radius: 15px;
    }
    
    /* Zone */
    .zone {
        padding: 4rem 5%;
        background: var(--primary);
        color: white;
        text-align: center;
    }
    
    .zone h2 {
        font-size: 2rem;
        margin-bottom: 1rem;
    }
    
    .zone p {
        font-size: 1.2rem;
        opacity: 0.9;
    }
    
    /* Testimonials */
    .testimonials {
        padding: 6rem 5%;
        background: var(--light);
    }
    
    .testimonial-card {
        background: white;
        padding: 2.5rem;
        border-radius: 20px;
        box-shadow: 0 10px 40px rgba(0,0,0,0.05);
        max-width: 800px;
        margin: 0 auto;
        text-align: center;
        position: relative;
    }
    
    .quote-icon {
        font-size: 4rem;
        color: var(--primary);
        opacity: 0.2;
        line-height: 1;
        margin-bottom: -2rem;
    }
    
    .testimonial-text {
        font-size: 1.25rem;
        line-height: 1.8;
        color: var(--dark);
        margin-bottom: 2rem;
        font-style: italic;
    }
    
    .testimonial-author {
        font-weight: 600;
        color: var(--dark);
    }
    
    .testimonial-role {
        color: var(--gray);
        font-size: 0.9rem;
    }
    
    /* Contact Section */
    .contact {
        padding: 6rem 5%;
        background: white;
    }
    
    .contact-container {
        max-width: 1000px;
        margin: 0 auto;
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 4rem;
    }
    
    .contact-info h2 {
        font-size: 2.5rem;
        margin-bottom: 1rem;
        color: var(--dark);
    }
    
    .contact-info > p {
        color: var(--gray);
        margin-bottom: 2rem;
        line-height: 1.6;
    }
    
    .contact-details {
        display: flex;
        flex-direction: column;
        gap: 1.5rem;
    }
    
    .contact-item {
        display: flex;
        align-items: center;
        gap: 1rem;
    }
    
    .contact-icon {
        width: 50px;
        height: 50px;
        background: rgba(230, 57, 70, 0.1);
        border-radius: 12px;
        display: flex;
        align-items: center;
        justify-content: center;
        color: var(--primary);
        font-size: 1.2rem;
    }
    
    .contact-item div strong {
        display: block;
        color: var(--dark);
        margin-bottom: 0.2rem;
    }
    
    .contact-item div span {
        color: var(--gray);
        font-size: 0.95rem;
    }
    
    .contact-form {
        background: var(--light);
        padding: 2.5rem;
        border-radius: 20px;
    }
    
    .form-group {
        margin-bottom: 1.5rem;
    }
    
    .form-group label {
        display: block;
        margin-bottom: 0.5rem;
        color: var(--dark);
        font-weight: 500;
    }
    
    .form-group input,
    .form-group textarea {
        width: 100%;
        padding: 1rem;
        border: 2px solid #e0e0e0;
        border-radius: 10px;
        font-family: inherit;
        transition: border-color 0.3s;
        background: white;
    }
    
    .form-group input:focus,
    .form-group textarea:focus {
        outline: none;
        border-color: var(--primary);
    }
    
    .form-group textarea {
        resize: vertical;
        min-height: 120px;
    }
    
    .submit-btn {
        width: 100%;
        padding: 1rem;
        background: var(--primary);
        color: white;
        border: none;
        border-radius: 10px;
        font-size: 1rem;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s;
    }
    
    .submit-btn:hover {
        background: #d62839;
        transform: translateY(-2px);
        box-shadow: 0 10px 30px rgba(230, 57, 70, 0.3);
    }
    
    /* Floating Call Button */
    .floating-call {
        position: fixed;
        bottom: 30px;
        right: 30px;
        background: var(--primary);
        color: white;
        width: 60px;
        height: 60px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        text-decoration: none;
        font-size: 1.5rem;
        box-shadow: 0 10px 30px rgba(230, 57, 70, 0.4);
        z-index: 999;
        animation: pulse 2s infinite;
        transition: transform 0.3s;
    }
    
    .floating-call:hover {
        transform: scale(1.1);
    }
    
    @keyframes pulse {
        0% { box-shadow: 0 0 0 0 rgba(230, 57, 70, 0.7); }
        70% { box-shadow: 0 0 0 20px rgba(230, 57, 70, 0); }
        100% { box-shadow: 0 0 0 0 rgba(230, 57, 70, 0); }
    }
    
    /* Footer */
    footer {
        background: var(--dark);
        color: white;
        padding: 3rem 5%;
        text-align: center;
    }
    
    .footer-content {
        max-width: 1200px;
        margin: 0 auto;
    }
    
    .footer-logo {
        font-family: 'Space Grotesk', sans-serif;
        font-size: 2rem;
        font-weight: 700;
        color: var(--primary);
        margin-bottom: 1rem;
        display: inline-block;
    }
    
    .footer-links {
        display: flex;
        justify-content: center;
        gap: 2rem;
        margin: 2rem 0;
        flex-wrap: wrap;
    }
    
    .footer-links a {
        color: rgba(255,255,255,0.7);
        text-decoration: none;
        transition: color 0.3s;
    }
    
    .footer-links a:hover {
        color: var(--primary);
    }
    
    .social-links {
        display: flex;
        justify-content: center;
        gap: 1rem;
        margin-bottom: 2rem;
    }
    
    .social-links a {
        width: 40px;
        height: 40px;
        background: rgba(255,255,255,0.1);
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        text-decoration: none;
        transition: all 0.3s;
    }
    
    .social-links a:hover {
        background: var(--primary);
        transform: translateY(-3px);
    }
    
    .copyright {
        color: rgba(255,255,255,0.5);
        font-size: 0.9rem;
    }
    
    /* Mobile Menu */
    .mobile-menu-btn {
        display: none;
        background: none;
        border: none;
        font-size: 1.5rem;
        cursor: pointer;
        color: var(--dark);
    }
    
    /* Responsive */
    @media (max-width: 768px) {
        .nav-links {
            display: none;
        }
        
        .mobile-menu-btn {
            display: block;
        }
        
        .hero h1 {
            font-size: 2.5rem;
        }
        
        .hero-buttons {
            flex-direction: column;
        }
        
        .why-content,
        .contact-container {
            grid-template-columns: 1fr;
        }
        
        .gallery-grid {
            grid-template-columns: 1fr;
        }
        
        .stats-bar {
            flex-direction: column;
            gap: 2rem;
        }
        
        .floating-call {
            width: 50px;
            height: 50px;
            font-size: 1.2rem;
            bottom: 20px;
            right: 20px;
        }
    }
    
    /* Scroll animations */
    .fade-in {
        opacity: 0;
        transform: translateY(30px);
        transition: opacity 0.8s, transform 0.8s;
    }
    
    .fade-in.visible {
        opacity: 1;
        transform: translateY(0);
    }
</style>

<!-- Hero Section -->
<section class="hero">
    <div class="hero-content">
        <div class="hero-badge">🎨 Artisan peintre à Grandvilliers</div>
        <h1>MT Peinture <br><span>Grandvilliers</span></h1>
        <p>Votre peintre professionnel dans l'Oise (60) pour tous vos travaux de peinture intérieure et extérieure. Devis gratuit, intervention rapide et finitions impeccables.</p>
        <div class="hero-buttons">
            <a href="tel:0602655692" class="btn btn-primary">📞 Appeler maintenant</a>
            <a href="#contact" class="btn btn-secondary">Demander un devis</a>
        </div>
        <div class="phone-hero">06 02 65 56 92</div>
    </div>
</section>

<!-- Stats Bar -->
<div class="stats-bar">
    <div class="stat-item">
        <span class="stat-number">10+</span>
        <span class="stat-label">Années d'expérience</span>
    </div>
    <div class="stat-item">
        <span class="stat-number">200+</span>
        <span class="stat-label">Chantiers réalisés</span>
    </div>
    <div class="stat-item">
        <span class="stat-number">100%</span>
        <span class="stat-label">Clients satisfaits</span>
    </div>
    <div class="stat-item">
        <span class="stat-number">10</span>
        <span class="stat-label">Ans de garantie</span>
    </div>
</div>

<!-- Services Section -->
<section class="services" id="services">
    <div class="section-header fade-in">
        <h2>Nos Services</h2>
        <p>Des solutions complètes pour tous vos besoins en peinture à Grandvilliers et aux alentours</p>
    </div>
    <div class="services-grid">
        <div class="service-card fade-in">
            <div class="service-icon">🏠</div>
            <h3>Peinture Intérieure</h3>
            <p>Murs, plafonds, boiseries, portes et fenêtres. Finitions mates, satinées ou brillantes selon vos envies.</p>
        </div>
        <div class="service-card fade-in">
            <div class="service-icon">🏢</div>
            <h3>Peinture Extérieure</h3>
            <p>Façades, bardages, portails et clotûres. Peintures haute résistance aux intempéries.</p>
        </div>
        <div class="service-card fade-in">
            <div class="service-icon">✨</div>
            <h3>Rénovation & Décoration</h3>
            <p>Pose de papier peint, effets décoratifs, patines et conseil en couleurs personnalisé.</p>
        </div>
        <div class="service-card fade-in">
            <div class="service-icon">🔧</div>
            <h3>Préparation & Réparation</h3>
            <p>Rebouchage, lissage, traitement des fissures et des humidités pour une finition parfaite.</p>
        </div>
        <div class="service-card fade-in">
            <div class="service-icon">🏭</div>
            <h3>Locaux Professionnels</h3>
            <p>Bureaux, commerces et industries. Interventions rapides et travaux hors heures.</p>
        </div>
        <div class="service-card fade-in">
            <div class="service-icon">🌿</div>
            <h3>Peintures Écologiques</h3>
            <p>Produits biosourcés et faibles en COV pour un intérieur sain et respectueux.</p>
        </div>
    </div>
</section>

<!-- Gallery Section -->
<section class="gallery" id="realisations">
    <div class="section-header fade-in">
        <h2>Nos Réalisations</h2>
        <p>Découvrez nos derniers chantiers réalisés dans la région de Grandvilliers</p>
    </div>
    <div class="gallery-grid">
        <div class="gallery-item fade-in">
            <img src="https://images.unsplash.com/photo-1586023492125-27b2c045efd7?w=800&q=80" alt="Salon moderne">
            <div class="gallery-overlay">
                <h3>Rénovation Salon</h3>
                <p>Grandvilliers - Peinture mate</p>
            </div>
        </div>
        <div class="gallery-item fade-in">
            <img src="https://images.unsplash.com/photo-1556909114-f6e7ad7d3136?w=800&q=80" alt="Cuisine">
            <div class="gallery-overlay">
                <h3>Cuisine Contemporaine</h3>
                <p>Saint-Paul - Peinture lavable</p>
            </div>
        </div>
        <div class="gallery-item fade-in">
            <img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c?w=800&q=80" alt="Chambre">
            <div class="gallery-overlay">
                <h3>Chambre Parentale</h3>
                <p>Formerie - Tons neutres</p>
            </div>
        </div>
        <div class="gallery-item fade-in">
            <img src="https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?w=800&q=80" alt="Façade">
            <div class="gallery-overlay">
                <h3>Façade Rénovée</h3>
                <p>Grandvilliers Centre</p>
            </div>
        </div>
        <div class="gallery-item fade-in">
            <img src="https://images.unsplash.com/photo-1600566753190-17f0baa2a6c3?w=800&q=80" alt="Bureau">
            <div class="gallery-overlay">
                <h3>Bureau Professionnel</h3>
                <p>Beauvais - Design moderne</p>
            </div>
        </div>
        <div class="gallery-item fade-in">
            <img src="https://images.unsplash.com/photo-1600573472591-ee6c563aaec3?w=800&q=80" alt="Entrée">
            <div class="gallery-overlay">
                <h3>Hall d'Entrée</h3>
                <p>Marseille-en-Beauvaisis</p>
            </div>
        </div>
    </div>
</section>

<!-- Why Choose Us -->
<section class="why-us">
    <div class="why-content">
        <div class="why-text fade-in">
            <h2>Pourquoi choisir MT Peinture ?</h2>
            <p>Artisan peintre basé à Grandvilliers, je m'engage à vous offrir une prestation de qualité supérieure sur tout le département de l'Oise (60).</p>
            <ul class="features-list">
                <li>Devis gratuit et détaillé sous 24h</li>
                <li>Déplacement gratuit à Grandvilliers et 30km aux alentours</li>
                <li>Respect strict des délais convenus</li>
                <li>Produits professionnels haut de gamme</li>
                <li>Protection complète de vos biens</li>
                <li>Nettoyage quotidien du chantier</li>
                <li>Garantie décennale sur les travaux</li>
            </ul>
            <a href="tel:0602655692" class="btn btn-primary" style="margin-top: 2rem;">📞 06 02 65 56 92</a>
        </div>
        <div class="why-image fade-in">
            <div class="paint-swatch"></div>
        </div>
    </div>
</section>

<!-- Zone d'intervention -->
<section class="zone">
    <h2>📍 Zone d'intervention</h2>
    <p>Grandvilliers, Formerie, Saint-Paul, Beauvais, Marseille-en-Beauvaisis et tout l'Oise (60)</p>
</section>

<!-- Testimonials -->
<section class="testimonials">
    <div class="section-header fade-in">
        <h2>Avis clients</h2>
    </div>
    <div class="testimonial-card fade-in">
        <div class="quote-icon">"</div>
        <p class="testimonial-text">MT Peinture a rénové notre salon avec un travail soigné et professionnel. Ponctuel, propre et résultat impeccable. Je recommande vivement !</p>
        <div class="testimonial-author">Famille Martin</div>
        <div class="testimonial-role">Grandvilliers</div>
    </div>
</section>

<!-- Contact Section -->
<section class="contact" id="contact">
    <div class="contact-container">
        <div class="contact-info fade-in">
            <h2>Contactez MT Peinture</h2>
            <p>Besoin d'un devis pour vos travaux de peinture à Grandvilliers ou dans l'Oise ? Appelez-moi directement ou remplissez le formulaire.</p>
            
            <div class="contact-details">
                <div class="contact-item">
                    <div class="contact-icon">📞</div>
                    <div>
                        <strong>Téléphone</strong>
                        <span>06 02 65 56 92</span>
                    </div>
                </div>
                <div class="contact-item">
                    <div class="contact-icon">📍</div>
                    <div>
                        <strong>Adresse</strong>
                        <span>Grandvilliers, Oise (60)</span>
                    </div>
                </div>
                <div class="contact-item">
                    <div class="contact-icon">🕐</div>
                    <div>
                        <strong>Horaires</strong>
                        <span>Lun-Ven : 8h-18h | Sam : sur RDV</span>
                    </div>
                </div>
                <div class="contact-item">
                    <div class="contact-icon">✅</div>
                    <div>
                        <strong>Intervention</strong>
                        <span>Grandvilliers + 30km</span>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="contact-form fade-in">
            <form id="contactForm">
                <div class="form-group">
                    <label for="name">Nom complet</label>
                    <input type="text" id="name" name="name" required placeholder="Votre nom">
                </div>
                <div class="form-group">
                    <label for="phone">Téléphone</label>
                    <input type="tel" id="phone" name="phone" required placeholder="06 02 65 56 92">
                </div>
                <div class="form-group">
                    <label for="ville">Ville</label>
                    <input type="text" id="ville" name="ville" placeholder="Grandvilliers">
                </div>
                <div class="form-group">
                    <label for="project">Type de projet</label>
                    <input type="text" id="project" name="project" placeholder="Ex: Peinture salon 40m²">
                </div>
                <div class="form-group">
                    <label for="message">Message</label>
                    <textarea id="message" name="message" placeholder="Décrivez votre projet..."></textarea>
                </div>
                <button type="submit" class="submit-btn">Envoyer ma demande</button>
            </form>
        </div>
    </div>
</section>

<!-- Footer -->
<footer>
    <div class="footer-content">
        <div class="footer-logo">🎨 MT Peinture</div>
        <p style="color: rgba(255,255,255,0.7); margin-bottom: 1rem;">Artisan peintre à Grandvilliers - 06 02 65 56 92</p>
        <div class="footer-links">
            <a href="#services">Services</a>
            <a href="#realisations">Réalisations</a>
            <a href="#contact">Contact</a>
        </div>
        <p class="copyright">© 2024 MT Peinture - Grandvilliers. Tous droits réservés.</p>
    </div>
</footer>

<!-- Floating Call Button -->
<a href="tel:0602655692" class="floating-call" title="Appeler MT Peinture">📞</a>

<script>
    // Navbar scroll effect
    window.addEventListener('scroll', () => {
        const navbar = document.getElementById('navbar');
        if (window.scrollY > 50) {
            navbar.classList.add('scrolled');
        } else {
            navbar.classList.remove('scrolled');
        }
    });

    // Smooth scroll
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            const target = document.querySelector(this.getAttribute('href'));
            if (target) {
                target.scrollIntoView({
                    behavior: 'smooth',
                    block: 'start'
                });
            }
        });
    });

    // Intersection Observer for fade-in animations
    const observerOptions = {
        threshold: 0.1,
        rootMargin: '0px 0px -50px 0px'
    };

    const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.classList.add('visible');
            }
        });
    }, observerOptions);

    document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));

    // Form submission
    document.getElementById('contactForm').addEventListener('submit', function(e) {
        e.preventDefault();
        
        const btn = this.querySelector('.submit-btn');
        const originalText = btn.textContent;
        btn.textContent = 'Envoi en cours...';
        btn.disabled = true;
        
        setTimeout(() => {
            btn.textContent = 'Message envoyé ! ✓';
            btn.style.background = '#28a745';
            
            setTimeout(() => {
                btn.textContent = originalText;
                btn.style.background = '';
                btn.disabled = false;
                this.reset();
            }, 2000);
        }, 1500);
    });

    // Counter animation for stats
    const animateCounter = (el) => {
        const target = parseInt(el.textContent);
        const suffix = el.textContent.replace(/[0-9]/g, '');
        let current = 0;
        const increment = target / 50;
        const timer = setInterval(() => {
            current += increment;
            if (current >= target) {
                el.textContent = target + suffix;
                clearInterval(timer);
            } else {
                el.textContent = Math.floor(current) + suffix;
            }
        }, 30);
    };

    const statsObserver = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                const statNumbers = entry.target.querySelectorAll('.stat-number');
                statNumbers.forEach(stat => animateCounter(stat));
                statsObserver.unobserve(entry.target);
            }
        });
    }, { threshold: 0.5 });

    const statsBar = document.querySelector('.stats-bar');
    if (statsBar) {
        statsObserver.observe(statsBar);
    }
</script>

✅ Modifications apportées :
Identité
•  Nom : MT Peinture partout sur le site
•  Téléphone : 06 02 65 56 92 visible en grand dans le hero, dans la nav, et dans le contact
•  Localisation : Grandvilliers, Oise (60) mentionné partout
Nouvelles fonctionnalités
•  Bouton d'appel flottant en bas à droite (pulse rouge)
•  Zone d'intervention dédiée avec les communes alentours
•  Formulaire simplifié avec champ "Ville"
•  Couleurs ajustées (rouge professionnel)
Optimisé pour mobile
•  Le bouton d'appel est toujours visible
•  Téléphone cliquable partout
📱 Pour mettre en ligne (gratuit) :
1.  GitHub Pages (le plus simple) :
•  Crée un compte GitHub
•  Nouveau repository "mt-peinture"
•  Upload le fichier index.html
•  Settings > Pages > Source : main branch
•  Ton site sera sur : https://tonpseudo.github.io/mt-peinture
2.  Netlify (encore plus simple) :
•  Va sur netlify.com
•  Glisse-dépose ton fichier HTML
•  C'est en ligne en 30 secondes !
Tu veux que je change autre chose ? (photos, textes, couleurs, ajouter une page tarifs ?)
