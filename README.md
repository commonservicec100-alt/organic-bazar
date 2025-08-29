<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>অর্গানিক ফ্রেশ - তাজা সবজি হোম ডেলিভারি</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts for "Inter" font -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7fdee;
            color: #2c5234;
        }

        /* Custom styles for the slider */
        .slider-container {
            overflow: hidden;
        }
        .slider-wrapper {
            display: flex;
            transition: transform 0.5s ease-in-out;
        }
        .testimonial-card {
            min-width: 100%; /* Each card takes up the full width */
        }

        @media (min-width: 768px) {
            .testimonial-card {
                min-width: calc(33.333% - 1.5rem); /* For desktop, show 3 cards */
            }
        }
    </style>
</head>
<body class="bg-gray-50">

    <!-- Header Section -->
    <header class="bg-white shadow-sm sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-4 flex flex-col md:flex-row items-center justify-between">
            <!-- Logo and Desktop Menu Wrapper -->
            <div class="flex items-center justify-between w-full md:w-auto mb-4 md:mb-0">
                <!-- Logo -->
                <a href="#" class="flex items-center space-x-2">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-green-600" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 16c-3.31 0-6-2.69-6-6s2.69-6 6-6 6 2.69 6 6-2.69 6-6 6z"/><path d="M12 18a6 6 0 1 0 0-12 6 6 0 0 0 0 12zM12 12a2 2 0 1 0 0-4 2 2 0 0 0 0 4z"/></svg>
                    <span class="text-xl md:text-2xl font-bold text-green-700">অর্গানিক ফ্রেশ</span>
                </a>
                <!-- Mobile Menu and Cart Icon -->
                <div class="flex items-center space-x-4 md:hidden">
                    <a href="#" class="relative">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-600" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="9" cy="21" r="1"/><circle cx="20" cy="21" r="1"/><path d="M1 1h4l2.68 12.56a2 2 0 0 0 1.96 1.44H19a2 2 0 0 0 1.96-1.44L23 6H6"/></svg>
                        <span class="absolute -top-1 -right-1 bg-red-500 text-white text-xs font-bold rounded-full h-4 w-4 flex items-center justify-center">0</span>
                    </a>
                </div>
            </div>

            <!-- Search Bar (Added as requested) -->
            <div class="relative w-full md:w-1/3 mx-auto md:mx-0">
                <input type="text" placeholder="পণ্য খুঁজুন..." class="w-full pl-10 pr-4 py-2 rounded-full border border-gray-300 focus:outline-none focus:ring-2 focus:ring-green-500 transition-shadow">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 absolute left-3 top-1/2 -translate-y-1/2 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="11" cy="11" r="8"/><line x1="21" y1="21" x2="16.65" y2="16.65"/></svg>
            </div>

            <!-- Desktop Menu -->
            <div class="hidden md:flex items-center space-x-8 mt-4 md:mt-0">
                <a href="#products" class="text-gray-600 hover:text-green-600 font-medium transition-colors">পণ্য</a>
                <a href="#subscriptions" class="text-gray-600 hover:text-green-600 font-medium transition-colors">সাবস্ক্রিপশন</a>
                <a href="#customers" class="text-gray-600 hover:text-green-600 font-medium transition-colors">গ্রাহক</a>
                <a href="#contact" class="text-gray-600 hover:text-green-600 font-medium transition-colors">যোগাযোগ</a>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <main>
        <section class="relative bg-white pt-16 pb-20 md:pt-24 md:pb-32 overflow-hidden">
            <div class="container mx-auto px-6 flex flex-col md:flex-row items-center justify-between">
                <!-- Text Content -->
                <div class="md:w-1/2 text-center md:text-left mb-10 md:mb-0">
                    <h1 class="text-3xl md:text-5xl lg:text-6xl font-extrabold text-green-800 leading-tight mb-4">
                        সরাসরি খামার থেকে, <br> আপনার দোরগোড়ায়
                    </h1>
                    <p class="text-lg md:text-xl text-gray-600 mb-8">
                        সবজি, ফল ও কাঁচামাল— ভেজালমুক্ত, তাজা এবং অর্গানিক।
                    </p>
                    <button class="bg-green-600 text-white font-semibold py-3 px-8 rounded-full shadow-lg hover:bg-green-700 transition-transform transform hover:scale-105 focus:outline-none focus:ring-2 focus:ring-green-500 focus:ring-offset-2">
                        অর্ডার করুন
                    </button>
                </div>
                <!-- Image -->
                <div class="md:w-1/2 flex justify-center">
                    <img src="https://placehold.co/600x400/D4EDD7/38743d?text=Organic+Products" alt="Organic Fresh Products" class="rounded-3xl shadow-2xl transform transition-transform hover:scale-105 duration-300">
                </div>
            </div>
        </section>

        <!-- Product Categories Section -->
        <section id="products" class="py-16 md:py-24 bg-green-50">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-3xl md:text-4xl font-bold text-green-800 mb-4">আমাদের পণ্য</h2>
                <p class="text-gray-600 text-lg mb-12">আপনার স্বাস্থ্যকর জীবনের জন্য সেরা অর্গানিক পণ্যগুলো বেছে নিন।</p>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                    <!-- Product Category Card 1 -->
                    <div class="bg-white rounded-2xl shadow-lg p-6 flex flex-col items-center transform transition-transform hover:scale-105 duration-300">
                        <img src="https://placehold.co/150x150/dcf8e5/5d9471?text=Vegetables" alt="Vegetables" class="w-24 h-24 mb-4 rounded-full">
                        <h3 class="text-xl font-bold text-green-700 mb-2">সবজি</h3>
                        <p class="text-gray-500 text-center">টাটকা ও বিষমুক্ত সবজি</p>
                    </div>
                    <!-- Product Category Card 2 -->
                    <div class="bg-white rounded-2xl shadow-lg p-6 flex flex-col items-center transform transition-transform hover:scale-105 duration-300">
                        <img src="https://placehold.co/150x150/dcf8e5/5d9471?text=Fruits" alt="Fruits" class="w-24 h-24 mb-4 rounded-full">
                        <h3 class="text-xl font-bold text-green-700 mb-2">ফল</h3>
                        <p class="text-gray-500 text-center">মৌসুমি ও রসালো ফল</p>
                    </div>
                    <!-- Product Category Card 3 -->
                    <div class="bg-white rounded-2xl shadow-lg p-6 flex flex-col items-center transform transition-transform hover:scale-105 duration-300">
                        <img src="https://placehold.co/150x150/dcf8e5/5d9471?text=Pulses" alt="Pulses" class="w-24 h-24 mb-4 rounded-full">
                        <h3 class="text-xl font-bold text-green-700 mb-2">ডাল ও চাল</h3>
                        <p class="text-gray-500 text-center">উচ্চ মানের ডাল ও চাল</p>
                    </div>
                    <!-- Product Category Card 4 -->
                    <div class="bg-white rounded-2xl shadow-lg p-6 flex flex-col items-center transform transition-transform hover:scale-105 duration-300">
                        <img src="https://placehold.co/150x150/dcf8e5/5d9471?text=Others" alt="Others" class="w-24 h-24 mb-4 rounded-full">
                        <h3 class="text-xl font-bold text-green-700 mb-2">অন্যান্য</h3>
                        <p class="text-gray-500 text-center">ডিম ও অন্যান্য কাঁচামাল</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Subscription Section -->
        <section id="subscriptions" class="py-16 md:py-24 bg-white">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-3xl md:text-4xl font-bold text-green-800 mb-4">আমাদের সাবস্ক্রিপশন প্যাকেজ</h2>
                <p class="text-gray-600 text-lg mb-12">আপনার প্রয়োজন অনুযায়ী বেছে নিন।</p>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
                    <!-- Weekly Package Card -->
                    <div class="bg-green-50 rounded-3xl shadow-xl p-8 transform transition-transform hover:scale-105 duration-300">
                        <h3 class="text-2xl font-bold text-green-800 mb-2">সাপ্তাহিক প্যাকেজ</h3>
                        <p class="text-gray-500 mb-6">সপ্তাহে ৩ দিন ডেলিভারি</p>
                        <ul class="text-left space-y-3 mb-8">
                            <li class="flex items-center space-x-2 text-green-700">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6L9 17l-5-5"/></svg>
                                <span>৩ দিনের তাজা সবজি</span>
                            </li>
                            <li class="flex items-center space-x-2 text-green-700">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6L9 17l-5-5"/></svg>
                                <span>সুবিধা ও সময় সাশ্রয়</span>
                            </li>
                            <li class="flex items-center space-x-2 text-green-700">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6L9 17l-5-5"/></svg>
                                <span>বিশেষ ছাড়</span>
                            </li>
                        </ul>
                        <button class="w-full bg-green-600 text-white font-semibold py-3 px-8 rounded-full shadow-lg hover:bg-green-700 transition-transform transform hover:scale-105">
                            সাবস্ক্রাইব করুন
                        </button>
                    </div>

                    <!-- Daily Package Card -->
                    <div class="bg-green-50 rounded-3xl shadow-xl p-8 transform transition-transform hover:scale-105 duration-300">
                        <h3 class="text-2xl font-bold text-green-800 mb-2">দৈনিক প্যাকেজ</h3>
                        <p class="text-gray-500 mb-6">প্রতিদিন তাজা সবজি</p>
                        <ul class="text-left space-y-3 mb-8">
                            <li class="flex items-center space-x-2 text-green-700">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6L9 17l-5-5"/></svg>
                                <span>প্রতিদিন তাজা সবজি ও ফল</span>
                            </li>
                            <li class="flex items-center space-x-2 text-green-700">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6L9 17l-5-5"/></svg>
                                <span>সকাল ৭টায় ডেলিভারি</span>
                            </li>
                            <li class="flex items-center space-x-2 text-green-700">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6L9 17l-5-5"/></svg>
                                <span>কাস্টমাইজড প্যাকেজ</span>
                            </li>
                        </ul>
                        <button class="w-full bg-green-600 text-white font-semibold py-3 px-8 rounded-full shadow-lg hover:bg-green-700 transition-transform transform hover:scale-105">
                            সাবস্ক্রাইব করুন
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Customer Testimonials Section -->
        <section id="customers" class="py-16 md:py-24 bg-green-50">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-3xl md:text-4xl font-bold text-green-800 mb-4">আমাদের সম্মানিত গ্রাহক</h2>
                <p class="text-gray-600 text-lg mb-12">আমাদের গ্রাহকদের কিছু অভিজ্ঞতা</p>
                
                <!-- Slider Container -->
                <div class="relative w-full max-w-4xl mx-auto">
                    <!-- Slider Navigation Buttons -->
                    <button id="prevBtn" class="absolute left-0 top-1/2 -translate-y-1/2 bg-white rounded-full p-2 shadow-lg hover:bg-gray-200 transition-colors z-10">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-600" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="15 18 9 12 15 6"/></svg>
                    </button>
                    <button id="nextBtn" class="absolute right-0 top-1/2 -translate-y-1/2 bg-white rounded-full p-2 shadow-lg hover:bg-gray-200 transition-colors z-10">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-600" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="9 18 15 12 9 6"/></svg>
                    </button>

                    <!-- Slider Wrapper -->
                    <div class="slider-container">
                        <div class="slider-wrapper">
                            <!-- Testimonial Card 1 -->
                            <div class="testimonial-card flex-shrink-0 p-4">
                                <div class="bg-white rounded-2xl shadow-lg p-6 flex flex-col items-center h-full">
                                    <img src="https://placehold.co/100x100/A8D1B2/38743d?text=User1" alt="গ্রাহক ১" class="w-24 h-24 rounded-full mb-4">
                                    <h3 class="text-xl font-bold text-green-700 mb-2">তানিয়া আহমেদ</h3>
                                    <p class="text-gray-500 text-center italic">"অর্গানিক ফ্রেশের সবজিগুলো সত্যিই টাটকা। ডেলিভারিও সময়মতো হয়। আমি খুবই সন্তুষ্ট।"</p>
                                </div>
                            </div>
                            <!-- Testimonial Card 2 -->
                            <div class="testimonial-card flex-shrink-0 p-4">
                                <div class="bg-white rounded-2xl shadow-lg p-6 flex flex-col items-center h-full">
                                    <img src="https://placehold.co/100x100/A8D1B2/38743d?text=User2" alt="গ্রাহক ২" class="w-24 h-24 rounded-full mb-4">
                                    <h3 class="text-xl font-bold text-green-700 mb-2">রহিম চৌধুরী</h3>
                                    <p class="text-gray-500 text-center italic">"তাদের সাবস্ক্রিপশন সার্ভিসটি আমার জন্য খুবই সুবিধাজনক। প্রতি সপ্তাহে বাজার করার ঝামেলা থেকে মুক্তি পেয়েছি।"</p>
                                </div>
                            </div>
                            <!-- Testimonial Card 3 -->
                            <div class="testimonial-card flex-shrink-0 p-4">
                                <div class="bg-white rounded-2xl shadow-lg p-6 flex flex-col items-center h-full">
                                    <img src="https://placehold.co/100x100/A8D1B2/38743d?text=User3" alt="গ্রাহক ৩" class="w-24 h-24 rounded-full mb-4">
                                    <h3 class="text-xl font-bold text-green-700 mb-2">ফারজানা বেগম</h3>
                                    <p class="text-gray-500 text-center italic">"আমি সবসময় অর্গানিক পণ্য খুঁজি। এই অ্যাপটি আমার সেই চাহিদা পূরণ করেছে। দামও সাশ্রয়ী।"</p>
                                </div>
                            </div>
                            <!-- You can add more cards here for the slider -->
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer id="contact" class="bg-white py-12">
        <div class="container mx-auto px-6 text-center">
            <h3 class="text-2xl font-bold text-green-800 mb-4">যোগাযোগ</h3>
            <p class="text-gray-600 mb-6">আমাদের সাথে যুক্ত থাকুন</p>
            <div class="flex items-center justify-center space-x-6 mb-6">
                <!-- Facebook Icon -->
                <a href="#" class="text-gray-600 hover:text-green-600 transition-colors">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"/></svg>
                </a>
                <!-- Instagram Icon -->
                <a href="#" class="text-gray-600 hover:text-green-600 transition-colors">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/></svg>
                </a>
                <!-- Twitter Icon -->
                <a href="#" class="text-gray-600 hover:text-green-600 transition-colors">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1a10.66 10.66 0 0 1-5.87-3.69 4.48 4.48 0 0 0 1.09 5.91 4.48 4.48 0 0 1-2.02-.56v.05a4.48 4.48 0 0 0 3.6 4.4 4.48 4.48 0 0 1-2.01.07 4.48 4.48 0 0 0 4.15 3.1 8.93 8.93 0 0 1-5.6 1.94 9.42 9.42 0 0 1-1.09-.06 12.72 12.72 0 0 0 6.84 2.02 12.72 12.72 0 0 0 6.84-2.02c.01-.01.02-.02.03-.03a12.72 12.72 0 0 0 6.84 2.02c.01-.01.02-.02.03-.03a12.72 12.72 0 0 0 6.84 2.02c.01-.01.02-.02.03-.03z"/></svg>
                </a>
            </div>
            <p class="text-gray-400 text-sm mt-8">&copy; 2024 অর্গানিক ফ্রেশ. সর্বস্বত্ব সংরক্ষিত।</p>
        </div>
    </footer>
    
    <script>
        const sliderWrapper = document.querySelector('.slider-wrapper');
        const prevBtn = document.getElementById('prevBtn');
        const nextBtn = document.getElementById('nextBtn');
        
        let currentIndex = 0;

        // Function to update the slider position
        function updateSlider() {
            // Calculate the translation value based on the current index
            const cards = document.querySelectorAll('.testimonial-card');
            // Adjust current index if it goes out of bounds
            if (currentIndex < 0) {
                currentIndex = 0;
            } else if (currentIndex >= cards.length) {
                currentIndex = cards.length - 1;
            }

            const offset = -currentIndex * 100;
            sliderWrapper.style.transform = `translateX(${offset}%)`;
        }

        // Event listener for the "Next" button
        nextBtn.addEventListener('click', () => {
            const cards = document.querySelectorAll('.testimonial-card');
            // Check if there are more cards to show
            if (currentIndex < cards.length - 1) {
                currentIndex++;
                updateSlider();
            }
        });

        // Event listener for the "Previous" button
        prevBtn.addEventListener('click', () => {
            // Check if we are not at the beginning
            if (currentIndex > 0) {
                currentIndex--;
                updateSlider();
            }
        });
        
        // This function adds touch events for mobile devices
        function setupTouchEvents() {
            let startX;
            let endX;

            sliderWrapper.addEventListener('touchstart', (e) => {
                startX = e.touches[0].clientX;
            });

            sliderWrapper.addEventListener('touchmove', (e) => {
                endX = e.touches[0].clientX;
            });

            sliderWrapper.addEventListener('touchend', () => {
                const diff = startX - endX;
                // Determine if it was a significant swipe left or right
                if (diff > 50) { // Swiped left
                    nextBtn.click();
                } else if (diff < -50) { // Swiped right
                    prevBtn.click();
                }
            });
        }
        
        // Setup touch events on page load
        window.addEventListener('load', setupTouchEvents);

    </script>
</body>
</html>
# organic-bazar
