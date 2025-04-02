# smartValleyTech
for learning technology
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>SmartValleyTech Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css" rel="stylesheet">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/Swiper/8.4.5/swiper-bundle.min.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/Swiper/8.4.5/swiper-bundle.min.js"></script>
    <style>
        :root {
            --primary: #2D3748;
            --secondary: #4A5568;
            --accent: #6B46C1;
            --highlight: #9F7AEA;
            --background: #F7FAFC;
            --text-primary: #2D3748;
            --text-secondary: #4A5568;
        }

        /* Previous styles remain the same until navigation */

        /* Navigation Styles */
        .nav-link {
            position: relative;
        }

        .nav-link::after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--accent);
            transition: width 0.3s ease;
        }

        .nav-link:hover::after,
        .nav-link.active::after {
            width: 100%;
        }

        /* Hero Section Styles */
        .hero-gradient {
            background: linear-gradient(135deg, var(--primary), var(--accent));
            position: relative;
            overflow: hidden;
        }

        .hero-gradient::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(45deg, rgba(0,0,0,0.2) 0%, rgba(0,0,0,0) 100%);
        }

        /* Course Card Styles */
        .course-card {
            background: white;
            border-radius: 1rem;
            overflow: hidden;
            transition: all 0.3s ease;
        }

        .course-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .course-image {
            position: relative;
            overflow: hidden;
        }

        .course-image img {
            transition: transform 0.3s ease;
        }

        .course-card:hover .course-image img {
            transform: scale(1.1);
        }

        /* Feature Card Styles */
        .feature-card {
            background: white;
            border-radius: 1rem;
            padding: 1.5rem;
            transition: all 0.3s ease;
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .feature-icon {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--accent), var(--highlight));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            margin-bottom: 1rem;
        }

        /* Previous styles remain the same */
    </style>
