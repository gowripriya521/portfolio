# portfolio
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gaddam Gowri Priya | Full-Stack Developer</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
  
  <style>
    body {
      font-family: 'Plus Jakarta Sans', sans-serif;
      background-color: #06060a;
      color: #f3f4f6;
    }
    .font-mono {
      font-family: 'JetBrains Mono', monospace;
    }
    .glass {
      background: rgba(13, 14, 24, 0.7);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border: 1px solid rgba(255, 255, 255, 0.08);
    }
    .glass-card {
      background: rgba(17, 18, 34, 0.6);
      backdrop-filter: blur(12px);
      border: 1px solid rgba(255, 255, 255, 0.06);
      transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    }
    .glass-card:hover {
      border-color: rgba(99, 102, 241, 0.4);
      transform: translateY(-4px);
      box-shadow: 0 16px 32px -8px rgba(99, 102, 241, 0.15);
    }
    .gradient-text {
      background: linear-gradient(135deg, #a855f7 0%, #6366f1 50%, #06b6d4 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
    .badge-glow {
      box-shadow: 0 0 15px rgba(99, 102, 241, 0.2);
    }
  </style>
</head>
<body class="relative overflow-x-hidden selection:bg-indigo-500 selection:text-white">

  <!-- Interactive Background Canvas -->
  <canvas id="bg-canvas" class="fixed inset-0 pointer-events-none z-0"></canvas>

  <!-- Ambient Glow Orbs -->
  <div class="fixed top-1/4 -left-32 w-96 h-96 bg-purple-600/15 rounded-full blur-[120px] pointer-events-none z-0"></div>
  <div class="fixed bottom-1/4 -right-32 w-96 h-96 bg-cyan-600/15 rounded-full blur-[120px] pointer-events-none z-0"></div>

  <!-- Navigation Bar -->
  <nav class="fixed top-0 left-0 right-0 z-50 glass">
    <div class="max-w-6xl mx-auto px-6 h-20 flex items-center justify-between">
      <a href="#" class="flex items-center gap-3 group">
        <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-purple-600 to-indigo-500 flex items-center justify-center font-bold text-white shadow-lg shadow-indigo-500/25 group-hover:scale-105 transition-transform">
          GP
        </div>
        <span class="font-bold tracking-tight text-lg text-white group-hover:text-indigo-400 transition-colors">Gaddam Gowri Priya</span>
      </a>
      
      <div class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-300">
        <a href="#about" class="hover:text-white transition-colors">About</a>
        <a href="#skills" class="hover:text-white transition-colors">Skills</a>
        <a href="#projects" class="hover:text-white transition-colors">Projects</a>
        <a href="#journey" class="hover:text-white transition-colors">Journey</a>
        <a href="#contact" class="px-5 py-2.5 rounded-full bg-gradient-to-r from-purple-600 to-indigo-600 text-white font-semibold hover:shadow-lg hover:shadow-indigo-500/30 transition-all hover:scale-105">
          Get in Touch
        </a>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="relative z-10 pt-40 pb-24 md:pt-48 md:pb-32 px-6 max-w-6xl mx-auto">
    <div class="flex flex-col items-start gap-6">
      
      <!-- Status Badge -->
      <div class="inline-flex items-center gap-2.5 px-4 py-2 rounded-full glass border border-emerald-500/30 text-emerald-400 text-xs font-medium badge-glow">
        <span class="w-2 h-2 rounded-full bg-emerald-400 animate-ping"></span>
        <span>Open to Internships & Full-Time Opportunities</span>
      </div>

      <!-- Headline -->
      <h1 class="text-4xl sm:text-6xl md:text-7xl font-extrabold tracking-tight leading-[1.1]">
        Hi, I'm <span class="gradient-text">Gaddam Gowri Priya</span><br>
        <span class="text-gray-300 text-3xl sm:text-5xl md:text-6xl block mt-3">
          I am a <span id="typewriter" class="text-indigo-400 border-b-4 border-indigo-500 pb-1"></span>
        </span>
      </h1>

      <!-- Catchphrase -->
      <p class="max-w-2xl text-lg sm:text-xl text-gray-400 leading-relaxed font-normal">
        "Turning ideas into intelligent, scalable, and user-friendly applications through clean code and innovative technology."
      </p>

      <!-- Location Indicator -->
      <div class="flex items-center gap-2 text-sm text-gray-400">
        <i class="fa-solid fa-location-dot text-indigo-400"></i>
        <span>Madanapalle / Bangalore, India</span>
      </div>

      <!-- CTAs -->
      <div class="flex flex-wrap items-center gap-4 pt-4">
        <a href="https://github.com/gowripriya521" target="_blank" rel="noreferrer" class="px-7 py-3.5 rounded-xl bg-gradient-to-r from-purple-600 to-indigo-600 text-white font-semibold flex items-center gap-3 shadow-lg shadow-indigo-600/30 hover:shadow-indigo-600/50 hover:scale-105 transition-all">
          <i class="fa-brands fa-github text-lg"></i>
          <span>Explore My GitHub</span>
        </a>
        <a href="#contact" class="px-7 py-3.5 rounded-xl glass font-semibold text-gray-200 hover:text-white hover:border-gray-500 transition-all flex items-center gap-2">
          <i class="fa-regular fa-envelope"></i>
          <span>Contact Me</span>
        </a>
        <a href="#" id="resume-btn" class="px-6 py-3.5 rounded-xl glass font-semibold text-gray-300 hover:text-white transition-all flex items-center gap-2">
          <i class="fa-solid fa-download text-sm"></i>
          <span>Download Resume</span>
        </a>
      </div>

    </div>
  </section>

  <!-- About Me & Metric Highlights -->
  <section id="about" class="relative z-10 py-20 px-6 max-w-6xl mx-auto border-t border-white/5">
    <div class="grid grid-cols-1 md:grid-cols-12 gap-10 items-center">
      
      <div class="md:col-span-7 flex flex-col gap-6">
        <div class="flex items-center gap-2 text-indigo-400 text-xs font-bold uppercase tracking-wider font-mono">
          <span class="w-8 h-[2px] bg-indigo-500"></span>
          <span>About My Journey</span>
        </div>
        <h2 class="text-3xl sm:text-4xl font-bold tracking-tight text-white">
          Architecting Clean Code & Next-Gen Systems
        </h2>
        <div class="space-y-4 text-gray-300 leading-relaxed">
          <p>
            Hello! I'm <strong class="text-white">Gaddam Gowri Priya</strong>, a passionate Full-Stack Developer with a B.Tech background and an interest in building modern, scalable, and intelligent applications.
          </p>
          <p>
            I specialize in <strong class="text-indigo-300">Python, FastAPI, Pydantic AI, HTML, CSS, and JavaScript</strong>. I enjoy crafting robust backend architectures, designing REST APIs, implementing CRUD operations, and exploring AI-powered agent development.
          </p>
          <p class="text-gray-400">
            My engineering philosophy centers on clean, readable, and maintainable code, continuous learning, and transforming real-world problems into production-ready software solutions.
          </p>
        </div>
      </div>

      <div class="md:col-span-5 grid grid-cols-2 gap-4">
        <div class="glass-card p-6 rounded-2xl flex flex-col items-center justify-center text-center">
          <span class="text-3xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-purple-400 to-indigo-400">B.Tech</span>
          <span class="text-xs uppercase tracking-wider text-gray-400 font-mono mt-1">Foundation</span>
        </div>
        <div class="glass-card p-6 rounded-2xl flex flex-col items-center justify-center text-center">
          <span class="text-3xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-indigo-400 to-cyan-400">6+</span>
          <span class="text-xs uppercase tracking-wider text-gray-400 font-mono mt-1">Core Techs</span>
        </div>
        <div class="glass-card p-6 rounded-2xl flex flex-col items-center justify-center text-center">
          <span class="text-3xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-emerald-400">100%</span>
          <span class="text-xs uppercase tracking-wider text-gray-400 font-mono mt-1">Dedication</span>
        </div>
        <div class="glass-card p-6 rounded-2xl flex flex-col items-center justify-center text-center">
          <span class="text-3xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-emerald-400 to-purple-400">Async</span>
          <span class="text-xs uppercase tracking-wider text-gray-400 font-mono mt-1">Architecture</span>
        </div>
      </div>

    </div>
  </section>

  <!-- Skills Matrix -->
  <section id="skills" class="relative z-10 py-20 px-6 max-w-6xl mx-auto border-t border-white/5">
    <div class="flex flex-col items-center text-center mb-16">
      <div class="flex items-center gap-2 text-indigo-400 text-xs font-bold uppercase tracking-wider font-mono mb-3">
        <span class="w-8 h-[2px] bg-indigo-500"></span>
        <span>Capabilities</span>
        <span class="w-8 h-[2px] bg-indigo-500"></span>
      </div>
      <h2 class="text-3xl sm:text-4xl font-bold tracking-tight text-white">Core Skills & Tech Stack</h2>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      
      <!-- Backend & Databases -->
      <div class="glass-card p-8 rounded-2xl">
        <div class="flex items-center gap-3 mb-6">
          <div class="w-10 h-10 rounded-xl bg-purple-500/10 border border-purple-500/30 flex items-center justify-center text-purple-400">
            <i class="fa-solid fa-server text-lg"></i>
          </div>
          <h3 class="text-xl font-bold text-white">Backend & Databases</h3>
        </div>
        <div class="flex flex-wrap gap-2.5">
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">Python</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-indigo-500/10 border border-indigo-500/30 text-sm font-mono text-indigo-300">FastAPI</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">Pydantic</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">REST APIs</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">SQL</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-cyan-500/10 border border-cyan-500/30 text-sm font-mono text-cyan-300">PostgreSQL</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">Celery</span>
        </div>
      </div>

      <!-- AI & Intelligent Systems -->
      <div class="glass-card p-8 rounded-2xl">
        <div class="flex items-center gap-3 mb-6">
          <div class="w-10 h-10 rounded-xl bg-cyan-500/10 border border-cyan-500/30 flex items-center justify-center text-cyan-400">
            <i class="fa-solid fa-brain text-lg"></i>
          </div>
          <h3 class="text-xl font-bold text-white">AI & Intelligent Systems</h3>
        </div>
        <div class="flex flex-wrap gap-2.5">
          <span class="px-3.5 py-1.5 rounded-lg bg-cyan-500/10 border border-cyan-500/30 text-sm font-mono text-cyan-300">Pydantic AI</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">AI Agent Development</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-purple-500/10 border border-purple-500/30 text-sm font-mono text-purple-300">Tool Calling</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">API Integration</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">Prompt Engineering</span>
        </div>
      </div>

      <!-- Frontend & Developer Tools -->
      <div class="glass-card p-8 rounded-2xl">
        <div class="flex items-center gap-3 mb-6">
          <div class="w-10 h-10 rounded-xl bg-indigo-500/10 border border-indigo-500/30 flex items-center justify-center text-indigo-400">
            <i class="fa-solid fa-code text-lg"></i>
          </div>
          <h3 class="text-xl font-bold text-white">Frontend & Dev Tools</h3>
        </div>
        <div class="flex flex-wrap gap-2.5">
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">HTML5</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">CSS3</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">JavaScript</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">Git</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">GitHub</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">VS Code</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-orange-500/10 border border-orange-500/30 text-sm font-mono text-orange-300">Postman</span>
        </div>
      </div>

      <!-- Core Competencies -->
      <div class="glass-card p-8 rounded-2xl">
        <div class="flex items-center gap-3 mb-6">
          <div class="w-10 h-10 rounded-xl bg-emerald-500/10 border border-emerald-500/30 flex items-center justify-center text-emerald-400">
            <i class="fa-solid fa-shield-halved text-lg"></i>
          </div>
          <h3 class="text-xl font-bold text-white">Core Competencies</h3>
        </div>
        <div class="flex flex-wrap gap-2.5">
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">CRUD Operations</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">Data Validation</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">API Testing</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">Async Task Queues</span>
          <span class="px-3.5 py-1.5 rounded-lg bg-white/5 border border-white/10 text-sm font-mono text-gray-200">Algorithmic Problem Solving</span>
        </div>
      </div>

    </div>
  </section>

  <!-- Featured Architectures & Projects -->
  <section id="projects" class="relative z-10 py-20 px-6 max-w-6xl mx-auto border-t border-white/5">
    <div class="flex flex-col items-center text-center mb-16">
      <div class="flex items-center gap-2 text-indigo-400 text-xs font-bold uppercase tracking-wider font-mono mb-3">
        <span class="w-8 h-[2px] bg-indigo-500"></span>
        <span>Showcase</span>
        <span class="w-8 h-[2px] bg-indigo-500"></span>
      </div>
      <h2 class="text-3xl sm:text-4xl font-bold tracking-tight text-white">Featured Projects & Architecture</h2>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      
      <!-- Project 1 -->
      <div class="glass-card rounded-2xl overflow-hidden flex flex-col">
        <div class="h-44 bg-gradient-to-br from-purple-900/40 via-indigo-950/50 to-[#0b0c16] border-b border-white/10 p-6 flex flex-col justify-between">
          <div class="flex justify-between items-center">
            <span class="text-xs font-mono text-purple-400 uppercase tracking-wider">AI Engineering</span>
            <i class="fa-solid fa-robot text-purple-400 text-xl"></i>
          </div>
          <h3 class="text-xl font-bold text-white">Pydantic AI Agent & Tool Calling Engine</h3>
        </div>
        <div class="p-6 flex-1 flex flex-col justify-between">
          <p class="text-sm text-gray-300 leading-relaxed mb-6">
            Autonomous agent leveraging Pydantic AI for structured outputs, dynamic tool calling, and strict schema validation for LLM responses.
          </p>
          <div>
            <div class="flex flex-wrap gap-2 mb-6">
              <span class="px-2.5 py-1 bg-white/5 rounded text-xs font-mono text-gray-300">Pydantic AI</span>
              <span class="px-2.5 py-1 bg-white/5 rounded text-xs font-mono text-gray-300">Python</span>
              <span class="px-2.5 py-1 bg-white/5 rounded text-xs font-mono text-gray-300">LLM APIs</span>
            </div>
            <a href="https://github.com/gowripriya521" target="_blank" rel="noreferrer" class="text-indigo-400 text-sm font-semibold flex items-center gap-2 hover:gap-3 transition-all">
              <span>View Source on GitHub</span>
              <i class="fa-solid fa-arrow-right text-xs"></i>
            </a>
          </div>
        </div>
      </div>

      <!-- Project 2 -->
      <div class="glass-card rounded-2xl overflow-hidden flex flex-col">
        <div class="h-44 bg-gradient-to-br from-indigo-900/40 via-slate-950/50 to-[#0b0c16] border-b border-white/10 p-6 flex flex-col justify-between">
          <div class="flex justify-between items-center">
            <span class="text-xs font-mono text-indigo-400 uppercase tracking-wider">Backend Systems</span>
            <i class="fa-solid fa-network-wired text-indigo-400 text-xl"></i>
          </div>
          <h3 class="text-xl font-bold text-white">FastAPI Async CRUD API & PostgreSQL</h3>
        </div>
        <div class="p-6 flex-1 flex flex-col justify-between">
          <p class="text-sm text-gray-300 leading-relaxed mb-6">
            High-performance asynchronous REST API supporting complete CRUD operations, dependency injection, and PostgreSQL integration.
          </p>
          <div>
            <div class="flex flex-wrap gap-2 mb-6">
              <span class="px-2.5 py-1 bg-white/5 rounded text-xs font-mono text-gray-300">FastAPI</span>
              <span class="px-2.5 py-1 bg-white/5 rounded text-xs font-mono text-gray-300">PostgreSQL</span>
              <span class="px-2.5 py-1 bg-white/5 rounded text-xs font-mono text-gray-300">Pydantic</span>
            </div>
            <a href="https://github.com/gowripriya521" target="_blank" rel="noreferrer" class="text-indigo-400 text-sm font-semibold flex items-center gap-2 hover:gap-3 transition-all">
              <span>View Source on GitHub</span>
              <i class="fa-solid fa-arrow-right text-xs"></i>
            </a>
          </div>
        </div>
      </div>

      <!-- Project 3 -->
      <div class="glass-card rounded-2xl overflow-hidden flex flex-col">
        <div class="h-44 bg-gradient-to-br from-cyan-900/40 via-emerald-950/50 to-[#0b0c16] border-b border-white/10 p-6 flex flex-col justify-between">
          <div class="flex justify-between items-center">
            <span class="text-xs font-mono text-cyan-400 uppercase tracking-wider">Distributed Queues</span>
            <i class="fa-solid fa-gears text-cyan-400 text-xl"></i>
          </div>
          <h3 class="text-xl font-bold text-white">Async Task Worker with Celery</h3>
        </div>
        <div class="p-6 flex-1 flex flex-col justify-between">
          <p class="text-sm text-gray-300 leading-relaxed mb-6">
            Background task queue implementation utilizing Celery and message brokers to offload heavy compute operations away from the main API thread.
          </p>
          <div>
            <div class="flex flex-wrap gap-2 mb-6">
              <span class="px-2.5 py-1 bg-white/5 rounded text-xs font-mono text-gray-300">Celery</span>
              <span class="px-2.5 py-1 bg-white/5 rounded text-xs font-mono text-gray-300">Python</span>
              <span class="px-2.5 py-1 bg-white/5 rounded text-xs font-mono text-gray-300">Redis</span>
            </div>
            <a href="https://github.com/gowripriya521" target="_blank" rel="noreferrer" class="text-indigo-400 text-sm font-semibold flex items-center gap-2 hover:gap-3 transition-all">
              <span>View Source on GitHub</span>
              <i class="fa-solid fa-arrow-right text-xs"></i>
            </a>
          </div>
        </div>
      </div>

    </div>
  </section>

  <!-- Journey / Roadmap -->
  <section id="journey" class="relative z-10 py-20 px-6 max-w-4xl mx-auto border-t border-white/5">
    <div class="flex flex-col items-center text-center mb-16">
      <div class="flex items-center gap-2 text-indigo-400 text-xs font-bold uppercase tracking-wider font-mono mb-3">
        <span class="w-8 h-[2px] bg-indigo-500"></span>
        <span>Timeline</span>
        <span class="w-8 h-[2px] bg-indigo-500"></span>
      </div>
      <h2 class="text-3xl sm:text-4xl font-bold tracking-tight text-white">Developer Journey & Focus</h2>
    </div>

    <div class="space-y-8 relative before:absolute before:inset-0 before:left-8 md:before:left-1/2 before:w-[2px] before:bg-white/10">
      
      <!-- Timeline Node 1 -->
      <div class="relative flex flex-col md:flex-row items-start md:items-center gap-6">
        <div class="md:w-1/2 md:text-right order-2 md:order-1 pl-16 md:pl-0">
          <span class="text-xs font-mono text-purple-400">Current Frontier</span>
          <h4 class="text-lg font-bold text-white mt-1">AI Agents & Asynchronous Systems</h4>
          <p class="text-sm text-gray-400 mt-2">
            Developing AI agents with Pydantic AI, exploring function calling, and scaling backend workloads with Celery task queues.
          </p>
        </div>
        <div class="absolute left-6 md:left-1/2 -translate-x-1/2 w-5 h-5 rounded-full bg-purple-500 border-4 border-[#06060a] z-10 order-1"></div>
        <div class="md:w-1/2 order-3 pl-16 md:pl-8">
          <span class="px-3 py-1 rounded-full bg-purple-500/10 border border-purple-500/30 text-xs text-purple-300 font-mono">Present</span>
        </div>
      </div>

      <!-- Timeline Node 2 -->
      <div class="relative flex flex-col md:flex-row items-start md:items-center gap-6">
        <div class="md:w-1/2 md:text-right order-2 md:order-1 pl-16 md:pl-0">
          <span class="px-3 py-1 rounded-full bg-indigo-500/10 border border-indigo-500/30 text-xs text-indigo-300 font-mono">Milestone</span>
        </div>
        <div class="absolute left-6 md:left-1/2 -translate-x-1/2 w-5 h-5 rounded-full bg-indigo-500 border-4 border-[#06060a] z-10 order-1"></div>
        <div class="md:w-1/2 order-3 pl-16 md:pl-8">
          <span class="text-xs font-mono text-indigo-400">Backend Specialization</span>
          <h4 class="text-lg font-bold text-white mt-1">FastAPI & Relational Databases</h4>
          <p class="text-sm text-gray-400 mt-2">
            Mastered asynchronous endpoints, Pydantic data schemas, CRUD operations, and PostgreSQL queries.
          </p>
        </div>
      </div>

      <!-- Timeline Node 3 -->
      <div class="relative flex flex-col md:flex-row items-start md:items-center gap-6">
        <div class="md:w-1/2 md:text-right order-2 md:order-1 pl-16 md:pl-0">
          <span class="text-xs font-mono text-cyan-400">Engineering Base</span>
          <h4 class="text-lg font-bold text-white mt-1">B.Tech Degree</h4>
          <p class="text-sm text-gray-400 mt-2">
            Built strong computer science foundations, algorithmic problem-solving techniques, and foundational web concepts.
          </p>
        </div>
        <div class="absolute left-6 md:left-1/2 -translate-x-1/2 w-5 h-5 rounded-full bg-cyan-500 border-4 border-[#06060a] z-10 order-1"></div>
        <div class="md:w-1/2 order-3 pl-16 md:pl-8">
          <span class="px-3 py-1 rounded-full bg-cyan-500/10 border border-cyan-500/30 text-xs text-cyan-300 font-mono">Completed</span>
        </div>
      </div>

    </div>
  </section>

  <!-- Contact & Footer -->
  <section id="contact" class="relative z-10 py-24 px-6 max-w-4xl mx-auto border-t border-white/5">
    <div class="glass-card p-8 md:p-14 rounded-3xl text-center flex flex-col items-center">
      <div class="w-16 h-16 rounded-2xl bg-gradient-to-tr from-purple-600 to-indigo-600 flex items-center justify-center text-white text-2xl mb-6 shadow-xl shadow-indigo-600/30">
        <i class="fa-solid fa-paper-plane"></i>
      </div>
      <h2 class="text-3xl sm:text-4xl font-extrabold text-white tracking-tight">Let's Connect & Collaborate</h2>
      <p class="text-gray-400 max-w-xl mt-3 text-base">
        I'm actively seeking internships, learning opportunities, and full-time software engineering roles. My inbox is always open!
      </p>

      <!-- Copy Email Widget -->
      <div class="mt-8 flex items-center gap-3 p-2 rounded-xl bg-black/40 border border-white/10 max-w-md w-full justify-between">
        <span class="text-xs sm:text-sm text-gray-300 font-mono truncate px-3">gowripriyagaddam@gmail.com</span>
        <button id="copy-email" class="px-4 py-2 rounded-lg bg-indigo-600 hover:bg-indigo-500 text-white text-xs font-semibold flex items-center gap-2 transition-all">
          <i class="fa-regular fa-copy"></i>
          <span>Copy</span>
        </button>
      </div>

      <!-- Social Links -->
      <div class="flex items-center gap-4 mt-8">
        <a href="https://github.com/gowripriya521" target="_blank" rel="noreferrer" class="w-12 h-12 rounded-xl glass flex items-center justify-center text-gray-300 hover:text-white hover:border-gray-400 transition-all text-xl">
          <i class="fa-brands fa-github"></i>
        </a>
        <a href="https://www.linkedin.com/in/gaddamgowripriya/" target="_blank" rel="noreferrer" class="w-12 h-12 rounded-xl glass flex items-center justify-center text-gray-300 hover:text-white hover:border-indigo-400 transition-all text-xl">
          <i class="fa-brands fa-linkedin-in text-indigo-400"></i>
        </a>
        <a href="mailto:gowripriyagaddam@gmail.com" class="w-12 h-12 rounded-xl glass flex items-center justify-center text-gray-300 hover:text-white hover:border-cyan-400 transition-all text-xl">
          <i class="fa-regular fa-envelope text-cyan-400"></i>
        </a>
      </div>
    </div>

    <footer class="mt-16 text-center text-xs text-gray-500 font-mono">
      Designed & Built with ❤️ for Gaddam Gowri Priya • Powered by Clean Code
    </footer>
  </section>

  <!-- Interactive Script -->
  <script>
    // 1. Particle Background Network
    const canvas = document.getElementById('bg-canvas');
    const ctx = canvas.getContext('2d');
    let particles = [];

    function resize() {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    }
    window.addEventListener('resize', resize);
    resize();

    class Particle {
      constructor() {
        this.x = Math.random() * canvas.width;
        this.y = Math.random() * canvas.height;
        this.vx = (Math.random() - 0.5) * 0.4;
        this.vy = (Math.random() - 0.5) * 0.4;
        this.radius = Math.random() * 1.5 + 0.5;
      }
      update() {
        this.x += this.vx;
        this.y += this.vy;
        if (this.x < 0 || this.x > canvas.width) this.vx *= -1;
        if (this.y < 0 || this.y > canvas.height) this.vy *= -1;
      }
      draw() {
        ctx.beginPath();
        ctx.arc(this.x, this.y, this.radius, 0, Math.PI * 2);
        ctx.fillStyle = 'rgba(168, 85, 247, 0.4)';
        ctx.fill();
      }
    }

    const count = Math.min(window.innerWidth / 15, 60);
    for (let i = 0; i < count; i++) {
      particles.push(new Particle());
    }

    function animate() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      for (let i = 0; i < particles.length; i++) {
        particles[i].update();
        particles[i].draw();
        for (let j = i + 1; j < particles.length; j++) {
          const dx = particles[i].x - particles[j].x;
          const dy = particles[i].y - particles[j].y;
          const dist = Math.sqrt(dx * dx + dy * dy);
          if (dist < 110) {
            ctx.beginPath();
            ctx.moveTo(particles[i].x, particles[i].y);
            ctx.lineTo(particles[j].x, particles[j].y);
            ctx.strokeStyle = `rgba(99, 102, 241, ${0.15 * (1 - dist / 110)})`;
            ctx.stroke();
          }
        }
      }
      requestAnimationFrame(animate);
    }
    animate();

    // 2. Dynamic Typewriter Effect
    const words = [
      "Python Developer.",
      "Backend Developer.",
      "AI Application Developer.",
      "FastAPI Developer."
    ];
    let wordIdx = 0, charIdx = 0, isDeleting = false;
    const typewriterEl = document.getElementById('typewriter');

    function type() {
      const current = words[wordIdx];
      if (isDeleting) {
        typewriterEl.textContent = current.substring(0, charIdx - 1);
        charIdx--;
      } else {
        typewriterEl.textContent = current.substring(0, charIdx + 1);
        charIdx++;
      }

      let speed = isDeleting ? 40 : 80;

      if (!isDeleting && charIdx === current.length) {
        speed = 1800;
        isDeleting = true;
      } else if (isDeleting && charIdx === 0) {
        isDeleting = false;
        wordIdx = (wordIdx + 1) % words.length;
        speed = 400;
      }

      setTimeout(type, speed);
    }
    type();

    // 3. One-Click Copy Email
    document.getElementById('copy-email').addEventListener('click', function() {
      navigator.clipboard.writeText('gowripriyagaddam@gmail.com');
      const btn = this;
      btn.innerHTML = '<i class="fa-solid fa-check text-emerald-400"></i><span>Copied!</span>';
      setTimeout(() => {
        btn.innerHTML = '<i class="fa-regular fa-copy"></i><span>Copy</span>';
      }, 2000);
    });

    // 4. Resume Prompt
    document.getElementById('resume-btn').addEventListener('click', function(e) {
      e.preventDefault();
      alert('Resume file is ready to link. You can replace the href with your Google Drive or PDF link in index.html!');
    });
  </script>
</body>
</html>
