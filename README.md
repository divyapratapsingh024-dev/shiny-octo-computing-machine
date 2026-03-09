<!doctype html>
<html lang="en" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio</title>
  <script src="https://cdn.tailwindcss.com/3.4.17"></script>
  <script src="https://cdn.jsdelivr.net/npm/lucide@0.263.0/dist/umd/lucide.min.js"></script>
  <script src="/_sdk/element_sdk.js"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800&amp;family=Crimson+Text:wght@400;600&amp;display=swap" rel="stylesheet">
  <style>
    * { box-sizing: border-box; }
    html, body, #app-wrapper { height: 100%; }
    
    .font-serif { font-family: 'Crimson Text', serif; }
    .font-sans { font-family: 'Outfit', sans-serif; }
    
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
    
    @keyframes float {
      0%, 100% { transform: translateY(0px); }
      50% { transform: translateY(-20px); }
    }
    
    @keyframes slideIn {
      from {
        opacity: 0;
        transform: translateX(-30px);
      }
      to {
        opacity: 1;
        transform: translateX(0);
      }
    }
    
    .animate-fade-in-up { animation: fadeInUp 0.8s ease-out forwards; }
    .animate-float { animation: float 6s ease-in-out infinite; }
    .animate-slide-in { animation: slideIn 0.6s ease-out forwards; }
    
    .hero-content > * {
      animation: fadeInUp 0.8s ease-out forwards;
    }
    
    .hero-content h1 { animation-delay: 0.1s; }
    .hero-content .subtitle { animation-delay: 0.2s; }
    .hero-content .description { animation-delay: 0.3s; }
    .hero-content .cta { animation-delay: 0.4s; }
    
    .project-card {
      transition: all 0.3s ease;
    }
    
    .project-card:hover {
      transform: translateY(-8px);
    }

    .service-card {
      transition: all 0.3s ease;
    }

    .service-card:hover {
      background: linear-gradient(135deg, #eff6ff 0%, #f0f9ff 100%);
      border-color: #0ea5e9;
    }

    .testimonial-card {
      transition: all 0.3s ease;
    }

    .testimonial-card:hover {
      box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
    }
    
    .gradient-text {
      background: linear-gradient(135deg, #3b82f6 0%, #06b6d4 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .stats-grid > div {
      animation: fadeInUp 0.8s ease-out forwards;
    }

    .stats-grid > div:nth-child(1) { animation-delay: 0.1s; }
    .stats-grid > div:nth-child(2) { animation-delay: 0.2s; }
    .stats-grid > div:nth-child(3) { animation-delay: 0.3s; }
    .stats-grid > div:nth-child(4) { animation-delay: 0.4s; }
  </style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
  <style>body { box-sizing: border-box; }</style>
 </head>
 <body class="h-full font-sans bg-white">
  <div id="app-wrapper" class="h-full w-full overflow-auto flex flex-col"><!-- Navigation -->
   <nav class="sticky top-0 z-50 bg-white/90 backdrop-blur-md border-b border-slate-100 shadow-sm">
    <div class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
     <div class="flex items-center gap-2">
      <div class="w-8 h-8 rounded-lg bg-gradient-to-br from-blue-500 to-cyan-500 shadow-lg"></div><span id="nav-name" class="font-bold text-lg text-slate-900">Portfolio</span>
     </div>
     <div class="hidden md:flex items-center gap-8"><a href="#work" class="text-sm text-slate-600 hover:text-blue-600 transition font-medium">Work</a> <a href="#services" class="text-sm text-slate-600 hover:text-blue-600 transition font-medium">Services</a> <a href="#about" class="text-sm text-slate-600 hover:text-blue-600 transition font-medium">About</a> <a href="#testimonials" class="text-sm text-slate-600 hover:text-blue-600 transition font-medium">Testimonials</a> <a href="#contact" class="text-sm text-slate-600 hover:text-blue-600 transition font-medium">Contact</a>
     </div><button class="md:hidden p-2 text-slate-600 hover:text-slate-900"><i data-lucide="menu" class="w-5 h-5"></i></button>
    </div>
   </nav><!-- Hero Section -->
   <section class="flex-1 flex items-center justify-center px-6 py-32 bg-gradient-to-br from-slate-50 via-blue-50 to-cyan-50">
    <div class="max-w-5xl mx-auto text-center hero-content">
     <h1 id="site-title" class="text-6xl sm:text-7xl lg:text-8xl font-bold text-slate-900 mb-6 leading-tight">Jane Designer</h1>
     <p id="tagline" class="subtitle text-2xl sm:text-3xl text-blue-600 mb-8 font-serif font-light">Creative Designer &amp; Developer</p>
     <p id="hero-description" class="description text-lg sm:text-xl text-slate-600 max-w-3xl mx-auto mb-10 leading-relaxed">I create beautiful, functional digital experiences that solve real problems. Specializing in design systems and modern web applications that drive results.</p>
     <div class="flex flex-col sm:flex-row gap-4 justify-center items-center"><button id="cta-btn" class="cta px-10 py-4 bg-gradient-to-r from-blue-600 to-cyan-600 text-white font-semibold rounded-xl hover:shadow-2xl hover:shadow-blue-500/40 transition-all text-lg">Get In Touch</button> <a href="#work" class="px-10 py-4 border-2 border-slate-300 text-slate-700 font-semibold rounded-xl hover:border-blue-600 hover:text-blue-600 transition-all text-lg">View Work</a>
     </div>
    </div>
   </section><!-- Stats Section -->
   <section class="px-6 py-20 bg-white border-b border-slate-100">
    <div class="max-w-6xl mx-auto">
     <div class="stats-grid grid grid-cols-2 md:grid-cols-4 gap-8">
      <div class="text-center">
       <div class="text-4xl font-bold text-blue-600 mb-2">
        50+
       </div>
       <p class="text-slate-600 font-medium">Projects Completed</p>
      </div>
      <div class="text-center">
       <div class="text-4xl font-bold text-cyan-600 mb-2">
        100+
       </div>
       <p class="text-slate-600 font-medium">Happy Clients</p>
      </div>
      <div class="text-center">
       <div class="text-4xl font-bold text-blue-600 mb-2">
        8+
       </div>
       <p class="text-slate-600 font-medium">Years Experience</p>
      </div>
      <div class="text-center">
       <div class="text-4xl font-bold text-cyan-600 mb-2">
        15+
       </div>
       <p class="text-slate-600 font-medium">Awards Won</p>
      </div>
     </div>
    </div>
   </section><!-- Services Section -->
   <section id="services" class="px-6 py-20 bg-slate-50">
    <div class="max-w-6xl mx-auto">
     <h2 id="services-title" class="text-4xl font-bold text-slate-900 mb-12 text-center">What I Offer</h2>
     <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8"><!-- Service 1 -->
      <div class="service-card p-8 bg-white rounded-2xl border border-slate-200">
       <div class="w-12 h-12 rounded-lg bg-gradient-to-br from-blue-500 to-cyan-500 flex items-center justify-center mb-4"><i data-lucide="palette" class="w-6 h-6 text-white"></i>
       </div>
       <h3 class="text-xl font-bold text-slate-900 mb-3">UI/UX Design</h3>
       <p class="text-slate-600 leading-relaxed">Beautiful, intuitive interfaces that users love. I combine research-driven insights with stunning visuals.</p>
      </div><!-- Service 2 -->
      <div class="service-card p-8 bg-white rounded-2xl border border-slate-200">
       <div class="w-12 h-12 rounded-lg bg-gradient-to-br from-purple-500 to-pink-500 flex items-center justify-center mb-4"><i data-lucide="code" class="w-6 h-6 text-white"></i>
       </div>
       <h3 class="text-xl font-bold text-slate-900 mb-3">Frontend Development</h3>
       <p class="text-slate-600 leading-relaxed">Modern, responsive web applications built with cutting-edge technologies and best practices.</p>
      </div><!-- Service 3 -->
      <div class="service-card p-8 bg-white rounded-2xl border border-slate-200">
       <div class="w-12 h-12 rounded-lg bg-gradient-to-br from-emerald-500 to-teal-500 flex items-center justify-center mb-4"><i data-lucide="grid" class="w-6 h-6 text-white"></i>
       </div>
       <h3 class="text-xl font-bold text-slate-900 mb-3">Design Systems</h3>
       <p class="text-slate-600 leading-relaxed">Scalable component libraries and design tokens for consistent, efficient product development.</p>
      </div><!-- Service 4 -->
      <div class="service-card p-8 bg-white rounded-2xl border border-slate-200">
       <div class="w-12 h-12 rounded-lg bg-gradient-to-br from-orange-500 to-red-500 flex items-center justify-center mb-4"><i data-lucide="zap" class="w-6 h-6 text-white"></i>
       </div>
       <h3 class="text-xl font-bold text-slate-900 mb-3">Performance Optimization</h3>
       <p class="text-slate-600 leading-relaxed">Fast-loading, efficient applications that provide excellent user experiences across all devices.</p>
      </div><!-- Service 5 -->
      <div class="service-card p-8 bg-white rounded-2xl border border-slate-200">
       <div class="w-12 h-12 rounded-lg bg-gradient-to-br from-indigo-500 to-blue-500 flex items-center justify-center mb-4"><i data-lucide="briefcase" class="w-6 h-6 text-white"></i>
       </div>
       <h3 class="text-xl font-bold text-slate-900 mb-3">Brand Strategy</h3>
       <p class="text-slate-600 leading-relaxed">Strategic brand positioning and visual identity that resonates with your target audience.</p>
      </div><!-- Service 6 -->
      <div class="service-card p-8 bg-white rounded-2xl border border-slate-200">
       <div class="w-12 h-12 rounded-lg bg-gradient-to-br from-rose-500 to-pink-500 flex items-center justify-center mb-4"><i data-lucide="users" class="w-6 h-6 text-white"></i>
       </div>
       <h3 class="text-xl font-bold text-slate-900 mb-3">User Research</h3>
       <p class="text-slate-600 leading-relaxed">Deep user insights and testing to ensure your product meets real needs and solves actual problems.</p>
      </div>
     </div>
    </div>
   </section><!-- Featured Work Section -->
   <section id="work" class="px-6 py-20 bg-white">
    <div class="max-w-6xl mx-auto">
     <h2 class="text-4xl font-bold text-slate-900 mb-12 text-center">Featured Work</h2>
     <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8"><!-- Project 1 -->
      <div class="project-card group overflow-hidden rounded-2xl bg-white border border-slate-200 hover:border-blue-300 hover:shadow-xl">
       <div class="h-48 bg-gradient-to-br from-blue-400 to-cyan-400 flex items-center justify-center overflow-hidden relative">
        <div class="absolute inset-0 opacity-0 group-hover:opacity-10 bg-black transition-opacity"></div><i data-lucide="layout-grid" class="w-24 h-24 text-white/40"></i>
       </div>
       <div class="p-6">
        <h3 class="text-xl font-bold text-slate-900 mb-2">Design System</h3>
        <p class="text-slate-600 mb-4">A comprehensive component library and design tokens for seamless collaboration across teams.</p>
        <div class="flex gap-2 flex-wrap"><span class="px-3 py-1 bg-blue-100 text-blue-700 text-xs rounded-full font-medium">Design</span> <span class="px-3 py-1 bg-cyan-100 text-cyan-700 text-xs rounded-full font-medium">Systems</span>
        </div>
       </div>
      </div><!-- Project 2 -->
      <div class="project-card group overflow-hidden rounded-2xl bg-white border border-slate-200 hover:border-blue-300 hover:shadow-xl">
       <div class="h-48 bg-gradient-to-br from-purple-400 to-pink-400 flex items-center justify-center overflow-hidden relative">
        <div class="absolute inset-0 opacity-0 group-hover:opacity-10 bg-black transition-opacity"></div><i data-lucide="smartphone" class="w-24 h-24 text-white/40"></i>
       </div>
       <div class="p-6">
        <h3 class="text-xl font-bold text-slate-900 mb-2">Mobile App</h3>
        <p class="text-slate-600 mb-4">Cross-platform app helping teams collaborate in real-time, anywhere in the world.</p>
        <div class="flex gap-2 flex-wrap"><span class="px-3 py-1 bg-purple-100 text-purple-700 text-xs rounded-full font-medium">iOS</span> <span class="px-3 py-1 bg-pink-100 text-pink-700 text-xs rounded-full font-medium">Android</span>
        </div>
       </div>
      </div><!-- Project 3 -->
      <div class="project-card group overflow-hidden rounded-2xl bg-white border border-slate-200 hover:border-blue-300 hover:shadow-xl">
       <div class="h-48 bg-gradient-to-br from-emerald-400 to-teal-400 flex items-center justify-center overflow-hidden relative">
        <div class="absolute inset-0 opacity-0 group-hover:opacity-10 bg-black transition-opacity"></div><i data-lucide="globe" class="w-24 h-24 text-white/40"></i>
       </div>
       <div class="p-6">
        <h3 class="text-xl font-bold text-slate-900 mb-2">Website Redesign</h3>
        <p class="text-slate-600 mb-4">Modern e-commerce platform achieving 40% improvement in conversion rates and user engagement.</p>
        <div class="flex gap-2 flex-wrap"><span class="px-3 py-1 bg-emerald-100 text-emerald-700 text-xs rounded-full font-medium">Web</span> <span class="px-3 py-1 bg-teal-100 text-teal-700 text-xs rounded-full font-medium">E-commerce</span>
        </div>
       </div>
      </div><!-- Project 4 -->
      <div class="project-card group overflow-hidden rounded-2xl bg-white border border-slate-200 hover:border-blue-300 hover:shadow-xl">
       <div class="h-48 bg-gradient-to-br from-orange-400 to-red-400 flex items-center justify-center overflow-hidden relative">
        <div class="absolute inset-0 opacity-0 group-hover:opacity-10 bg-black transition-opacity"></div><i data-lucide="barChart3" class="w-24 h-24 text-white/40"></i>
       </div>
       <div class="p-6">
        <h3 class="text-xl font-bold text-slate-900 mb-2">Analytics Dashboard</h3>
        <p class="text-slate-600 mb-4">Real-time data visualization platform for business intelligence and decision making.</p>
        <div class="flex gap-2 flex-wrap"><span class="px-3 py-1 bg-orange-100 text-orange-700 text-xs rounded-full font-medium">Analytics</span> <span class="px-3 py-1 bg-red-100 text-red-700 text-xs rounded-full font-medium">Data</span>
        </div>
       </div>
      </div><!-- Project 5 -->
      <div class="project-card group overflow-hidden rounded-2xl bg-white border border-slate-200 hover:border-blue-300 hover:shadow-xl">
       <div class="h-48 bg-gradient-to-br from-indigo-400 to-purple-400 flex items-center justify-center overflow-hidden relative">
        <div class="absolute inset-0 opacity-0 group-hover:opacity-10 bg-black transition-opacity"></div><i data-lucide="music" class="w-24 h-24 text-white/40"></i>
       </div>
       <div class="p-6">
        <h3 class="text-xl font-bold text-slate-900 mb-2">Music Platform</h3>
        <p class="text-slate-600 mb-4">Streaming service with personalized recommendations and social features for music lovers.</p>
        <div class="flex gap-2 flex-wrap"><span class="px-3 py-1 bg-indigo-100 text-indigo-700 text-xs rounded-full font-medium">Streaming</span> <span class="px-3 py-1 bg-purple-100 text-purple-700 text-xs rounded-full font-medium">Social</span>
        </div>
       </div>
      </div><!-- Project 6 -->
      <div class="project-card group overflow-hidden rounded-2xl bg-white border border-slate-200 hover:border-blue-300 hover:shadow-xl">
       <div class="h-48 bg-gradient-to-br from-rose-400 to-pink-400 flex items-center justify-center overflow-hidden relative">
        <div class="absolute inset-0 opacity-0 group-hover:opacity-10 bg-black transition-opacity"></div><i data-lucide="heart" class="w-24 h-24 text-white/40"></i>
       </div>
       <div class="p-6">
        <h3 class="text-xl font-bold text-slate-900 mb-2">Health App</h3>
        <p class="text-slate-600 mb-4">Wellness platform connecting users with fitness coaches and personalized health tracking.</p>
        <div class="flex gap-2 flex-wrap"><span class="px-3 py-1 bg-rose-100 text-rose-700 text-xs rounded-full font-medium">Wellness</span> <span class="px-3 py-1 bg-pink-100 text-pink-700 text-xs rounded-full font-medium">Health</span>
        </div>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Testimonials Section -->
   <section id="testimonials" class="px-6 py-20 bg-slate-50">
    <div class="max-w-6xl mx-auto">
     <h2 class="text-4xl font-bold text-slate-900 mb-12 text-center">What Clients Say</h2>
     <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8"><!-- Testimonial 1 -->
      <div class="testimonial-card p-8 bg-white rounded-2xl border border-slate-200">
       <div class="flex gap-1 mb-4"><i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i>
       </div>
       <p class="text-slate-600 mb-6 leading-relaxed">"Jane transformed our product vision into reality. Her attention to detail and user-centric approach resulted in a 300% increase in user engagement."</p>
       <div class="flex items-center gap-3">
        <div class="w-10 h-10 rounded-full bg-gradient-to-br from-blue-500 to-cyan-500"></div>
        <div>
         <p class="font-semibold text-slate-900">Sarah Johnson</p>
         <p class="text-sm text-slate-600">CEO, TechStart</p>
        </div>
       </div>
      </div><!-- Testimonial 2 -->
      <div class="testimonial-card p-8 bg-white rounded-2xl border border-slate-200">
       <div class="flex gap-1 mb-4"><i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i>
       </div>
       <p class="text-slate-600 mb-6 leading-relaxed">"Working with Jane was a game-changer. She combines creativity with technical expertise, delivering beautiful designs that actually work flawlessly."</p>
       <div class="flex items-center gap-3">
        <div class="w-10 h-10 rounded-full bg-gradient-to-br from-purple-500 to-pink-500"></div>
        <div>
         <p class="font-semibold text-slate-900">Michael Chen</p>
         <p class="text-sm text-slate-600">Product Manager, InnovateCo</p>
        </div>
       </div>
      </div><!-- Testimonial 3 -->
      <div class="testimonial-card p-8 bg-white rounded-2xl border border-slate-200">
       <div class="flex gap-1 mb-4"><i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i> <i data-lucide="star" class="w-5 h-5 fill-yellow-400 text-yellow-400"></i>
       </div>
       <p class="text-slate-600 mb-6 leading-relaxed">"Her design system work elevated our entire product suite. The ROI was immediate with faster development cycles and consistent user experiences."</p>
       <div class="flex items-center gap-3">
        <div class="w-10 h-10 rounded-full bg-gradient-to-br from-emerald-500 to-teal-500"></div>
        <div>
         <p class="font-semibold text-slate-900">Emma Rodriguez</p>
         <p class="text-sm text-slate-600">Design Director, Global Tech</p>
        </div>
       </div>
      </div>
     </div>
    </div>
   </section><!-- About Section -->
   <section id="about" class="px-6 py-20 bg-white">
    <div class="max-w-6xl mx-auto">
     <h2 id="about-title" class="text-4xl font-bold text-slate-900 mb-12 text-center">About Me</h2>
     <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
      <div>
       <p id="about-description" class="text-lg text-slate-600 mb-6 leading-relaxed">With 8+ years of experience in digital design and development, I've worked with startups to Fortune 500 companies to create impactful digital products that drive real business results.</p>
       <p class="text-lg text-slate-600 mb-6 leading-relaxed">I specialize in translating complex problems into elegant, user-centered solutions. My approach combines strategic thinking with practical execution, backed by data and user research.</p>
       <p class="text-lg text-slate-600 mb-6 leading-relaxed">Whether it's building a design system from scratch or optimizing an existing product, I'm passionate about creating experiences that matter.</p>
      </div>
      <div>
       <h3 class="text-2xl font-bold text-slate-900 mb-6">Skills &amp; Expertise</h3>
       <div class="space-y-4">
        <div class="flex items-start gap-4">
         <div class="w-8 h-8 rounded-lg bg-blue-100 flex items-center justify-center flex-shrink-0 mt-1"><i data-lucide="check" class="w-5 h-5 text-blue-600"></i>
         </div>
         <div>
          <h4 class="font-semibold text-slate-900 mb-1">Product Design &amp; UX</h4>
          <p class="text-slate-600">User research, wireframing, prototyping, and user testing</p>
         </div>
        </div>
        <div class="flex items-start gap-4">
         <div class="w-8 h-8 rounded-lg bg-cyan-100 flex items-center justify-center flex-shrink-0 mt-1"><i data-lucide="check" class="w-5 h-5 text-cyan-600"></i>
         </div>
         <div>
          <h4 class="font-semibold text-slate-900 mb-1">Design Systems</h4>
          <p class="text-slate-600">Component libraries, design tokens, documentation</p>
         </div>
        </div>
        <div class="flex items-start gap-4">
         <div class="w-8 h-8 rounded-lg bg-blue-100 flex items-center justify-center flex-shrink-0 mt-1"><i data-lucide="check" class="w-5 h-5 text-blue-600"></i>
         </div>
         <div>
          <h4 class="font-semibold text-slate-900 mb-1">Frontend Development</h4>
          <p class="text-slate-600">React, Vue, TypeScript, responsive design, performance</p>
         </div>
        </div>
        <div class="flex items-start gap-4">
         <div class="w-8 h-8 rounded-lg bg-cyan-100 flex items-center justify-center flex-shrink-0 mt-1"><i data-lucide="check" class="w-5 h-5 text-cyan-600"></i>
         </div>
         <div>
          <h4 class="font-semibold text-slate-900 mb-1">Brand &amp; Visual Design</h4>
          <p class="text-slate-600">Logo design, brand guidelines, visual identity systems</p>
         </div>
        </div>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Process Section -->
   <section class="px-6 py-20 bg-slate-50">
    <div class="max-w-6xl mx-auto">
     <h2 class="text-4xl font-bold text-slate-900 mb-12 text-center">My Process</h2>
     <div class="grid grid-cols-1 md:grid-cols-4 gap-6">
      <div class="relative">
       <div class="flex flex-col items-center">
        <div class="w-16 h-16 rounded-full bg-gradient-to-br from-blue-500 to-cyan-500 flex items-center justify-center text-white font-bold text-xl mb-4 shadow-lg">
         1
        </div>
        <h3 class="text-xl font-bold text-slate-900 mb-2 text-center">Discovery</h3>
        <p class="text-slate-600 text-center">Research and understand your goals, users, and market</p>
       </div>
       <div class="hidden md:block absolute top-16 left-[calc(50%+40px)] w-[calc(100%-80px)] h-1 bg-gradient-to-r from-blue-500 to-cyan-500"></div>
      </div>
      <div class="relative">
       <div class="flex flex-col items-center">
        <div class="w-16 h-16 rounded-full bg-gradient-to-br from-cyan-500 to-teal-500 flex items-center justify-center text-white font-bold text-xl mb-4 shadow-lg">
         2
        </div>
        <h3 class="text-xl font-bold text-slate-900 mb-2 text-center">Design</h3>
        <p class="text-slate-600 text-center">Create beautiful, functional solutions with prototypes</p>
       </div>
       <div class="hidden md:block absolute top-16 left-[calc(50%+40px)] w-[calc(100%-80px)] h-1 bg-gradient-to-r from-cyan-500 to-teal-500"></div>
      </div>
      <div class="relative">
       <div class="flex flex-col items-center">
        <div class="w-16 h-16 rounded-full bg-gradient-to-br from-teal-500 to-emerald-500 flex items-center justify-center text-white font-bold text-xl mb-4 shadow-lg">
         3
        </div>
        <h3 class="text-xl font-bold text-slate-900 mb-2 text-center">Development</h3>
        <p class="text-slate-600 text-center">Build performant, scalable applications</p>
       </div>
       <div class="hidden md:block absolute top-16 left-[calc(50%+40px)] w-[calc(100%-80px)] h-1 bg-gradient-to-r from-teal-500 to-emerald-500"></div>
      </div>
      <div class="relative">
       <div class="flex flex-col items-center">
        <div class="w-16 h-16 rounded-full bg-gradient-to-br from-emerald-500 to-green-500 flex items-center justify-center text-white font-bold text-xl mb-4 shadow-lg">
         4
        </div>
        <h3 class="text-xl font-bold text-slate-900 mb-2 text-center">Optimize</h3>
        <p class="text-slate-600 text-center">Test, refine, and deliver exceptional results</p>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Contact Section -->
   <section id="contact" class="px-6 py-20 bg-gradient-to-br from-slate-900 to-slate-800">
    <div class="max-w-4xl mx-auto text-center">
     <h2 class="text-4xl font-bold text-white mb-4">Let's Work Together</h2>
     <p class="text-xl text-slate-300 mb-12">Have a project in mind? I'd love to hear about it and discuss how we can create something amazing.</p>
     <div class="flex flex-col sm:flex-row gap-4 justify-center items-center"><a href="mailto:hello@example.com" class="px-10 py-4 bg-white text-slate-900 font-semibold rounded-xl hover:bg-slate-100 transition-all text-lg flex items-center gap-2"> <i data-lucide="mail" class="w-5 h-5"></i> Email Me </a> <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer" class="px-10 py-4 border-2 border-white text-white font-semibold rounded-xl hover:bg-white/10 transition-all text-lg flex items-center gap-2"> <i data-lucide="linkedin" class="w-5 h-5"></i> LinkedIn </a> <a href="https://github.com" target="_blank" rel="noopener noreferrer" class="px-10 py-4 border-2 border-white text-white font-semibold rounded-xl hover:bg-white/10 transition-all text-lg flex items-center gap-2"> <i data-lucide="github" class="w-5 h-5"></i> GitHub </a>
     </div>
    </div>
   </section><!-- Footer -->
   <footer class="bg-slate-950 text-slate-400 py-12 px-6 border-t border-slate-800">
    <div class="max-w-6xl mx-auto">
     <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-8">
      <div>
       <h3 class="font-bold text-white mb-4">Portfolio</h3>
       <p class="text-sm leading-relaxed">Creating beautiful digital experiences that solve real problems.</p>
      </div>
      <div>
       <h3 class="font-bold text-white mb-4">Services</h3>
       <ul class="space-y-2 text-sm">
        <li><a href="#services" class="hover:text-white transition">UI/UX Design</a></li>
        <li><a href="#services" class="hover:text-white transition">Development</a></li>
        <li><a href="#services" class="hover:text-white transition">Consulting</a></li>
       </ul>
      </div>
      <div>
       <h3 class="font-bold text-white mb-4">Quick Links</h3>
       <ul class="space-y-2 text-sm">
        <li><a href="#work" class="hover:text-white transition">Work</a></li>
        <li><a href="#about" class="hover:text-white transition">About</a></li>
        <li><a href="#contact" class="hover:text-white transition">Contact</a></li>
       </ul>
      </div>
      <div>
       <h3 class="font-bold text-white mb-4">Connect</h3>
       <div class="flex gap-4"><a href="#" class="hover:text-white transition"><i data-lucide="twitter" class="w-5 h-5"></i></a> <a href="#" class="hover:text-white transition"><i data-lucide="linkedin" class="w-5 h-5"></i></a> <a href="#" class="hover:text-white transition"><i data-lucide="github" class="w-5 h-5"></i></a>
       </div>
      </div>
     </div>
     <div class="border-t border-slate-800 pt-8 flex flex-col md:flex-row items-center justify-between gap-4 text-sm">
      <p id="footer-text">© 2024 Portfolio. All rights reserved.</p>
      <div class="flex gap-6"><a href="#" class="hover:text-white transition">Privacy Policy</a> <a href="#" class="hover:text-white transition">Terms of Service</a> <a href="#" class="hover:text-white transition">Sitemap</a>
      </div>
     </div>
    </div>
   </footer>
  </div>
  <script>
    const defaultConfig = {
      site_title: 'Jane Designer',
      tagline: 'Creative Designer & Developer',
      hero_description: 'I create beautiful, functional digital experiences that solve real problems. Specializing in design systems and modern web applications that drive results.',
      about_title: 'About Me',
      about_description: 'With 8+ years of experience in digital design and development, I\'ve worked with startups to Fortune 500 companies to create impactful digital products that drive real business results.',
      services_title: 'What I Offer',
      cta_button: 'Get In Touch',
      footer_text: '© 2024 Portfolio. All rights reserved.'
    };

    // Initialize Element SDK
    window.elementSdk.init({
      defaultConfig,
      onConfigChange: async (config) => {
        document.getElementById('site-title').textContent = config.site_title || defaultConfig.site_title;
        document.getElementById('tagline').textContent = config.tagline || defaultConfig.tagline;
        document.getElementById('hero-description').textContent = config.hero_description || defaultConfig.hero_description;
        document.getElementById('about-title').textContent = config.about_title || defaultConfig.about_title;
        document.getElementById('about-description').textContent = config.about_description || defaultConfig.about_description;
        document.getElementById('services-title').textContent = config.services_title || defaultConfig.services_title;
        document.getElementById('cta-btn').textContent = config.cta_button || defaultConfig.cta_button;
        document.getElementById('nav-name').textContent = config.site_title || defaultConfig.site_title;
        document.getElementById('footer-text').textContent = config.footer_text || defaultConfig.footer_text;
      },
      mapToCapabilities: (config) => ({
        recolorables: [],
        borderables: [],
        fontEditable: undefined,
        fontSizeable: undefined
      }),
      mapToEditPanelValues: (config) => new Map([
        ['site_title', config.site_title || defaultConfig.site_title],
        ['tagline', config.tagline || defaultConfig.tagline],
        ['hero_description', config.hero_description || defaultConfig.hero_description],
        ['about_title', config.about_title || defaultConfig.about_title],
        ['about_description', config.about_description || defaultConfig.about_description],
        ['services_title', config.services_title || defaultConfig.services_title],
        ['cta_button', config.cta_button || defaultConfig.cta_button],
        ['footer_text', config.footer_text || defaultConfig.footer_text]
      ])
    });

    // Initialize Lucide icons
    lucide.createIcons();

    // Smooth scroll for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        const href = this.getAttribute('href');
        if (href === '#') return;
        e.preventDefault();
        const element = document.querySelector(href);
        if (element) {
          element.scrollIntoView({ behavior: 'smooth' });
        }
      });
    });

    // CTA button action
    document.getElementById('cta-btn').addEventListener('click', () => {
      const contactSection = document.getElementById('contact');
      contactSection.scrollIntoView({ behavior: 'smooth' });
    });
  </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9d9afe2a2354de4c',t:'MTc3MzA2ODg4My4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
