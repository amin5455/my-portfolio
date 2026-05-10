<template>
  <div class="min-h-screen bg-slate-900 text-slate-100 font-sans selection:bg-cyan-500 selection:text-white">
    
    <nav class="fixed w-full z-50 backdrop-blur-md bg-slate-900/70 border-b border-slate-800">
      <div class="max-w-7xl mx-auto px-6 md:px-8 py-4 md:py-5 flex justify-between items-center">
        <div class="text-xl md:text-2xl font-black bg-gradient-to-r from-cyan-400 to-blue-500 bg-clip-text text-transparent tracking-tighter">
          AMIN<span class="text-white">.DEV</span>
        </div>

        <div class="hidden md:flex items-center space-x-10 text-xs font-bold uppercase tracking-widest text-slate-400">
          <a href="#work" class="hover:text-cyan-400 transition">Portfolio</a>
          <a href="#services" class="hover:text-cyan-400 transition">Services</a>
          <a href="mailto:amindvlpr5554@gmail.com" class="bg-cyan-600 hover:bg-cyan-500 text-white px-6 py-2.5 rounded-full transition-all duration-300 shadow-lg shadow-cyan-900/20">
            Hire Me
          </a>
        </div>

        <button @click="isMenuOpen = !isMenuOpen" class="md:hidden text-white focus:outline-none">
          <svg v-if="!isMenuOpen" xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
          </svg>
          <svg v-else xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </div>

      <div v-if="isMenuOpen" class="md:hidden bg-slate-900 border-b border-slate-800 px-8 py-6 space-y-4 animate-fade-in-down">
        <a href="#work" @click="isMenuOpen = false" class="block text-sm font-bold uppercase tracking-widest text-slate-400 hover:text-cyan-400">Portfolio</a>
        <a href="#services" @click="isMenuOpen = false" class="block text-sm font-bold uppercase tracking-widest text-slate-400 hover:text-cyan-400">Services</a>
        <a href="mailto:amindvlpr5554@gmail.com" class="block text-center bg-cyan-600 text-white py-3 rounded-xl font-bold uppercase tracking-widest text-xs">Hire Me</a>
      </div>
    </nav>

    <header class="pt-32 md:pt-48 pb-20 md:pb-32 px-6 md:px-8">
      <div class="max-w-7xl mx-auto flex flex-col-reverse md:flex-row items-center gap-12 md:gap-16">
        <div class="flex-1 space-y-6 md:space-y-8 text-center md:text-left">
          <h2 class="text-cyan-400 font-mono tracking-[0.3em] text-xs md:text-sm uppercase flex items-center justify-center md:justify-start gap-3">
            <span class="hidden md:block w-12 h-[1px] bg-cyan-500"></span> Available for Projects
          </h2>
          <h1 class="text-5xl md:text-8xl font-extrabold text-white leading-tight tracking-tighter">
            Full-Stack <br class="hidden md:block"> <span class="underline decoration-cyan-500">Web Architect.</span>
          </h1>
          <p class="text-lg md:text-xl text-slate-400 max-w-2xl leading-relaxed mx-auto md:mx-0">
            Expert in custom <span class="text-white font-medium">WordPress development</span> and high-performance <span class="text-white font-medium">Laravel & Vue 3</span> systems. Specializing in AI-integrated solutions.
          </p>
          <div class="flex flex-col sm:flex-row justify-center md:justify-start gap-4 md:gap-6">
            <a href="#work" class="px-8 md:px-10 py-4 md:py-5 bg-cyan-600 hover:shadow-[0_0_20px_rgba(8,145,178,0.4)] transition-all rounded-xl font-bold uppercase tracking-widest text-[10px] md:text-xs">View My Work</a>
            <a href="https://wa.me/923139347946" target="_blank" class="px-8 md:px-10 py-4 md:py-5 border border-slate-700 hover:bg-slate-800 transition rounded-xl font-bold uppercase tracking-widest text-[10px] md:text-xs">Quick Chat</a>
          </div>
        </div>
        
        <div class="relative group">
          <div class="w-64 h-64 md:w-96 md:h-96 rounded-2xl overflow-hidden border-2 border-cyan-500/50 rotate-3 md:group-hover:rotate-0 transition-transform duration-500 bg-slate-800 shadow-2xl">
            <img src="/public/am.png" alt="Amin Ali" class="object-cover w-full h-full">
          </div>
          <div class="absolute -bottom-6 -right-6 w-full h-full bg-cyan-500/10 rounded-full blur-3xl -z-10 animate-pulse"></div>
        </div>
      </div>
    </header>

    <section id="work" class="py-20 md:py-32 bg-slate-800/30 border-y border-slate-800 px-6 md:px-8">
      <div class="max-w-7xl mx-auto">
        <div class="mb-16 md:mb-20 text-center md:text-left">
          <h3 class="text-xs font-black text-cyan-500 uppercase tracking-[0.5em] mb-4">Case Studies</h3>
          <h4 class="text-3xl md:text-4xl font-black text-white italic">Featured Commercial Projects</h4>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 md:gap-10">
          
          <div class="group bg-slate-800 border border-slate-700 rounded-3xl p-8 md:p-10 hover:border-cyan-500 transition-all duration-500">
            <div class="flex justify-between items-start mb-8">
              <div class="flex gap-2">
                <span class="px-3 py-1 bg-cyan-500/10 text-cyan-400 text-[9px] font-black rounded border border-cyan-500/20 uppercase">WordPress</span>
                <span class="px-3 py-1 bg-white/5 text-slate-500 text-[9px] font-black rounded border border-white/10 uppercase">Vue.js</span>
              </div>
              <span class="text-3xl opacity-20 group-hover:opacity-100 transition">🚀</span>
            </div>
            <h5 class="text-2xl md:text-3xl font-black text-white mb-4">Nestly.site</h5>
            <p class="text-slate-400 mb-8 leading-relaxed text-sm md:text-base">Custom WordPress experience with ACF and a dedicated Vue.js dashboard for real estate management.</p>
            <a href="https://nestly.site" target="_blank" class="text-cyan-400 font-bold flex items-center gap-2 group-hover:gap-4 transition-all uppercase text-[10px] tracking-widest">Visit Project ↗</a>
          </div>

          <div class="group bg-slate-800 border border-slate-700 rounded-3xl p-8 md:p-10 hover:border-orange-500 transition-all duration-500">
            <div class="flex justify-between items-start mb-8">
              <div class="flex gap-2">
                <span class="px-3 py-1 bg-orange-500/10 text-orange-400 text-[9px] font-black rounded border border-orange-500/20 uppercase">WordPress</span>
                <span class="px-3 py-1 bg-white/5 text-slate-500 text-[9px] font-black rounded border border-white/10 uppercase">Medical</span>
              </div>
              <span class="text-3xl opacity-20 group-hover:opacity-100 transition">🏥</span>
            </div>
            <h5 class="text-2xl md:text-3xl font-black text-white mb-4">DocPortal</h5>
            <p class="text-slate-400 mb-8 leading-relaxed text-sm md:text-base">Specialized medical directory with custom post types and AJAX-powered booking systems.</p>
            <a href="http://docportal.42web.io/" target="_blank" class="text-orange-400 font-bold flex items-center gap-2 group-hover:gap-4 transition-all uppercase text-[10px] tracking-widest">Live Site ↗</a>
          </div>

          <div class="group bg-slate-800 border border-slate-700 rounded-3xl p-8 md:p-10 hover:border-blue-500 transition-all duration-500">
            <div class="flex justify-between items-start mb-8">
              <div class="flex gap-2">
                <span class="px-3 py-1 bg-blue-500/10 text-blue-400 text-[9px] font-black rounded border border-blue-500/20 uppercase">Laravel</span>
                <span class="px-3 py-1 bg-white/5 text-slate-500 text-[9px] font-black rounded border border-white/10 uppercase">SaaS</span>
              </div>
              <span class="text-3xl opacity-20 group-hover:opacity-100 transition">🏫</span>
            </div>
            <h5 class="text-2xl md:text-3xl font-black text-white mb-4">LMS</h5>
            <p class="text-slate-400 mb-8 leading-relaxed text-sm md:text-base">Comprehensive multi-school platform for stylist education and attendance management.</p>
            <a href="https://multischoolsystem.com/" target="_blank" class="text-blue-400 font-bold flex items-center gap-2 group-hover:gap-4 transition-all uppercase text-[10px] tracking-widest">Live Demo ↗</a>
          </div>

          <div class="group bg-slate-800 border border-slate-700 rounded-3xl p-8 md:p-10 hover:border-purple-500 transition-all duration-500">
            <div class="flex justify-between items-start mb-8">
              <div class="flex gap-2">
                <span class="px-3 py-1 bg-purple-500/10 text-purple-400 text-[9px] font-black rounded border border-purple-500/20 uppercase">Gemini AI</span>
                <span class="px-3 py-1 bg-white/5 text-slate-500 text-[9px] font-black rounded border border-white/10 uppercase">RAG</span>
              </div>
              <span class="text-3xl opacity-20 group-hover:opacity-100 transition">🤖</span>
            </div>
            <h5 class="text-2xl md:text-3xl font-black text-white mb-4">Smart Inventory</h5>
            <p class="text-slate-400 mb-8 leading-relaxed text-sm md:text-base">AI-driven natural language querying system for inventory assets using Gemini LLM.</p>
            <a href="https://youtu.be/F03SWFw1Iy4" target="_blank" class="text-purple-400 font-bold flex items-center gap-2 group-hover:gap-4 transition-all uppercase text-[10px] tracking-widest">Watch Showcase ↗</a>
          </div>
        </div>
      </div>
    </section>

    <section id="services" class="py-20 md:py-32 px-6 md:px-8">
      <div class="max-w-7xl mx-auto flex flex-col lg:flex-row gap-12 md:gap-20">
        <div class="lg:w-1/3 text-center lg:text-left">
          <h3 class="text-xs font-black text-cyan-500 uppercase tracking-[0.5em] mb-4">Services</h3>
          <h4 class="text-4xl md:text-5xl font-black text-white leading-tight italic mb-6">Performance <br class="hidden lg:block"> Guaranteed.</h4>
          <p class="text-slate-500 text-sm md:text-base">Focusing on custom code to keep websites fast and avoid heavy plugin bloat.</p>
        </div>
        <div class="lg:w-2/3 grid grid-cols-1 sm:grid-cols-2 gap-6">
          <div v-for="service in services" :key="service.title" class="p-8 md:p-10 border border-slate-800 rounded-3xl bg-slate-800/20 hover:border-slate-700 transition">
            <h6 class="text-white font-black text-lg md:text-xl mb-3">{{ service.title }}</h6>
            <p class="text-slate-500 text-xs md:text-sm leading-relaxed">{{ service.desc }}</p>
          </div>
        </div>
      </div>
    </section>

    <footer class="py-16 md:py-20 bg-slate-950 border-t border-slate-900 px-6 md:px-8">
      <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-10">
        <div class="text-center md:text-left">
          <h2 class="text-3xl md:text-4xl font-black text-white mb-2">Let's Build.</h2>
          <a href="mailto:amindvlpr5554@gmail.com" class="text-cyan-400 font-bold hover:text-white transition text-sm md:text-base">amindvlpr5554@gmail.com</a>
        </div>
        
        <div class="flex gap-6 md:gap-8 text-[9px] font-black uppercase tracking-[0.4em] text-slate-600">
          <a href="https://linkedin.com/in/amin-ali-6860753a8" target="_blank" class="hover:text-cyan-500 transition">LinkedIn</a>
          <a href="https://github.com/amin5455" target="_blank" class="hover:text-cyan-500 transition">GitHub</a>
        </div>
        
        <p class="text-[9px] font-black text-slate-800 uppercase tracking-widest text-center">© 2026 AMIN ALI &bull; ISLAMABAD</p>
      </div>
    </footer>

  </div>
</template>

<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

const services = [
  { title: 'WordPress Specialist', desc: 'Custom theme and plugin development focusing on speed and zero bloat.' },
  { title: 'Full-Stack Apps', desc: 'Enterprise-grade applications built with Laravel, Vue.js, and Inertia.' },
  { title: 'AI Integration', desc: 'Connecting businesses with Gemini LLMs for smart automation and data analysis.' },
  { title: 'E-commerce', desc: 'Bespoke shopping experiences tailored for high conversion and security.' }
]
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700;900&display=swap');

html { scroll-behavior: smooth; }
body { font-family: 'Inter', sans-serif; background-color: #0f172a; }

.animate-fade-in-down {
  animation: fadeInDown 0.3s ease-out;
}

@keyframes fadeInDown {
  0% { opacity: 0; transform: translateY(-10px); }
  100% { opacity: 1; transform: translateY(0); }
}
</style>