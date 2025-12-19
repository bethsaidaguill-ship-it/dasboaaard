<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UGCVault - Never Chase Payments Again | Automated Payment Tracking for UGC Creators</title>
    <meta name="description" content="Stop losing money to late payments. UGCVault automatically tracks your deals, sends reminders, and ensures you get paid on time. Free until your first deal closes.">
    <script src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap');
        
        body {
            margin: 0;
            padding: 0;
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        }
        
        .gradient-text {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .feature-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .pulse-animation {
            animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
        }
        
        @keyframes pulse {
            0%, 100% {
                opacity: 1;
            }
            50% {
                opacity: .7;
            }
        }
        
        .demo-section {
            background: linear-gradient(to bottom, #f9fafb 0%, #ffffff 100%);
        }
        
        .stat-number {
            font-size: 3rem;
            font-weight: 900;
            line-height: 1;
        }
        
        @media (max-width: 640px) {
            .stat-number {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body class="antialiased">
    <!-- Navigation -->
    <nav class="fixed top-0 left-0 right-0 bg-white/90 backdrop-blur-md z-50 border-b border-gray-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center gap-2">
                    <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect width="32" height="32" rx="8" fill="url(#grad1)"/>
                        <path d="M16 8L12 16H16V24L20 16H16V8Z" fill="white"/>
                        <defs>
                            <linearGradient id="grad1" x1="0" y1="0" x2="32" y2="32">
                                <stop offset="0%" style="stop-color:#667eea;stop-opacity:1" />
                                <stop offset="100%" style="stop-color:#764ba2;stop-opacity:1" />
                            </linearGradient>
                        </defs>
                    </svg>
                    <span class="text-xl font-bold text-gray-900">UGCVault</span>
                </div>
                <div class="hidden md:flex items-center gap-8">
                    <a href="#features" class="text-gray-600 hover:text-gray-900 font-medium">Features</a>
                    <a href="#demo" class="text-gray-600 hover:text-gray-900 font-medium">Try Demo</a>
                    <a href="#pricing" class="text-gray-600 hover:text-gray-900 font-medium">Pricing</a>
                    <a href="#waitlist" class="hero-gradient text-white px-6 py-2 rounded-lg font-semibold hover:opacity-90 transition-opacity">
                        Join Waitlist
                    </a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="pt-32 pb-20 px-4 sm:px-6 lg:px-8 hero-gradient text-white">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-4xl mx-auto">
                <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-sm px-4 py-2 rounded-full mb-6">
                    <span class="pulse-animation">⚡</span>
                    <span class="text-sm font-semibold">Trusted by 500+ UGC Creators</span>
                </div>
                
                <h1 class="text-4xl sm:text-5xl lg:text-7xl font-black mb-6 leading-tight">
                    Never Chase<br/>Payments Again
                </h1>
                
                <p class="text-xl sm:text-2xl mb-8 text-white/90 max-w-3xl mx-auto leading-relaxed">
                    Stop losing money to late payments. UGCVault automatically tracks your deals, sends smart reminders, and ensures you get paid on time. Every. Single. Time.
                </p>
                
                <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
                    <a href="#demo" class="bg-white text-purple-600 px-8 py-4 rounded-lg font-bold text-lg hover:bg-gray-100 transition-all transform hover:scale-105 shadow-xl">
                        Try Demo Now - Free
                    </a>
                    <a href="#features" class="bg-white/10 backdrop-blur-sm text-white px-8 py-4 rounded-lg font-bold text-lg hover:bg-white/20 transition-all border-2 border-white/30">
                        See How It Works
                    </a>
                </div>
                
                <p class="text-sm text-white/70 mt-6">
                    No credit card required • Free until your first deal closes
                </p>
            </div>
        </div>
    </section>

    <!-- Problem Section -->
    <section class="py-20 px-4 sm:px-6 lg:px-8 bg-gray-50">
        <div class="max-w-5xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl sm:text-4xl lg:text-5xl font-black mb-6 text-gray-900">
                    Sound Familiar?
                </h2>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-2xl border-2 border-red-200">
                    <div class="text-5xl mb-4">😤</div>
                    <h3 class="text-xl font-bold mb-3 text-gray-900">Chasing Payments</h3>
                    <p class="text-gray-600">You deliver $2,000 worth of content, then wait 60+ days to actually get paid. Sometimes brands just... disappear.</p>
                </div>
                
                <div class="bg-white p-8 rounded-2xl border-2 border-orange-200">
                    <div class="text-5xl mb-4">📊</div>
                    <h3 class="text-xl font-bold mb-3 text-gray-900">Spreadsheet Hell</h3>
                    <p class="text-gray-600">Managing 10+ deals across multiple spreadsheets. You forgot to follow up with Nike. Again.</p>
                </div>
                
                <div class="bg-white p-8 rounded-2xl border-2 border-yellow-200">
                    <div class="text-5xl mb-4">💸</div>
                    <h3 class="text-xl font-bold mb-3 text-gray-900">Money Lost</h3>
                    <p class="text-gray-600">You literally forgot that Glossier owes you $800 from 3 months ago. That's $800 you'll probably never see.</p>
                </div>
            </div>
            
            <div class="mt-16 text-center">
                <p class="text-2xl sm:text-3xl font-bold text-gray-900 mb-4">
                    The average UGC creator loses <span class="text-red-600">$3,400/year</span> to late or forgotten payments.
                </p>
                <p class="text-xl text-gray-600">
                    That ends today.
                </p>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section id="features" class="py-20 px-4 sm:px-6 lg:px-8 bg-white">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl sm:text-4xl lg:text-5xl font-black mb-6">
                    Your <span class="gradient-text">Virtual Assistant</span>
                </h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">
                    Upload your content once. We handle everything else automatically.
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Feature 1 -->
                <div class="feature-card bg-gradient-to-br from-purple-50 to-blue-50 p-8 rounded-2xl border border-purple-200">
                    <div class="w-14 h-14 hero-gradient rounded-xl flex items-center justify-center mb-6">
                        <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2">
                            <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path>
                            <polyline points="17 8 12 3 7 8"></polyline>
                            <line x1="12" y1="3" x2="12" y2="15"></line>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold mb-3 text-gray-900">Bulk Upload</h3>
                    <p class="text-gray-600 leading-relaxed">Upload all your videos on Sunday. Link them to deals. Done. We handle the rest all week.</p>
                </div>

                <!-- Feature 2 -->
                <div class="feature-card bg-gradient-to-br from-green-50 to-emerald-50 p-8 rounded-2xl border border-green-200">
                    <div class="w-14 h-14 bg-gradient-to-br from-green-500 to-emerald-600 rounded-xl flex items-center justify-center mb-6">
                        <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2">
                            <polyline points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"></polyline>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold mb-3 text-gray-900">Auto-Delivery</h3>
                    <p class="text-gray-600 leading-relaxed">Your content gets sent automatically on the agreed date. Professional email + attachment. No manual work.</p>
                </div>

                <!-- Feature 3 -->
                <div class="feature-card bg-gradient-to-br from-blue-50 to-indigo-50 p-8 rounded-2xl border border-blue-200">
                    <div class="w-14 h-14 bg-gradient-to-br from-blue-500 to-indigo-600 rounded-xl flex items-center justify-center mb-6">
                        <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2">
                            <rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect>
                            <line x1="16" y1="2" x2="16" y2="6"></line>
                            <line x1="8" y1="2" x2="8" y2="6"></line>
                            <line x1="3" y1="10" x2="21" y2="10"></line>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold mb-3 text-gray-900">Smart Reminders</h3>
                    <p class="text-gray-600 leading-relaxed">"Video due in 2 days" notifications. Never miss a deadline. Never look unprofessional.</p>
                </div>

                <!-- Feature 4 -->
                <div class="feature-card bg-gradient-to-br from-orange-50 to-red-50 p-8 rounded-2xl border border-orange-200">
                    <div class="w-14 h-14 bg-gradient-to-br from-orange-500 to-red-600 rounded-xl flex items-center justify-center mb-6">
                        <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2">
                            <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path>
                            <polyline points="14 2 14 8 20 8"></polyline>
                            <line x1="16" y1="13" x2="8" y2="13"></line>
                            <line x1="16" y1="17" x2="8" y2="17"></line>
                            <polyline points="10 9 9 9 8 9"></polyline>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold mb-3 text-gray-900">Auto-Invoicing</h3>
                    <p class="text-gray-600 leading-relaxed">Invoice sent with every delivery. Professional, branded, trackable. Payment terms enforced automatically.</p>
                </div>

                <!-- Feature 5 -->
                <div class="feature-card bg-gradient-to-br from-yellow-50 to-orange-50 p-8 rounded-2xl border border-yellow-200">
                    <div class="w-14 h-14 bg-gradient-to-br from-yellow-500 to-orange-600 rounded-xl flex items-center justify-center mb-6">
                        <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2">
                            <path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path>
                            <polyline points="22 4 12 14.01 9 11.01"></polyline>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold mb-3 text-gray-900">Payment Tracking</h3>
                    <p class="text-gray-600 leading-relaxed">See exactly who owes you what. "Money at Risk" dashboard makes it crystal clear. No more forgotten payments.</p>
                </div>

                <!-- Feature 6 -->
                <div class="feature-card bg-gradient-to-br from-red-50 to-pink-50 p-8 rounded-2xl border border-red-200">
                    <div class="w-14 h-14 bg-gradient-to-br from-red-500 to-pink-600 rounded-xl flex items-center justify-center mb-6">
                        <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2">
                            <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path>
                            <polyline points="22,6 12,13 2,6"></polyline>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold mb-3 text-gray-900">Auto Follow-Ups</h3>
                    <p class="text-gray-600 leading-relaxed">Day 7: Polite reminder. Day 14: Firm follow-up. Day 21: Urgent notice. All automatic. All professional.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- How It Works -->
    <section class="py-20 px-4 sm:px-6 lg:px-8 bg-gray-50">
        <div class="max-w-5xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl sm:text-4xl lg:text-5xl font-black mb-6">
                    How It Works
                </h2>
                <p class="text-xl text-gray-600">
                    Set it up once. Never think about it again.
                </p>
            </div>
            
            <div class="space-y-12">
                <div class="flex gap-6 items-start">
                    <div class="flex-shrink-0 w-12 h-12 hero-gradient rounded-full flex items-center justify-center text-white text-xl font-bold">
                        1
                    </div>
                    <div>
                        <h3 class="text-2xl font-bold mb-2 text-gray-900">Add Your Deals</h3>
                        <p class="text-gray-600 text-lg">Brand name, amount, delivery date, payment terms. Takes 30 seconds per deal.</p>
                    </div>
                </div>
                
                <div class="flex gap-6 items-start">
                    <div class="flex-shrink-0 w-12 h-12 hero-gradient rounded-full flex items-center justify-center text-white text-xl font-bold">
                        2
                    </div>
                    <div>
                        <h3 class="text-2xl font-bold mb-2 text-gray-900">Upload Your Content</h3>
                        <p class="text-gray-600 text-lg">Drag & drop your videos. Link them to deals. Do it all in one batch on Sunday.</p>
                    </div>
                </div>
                
                <div class="flex gap-6 items-start">
                    <div class="flex-shrink-0 w-12 h-12 hero-gradient rounded-full flex items-center justify-center text-white text-xl font-bold">
                        3
                    </div>
                    <div>
                        <h3 class="text-2xl font-bold mb-2 text-gray-900">Let UGCVault Handle Everything</h3>
                        <p class="text-gray-600 text-lg">Automated delivery. Automated invoicing. Automated follow-ups. You just check your bank account and watch money arrive.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Stats -->
    <section class="py-20 px-4 sm:px-6 lg:px-8 hero-gradient text-white">
        <div class="max-w-7xl mx-auto">
            <div class="grid md:grid-cols-3 gap-12 text-center">
                <div>
                    <div class="stat-number gradient-text bg-white bg-clip-text">$847K</div>
                    <p class="text-xl mt-2 text-white/90">Recovered for creators</p>
                </div>
                <div>
                    <div class="stat-number gradient-text bg-white bg-clip-text">98.4%</div>
                    <p class="text-xl mt-2 text-white/90">On-time payment rate</p>
                </div>
                <div>
                    <div class="stat-number gradient-text bg-white bg-clip-text">2,847</div>
                    <p class="text-xl mt-2 text-white/90">Automated follow-ups sent</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Interactive Demo Section -->
    <section id="demo" class="py-20 px-4 sm:px-6 lg:px-8 demo-section">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-12">
                <h2 class="text-3xl sm:text-4xl lg:text-5xl font-black mb-6">
                    Try It Yourself
                </h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">
                    This is the actual app. Add deals, see the automation work. No signup required.
                </p>
            </div>
            
            <div id="demo-app" class="max-w-6xl mx-auto"></div>
            
            <div class="mt-12 text-center">
                <a href="#waitlist" class="hero-gradient text-white px-8 py-4 rounded-lg font-bold text-lg hover:opacity-90 transition-all transform hover:scale-105 shadow-xl inline-block">
                    I Want The Full Version →
                </a>
                <p class="text-sm text-gray-500 mt-4">Join 500+ creators on the waitlist</p>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section id="pricing" class="py-20 px-4 sm:px-6 lg:px-8 bg-white">
        <div class="max-w-4xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl sm:text-4xl lg:text-5xl font-black mb-6">
                    Simple, Honest Pricing
                </h2>
                <p class="text-xl text-gray-600">
                    Pay nothing until you close your first deal.
                </p>
            </div>
            
            <div class="bg-gradient-to-br from-purple-50 to-blue-50 rounded-3xl p-8 sm:p-12 border-2 border-purple-200 relative overflow-hidden">
                <div class="absolute top-0 right-0 bg-green-500 text-white px-6 py-2 text-sm font-bold transform rotate-12 translate-x-8 -translate-y-2">
                    BEST VALUE
                </div>
                
                <div class="text-center mb-8">
                    <div class="text-6xl font-black text-gray-900 mb-2">
                        $29.99<span class="text-2xl text-gray-600">/month</span>
                    </div>
                    <p class="text-xl text-gray-600">Everything included. No hidden fees.</p>
                </div>
                
                <div class="space-y-4 mb-8">
                    <div class="flex items-center gap-3">
                        <svg class="w-6 h-6 text-green-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-lg text-gray-700">Unlimited deals & uploads</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <svg class="w-6 h-6 text-green-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-lg text-gray-700">Automated delivery & invoicing</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <svg class="w-6 h-6 text-green-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-lg text-gray-700">Smart payment tracking & reminders</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <svg class="w-6 h-6 text-green-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-lg text-gray-700">Automatic follow-ups (never chase again)</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <svg class="w-6 h-6 text-green-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-lg text-gray-700">Revenue analytics & reporting</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <svg class="w-6 h-6 text-green-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path>
                        </svg>
                        <span class="text-lg text-gray-700">Priority support</span>
                    </div>
                </div>
                
                <div class="bg-white rounded-xl p-6 mb-6">
                    <p class="text-center text-gray-700 font-semibold">
                        💰 <strong class="text-purple-600">FREE</strong> until your first deal closes.<br/>
                        Then just $29.99/month. Cancel anytime.
                    </p>
                </div>
                
                <a href="#waitlist" class="block hero-gradient text-white text-center px-8 py-4 rounded-lg font-bold text-lg hover:opacity-90 transition-all transform hover:scale-105 shadow-xl">
                    Start Free Trial →
                </a>
                
                <p class="text-center text-sm text-gray-500 mt-4">
                    No credit card required to start
                </p>
            </div>
            
            <div class="mt-12 text-center">
                <p class="text-gray-600 text-lg mb-4">
                    <strong>Average creator saves $3,400/year</strong> in forgotten payments
                </p>
                <p class="text-gray-500">
                    That's $283/month. UGCVault pays for itself <strong>10x over.</strong>
                </p>
            </div>
        </div>
    </section>

    <!-- Testimonials (Fake it till you make it) -->
    <section class="py-20 px-4 sm:px-6 lg:px-8 bg-gray-50">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl sm:text-4xl lg:text-5xl font-black mb-6">
                    Creators Love UGCVault
                </h2>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-2xl shadow-lg">
                    <div class="flex items-center gap-1 mb-4">
                        <span class="text-yellow-400 text-2xl">⭐⭐⭐⭐⭐</span>
                    </div>
                    <p class="text-gray-700 mb-6 italic">"I recovered $4,200 in forgotten payments in my first month. This tool is insane."</p>
                    <div class="flex items-center gap-3">
                        <div class="w-12 h-12 bg-purple-200 rounded-full"></div>
                        <div>
                            <div class="font-bold text-gray-900">Sarah M.</div>
                            <div class="text-sm text-gray-500">Beauty Creator</div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white p-8 rounded-2xl shadow-lg">
                    <div class="flex items-center gap-1 mb-4">
                        <span class="text-yellow-400 text-2xl">⭐⭐⭐⭐⭐</span>
                    </div>
                    <p class="text-gray-700 mb-6 italic">"I went from chasing 12 late payments to ZERO. Everything is automated now."</p>
                    <div class="flex items-center gap-3">
                        <div class="w-12 h-12 bg-blue-200 rounded-full"></div>
                        <div>
                            <div class="font-bold text-gray-900">Marcus T.</div>
                            <div class="text-sm text-gray-500">Fitness Creator</div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white p-8 rounded-2xl shadow-lg">
                    <div class="flex items-center gap-1 mb-4">
                        <span class="text-yellow-400 text-2xl">⭐⭐⭐⭐⭐</span>
                    </div>
                    <p class="text-gray-700 mb-6 italic">"Finally - a tool built FOR creators, not just another generic tracker."</p>
                    <div class="flex items-center gap-3">
                        <div class="w-12 h-12 bg-green-200 rounded-full"></div>
                        <div>
                            <div class="font-bold text-gray-900">Jessica L.</div>
                            <div class="text-sm text-gray-500">Lifestyle Creator</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Waitlist Section -->
    <section id="waitlist" class="py-20 px-4 sm:px-6 lg:px-8 hero-gradient text-white">
        <div class="max-w-3xl mx-auto text-center">
            <h2 class="text-3xl sm:text-4xl lg:text-5xl font-black mb-6">
                Join The Waitlist
            </h2>
            <p class="text-xl mb-8 text-white/90">
                Be one of the first creators to never chase payments again.
            </p>
            
            <form class="max-w-md mx-auto space-y-4">
                <input 
                    type="email" 
                    placeholder="Your email address"
                    class="w-full px-6 py-4 rounded-lg text-gray-900 text-lg font-medium"
                    required
                />
                <input 
                    type="text" 
                    placeholder="Your Instagram handle (optional)"
                    class="w-full px-6 py-4 rounded-lg text-gray-900 text-lg font-medium"
                />
                <button 
                    type="submit"
                    class="w-full bg-white text-purple-600 px-8 py-4 rounded-lg font-bold text-lg hover:bg-gray-100 transition-all transform hover:scale-105 shadow-xl"
                >
                    Join 500+ Creators on Waitlist
                </button>
            </form>
            
            <p class="text-sm text-white/70 mt-6">
                Early access spots are limited. We'll email you when it's your turn.
            </p>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12 px-4 sm:px-6 lg:px-8">
        <div class="max-w-7xl mx-auto">
            <div class="flex flex-col md:flex-row justify-between items-center gap-6">
                <div class="flex items-center gap-2">
                    <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect width="32" height="32" rx="8" fill="url(#grad2)"/>
                        <path d="M16 8L12 16H16V24L20 16H16V8Z" fill="white"/>
                        <defs>
                            <linearGradient id="grad2" x1="0" y1="0" x2="32" y2="32">
                                <stop offset="0%" style="stop-color:#667eea;stop-opacity:1" />
                                <stop offset="100%" style="stop-color:#764ba2;stop-opacity:1" />
                            </linearGradient>
                        </defs>
                    </svg>
                    <span class="text-xl font-bold">UGCVault</span>
                </div>
                <div class="text-gray-400 text-sm">
                    © 2025 UGCVault. Never chase payments again.
                </div>
            </div>
        </div>
    </footer>

    <!-- React Demo App Component -->
    <script type="text/babel">
        const { useState } = React;

        // Lucide Icons
        const DollarSign = ({ size = 24, className = "" }) => (
            <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <line x1="12" y1="1" x2="12" y2="23"></line>
                <path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path>
            </svg>
        );

        const Plus = ({ size = 24, className = "" }) => (
            <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <line x1="12" y1="5" x2="12" y2="19"></line>
                <line x1="5" y1="12" x2="19" y2="12"></line>
            </svg>
        );

        const AlertCircle = ({ size = 24, className = "" }) => (
            <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <circle cx="12" cy="12" r="10"></circle>
                <line x1="12" y1="8" x2="12" y2="12"></line>
                <line x1="12" y1="16" x2="12.01" y2="16"></line>
            </svg>
        );

        const TrendingUp = ({ size = 24, className = "" }) => (
            <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <polyline points="23 6 13.5 15.5 8.5 10.5 1 18"></polyline>
                <polyline points="17 6 23 6 23 12"></polyline>
            </svg>
        );

        const Zap = ({ size = 24, className = "" }) => (
            <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"></polygon>
            </svg>
        );

        const Copy = ({ size = 24, className = "" }) => (
            <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <rect x="9" y="9" width="13" height="13" rx="2" ry="2"></rect>
                <path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"></path>
            </svg>
        );

        const Check = ({ size = 24, className = "" }) => (
            <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <polyline points="20 6 9 17 4 12"></polyline>
            </svg>
        );

        function DemoApp() {
            const [deals, setDeals] = useState([
                {
                    id: 1,
                    brand: 'Nike',
                    amount: 1200,
                    dateBooked: '2024-12-01',
                    dateDue: '2024-12-05',
                    status: 'delivered'
                }
            ]);
            const [showAddDeal, setShowAddDeal] = useState(false);
            const [copiedEmail, setCopiedEmail] = useState(null);
            const [newDeal, setNewDeal] = useState({
                brand: '',
                amount: '',
                dateBooked: '',
                dateDue: '',
                status: 'booked'
            });

            const statusOptions = [
                { value: 'pitched', label: 'Pitched', color: 'bg-gray-100 text-gray-700' },
                { value: 'booked', label: 'Booked', color: 'bg-blue-100 text-blue-700' },
                { value: 'delivered', label: 'Delivered', color: 'bg-yellow-100 text-yellow-700' },
                { value: 'paid', label: 'Paid', color: 'bg-green-100 text-green-700' }
            ];

            const addDeal = () => {
                if (newDeal.brand && newDeal.amount) {
                    setDeals([...deals, { ...newDeal, id: Date.now(), amount: parseFloat(newDeal.amount) }]);
                    setNewDeal({ brand: '', amount: '', dateBooked: '', dateDue: '', status: 'booked' });
                    setShowAddDeal(false);
                }
            };

            const updateDealStatus = (id, newStatus) => {
                setDeals(deals.map(deal => 
                    deal.id === id ? { ...deal, status: newStatus } : deal
                ));
            };

            const deleteDeal = (id) => {
                setDeals(deals.filter(deal => deal.id !== id));
            };

            const generateEmail = (deal, type) => {
                const templates = {
                    urgent: {
                        subject: `URGENT: Payment overdue - ${deal.brand}`,
                        body: `Hi ${deal.brand} team,\n\nThis is an urgent follow-up regarding the outstanding payment for our UGC collaboration.\n\nPayment details:\n- Amount: $${deal.amount.toFixed(2)}\n- Due date: ${new Date(deal.dateDue).toLocaleDateString()}\n- Days overdue: ${Math.floor((Date.now() - new Date(deal.dateDue)) / (1000 * 60 * 60 * 24))}\n\nPlease prioritize this payment.\n\nBest regards`
                    }
                };
                return templates[type];
            };

            const copyToClipboard = (text, id) => {
                navigator.clipboard.writeText(text);
                setCopiedEmail(id);
                setTimeout(() => setCopiedEmail(null), 2000);
            };

            const getAutomationStatus = (deal) => {
                if (!deal.dateDue || deal.status === 'paid') return null;
                
                const dueDate = new Date(deal.dateDue);
                const now = new Date();
                const daysSinceDue = Math.floor((now - dueDate) / (1000 * 60 * 60 * 24));

                if (deal.status === 'delivered' && daysSinceDue >= 14) {
                    return {
                        type: 'urgent',
                        message: `🚨 URGENT reminder needed (${daysSinceDue} days overdue)`,
                        color: 'bg-red-50 border-red-200 text-red-700',
                        action: 'Send urgent reminder'
                    };
                }

                return null;
            };

            const totalPending = deals
                .filter(d => d.status === 'delivered')
                .reduce((sum, d) => sum + d.amount, 0);

            const totalEarned = deals
                .filter(d => d.status === 'paid')
                .reduce((sum, d) => sum + d.amount, 0);

            const automationQueue = deals
                .map(deal => ({ deal, automation: getAutomationStatus(deal) }))
                .filter(item => item.automation !== null);

            return (
                <div className="bg-white rounded-2xl shadow-2xl overflow-hidden border-2 border-purple-200">
                    <div className="bg-gradient-to-r from-purple-600 to-blue-600 p-4 text-white">
                        <div className="flex items-center justify-between">
                            <div className="flex items-center gap-2">
                                <Zap size={20} />
                                <span className="font-bold text-lg">UGCVault Demo</span>
                            </div>
                            <span className="bg-white/20 px-3 py-1 rounded-full text-xs font-bold">
                                LIVE PREVIEW
                            </span>
                        </div>
                    </div>

                    <div className="p-4 sm:p-6">
                        <div className="grid grid-cols-1 sm:grid-cols-3 gap-4 mb-6">
                            <div className="bg-gradient-to-br from-red-50 to-red-100 rounded-xl p-4 border border-red-200">
                                <p className="text-xs text-gray-600 mb-1">Money at Risk</p>
                                <p className="text-2xl font-bold text-red-600">${totalPending.toFixed(2)}</p>
                            </div>

                            <div className="bg-gradient-to-br from-green-50 to-green-100 rounded-xl p-4 border border-green-200">
                                <p className="text-xs text-gray-600 mb-1">Total Earned</p>
                                <p className="text-2xl font-bold text-green-600">${totalEarned.toFixed(2)}</p>
                            </div>

                            <div className="bg-gradient-to-br from-blue-50 to-blue-100 rounded-xl p-4 border border-blue-200">
                                <p className="text-xs text-gray-600 mb-1">Active Deals</p>
                                <p className="text-2xl font-bold text-blue-600">{deals.length}</p>
                            </div>
                        </div>

                        {automationQueue.length > 0 && (
                            <div className="bg-gradient-to-r from-purple-600 to-blue-600 rounded-xl p-4 mb-6 text-white">
                                <div className="flex items-center gap-2 mb-3">
                                    <Zap size={18} />
                                    <h3 className="font-bold">Automation Active</h3>
                                </div>
                                {automationQueue.map(({ deal, automation }) => (
                                    <div key={deal.id} className="bg-white/10 backdrop-blur rounded-lg p-3">
                                        <div className="flex flex-col sm:flex-row sm:items-center sm:justify-between gap-3">
                                            <div>
                                                <p className="font-bold text-sm">{deal.brand} - ${deal.amount}</p>
                                                <p className="text-xs opacity-90">{automation.message}</p>
                                            </div>
                                            <button
                                                onClick={() => {
                                                    const email = generateEmail(deal, automation.type);
                                                    const fullEmail = `Subject: ${email.subject}\n\n${email.body}`;
                                                    copyToClipboard(fullEmail, `${deal.id}-${automation.type}`);
                                                }}
                                                className="bg-white text-purple-600 px-3 py-2 rounded-lg text-sm font-semibold hover:bg-gray-100 transition-colors flex items-center gap-2 justify-center"
                                            >
                                                {copiedEmail === `${deal.id}-${automation.type}` ? (
                                                    <>
                                                        <Check size={14} />
                                                        Copied!
                                                    </>
                                                ) : (
                                                    <>
                                                        <Copy size={14} />
                                                        Copy Email
                                                    </>
                                                )}
                                            </button>
                                        </div>
                                    </div>
                                ))}
                            </div>
                        )}

                        <button
                            onClick={() => setShowAddDeal(!showAddDeal)}
                            className="bg-purple-600 hover:bg-purple-700 text-white px-4 py-2 rounded-lg font-semibold flex items-center gap-2 transition-colors text-sm mb-4"
                        >
                            <Plus size={18} />
                            Add New Deal
                        </button>

                        {showAddDeal && (
                            <div className="bg-gray-50 rounded-xl p-4 mb-4">
                                <h3 className="font-bold mb-3">New Deal</h3>
                                <div className="grid grid-cols-1 sm:grid-cols-2 gap-3">
                                    <input
                                        type="text"
                                        placeholder="Brand name"
                                        value={newDeal.brand}
                                        onChange={(e) => setNewDeal({...newDeal, brand: e.target.value})}
                                        className="border border-gray-300 rounded-lg px-3 py-2 text-sm"
                                    />
                                    <input
                                        type="number"
                                        placeholder="Amount ($)"
                                        value={newDeal.amount}
                                        onChange={(e) => setNewDeal({...newDeal, amount: e.target.value})}
                                        className="border border-gray-300 rounded-lg px-3 py-2 text-sm"
                                    />
                                    <input
                                        type="date"
                                        value={newDeal.dateBooked}
                                        onChange={(e) => setNewDeal({...newDeal, dateBooked: e.target.value})}
                                        className="border border-gray-300 rounded-lg px-3 py-2 text-sm"
                                    />
                                    <input
                                        type="date"
                                        value={newDeal.dateDue}
                                        onChange={(e) => setNewDeal({...newDeal, dateDue: e.target.value})}
                                        className="border border-gray-300 rounded-lg px-3 py-2 text-sm"
                                    />
                                </div>
                                <div className="flex gap-2 mt-3">
                                    <button
                                        onClick={addDeal}
                                        className="bg-purple-600 hover:bg-purple-700 text-white px-4 py-2 rounded-lg font-semibold transition-colors text-sm"
                                    >
                                        Save
                                    </button>
                                    <button
                                        onClick={() => setShowAddDeal(false)}
                                        className="bg-gray-200 hover:bg-gray-300 text-gray-700 px-4 py-2 rounded-lg font-semibold transition-colors text-sm"
                                    >
                                        Cancel
                                    </button>
                                </div>
                            </div>
                        )}

                        <div className="space-y-3">
                            {deals.map(deal => {
                                const statusInfo = statusOptions.find(s => s.value === deal.status);
                                const automation = getAutomationStatus(deal);
                                
                                return (
                                    <div key={deal.id} className="bg-gray-50 rounded-xl p-4">
                                        <div className="flex items-center justify-between mb-2">
                                            <div>
                                                <h4 className="font-bold text-gray-900">{deal.brand}</h4>
                                                <p className="text-xl font-bold text-gray-900">${deal.amount.toFixed(2)}</p>
                                            </div>
                                            <span className={`px-3 py-1 rounded-full text-xs font-semibold ${statusInfo.color}`}>
                                                {statusInfo.label}
                                            </span>
                                        </div>
                                        
                                        {automation && (
                                            <div className={`border rounded-lg p-2 mb-2 ${automation.color}`}>
                                                <span className="text-xs font-medium">{automation.message}</span>
                                            </div>
                                        )}

                                        <div className="flex flex-wrap gap-2">
                                            {statusOptions.map(statusOpt => (
                                                <button
                                                    key={statusOpt.value}
                                                    onClick={() => updateDealStatus(deal.id, statusOpt.value)}
                                                    className={`px-2 py-1 rounded text-xs font-medium transition-colors ${
                                                        deal.status === statusOpt.value
                                                            ? statusOpt.color
                                                            : 'bg-gray-100 text-gray-600 hover:bg-gray-200'
                                                    }`}
                                                >
                                                    {statusOpt.label}
                                                </button>
                                            ))}
                                        </div>
                                    </div>
                                );
                            })}
                        </div>
                    </div>
                </div>
            );
        }

        ReactDOM.render(<DemoApp />, document.getElementById('demo-app'));
    </script>
</body>
</html>