</head>
<body class="bg-[var(--background)]">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg fixed w-full z-50">
        <div class="max-w-7xl mx-auto px-4">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <h1 class="text-xl md:text-2xl font-bold gradient-text">SmartValleyTech</h1>
                </div>
                <button class="mobile-menu-button md:hidden focus:outline-none">
                    <i class="fas fa-bars text-2xl text-[var(--text-primary)]"></i>
                </button>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="nav-link text-[var(--text-primary)] hover:text-[var(--accent)] transition">Home</a>
                    <a href="#courses" class="nav-link text-[var(--text-primary)] hover:text-[var(--accent)] transition">Courses</a>
                    <a href="#about" class="nav-link text-[var(--text-primary)] hover:text-[var(--accent)] transition">About</a>
                    <a href="#contact" class="nav-link text-[var(--text-primary)] hover:text-[var(--accent)] transition">Contact</a>
                </div>
                <button class="primary-button px-6 py-2 rounded-full hidden md:block">
                    Register Now
                </button>
            </div>
            <div class="mobile-menu md:hidden">
                <a href="#home" class="block text-[var(--text-primary)] hover:text-[var(--accent)] transition py-2">Home</a>
                <a href="#courses" class="block text-[var(--text-primary)] hover:text-[var(--accent)] transition py-2">Courses</a>
                <a href="#about" class="block text-[var(--text-primary)] hover:text-[var(--accent)] transition py-2">About</a>
                <a href="#contact" class="block text-[var(--text-primary)] hover:text-[var(--accent)] transition py-2">Contact</a>
                <button class="primary-button w-full py-2 rounded-full mt-4">
                    Register Now
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-gradient pt-24 pb-12 md:pt-32 md:pb-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row items-center justify-between">
                <div class="md:w-1/2 text-white text-center md:text-left mb-8 md:mb-0">
                    <h1 class="text-3xl md:text-5xl font-bold mb-6 animate__animated animate__fadeInLeft">Transform Your Tech Career with SmartValleyTech</h1>
                    <p class="text-lg md:text-xl mb-8 text-gray-100 animate__animated animate__fadeInLeft animate__delay-1s">Master the latest technologies with our industry-leading courses in Nigeria.</p>
                    <div class="flex flex-col md:flex-row space-y-4 md:space-y-0 md:space-x-4 animate__animated animate__fadeInUp animate__delay-2s">
                        <button class="primary-button px-8 py-3 rounded-full font-semibold">
                            Get Started
                        </button>
                        <button class="secondary-button px-8 py-3 rounded-full font-semibold">
                            Learn More
                        </button>
                    </div>
                </div>
                <div class="md:w-1/2 animate__animated animate__fadeInRight">
                    <img src="https://placehold.co/600x400" alt="Tech Education" class="rounded-lg shadow-2xl">
                </div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="py-12 md:py-20">
        <div class="max-w-7xl mx-auto px-4">
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4 md:gap-8">
                <div class="stats-card slide-up">
                    <h3 class="text-3xl md:text-4xl font-bold text-[var(--accent)] mb-2">500+</h3>
                    <p class="text-sm md:text-base text-[var(--text-secondary)]">Graduates</p>
                </div>
                <div class="stats-card slide-up" style="animation-delay: 0.2s;">
                    <h3 class="text-3xl md:text-4xl font-bold text-[var(--accent)] mb-2">95%</h3>
                    <p class="text-sm md:text-base text-[var(--text-secondary)]">Employment Rate</p>
                </div>
                <div class="stats-card slide-up" style="animation-delay: 0.4s;">
                    <h3 class="text-3xl md:text-4xl font-bold text-[var(--accent)] mb-2">15+</h3>
                    <p class="text-sm md:text-base text-[var(--text-secondary)]">Industry Partners</p>
                </div>
                <div class="stats-card slide-up" style="animation-delay: 0.6s;">
                    <h3 class="text-3xl md:text-4xl font-bold text-[var(--accent)] mb-2">6</h3>
                    <p class="text-sm md:text-base text-[var(--text-secondary)]">Professional Courses</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="py-12 md:py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-12 gradient-text">Why Choose SmartValleyTech?</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-laptop-code text-xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-3">Practical Training</h3>
                    <p class="text-[var(--text-secondary)]">Hands-on experience with real-world projects and industry-standard tools.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-certificate text-xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-3">Certified Courses</h3>
                    <p class="text-[var(--text-secondary)]">Internationally recognized certifications to boost your career.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-users text-xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-3">Expert Instructors</h3>
                    <p class="text-[var(--text-secondary)]">Learn from industry professionals with years of experience.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Courses Section -->
    <section id="courses" class="py-12 md:py-20">
        <div class="max-w-7xl mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-12 gradient-text">Our Featured Courses</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Course Card 1 -->
                <div class="course-card">
                    <div class="course-image">
                        <img src="https://placehold.co/400x250" alt="Networking" class="w-full h-48 object-cover">
                        <div class="absolute top-4 right-4 bg-white px-3 py-1 rounded-full text-sm font-semibold text-[var(--accent)]">
                            Popular
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Computer Networking</h3>
                        <p class="text-[var(--text-secondary)] mb-4">Master network infrastructure, protocols, and security fundamentals.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-[var(--accent)] font-semibold">₦75,000</span>
                            <button class="primary-button px-4 py-2 rounded-full">Enroll Now</button>
                        </div>
                    </div>
                </div>

                <!-- Course Card 2 -->
                <div class="course-card">
                    <div class="course-image">
                        <img src="https://placehold.co/400x250" alt="Cybersecurity" class="w-full h-48 object-cover">
                        <div class="absolute top-4 right-4 bg-white px-3 py-1 rounded-full text-sm font-semibold text-[var(--accent)]">
                            New
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Cybersecurity</h3>
                        <p class="text-[var(--text-secondary)] mb-4">Learn advanced security techniques and threat prevention.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-[var(--accent)] font-semibold">₦90,000</span>
                            <button class="primary-button px-4 py-2 rounded-full">Enroll Now</button>
                        </div>
                    </div>
                </div>

                <!-- Course Card 3 -->
                <div class="course-card">
                    <div class="course-image">
                        <img src="https://placehold.co/400x250" alt="Database" class="w-full h-48 object-cover">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Database Management</h3>
                        <p class="text-[var(--text-secondary)] mb-4">Expert training in Oracle and Microsoft SQL databases.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-[var(--accent)] font-semibold">₦85,000</span>
                            <button class="primary-button px-4 py-2 rounded-full">Enroll Now</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="text-center mt-12">
                <button class="secondary-button px-8 py-3 rounded-full font-semibold text-[var(--accent)] border-[var(--accent)]">
                    View All Courses
                </button>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-12 md:py-20 bg-gradient-to-b from-[var(--background)] to-white">
        <div class="max-w-7xl mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 md:gap-12 items-center">
                <div class="space-y-6">
                    <h2 class="text-2xl md:text-3xl font-bold gradient-text">About SmartValleyTech Academy</h2>
                    <p class="text-[var(--text-secondary)] leading-relaxed">
                        Founded with a vision to bridge the tech talent gap in Nigeria, SmartValleyTech Academy has emerged as a leading technology education institution. We specialize in providing hands-on, industry-relevant training that transforms beginners into skilled tech professionals.
                    </p>
                    <div class="space-y-4">
                        <div class="feature-item">
                            <i class="fas fa-check-circle text-[var(--accent)] text-xl mr-3"></i>
                            <div>
                                <h4 class="font-semibold">Industry Expert Instructors</h4>
                                <p class="text-sm text-[var(--text-secondary)]">Learn from professionals with real-world experience</p>
                            </div>
                        </div>
                        <div class="feature-item">
                            <i class="fas fa-laptop-code text-[var(--accent)] text-xl mr-3"></i>
                            <div>
                                <h4 class="font-semibold">Hands-on Training</h4>
                                <p class="text-sm text-[var(--text-secondary)]">Practice with real projects and case studies</p>
                            </div>
                        </div>
                        <div class="feature-item">
                            <i class="fas fa-certificate text-[var(--accent)] text-xl mr-3"></i>
                            <div>
                                <h4 class="font-semibold">Industry Certification</h4>
                                <p class="text-sm text-[var(--text-secondary)]">Get certified and ready for the job market</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-4">
                    <img src="https://placehold.co/300x400" alt="Training" class="rounded-lg shadow-lg">
                    <img src="https://placehold.co/300x400" alt="Students" class="rounded-lg shadow-lg mt-8">
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="py-12 md:py-20 bg-gradient-to-b from-white to-[var(--background)]">
        <div class="max-w-7xl mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-12 gradient-text">Student Success Stories</h2>
            <div class="swiper-container">
                <div class="swiper-wrapper">
                    <div class="swiper-slide">
                        <div class="testimonial-card">
                            <div class="flex items-center mb-4">
                                <img src="https://placehold.co/60x60" alt="Student" class="rounded-full w-12 h-12">
                                <div class="ml-4">
                                    <h4 class="font-semibold">Chioma Okafor</h4>
                                    <p class="text-sm text-[var(--text-secondary)]">Cybersecurity Graduate</p>
                                </div>
                            </div>
                            <p class="text-[var(--text-secondary)]">"The practical approach to learning at SmartValleyTech transformed my career. I'm now working as a Security Analyst at a major bank."</p>
                        </div>
                    </div>
                    <div class="swiper-slide">
                        <div class="testimonial-card">
                            <div class="flex items-center mb-4">
                                <img src="https://placehold.co/60x60" alt="Student" class="rounded-full w-12 h-12">
                                <div class="ml-4">
                                    <h4 class="font-semibold">Oluwaseun Adebayo</h4>
                                    <p class="text-sm text-[var(--text-secondary)]">Network Engineer</p>
                                </div>
                            </div>
                            <p class="text-[var(--text-secondary)]">"The networking course provided me with hands-on experience that made me stand out in job interviews. Highly recommended!"</p>
                        </div>
                    </div>
                    <div class="swiper-slide">
                        <div class="testimonial-card">
                            <div class="flex items-center mb-4">
                                <img src="https://placehold.co/60x60" alt="Student" class="rounded-full w-12 h-12">
                                <div class="ml-4">
                                    <h4 class="font-semibold">Amina Ibrahim</h4>
                                    <p class="text-sm text-[var(--text-secondary)]">Database Administrator</p>
                                </div>
                            </div>
                            <p class="text-[var(--text-secondary)]">"The database management course was comprehensive and practical. I secured a job even before completing the program."</p>
                        </div>
                    </div>
                </div>
                <div class="swiper-pagination"></div>
                <div class="swiper-button-next"></div>
                <div class="swiper-button-prev"></div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-12 md:py-20">
        <div class="max-w-3xl mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-12 gradient-text">Start Your Journey Today</h2>
            <form class="bg-white p-8 rounded-xl shadow-lg">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div>
                        <label class="block text-[var(--text-primary)] mb-2">First Name</label>
                        <input type="text" class="custom-input w-full px-4 py-2 border rounded-lg focus:outline-none" required>
                    </div>
                    <div>
                        <label class="block text-[var(--text-primary)] mb-2">Last Name</label>
                        <input type="text" class="custom-input w-full px-4 py-2 border rounded-lg focus:outline-none" required>
                    </div>
                    <div>
                        <label class="block text-[var(--text-primary)] mb-2">Email</label>
                        <input type="email" class="custom-input w-full px-4 py-2 border rounded-lg focus:outline-none" required>
                    </div>
                    <div>
                        <label class="block text-[var(--text-primary)] mb-2">Phone</label>
                        <input type="tel" class="custom-input w-full px-4 py-2 border rounded-lg focus:outline-none" required>
                    </div>
                    <div class="md:col-span-2">
                        <label class="block text-[var(--text-primary)] mb-2">Course Interest</label>
                        <select class="custom-input w-full px-4 py-2 border rounded-lg focus:outline-none" required>
                            <option value="">Select a course</option>
                            <option>Computer Networking</option>
                            <option>Cybersecurity</option>
                            <option>Database Management</option>
                            <option>AI Graphics Design</option>
                            <option>Ethical Hacking</option>
                        </select>
                    </div>
                    <div class="md:col-span-2">
                        <label class="block text-[var(--text-primary)] mb-2">Message (Optional)</label>
                        <textarea class="custom-input w-full px-4 py-2 border rounded-lg focus:outline-none h-32 resize-none"></textarea>
                    </div>
                </div>
                <button type="submit" class="primary-button w-full py-3 rounded-lg mt-6 relative">
                    <span class="button-text">Submit Application</span>
                    <div class="spinner absolute inset-0 m-auto" style="display: none;"></div>
                </button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-[var(--primary)] text-white py-12">
        <div class="max-w-7xl mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">SmartValleyTech</h3>
                    <p class="text-gray-300">Empowering Nigerian tech professionals with world-class education.</p>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#about" class="text-gray-300 hover:text-white transition">About Us</a></li>
                        <li><a href="#courses" class="text-gray-300 hover:text-white transition">Courses</a></li>
                        <li><a href="#contact" class="text-gray-300 hover:text-white transition">Contact</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition">Privacy Policy</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Contact Info</h4>
                    <ul class="space-y-2">
                        <li><i class="fas fa-map-marker-alt mr-2"></i> Lagos, Nigeria</li>
                        <li><i class="fas fa-phone mr-2"></i> +234 123 456 7890</li>
                        <li><i class="fas fa-envelope mr-2"></i> info@smartvalleytech.com</li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Follow Us</h4>
                    <div class="flex space-x-4">
                        <a href="#" class="hover:text-[var(--highlight)] transition"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="hover:text-[var(--highlight)] transition"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="hover:text-[var(--highlight)] transition"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#" class="hover:text-[var(--highlight)] transition"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-8 text-center">
                <p class="text-gray-300">&copy; 2024 SmartValleyTech Academy. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const mobileMenuButton = document.querySelector('.mobile-menu-button');
        const mobileMenu = document.querySelector('.mobile-menu');
        let isMenuOpen = false;

        function toggleMenu() {
            isMenuOpen = !isMenuOpen;
            mobileMenu.classList.toggle('active');
            const icon = mobileMenuButton.querySelector('i');
            icon.classList.toggle('fa-bars');
            icon.classList.toggle('fa-times');
            
            if (isMenuOpen) {
                document.body.style.overflow = 'hidden';
            } else {
                document.body.style.overflow = '';
            }
        }

        mobileMenuButton.addEventListener('click', toggleMenu);

        // Close menu on link click
        document.querySelectorAll('.mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                if (isMenuOpen) toggleMenu();
            });
        });

        // Testimonials Slider
        const swiper = new Swiper('.swiper-container', {
            slidesPerView: 1,
            spaceBetween: 30,
            loop: true,
            autoplay: {
                delay: 3000,
                disableOnInteraction: false,
            },
            pagination: {
                el: '.swiper-pagination',
                clickable: true,
            },
            navigation: {
                nextEl: '.swiper-button-next',
                prevEl: '.swiper-button-prev',
            },
            breakpoints: {
                640: {
                    slidesPerView: 1,
                },
                768: {
                    slidesPerView: 2,
                },
                1024: {
                    slidesPerView: 3,
                },
            }
        });

        // Form Validation and Submission
        const form = document.querySelector('form');
        const inputs = form.querySelectorAll('input, select, textarea');

        form.addEventListener('submit', async (e) => {
            e.preventDefault();
            let isValid = true;

            inputs.forEach(input => {
                if (input.required && !input.value.trim()) {
                    isValid = false;
                    input.classList.add('error');
                } else {
                    input.classList.remove('error');
                }
            });

            if (isValid) {
                const submitButton = form.querySelector('button[type="submit"]');
                const buttonText = submitButton.querySelector('.button-text');
                const spinner = submitButton.querySelector('.spinner');
                
                // Show loading state
                buttonText.style.opacity = '0';
                spinner.style.display = 'block';
                submitButton.disabled = true;

                // Simulate form submission
                await new Promise(resolve => setTimeout(resolve, 2000));

                // Show success state
                buttonText.textContent = 'Application Submitted!';
                buttonText.style.opacity = '1';
                spinner.style.display = 'none';
                submitButton.style.background = '#48BB78';

                // Reset form after delay
                setTimeout(() => {
                    form.reset();
                    buttonText.textContent = 'Submit Application';
                    submitButton.style.background = '';
                    submitButton.disabled = false;
                }, 3000);
            }
        });

        // Remove error class on input
        inputs.forEach(input => {
            input.addEventListener('input', () => {
                if (input.value.trim()) {
                    input.classList.remove('error');
                }
            });
        });

        // Smooth Scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    const headerOffset = 80;
