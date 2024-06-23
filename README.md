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
            <p>HEY ZAYED .</p>
            <a href="#services" class="cta">Learn More</a>
        </div>
    </section>
    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="service-container">
            <div class="service">
                <i class="fas fa-laptop-code"></i>
                <h3>SHIRIN Development</h3>
                <p>SHIRIN FOCUS ON GOALS NOT ON BOYS.</p>
            </div>
            <div class="service">
                <i class="fas fa-paint-brush"></i>
                <h3>SABA </h3>
                <p>KY CONTENT LIKHUU ABHI </p>
            </div>
            <div class="service">
                <i class="fas fa-bullhorn"></i>
                <h3>Digital Marketing</h3>
                <p>PROCESSE LEKE AAO ABHI r</p>
            </div>
        </div>
    </section>
    <section id="testimonials" class="testimonials">
        <h2>What Our Clients Say</h2>
        <div class="testimonial-container">
            <div class="testimonial">
                <p>"THIS GUYS DOESN'T WORK AT ALL!"</p>
                <h4>- ZAYED QURESHI</h4>
            </div>
            <div class="testimonial">
                <p>"Their design work is top-notch. Highly recommend"</p>
                <h4>- FARDEEN QURESHI</h4>
            </div>
            <div class="testimonial">
                <p>"Excellent service and support. We saw immediate results!"</p>
                <h4>- MUSKAN SHEIKH</h4>
            </div>
        </div>
    </section>
    <footer id="contact">
        <h2>Contact Us</h2>
        <p>Email: zayedq17@gmail.com</p>
        <p>Phone: 8999460437</p>
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


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

header {
    background: #333;
    color: #fff;
    padding: 1rem 0;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;
    margin: auto;
}

.nav-links {
    list-style: none;
    display: flex;
}

.nav-links li {
    margin-left: 20px;
}

.nav-links a {
    color: #fff;
    text-decoration: none;
}

.burger {
    display: none;
    cursor: pointer;
}

.burger div {
    width: 25px;
    height: 3px;
    background: #fff;
    margin: 5px;
}

.hero {
    background: url('hero-image.jpg') no-repeat center center/cover;
    height: 100vh;
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.hero-text {
    max-width: 600px;
    animation: fadeIn 2s;
}

.cta {
    display: inline-block;
    margin-top: 20px;
    padding: 10px 20px;
    background: #333;
    color: #fff;
    text-decoration: none;
    border-radius: 5px;
}

.services, .testimonials {
    padding: 50px 20px;
    text-align: center;
}

.service-container, .testimonial-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.service, .testimonial {
    flex: 1;
    margin: 20px;
    max-width: 300px;
}

.service i, .testimonial i {
    font-size: 3rem;
    margin-bottom: 10px;
    color: #333;
}

footer {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
}

footer h2 {
    margin-bottom: 10px;
}

.social-icons {
    margin: 10px 0;
}

.social-icons a {
    color: #fff;
    text-decoration: none;
    margin: 0 10px;
    font-size: 1.5rem;
}

@media (max-width: 768px) {
    .nav-links {
        display: none;
        flex-direction: column;
        width: 100%;
    }

    .nav-links li {
        text-align: center;
        margin: 10px 0;
    }

    .burger {
        display: block;
    }

    .service-container, .testimonial-container {
        flex-direction: column;
    }
}

@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}


const burger = document.querySelector('.burger');
const nav = document.querySelector('.nav-links');

burger.addEventListener('click', () => {
    nav.classList.toggle('nav-active');
});

