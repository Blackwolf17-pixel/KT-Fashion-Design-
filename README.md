# KT-Fashion-Design-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KT Fashion Design - Tigray</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700&family=Inter:wght@300;400;500;600&display=swap');
        
        .font-playfair { font-family: 'Playfair Display', serif; }
        .font-inter { font-family: 'Inter', sans-serif; }
        
        .hero-gradient {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .card-hover {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .fade-in {
            animation: fadeIn 0.8s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body class="font-inter bg-gray-50">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg fixed w-full top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <h1 class="font-playfair text-2xl font-bold text-gray-800">KT Fashion Design</h1>
                    <span class="ml-2 text-sm text-purple-600 font-medium">Tigray</span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="text-gray-700 hover:text-purple-600 transition-colors">Home</a>
                    <a href="#collections" class="text-gray-700 hover:text-purple-600 transition-colors">Collections</a>
                    <a href="#services" class="text-gray-700 hover:text-purple-600 transition-colors">Services</a>
                    <a href="#about" class="text-gray-700 hover:text-purple-600 transition-colors">About</a>
                    <a href="#contact" class="text-gray-700 hover:text-purple-600 transition-colors">Contact</a>
                </div>
                <button class="md:hidden text-gray-700" onclick="toggleMenu()">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t">
            <div class="px-2 pt-2 pb-3 space-y-1">
                <a href="#home" class="block px-3 py-2 text-gray-700 hover:text-purple-600">Home</a>
                <a href="#collections" class="block px-3 py-2 text-gray-700 hover:text-purple-600">Collections</a>
                <a href="#services" class="block px-3 py-2 text-gray-700 hover:text-purple-600">Services</a>
                <a href="#about" class="block px-3 py-2 text-gray-700 hover:text-purple-600">About</a>
                <a href="#contact" class="block px-3 py-2 text-gray-700 hover:text-purple-600">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-gradient text-white pt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20">
            <div class="text-center fade-in">
                <h2 class="font-playfair text-5xl md:text-6xl font-bold mb-6">Elegant Fashion Design</h2>
                <p class="text-xl md:text-2xl mb-8 text-purple-100">Crafting beautiful, authentic designs in the heart of Tigray</p>
                <div class="space-x-4">
                    <button onclick="scrollToSection('collections')" class="bg-white text-purple-600 px-8 py-3 rounded-full font-semibold hover:bg-purple-50 transition-colors">
                        View Collections
                    </button>
                    <button onclick="scrollToSection('contact')" class="border-2 border-white text-white px-8 py-3 rounded-full font-semibold hover:bg-white hover:text-purple-600 transition-colors">
                        Get in Touch
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Collections Section -->
    <section id="collections" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h3 class="font-playfair text-4xl font-bold text-gray-800 mb-4">Our Collections</h3>
                <p class="text-lg text-gray-600 max-w-2xl mx-auto">Discover our latest fashion collections, blending traditional Tigrayan aesthetics with contemporary design</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="card-hover bg-gray-50 rounded-lg overflow-hidden">
                    <div class="h-64 bg-gradient-to-br from-pink-400 to-purple-500 flex items-center justify-center">
                        <div class="text-center text-white">
                            <svg class="w-16 h-16 mx-auto mb-4" fill="currentColor" viewBox="0 0 20 20">
                                <path d="M3 4a1 1 0 011-1h12a1 1 0 011 1v2a1 1 0 01-1 1H4a1 1 0 01-1-1V4zM3 10a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H4a1 1 0 01-1-1v-6zM14 9a1 1 0 00-1 1v6a1 1 0 001 1h2a1 1 0 001-1v-6a1 1 0 00-1-1h-2z"/>
                            </svg>
                            <h4 class="text-xl font-semibold">Traditional Wear</h4>
                        </div>
                    </div>
                    <div class="p-6">
                        <h4 class="font-playfair text-xl font-semibold mb-2">Traditional Collection</h4>
                        <p class="text-gray-600 mb-4">Authentic Tigrayan traditional clothing with modern touches</p>
                        <button class="text-purple-600 font-semibold hover:text-purple-800 transition-colors">Explore →</button>
                    </div>
                </div>

                <div class="card-hover bg-gray-50 rounded-lg overflow-hidden">
                    <div class="h-64 bg-gradient-to-br from-blue-400 to-indigo-500 flex items-center justify-center">
                        <div class="text-center text-white">
                            <svg class="w-16 h-16 mx-auto mb-4" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM7 9a1 1 0 100-2 1 1 0 000 2zM14 9a1 1 0 11-2 0 1 1 0 012 0zm-7 3a1 1 0 011-1h4a1 1 0 110 2H8a1 1 0 01-1-1z" clip-rule="evenodd"/>
                            </svg>
                            <h4 class="text-xl font-semibold">Contemporary</h4>
                        </div>
                    </div>
                    <div class="p-6">
                        <h4 class="font-playfair text-xl font-semibold mb-2">Contemporary Line</h4>
                        <p class="text-gray-600 mb-4">Modern fashion with Ethiopian cultural influences</p>
                        <button class="text-purple-600 font-semibold hover:text-purple-800 transition-colors">Explore →</button>
                    </div>
                </div>

                <div class="card-hover bg-gray-50 rounded-lg overflow-hidden">
                    <div class="h-64 bg-gradient-to-br from-green-400 to-teal-500 flex items-center justify-center">
                        <div class="text-center text-white">
                            <svg class="w-16 h-16 mx-auto mb-4" fill="currentColor" viewBox="0 0 20 20">
                                <path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/>
                            </svg>
                            <h4 class="text-xl font-semibold">Custom Design</h4>
                        </div>
                    </div>
                    <div class="p-6">
                        <h4 class="font-playfair text-xl font-semibold mb-2">Custom Designs</h4>
                        <p class="text-gray-600 mb-4">Bespoke fashion tailored to your unique style</p>
                        <button class="text-purple-600 font-semibold hover:text-purple-800 transition-colors">Explore →</button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h3 class="font-playfair text-4xl font-bold text-gray-800 mb-4">Our Services</h3>
                <p class="text-lg text-gray-600 max-w-2xl mx-auto">From concept to creation, we offer comprehensive fashion design services</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="text-center">
                    <div class="w-16 h-16 bg-purple-100 rounded-full flex items-center justify-center mx-auto mb-4">
                        <svg class="w-8 h-8 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
                            <path d="M13.586 3.586a2 2 0 112.828 2.828l-.793.793-2.828-2.828.793-.793zM11.379 5.793L3 14.172V17h2.828l8.38-8.379-2.83-2.828z"/>
                        </svg>
                    </div>
                    <h4 class="font-semibold text-lg mb-2">Design Consultation</h4>
                    <p class="text-gray-600">Personalized design sessions to bring your vision to life</p>
                </div>

                <div class="text-center">
                    <div class="w-16 h-16 bg-purple-100 rounded-full flex items-center justify-center mx-auto mb-4">
                        <svg class="w-8 h-8 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
                            <path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"/>
                        </svg>
                    </div>
                    <h4 class="font-semibold text-lg mb-2">Custom Tailoring</h4>
                    <p class="text-gray-600">Expert tailoring services for the perfect fit</p>
                </div>

                <div class="text-center">
                    <div class="w-16 h-16 bg-purple-100 rounded-full flex items-center justify-center mx-auto mb-4">
                        <svg class="w-8 h-8 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
                            <path d="M3 4a1 1 0 011-1h12a1 1 0 011 1v2a1 1 0 01-1 1H4a1 1 0 01-1-1V4zM3 10a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H4a1 1 0 01-1-1v-6zM14 9a1 1 0 00-1 1v6a1 1 0 001 1h2a1 1 0 001-1v-6a1 1 0 00-1-1h-2z"/>
                        </svg>
                    </div>
                    <h4 class="font-semibold text-lg mb-2">Alterations</h4>
                    <p class="text-gray-600">Professional alterations and adjustments</p>
                </div>

                <div class="text-center">
                    <div class="w-16 h-16 bg-purple-100 rounded-full flex items-center justify-center mx-auto mb-4">
                        <svg class="w-8 h-8 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                        </svg>
                    </div>
                    <h4 class="font-semibold text-lg mb-2">Fashion Styling</h4>
                    <p class="text-gray-600">Complete styling services for any occasion</p>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid lg:grid-cols-2 gap-12 items-center">
                <div>
                    <h3 class="font-playfair text-4xl font-bold text-gray-800 mb-6">About KT Fashion Design</h3>
                    <p class="text-lg text-gray-600 mb-6">
                        Based in the beautiful region of Tigray, KT Fashion Design is dedicated to creating exceptional fashion that celebrates both traditional Ethiopian heritage and contemporary style. Our passion lies in crafting unique pieces that tell stories and express individuality.
                    </p>
                    <p class="text-lg text-gray-600 mb-8">
                        With years of experience in fashion design and a deep appreciation for Tigrayan culture, we bring authenticity and innovation to every piece we create. From traditional ceremonial wear to modern everyday fashion, we ensure quality and attention to detail in all our work.
                    </p>
                    <div class="flex space-x-8">
                        <div class="text-center">
                            <div class="text-3xl font-bold text-purple-600">5+</div>
                            <div class="text-gray-600">Years Experience</div>
                        </div>
                        <div class="text-center">
                            <div class="text-3xl font-bold text-purple-600">200+</div>
                            <div class="text-gray-600">Happy Clients</div>
                        </div>
                        <div class="text-center">
                            <div class="text-3xl font-bold text-purple-600">50+</div>
                            <div class="text-gray-600">Unique Designs</div>
                        </div>
                    </div>
                </div>
                <div class="bg-gradient-to-br from-purple-400 to-pink-400 rounded-lg h-96 flex items-center justify-center">
                    <div class="text-center text-white">
                        <svg class="w-24 h-24 mx-auto mb-4" fill="currentColor" viewBox="0 0 20 20">
                            <path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/>
                        </svg>
                        <h4 class="text-2xl font-semibold">Quality Craftsmanship</h4>
                        <p class="mt-2">Every piece is made with care and attention to detail</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h3 class="font-playfair text-4xl font-bold text-gray-800 mb-4">Get in Touch</h3>
                <p class="text-lg text-gray-600 max-w-2xl mx-auto">Ready to create something beautiful together? Contact us to discuss your fashion needs</p>
            </div>
            
            <div class="grid lg:grid-cols-2 gap-12">
                <div>
                    <div class="bg-white rounded-lg p-8 shadow-lg">
                        <h4 class="font-playfair text-2xl font-semibold mb-6">Contact Information</h4>
                        
                        <div class="space-y-4">
                            <div class="flex items-center">
                                <div class="w-10 h-10 bg-purple-100 rounded-full flex items-center justify-center mr-4">
                                    <svg class="w-5 h-5 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
                                        <path fill-rule="evenodd" d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a2 2 0 100-4 2 2 0 000 4z" clip-rule="evenodd"/>
                                    </svg>
                                </div>
                                <div>
                                    <div class="font-semibold">Location</div>
                                    <div class="text-gray-600">Tigray, Ethiopia</div>
                                </div>
                            </div>
                            
                            <div class="flex items-center">
                                <div class="w-10 h-10 bg-purple-100 rounded-full flex items-center justify-center mr-4">
                                    <svg class="w-5 h-5 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
                                        <path d="M2 3a1 1 0 011-1h2.153a1 1 0 01.986.836l.74 4.435a1 1 0 01-.54 1.06l-1.548.773a11.037 11.037 0 006.105 6.105l.774-1.548a1 1 0 011.059-.54l4.435.74a1 1 0 01.836.986V17a1 1 0 01-1 1h-2C7.82 18 2 12.18 2 5V3z"/>
                                    </svg>
                                </div>
                                <div>
                                    <div class="font-semibold">Phone</div>
                                    <div class="text-gray-600">+251 XXX XXX XXX</div>
                                </div>
                            </div>
                            
                            <div class="flex items-center">
                                <div class="w-10 h-10 bg-purple-100 rounded-full flex items-center justify-center mr-4">
                                    <svg class="w-5 h-5 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
                                        <path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z"/>
                                        <path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z"/>
                                    </svg>
                                </div>
                                <div>
                                    <div class="font-semibold">Email</div>
                                    <div class="text-gray-600">info@ktfashiondesign.com</div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-8">
                            <h5 class="font-semibold mb-4">Business Hours</h5>
                            <div class="space-y-2 text-gray-600">
                                <div class="flex justify-between">
                                    <span>Monday - Friday</span>
                                    <span>9:00 AM - 6:00 PM</span>
                                </div>
                                <div class="flex justify-between">
                                    <span>Saturday</span>
                                    <span>10:00 AM - 4:00 PM</span>
                                </div>
                                <div class="flex justify-between">
                                    <span>Sunday</span>
                                    <span>Closed</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg p-8 shadow-lg">
                    <h4 class="font-playfair text-2xl font-semibold mb-6">Send us a Message</h4>
                    <div class="bg-yellow-50 border border-yellow-200 rounded-lg p-4 mb-6">
                        <div class="flex items-center">
                            <svg class="w-5 h-5 text-yellow-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M8.257 3.099c.765-1.36 2.722-1.36 3.486 0l5.58 9.92c.75 1.334-.213 2.98-1.742 2.98H4.42c-1.53 0-2.493-1.646-1.743-2.98l5.58-9.92zM11 13a1 1 0 11-2 0 1 1 0 012 0zm-1-8a1 1 0 00-1 1v3a1 1 0 002 0V6a1 1 0 00-1-1z" clip-rule="evenodd"/>
                            </svg>
     
