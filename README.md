<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Concienciación: Tráfico Ilegal de Vida Silvestre - Canelos, Pastaza</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&family=Playfair+Display:ital,wght@0,700;1,700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        jungle: {
                            50: '#f2f8f4',
                            100: '#e1eee5',
                            200: '#c5ddce',
                            300: '#9bc2ab',
                            400: '#6da184',
                            500: '#4b8466',
                            600: '#396a51',
                            700: '#2f5542',
                            800: '#284537',
                            900: '#223a2f',
                            950: '#11211b',
                        },
                        'amazon-gold': '#d4af37',
                        'amazon-crimson': '#8b0000',
                    },
                    fontFamily: {
                        sans: ['Outfit', 'sans-serif'],
                        serif: ['Playfair Display', 'serif'],
                    }
                }
            }
        }
    </script>
    <style>
        .glass-morphism {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        .hero-gradient {
            background: linear-gradient(rgba(17, 33, 27, 0.7), rgba(17, 33, 27, 0.9)), 
                        url('https://images.unsplash.com/photo-1518709268805-4e9042af9f23?q=80&w=2000&auto=format&fit=crop');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }
    </style>
</head>
<body class="bg-jungle-950 text-jungle-50 font-sans">

    <nav class="fixed w-full z-50 glass-morphism px-6 py-4 flex justify-between items-center">
        <div class="text-2xl font-extrabold tracking-tighter text-amazon-gold">CANELOS PRESERVA</div>
        <div class="hidden md:flex space-x-8 text-sm font-semibold uppercase tracking-widest">
            <a href="#inicio" class="hover:text-amazon-gold transition">Inicio</a>
            <a href="#problematica" class="hover:text-amazon-gold transition">Problemática</a>
            <a href="#leyes" class="hover:text-amazon-gold transition">Leyes</a>
            <a href="#reportar" class="bg-amazon-gold text-jungle-950 px-4 py-2 rounded-full hover:bg-white transition">Reportar</a>
        </div>
    </nav>

    <section id="inicio" class="hero-gradient min-h-screen flex items-center justify-center text-center px-4">
        <div class="max-w-4xl">
            <h1 class="font-serif text-5xl md:text-7xl mb-6 italic">Guardianes de la Selva</h1>
            <p class="text-xl md:text-2xl mb-8 font-light leading-relaxed">Protegiendo la biodiversidad de Canelos contra el tráfico ilegal de vida silvestre.</p>
            <div class="flex flex-col md:flex-row gap-4 justify-center">
                <a href="#problematica" class="border border-white/30 hover:bg-white hover:text-jungle-950 px-8 py-4 transition-all duration-300 uppercase text-xs tracking-widest font-bold">Descubrir la Realidad</a>
            </div>
        </div>
    </section>

    <section id="problematica" class="py-24 px-6 bg-white text-jungle-900">
        <div class="max-w-6xl mx-auto">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div>
                    <h2 class="text-4xl font-serif mb-8 text-jungle-800">Una Crisis Silenciosa</h2>
                    <p class="mb-6 leading-relaxed text-lg">El tráfico de especies en Pastaza no solo amenaza la supervivencia de animales emblemáticos, sino que desestabiliza todo el ecosistema amazónico que sostiene a la comunidad de Canelos.</p>
                    <div class="space-y-4">
                        <div class="flex items-center space-x-4">
                            <span class="text-3xl font-bold text-amazon-gold">80%</span>
                            <span class="text-sm font-semibold">De los animales mueren durante el transporte ilegal.</span>
                        </div>
                        <hr>
                        <div class="flex items-center space-x-4">
                            <span class="text-3xl font-bold text-amazon-gold">#3</span>
                            <span class="text-sm font-semibold">Tercer mercado ilegal más lucrativo del mundo.</span>
                        </div>
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-4">
                    <img src="https://images.unsplash.com/photo-1589182373726-e4f658ab50f0?q=80&w=600&auto=format&fit=crop" class="rounded-lg shadow-2xl mt-8" alt="Naturaleza">
                    <img src="https://images.unsplash.com/photo-1550461716-dbf266b2a8a7?q=80&w=600&auto=format&fit=crop" class="rounded-lg shadow-2xl" alt="Especies">
                </div>
            </div>
        </div>
    </section>

    <section class="py-20 bg-jungle-900 px-6">
        <div class="max-w-3xl mx-auto glass-morphism p-10 rounded-2xl text-center">
            <h3 class="text-2xl mb-6 font-serif italic text-amazon-gold">¿Sabías qué?</h3>
            <p id="quiz-text" class="text-xl mb-8">¿Es legal tener un loro amazónico como mascota si lo cuido bien?</p>
            <div class="flex justify-center space-x-4">
                <button onclick="checkAnswer(false)" class="bg-amazon-crimson px-8 py-3 rounded-full hover:scale-105 transition">NO es legal</button>
                <button onclick="checkAnswer(true)" class="bg-jungle-700 px-8 py-3 rounded-full hover:scale-105 transition">SÍ es legal</button>
            </div>
            <p id="feedback" class="mt-6 font-bold hidden"></p>
        </div>
    </section>

    <section id="leyes" class="py-24 px-6">
        <div class="max-w-6xl mx-auto text-center mb-16">
            <h2 class="text-4xl font-serif mb-4 italic">Marco Legal</h2>
            <div class="w-24 h-1 bg-amazon-gold mx-auto"></div>
        </div>
        <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
            <div class="p-8 border border-white/10 hover:border-amazon-gold transition">
                <h4 class="text-amazon-gold font-bold mb-4 uppercase text-sm">COIP Art. 247</h4>
                <p class="text-sm leading-relaxed">Sanciona con pena privativa de libertad de uno a tres años los delitos contra la flora y fauna silvestres.</p>
            </div>
            <div class="p-8 border border-white/10 hover:border-amazon-gold transition">
                <h4 class="text-amazon-gold font-bold mb-4 uppercase text-sm">Constitución Art. 71</h4>
                <p class="text-sm leading-relaxed">La naturaleza tiene derecho a que se respete integralmente su existencia y el mantenimiento de sus ciclos vitales.</p>
            </div>
            <div class="p-8 border border-white/10 hover:border-amazon-gold transition">
                <h4 class="text-amazon-gold font-bold mb-4 uppercase text-sm">Ley Ambiental</h4>
                <p class="text-sm leading-relaxed">Prohíbe estrictamente la captura, transporte y comercialización de especies nativas sin autorización.</p>
            </div>
        </div>
    </section>

    <section id="reportar" class="py-24 bg-jungle-50 text-jungle-950 px-6">
        <div class="max-w-4xl mx-auto">
            <div class="bg-white p-12 shadow-2xl rounded-sm">
                <h2 class="text-3xl font-serif mb-8 text-center italic">Denuncia el Tráfico Ilegal</h2>
                <form id="reportForm" onsubmit="handleSubmit(event)" class="space-y-6">
                    <div class="grid md:grid-cols-2 gap-6">
                        <input type="text" placeholder="Ubicación del incidente" class="w-full p-4 border-b-2 border-jungle-100 focus:border-amazon-gold outline-none transition" required>
                        <input type="text" placeholder="Especie involucrada (si se conoce)" class="w-full p-4 border-b-2 border-jungle-100 focus:border-amazon-gold outline-none transition">
                    </div>
                    <textarea placeholder="Describe lo que viste..." rows="4" class="w-full p-4 border-b-2 border-jungle-100 focus:border-amazon-gold outline-none transition" required></textarea>
                    <button type="submit" class="w-full bg-jungle-950 text-white py-4 font-bold uppercase tracking-widest hover:bg-amazon-gold transition duration-500">Enviar Reporte Anónimo</button>
                    <p id="formFeedback" class="text-center text-sm font-bold text-jungle-600 hidden">¡Gracias! Tu reporte ayuda a salvar vidas.</p>
                </form>
            </div>
        </div>
    </section>

    <footer class="py-12 border-t border-white/10 px-6 text-center text-xs tracking-widest text-jungle-400 uppercase">
        <p>&copy; 2026 Proyecto Concienciación Canelos - 3ro BGU "B"</p>
        <p class="mt-2 text-amazon-gold">David Maza</p>
    </footer>

    <script>
        // Quiz Logic
        function checkAnswer(isYes) {
            const feedback = document.getElementById('feedback');
            feedback.classList.remove('hidden');
            if (!isYes) {
                feedback.innerText = "¡Correcto! Es un delito penal en Ecuador. La vida silvestre pertenece a su hábitat.";
                feedback.classList.add('text-amazon-gold');
                feedback.classList.remove('text-amazon-crimson');
            } else {
                feedback.innerText = "Incorrecto. Capturar o comprar animales silvestres es ilegal y destruye la biodiversidad.";
                feedback.classList.add('text-amazon-crimson');
            }
        }

        // Form Submission
        function handleSubmit(event) {
            event.preventDefault();
            const form = document.getElementById('reportForm');
            const feedback = document.getElementById('formFeedback');
            
            form.querySelectorAll('input, textarea, button').forEach(el => el.disabled = true);
            feedback.classList.remove('hidden');
            form.classList.add('opacity-50');
            
            setTimeout(() => {
                alert('Simulación de reporte enviada con éxito. En un entorno real, esto se enviaría a las autoridades competentes (MAATE/UPMA).');
            }, 500);
        }

        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('opacity-100', 'translate-y-0');
                    entry.target.classList.remove('opacity-0', 'translate-y-10');
                }
            });
        }, observerOptions);

        document.querySelectorAll('section').forEach(section => {
            section.classList.add('transition-all', 'duration-1000', 'opacity-0', 'translate-y-10');
            observer.observe(section);
        });
    </script>
</body>
</html>
