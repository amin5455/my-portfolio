<template>
  <div class="min-h-screen bg-[#020617] text-slate-300 font-sans selection:bg-blue-500/30 p-4 md:p-8">
    
    <div class="fixed top-0 left-0 w-full h-full overflow-hidden pointer-events-none z-0">
      <div class="absolute top-[-10%] left-[-10%] w-[50%] h-[50%] bg-blue-600/10 blur-[140px] rounded-full animate-pulse"></div>
      <div class="absolute bottom-[-10%] right-[-10%] w-[40%] h-[40%] bg-indigo-600/10 blur-[140px] rounded-full"></div>
    </div>

    <div class="max-w-6xl mx-auto relative z-10">
      <header class="flex justify-between items-center mb-10">
        <div class="text-xl font-black tracking-tighter text-white group cursor-default">
          AMIN<span class="text-blue-500 underline decoration-2 underline-offset-4 group-hover:text-indigo-400 transition-colors">.DEV</span>
        </div>
        <div class="flex gap-4">
          <span class="px-3 py-1 bg-green-500/10 text-green-400 text-[10px] font-bold rounded-full border border-green-500/20 flex items-center gap-1 backdrop-blur-sm">
            <span class="w-1.5 h-1.5 bg-green-500 rounded-full animate-pulse"></span> Available for Work
          </span>
        </div>
      </header>

      <div class="grid grid-cols-1 md:grid-cols-4 gap-4 lg:gap-6">

        <div class="md:col-span-2 md:row-span-2 bg-slate-900/40 backdrop-blur-md border border-slate-800 rounded-[2.5rem] p-8 md:p-12 flex flex-col justify-between hover:border-blue-500/50 hover:-translate-y-2 hover:shadow-[0_20px_50px_rgba(59,130,246,0.1)] transition-all duration-700 group">
          <div>
            <div class="w-16 h-16 bg-gradient-to-br from-blue-600 to-indigo-600 rounded-2xl mb-8 flex items-center justify-center shadow-xl shadow-blue-500/20 group-hover:rotate-[15deg] transition-transform duration-500 italic font-black text-white text-3xl">
              A
            </div>
            <h1 class="text-4xl md:text-5xl lg:text-7xl font-black text-white leading-[1.05] tracking-tight">
              Full-Stack <br /> 
              <span class="text-transparent bg-clip-text bg-gradient-to-r from-blue-400 via-indigo-400 to-cyan-400">
                Web Architect
              </span>
            </h1>
            <p class="mt-8 text-slate-400 text-lg leading-relaxed max-w-md">
              Crafting high-performance ERPs and POS systems with <span class="text-white font-medium">Laravel & Vue 3</span>. Specialist in 
              <span class="text-blue-400 font-semibold underline decoration-blue-500/30 underline-offset-4">AI-Driven Applications</span>.
            </p>
          </div>
          
          <div class="mt-12 flex flex-wrap gap-4">
            <a href="/amin-cv.pdf" download="amin-cv.pdf"
              class="bg-white text-black px-8 py-4 rounded-2xl font-bold hover:bg-blue-500 hover:text-white transition-all duration-500 active:scale-95 shadow-xl flex items-center gap-2 text-sm">
              <span>Download CV</span>
              <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16l5 5m0 0l5-5m-5 5V3"></path>
              </svg>
            </a>
            
            <a href="https://github.com/amin5455" target="_blank"
              class="flex items-center gap-4 bg-slate-800/40 backdrop-blur-md border border-slate-700 hover:border-blue-500/50 p-4 px-6 rounded-2xl transition-all group shadow-lg">
              <svg class="w-7 h-7 fill-white group-hover:scale-110 transition-transform" viewBox="0 0 24 24">
                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.041-1.412-4.041-1.412-.546-1.387-1.333-1.756-1.333-1.756-1.089-.744.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z" />
              </svg>
              <div class="text-left">
                <div class="text-white font-bold text-sm group-hover:text-blue-400 transition">@amin5455</div>
                <div class="text-slate-500 text-[10px] uppercase font-black tracking-[0.2em]">Engineer</div>
              </div>
            </a>
          </div>
        </div>

        <div class="md:col-span-2 bg-slate-900/40 backdrop-blur-md border border-slate-800 rounded-[2.5rem] p-8 hover:border-slate-600 transition-all group">
          <h3 class="text-xs font-bold uppercase tracking-widest text-slate-500 mb-8 flex items-center gap-2">
            <span class="w-4 h-[1px] bg-slate-700"></span> Expert Stack
          </h3>
          <div class="flex flex-wrap gap-3">
            <span v-for="tech in ['Laravel', 'PHP 8.x', 'Vue 3', 'Tailwind', 'MySQL', 'Inertia.js', 'Git', 'Ajax', 'REST APIs']" :key="tech"
              class="px-5 py-2.5 bg-[#020617]/80 border border-slate-800 rounded-2xl text-sm font-semibold text-slate-400 hover:border-blue-500/50 hover:text-white hover:scale-105 hover:bg-blue-500/5 transition-all cursor-default">
              {{ tech }}
            </span>
          </div>
        </div>

        <div class="md:col-span-2 bg-gradient-to-br from-blue-900/30 to-slate-900/80 backdrop-blur-lg border border-slate-800 rounded-[2.5rem] p-8 relative overflow-hidden group hover:border-blue-500/60 hover:-translate-y-2 transition-all duration-700 shadow-2xl shadow-blue-500/5">
          <div class="relative z-10 flex flex-col h-full justify-between">
            <div>
              <div class="flex justify-between items-start mb-6">
                <div class="text-5xl group-hover:rotate-12 transition-transform duration-500">🛒</div>
                <div class="flex items-center gap-2 px-3 py-1.5 bg-blue-500/20 border border-blue-500/40 rounded-full text-[10px] text-blue-300 font-black uppercase tracking-widest animate-pulse">
                  <span class="w-2 h-2 bg-blue-400 rounded-full shadow-[0_0_8px_rgba(96,165,250,0.8)]"></span>
                  Gemini AI Integrated
                </div>
              </div>
              <h3 class="text-3xl font-black text-white mb-3 tracking-tight italic">Smart Inventory & AI-POS</h3>
              <p class="text-slate-400 text-base leading-relaxed mb-8">
                Revolutionizing stock management with <span class="text-blue-400 font-bold">Natural Language Querying (RAG)</span>. Interrogate your data like a human expert.
              </p>
              <div class="flex flex-wrap gap-2 mb-10">
                <span class="text-[10px] bg-blue-500/5 text-blue-400/80 px-3 py-1.5 rounded-lg border border-blue-500/20 font-bold">LLM Implementation</span>
                <span class="text-[10px] bg-slate-800/80 text-slate-400 px-3 py-1.5 rounded-lg border border-slate-700">Real-time Stock</span>
              </div>
            </div>
            <div class="flex flex-col sm:flex-row gap-4">
              <a href="https://youtu.be/F03SWFw1Iy4" target="_blank"
                class="flex-1 flex items-center justify-center gap-3 bg-red-600 hover:bg-red-700 text-white px-6 py-4 rounded-2xl font-black text-sm transition-all active:scale-95 shadow-lg shadow-red-600/30 group/btn">
                <svg class="w-6 h-6 group-hover/btn:scale-125 transition-transform" fill="currentColor" viewBox="0 0 24 24"><path d="M23.498 6.186a3.016 3.016 0 0 0-2.122-2.136C19.505 3.545 12 3.545 12 3.545s-7.505 0-9.377.505A3.017 3.017 0 0 0 .502 6.186C0 8.07 0 12 0 12s0 3.93.502 5.814a3.016 3.016 0 0 0 2.122 2.136c1.871.505 9.376.505 9.376.505s7.505 0 9.377-.505a3.015 3.015 0 0 0 2.122-2.136C24 15.93 24 12 24 12s0-3.93-.502-5.814zM9.545 15.568V8.432L15.818 12l-6.273 3.568z"/></svg>
                Watch AI Demo
              </a>
              <a href="https://github.com/amin5455" target="_blank"
                class="px-6 py-4 bg-slate-800 hover:bg-slate-700 text-white rounded-2xl transition-all flex items-center justify-center border border-slate-700 shadow-xl">
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg>
              </a>
            </div>
          </div>
          <div class="absolute -right-6 -bottom-6 w-40 h-40 bg-blue-600/10 blur-3xl rounded-full group-hover:bg-blue-600/30 transition-all duration-1000"></div>
        </div>

        <div class="md:col-span-2 bg-[#0a1120]/60 backdrop-blur-md border border-blue-500/10 rounded-[2.5rem] p-10 group relative overflow-hidden hover:border-blue-500/40 hover:-translate-y-2 transition-all duration-700 shadow-2xl">
          <div class="absolute top-0 right-0 p-8">
            <a href="https://multischoolsystem.com/" target="_blank"
              class="bg-blue-600/10 hover:bg-blue-600 border border-blue-500/30 text-blue-400 hover:text-white px-5 py-2.5 rounded-full transition-all flex items-center justify-center backdrop-blur-md shadow-lg group/demo">
              <span class="text-[10px] font-black uppercase tracking-[0.2em] group-hover/demo:scale-105 transition-transform">Live System ↗</span>
            </a>
          </div>
          <div class="mb-6 text-4xl">🏫</div>
          <h3 class="text-3xl font-black text-white mb-4">Enterprise School SaaS</h3>
          <p class="text-slate-400 text-base mb-8 leading-relaxed max-w-sm">
            High-scale management platform for Attendance, Fee Portals, and Exams. Engineered for heavy data using
            <span class="text-blue-400 font-bold">Laravel & MySQL Optimization</span>.
          </p>
          <div class="flex flex-wrap gap-3 text-[10px] font-black uppercase tracking-widest">
            <span class="bg-slate-800/80 text-slate-400 px-4 py-2 rounded-xl border border-slate-700">Financial Ledger</span>
            <span class="bg-slate-800/80 text-slate-400 px-4 py-2 rounded-xl border border-slate-700">Exam SaaS</span>
          </div>
        </div>

        <div class="md:col-span-1 bg-gradient-to-b from-slate-900 to-indigo-950/40 backdrop-blur-md border border-slate-800 rounded-[2.5rem] p-8 group hover:border-indigo-500/50 hover:-translate-y-2 transition-all duration-500">
          <div class="flex flex-col h-full justify-between">
            <div>
              <div class="text-4xl mb-6 group-hover:scale-125 transition-transform duration-500">🎙️</div>
              <h4 class="text-xl font-bold text-white mb-3 tracking-tight">Voice Bill Calc</h4>
              <p class="text-slate-500 text-sm leading-relaxed">Flutter application utilizing Speech-to-Text for ultra-fast retail billing.</p>
            </div>
            <div class="mt-8">
              <span class="text-[9px] text-indigo-400 font-black tracking-[0.2em] uppercase bg-indigo-500/10 px-3 py-1.5 rounded-lg border border-indigo-500/20">Flutter Mobile</span>
            </div>
          </div>
        </div>

        <div class="md:col-span-1 bg-slate-900/40 backdrop-blur-md border border-slate-800 rounded-[2.5rem] p-8 flex flex-col justify-center items-center text-center group hover:border-slate-500 hover:-translate-y-2 transition-all duration-500">
          <div class="text-blue-500 text-4xl mb-4 group-hover:animate-bounce transition-transform">💻</div>
          <div class="text-2xl font-black text-white tracking-tight italic">Always Coding</div>
          <div class="text-[10px] text-slate-500 uppercase mt-2 font-black tracking-[0.3em]">Pure Consistency</div>
        </div>

        <div class="bg-slate-900/40 backdrop-blur-md border border-slate-800 rounded-[2.5rem] p-8 flex flex-col items-center justify-center text-center hover:bg-slate-800 hover:-translate-y-2 transition-all duration-500">
          <div class="text-4xl font-black text-white">01+</div>
          <div class="text-[10px] text-slate-500 uppercase font-black mt-2 tracking-widest">Year Exp.</div>
        </div>

        <div class="bg-slate-900/40 backdrop-blur-md border border-slate-800 rounded-[2.5rem] p-8 flex flex-col items-center justify-center text-center hover:bg-slate-800 hover:-translate-y-2 transition-all duration-500">
          <div class="text-4xl font-black text-white italic">100%</div>
          <div class="text-[10px] text-slate-500 uppercase font-black mt-2 tracking-widest">Clean Code</div>
        </div>

      </div>

      <section class="mt-20 mb-16">
        <div class="bg-gradient-to-r from-blue-900/10 to-indigo-900/10 backdrop-blur-xl border border-slate-800 rounded-[4rem] p-10 md:p-20 text-center relative overflow-hidden group hover:border-blue-500/30 transition-all duration-1000 shadow-2xl">
          <div class="absolute inset-0 bg-blue-500/5 opacity-0 group-hover:opacity-100 transition-opacity duration-1000"></div>
          <div class="relative z-10">
            <h2 class="text-4xl md:text-6xl font-black text-white mb-8 tracking-tighter">Let's build something <span class="text-blue-500 italic">extraordinary</span>.</h2>
            <p class="text-slate-400 text-xl mb-12 max-w-2xl mx-auto leading-relaxed">
              Available for <span class="text-white font-bold border-b border-blue-500/50">Full-Stack Laravel/Vue</span> roles. 
              Turning complex logic into elegant solutions.
            </p>
            <div class="flex flex-wrap justify-center gap-6">
              <a href="mailto:amindvlpr5554@gmail.com" class="bg-blue-600 hover:bg-blue-700 text-white px-12 py-5 rounded-3xl font-black transition-all transform active:scale-90 shadow-[0_15px_30px_rgba(37,99,235,0.3)] flex items-center gap-3">
                <span>Hire Me Now</span>
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
              </a>
              <a href="https://wa.me/923139347946" target="_blank" class="bg-slate-800/80 border border-slate-700 text-white px-12 py-5 rounded-3xl font-black hover:bg-slate-700 transition-all flex items-center gap-3 backdrop-blur-md">
                <span>Quick Chat</span>
                <svg class="w-6 h-6 text-green-500" fill="currentColor" viewBox="0 0 24 24"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413Z"/></svg>
              </a>
            </div>
            <div class="mt-16 flex justify-center gap-12 text-slate-500 font-black text-xs tracking-[0.4em] uppercase">
              <a href="https://linkedin.com/in/amin-ali-6860753a8" target="_blank" class="hover:text-blue-500 transition-colors">LinkedIn</a>
              <a href="https://github.com/amin5455" target="_blank" class="hover:text-white transition-colors">GitHub</a>
            </div>
          </div>
        </div>
      </section>

      <footer class="pb-12 text-center text-slate-500 text-[10px] uppercase tracking-[0.5em] font-black opacity-40">
        &copy; 2026 Amin Ali &bull; Engineering with Laravel & Vue 3
      </footer>
    </div>
  </div>
</template>

<style>
/* Global Smoothness */
* {
  transition-timing-function: cubic-bezier(0.23, 1, 0.32, 1);
}

/* Scrollbar Style */
::-webkit-scrollbar {
  width: 6px;
}
::-webkit-scrollbar-track {
  background: #020617;
}
::-webkit-scrollbar-thumb {
  background: #1e293b;
  border-radius: 10px;
}
::-webkit-scrollbar-thumb:hover {
  background: #3b82f6;
}
</style>