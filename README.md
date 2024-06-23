<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced Front Page</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">MyWebsite</div>
            <ul class="nav-links">
                <li><a href="#">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#testimonials">Testimonials</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="burger">
                <div class="line1"></div>
                <div class="line2"></div>
                <div class="line3"></div>
            </div>
        </nav>
    </header>
    <section class="hero">
        <div class="hero-text">
            <h1>Welcome to MyWebsite</h1>
            <p>We provide amazing services for you.</p>
            <a href="#services" class="cta">Learn More</a>
        </div>
    </section>
    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="service-container">
            <div class="service">
                <i class="fas fa-laptop-code"></i>
                <h3>Web Development</h3>
                <p>Building responsive and functional websites.</p>
            </div>
            <div class="service">
                <i class="fas fa-paint-brush"></i>
                <h3>Graphic Design</h3>
                <p>Creating stunning visual content.</p>
            </div>
            <div class="service">
                <i class="fas fa-bullhorn"></i>
                <h3>Digital Marketing</h3>
                <p>Boosting your online presence.</p>
            </div>
        </div>
    </section>
    <section id="testimonials" class="testimonials">
        <h2>What Our Clients Say</h2>
        <div class="testimonial-container">
            <div class="testimonial">
                <p>"MyWebsite transformed our business with a fantastic website!"</p>
                <h4>- John Doe</h4>
            </div>
            <div class="testimonial">
                <p>"Their design work is top-notch. Highly recommend!"</p>
                <h4>- Jane Smith</h4>
            </div>
            <div class="testimonial">
                <p>"Excellent service and support. We saw immediate results!"</p>
                <h4>- Mike Johnson</h4>
            </div>
        </div>
    </section>
    <footer id="contact">
        <h2>Contact Us</h2>
        <p>Email: info@mywebsite.com</p>
        <p>Phone: +123 456 7890</p>
        <div class="social-icons">
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-linkedin-in"></i></a>
        </div>
        <p>&copy; 2024 MyWebsite. All rights reserved.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
