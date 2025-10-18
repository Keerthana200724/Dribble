# Project Responsive Web Design using Bootstrap
## Date:16.10.2025

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .card-img-top {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }
        footer {
            background-color: #f8f9fa;
            padding: 20px 0;
            text-align: center;
            width: 100%;
            bottom: 0px;
        }
    </style>
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-light shadow-sm">
        <div class="container">
            <a class="navbar-brand fw-bold text-primary" href="#">Dribbble Clone</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#features">Features</a></li>
                    <li class="nav-item"><a class="nav-link" href="#portfolio">Portfolio</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
                    <li class="nav-item"><a class="nav-link btn btn-primary text-white" href="signup.html">Sign Up</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <header class="bg-primary text-white text-center py-5">
        <div class="container">
            <h1 class="fw-bold">Show Your Creativity to the World</h1>
            <p class="lead">Join the platform where designers share, grow, and inspire.</p>
            <a href="#portfolio" class="btn btn-light btn-lg">Get Started</a>
        </div>
    </header>

    <section id="features" class="py-5">
        <div class="container">
            <h2 class="text-center mb-4 fw-bold">Features</h2>
            <div class="row text-center">
                <div class="col-md-4">
                    <div class="card shadow-sm">
                        <div class="card-body">
                            <h5 class="card-title">For Designers</h5>
                            <p class="card-text">Showcase your portfolio and gain exposure to potential clients. Build your brand and get noticed by top businesses and teams.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card shadow-sm">
                        <div class="card-body">
                            <h5 class="card-title">For Inspiration</h5>
                            <p class="card-text">Discover creative ideas from a global community of designers. Get inspired by the latest trends and innovative designs.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card shadow-sm">
                        <div class="card-body">
                            <h5 class="card-title">For Businesses</h5>
                            <p class="card-text">Connect with top designers to bring your ideas to life. Find the right creative talent to help you design and build your brand’s future.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="portfolio" class="py-5 bg-light">
        <div class="container">
            <h2 class="text-center mb-4 fw-bold">Portfolio</h2>
            <p class="text-center mb-4">Explore some of the best creative works shared by the community.</p>
            <div class="row">
                <div class="col-md-4 mb-4">
                    <div class="card">
                       <img src="{% static 'retro.jpg' %}" class="card-img-top" alt="Retrospective Branding Design">

                        <div class="card-body">
                            <h5 class="card-title">Retrospective Branding Design</h5>
                            <p class="card-text">A modern take on retro branding elements, blending classic typography with contemporary aesthetics.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                       <img src="{% static 'house.jpg' %}" class="card-img-top" alt="Home Swap Platform UI Elements">


                        <div class="card-body">
                            <h5 class="card-title">Home Swap Platform UI Elements</h5>
                            <p class="card-text">UI design for a home exchange platform, featuring intuitive navigation and user-friendly interfaces.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                        <img src="{% static 'jewel.jpg' %}" class="card-img-top" alt="Jewelry Website Design">

                        <div class="card-body">
                            <h5 class="card-title">Jewelry Website Design</h5>
                            <p class="card-text">An elegant e-commerce website design for a jewelry brand, emphasizing luxury and user experience.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                       <img src="{% static 'ev.jpg' %}" class="card-img-top" alt="EV Charging Station Branding">

                        <div class="card-body">
                            <h5 class="card-title">EV Charging Station Branding</h5>
                            <p class="card-text">Brand identity design for an electric vehicle charging station, incorporating eco-friendly themes.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                        <img src="{% static 'fitness.jpg' %}" class="card-img-top" alt="Fitness App UI Design">

                        <div class="card-body">
                            <h5 class="card-title">Fitness App UI Design</h5>
                            <p class="card-text">A sleek and modern user interface design for a fitness tracking mobile application.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                       <img src="{% static 'coffee.jpg' %}" class="card-img-top" alt="Coffee Shop Logo Design">


                        <div class="card-body">
                            <h5 class="card-title">Coffee Shop Logo Design</h5>
                            <p class="card-text">A minimalist and cozy logo design for a local coffee shop, capturing the essence of warmth.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="py-5">
        <div class="container contact-container">
            <h2 class="text-center mb-4 fw-bold">Contact Us</h2>
            <p class="text-center mb-4">We'd love to hear from you! Whether you have a question, feedback, or suggestion, feel free to reach out using the form below.</p>
            <form action="#" method="POST">
                <div class="mb-3">
                    <label for="name" class="form-label">Full Name</label>
                    <input type="text" class="form-control" id="name" name="name" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" id="email" name="email" required>
                </div>
                <div class="mb-3">
                    <label for="subject" class="form-label">Subject</label>
                    <input type="text" class="form-control" id="subject" name="subject" required>
                </div>
                <div class="mb-3">
                    <label for="message" class="form-label">Message</label>
                    <textarea class="form-control" id="message" name="message" rows="4" required></textarea>
                </div>
                <button type="submit" class="btn btn-primary w-100">Send Message</button>
            </form>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 All rights reserved.</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```


## OUTPUT:
<img width="1078" height="400" alt="image" src="https://github.com/user-attachments/assets/a7eaa1b1-02f8-4abb-8b96-31424b261aa5" />
<img width="976" height="638" alt="image" src="https://github.com/user-attachments/assets/34baebb0-7c9f-443b-860f-7efe484dc8a8" />
<img width="966" height="442" alt="image" src="https://github.com/user-attachments/assets/88b44752-fe03-4e61-ad95-eff03e43a38a" />





## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
