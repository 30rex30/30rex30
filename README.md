<!DOCTYPE html>
<html lang="pt" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Renato Bento — Developer & Builder</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    animation: {
                        'gradient-xy': 'gradientXY 15s ease infinite',
                        'float': 'float 6s ease-in-out infinite',
                    },
                    keyframes: {
                        gradientXY: {
                            '0%, 100%': {
                                'background-size': '400% 400%',
                                'background-position': 'left center'
                            },
                            '50%': {
                                'background-size': '400% 400%',
                                'background-position': 'right center'
                            }
                        },
                        float: {
                            '0%, 100%': { transform: 'translateY(0)' },
                            '50%': { transform: 'translateY(-10px)' },
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Gradiente animado de texto */
        .animated-gradient-text {
            background: linear-gradient(-45deg, #ff758c, #ff7eb3, #7928ca, #ff0080, #7928ca);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradientXY 8s ease infinite;
        }
        /* Brilho animado de fundo subtil */
        .animated-glow {
            background: linear-gradient(-45deg, rgba(121, 40, 202, 0.15), rgba(255, 0, 128, 0.15), rgba(0, 224, 255, 0.15));
            background-size: 400% 400%;
            animation: gradientXY 12s ease infinite;
        }
    </style>
</head>
<body class="bg-black text-zinc-100 min-h-screen flex flex-col justify-between selection:bg-zinc-800 selection:text-white font-sans antialiased relative overflow-x-hidden">

    <!-- Elemento de luz/cor animado no fundo -->
    <div class="absolute top-0 left-1/2 -translate-x-1/2 w-[600px] h-[300px] animated-glow blur-[120px] rounded-full pointer-events-none -z-10"></div>

    <!-- Main Container -->
    <main class="max-w-2xl mx-auto px-6 py-16 md:py-24 w-full space-y-12">

        <!-- Header / Bio -->
        <section class="space-y-4 animate-fade-in">
            <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full border border-zinc-800 bg-zinc-900/50 text-xs text-zinc-400 backdrop-blur-md">
                <span>🇵🇹 Portugal</span>
                <span class="w-1 h-1 rounded-full bg-emerald-500 animate-pulse"></span>
                <span>Available for new projects</span>
            </div>
            
            <h1 class="text-4xl md:text-5xl font-bold tracking-tight">
                Hi, I'm <span class="animated-gradient-text">Renato Bento</span> 👋
            </h1>
            
            <p class="text-lg text-zinc-400 font-medium">
                Developer & Builder focused on crafting exceptional digital experiences.
            </p>
        </section>

        <div class="h-px bg-gradient-to-r from-transparent via-zinc-800 to-transparent"></div>

        <!-- Overview -->
        <section class="space-y-4">
            <h2 class="text-xs font-mono uppercase tracking-widest text-zinc-500">Overview</h2>
            <div class="grid grid-cols-1 gap-3">
                <div class="p-4 rounded-xl border border-zinc-800/80 bg-zinc-900/30 hover:border-zinc-700 transition-all duration-300 flex items-center gap-4">
                    <span class="text-2xl">💻</span>
                    <div>
                        <h3 class="text-sm font-semibold text-zinc-200">Experience</h3>
                        <p class="text-sm text-zinc-400">3 years exploring and building software.</p>
                    </div>
                </div>

                <div class="p-4 rounded-xl border border-zinc-800/80 bg-zinc-900/30 hover:border-zinc-700 transition-all duration-300 flex items-center gap-4">
                    <span class="text-2xl">🚀</span>
                    <div>
                        <h3 class="text-sm font-semibold text-zinc-200">Focus</h3>
                        <p class="text-sm text-zinc-400">Clean code, mobile apps, and high-performance web solutions.</p>
                    </div>
                </div>

                <div class="p-4 rounded-xl border border-zinc-800/80 bg-zinc-900/30 hover:border-zinc-700 transition-all duration-300 flex items-center gap-4">
                    <span class="text-2xl">🤖</span>
                    <div>
                        <h3 class="text-sm font-semibold text-zinc-200">Workflow</h3>
                        <p class="text-sm text-zinc-400">Powered by modern AI tooling to ship faster and better.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Tech Stack -->
        <section class="space-y-4">
            <h2 class="text-xs font-mono uppercase tracking-widest text-zinc-500">Tech Stack</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                
                <div class="p-4 rounded-xl border border-zinc-800/80 bg-zinc-900/30 space-y-2">
                    <h3 class="text-xs font-mono text-zinc-400 uppercase">Frontend & Mobile</h3>
                    <p class="text-sm text-zinc-200 font-medium">React, React Native, Expo, JavaScript, TypeScript</p>
                </div>

                <div class="p-4 rounded-xl border border-zinc-800/80 bg-zinc-900/30 space-y-2">
                    <h3 class="text-xs font-mono text-zinc-400 uppercase">Backend & Systems</h3>
                    <p class="text-sm text-zinc-200 font-medium">PHP, C++, Supabase</p>
                </div>

                <div class="p-4 rounded-xl border border-zinc-800/80 bg-zinc-900/30 space-y-2">
                    <h3 class="text-xs font-mono text-zinc-400 uppercase">Workflow & AI</h3>
                    <p class="text-sm text-zinc-200 font-medium">Cursor, Claude, Git, VS Code</p>
                </div>

            </div>
        </section>

        <!-- Connect -->
        <section class="space-y-4">
            <h2 class="text-xs font-mono uppercase tracking-widest text-zinc-500">Connect</h2>
            <div class="flex flex-wrap gap-3">
                <a href="https://github.com/30rex30" target="_blank" class="px-4 py-2 rounded-lg border border-zinc-800 bg-zinc-900 hover:bg-zinc-800 hover:border-zinc-700 text-sm font-medium transition-all flex items-center gap-2">
                    <span>GitHub</span>
                    <span class="text-zinc-500 text-xs">@30rex30</span>
                </a>
                <a href="https://instagram.com/o_renatobento" target="_blank" class="px-4 py-2 rounded-lg border border-zinc-800 bg-zinc-900 hover:bg-zinc-800 hover:border-zinc-700 text-sm font-medium transition-all flex items-center gap-2">
                    <span>Instagram</span>
                    <span class="text-zinc-500 text-xs">@o_renatobento</span>
                </a>
            </div>
        </section>

        <!-- Quote -->
        <blockquote class="p-4 rounded-xl border border-dashed border-zinc-800 text-center text-zinc-400 text-sm italic">
            "Building things, learning every day."
        </blockquote>

    </main>

    <!-- Footer -->
    <footer class="max-w-2xl mx-auto px-6 py-8 w-full text-center text-xs text-zinc-600 border-t border-zinc-900">
        © 2026 Renato Bento. All rights reserved.
    </footer>

</body>
</html>
