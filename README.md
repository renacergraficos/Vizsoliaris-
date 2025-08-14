# Vizsoliaris-
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vis Solaris - Diseño Gráfico y Marketing Digital</title>
    <meta name="description" content="Agencia de diseño gráfico y marketing digital. Creatividad sin límites para tu marca.">
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'vis-red': '#DC2626',
                        'vis-black': '#1F2937'
                    }
                }
            }
        }
    </script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <!-- Threads icon CDN (Bootstrap Icons) -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        body { font-family: 'Inter', sans-serif; }
        .gradient-bg { background: linear-gradient(135deg, #DC2626 0%, #1F2937 100%); }
        .live-indicator { animation: pulse 2s infinite; }
        @keyframes pulse { 0% { opacity: 1; } 50% { opacity: 0.5; } 100% { opacity: 1; } }
        .fade-in { opacity: 0; transform: translateY(30px); animation: fadeInUp 0.8s ease-out forwards; }
        .fade-in-delay-1 { animation-delay: 0.2s; }
        .fade-in-delay-2 { animation-delay: 0.4s; }
        .fade-in-delay-3 { animation-delay: 0.6s; }
        @keyframes fadeInUp { to { opacity: 1; transform: translateY(0); } }
        .float { animation: float 3s ease-in-out infinite; }
        @keyframes float { 0%,100% { transform: translateY(0px);} 50% { transform: translateY(-10px);} }
        .slide-in-left { opacity: 0; transform: translateX(-50px); animation: slideInLeft 0.8s ease-out forwards;}
        .slide-in-right { opacity: 0; transform: translateX(50px); animation: slideInRight 0.8s ease-out forwards;}
        @keyframes slideInLeft { to { opacity: 1; transform: translateX(0); } }
        @keyframes slideInRight { to { opacity: 1; transform: translateX(0); } }
        .scale-in { opacity: 0; transform: scale(0.8); animation: scaleIn 0.6s ease-out forwards;}
        @keyframes scaleIn { to { opacity: 1; transform: scale(1); } }
        .hover-lift { transition: transform 0.3s ease, box-shadow 0.3s ease; }
        .hover-lift:hover { transform: translateY(-5px); box-shadow: 0 15px 35px rgba(0,0,0,0.1);}
        .glow { animation: glow 2s ease-in-out infinite alternate;}
        @keyframes glow { from { box-shadow: 0 0 20px rgba(220, 38, 38, 0.3);} to { box-shadow: 0 0 30px rgba(220, 38, 38, 0.6);} }
    </style>
</head>
<body class="bg-white text-vis-black">

    <!-- Botón flotante de WhatsApp -->
    <a href="https://wa.me/qr/SXKYVC4CN6KCA1" target="_blank" rel="noopener noreferrer"
       class="fixed bottom-6 right-6 bg-green-500 hover:bg-green-600 text-white p-4 rounded-full shadow-lg z-50 flex items-center justify-center"
       aria-label="Chatea por WhatsApp">
        <i class="fab fa-whatsapp text-2xl"></i>
    </a>

    <!-- Header -->
    <header class="bg-white shadow-lg sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="text-2xl font-bold text-vis-red">
                    VIS SOLARIS
                    <span class="text-sm text-gray-600 block">2025</span>
                </div>
                <div class="hidden md:flex space-x-8" id="main-menu">
                    <a href="#servicios" class="text-vis-black hover:text-vis-red transition">Servicios</a>
                    <a href="#portafolio" class="text-vis-black hover:text-vis-red transition">Portafolio</a>
                    <a href="#live" class="text-vis-black hover:text-vis-red transition">En Vivo</a>
                    <a href="#contacto" class="text-vis-black hover:text-vis-red transition">Contacto</a>
                </div>
                <button class="md:hidden text-vis-black" id="mobile-menu-btn" aria-label="Abrir menú">
                    <i class="fas fa-bars text-xl"></i>
                </button>
            </div>
            <!-- Menú móvil -->
            <div class="md:hidden" id="mobile-menu" style="display:none;">
                <a href="#servicios" class="block py-2 text-vis-black hover:text-vis-red transition">Servicios</a>
                <a href="#portafolio" class="block py-2 text-vis-black hover:text-vis-red transition">Portafolio</a>
                <a href="#live" class="block py-2 text-vis-black hover:text-vis-red transition">En Vivo</a>
                <a href="#contacto" class="block py-2 text-vis-black hover:text-vis-red transition">Contacto</a>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <main>
    <section class="gradient-bg text-white py-20">
        <div class="container mx-auto px-6 text-center">
            <h1 class="text-5xl md:text-6xl font-bold mb-6 fade-in">VIS SOLARIS</h1>
            <p class="text-xl md:text-2xl mb-8 opacity-90 fade-in fade-in-delay-1">Diseño Gráfico • Marketing Digital • Creatividad Sin Límites</p>
            <div class="flex flex-wrap justify-center gap-4 mb-8 fade-in fade-in-delay-2">
                <span class="bg-white/20 px-4 py-2 rounded-full hover-lift">Diseño Gráfico</span>
                <span class="bg-white/20 px-4 py-2 rounded-full hover-lift">Diseño Web</span>
                <span class="bg-white/20 px-4 py-2 rounded-full hover-lift">Marketing Digital</span>
                <span class="bg-white/20 px-4 py-2 rounded-full hover-lift">Community Manager</span>
            </div>
            <a href="#contacto">
                <button class="bg-white text-vis-red px-8 py-3 rounded-lg font-semibold hover:bg-gray-100 transition fade-in fade-in-delay-3 glow">
                    Comenzar Proyecto
                </button>
            </a>
        </div>
    </section>

    <!-- Live Section -->
    <section id="live" class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center mb-12 fade-in">🔴 Estamos EN VIVO</h2>
            <div class="grid md:grid-cols-2 gap-8 max-w-4xl mx-auto">
                <div class="bg-white rounded-lg shadow-lg p-6 text-center hover-lift slide-in-left">
                    <div class="live-indicator bg-vis-red text-white px-3 py-1 rounded-full text-sm mb-4 inline-block">
                        <i class="fas fa-circle text-xs mr-1" aria-hidden="true"></i> EN VIVO
                    </div>
                    <i class="fab fa-tiktok text-4xl text-black mb-4 float" aria-label="TikTok"></i>
                    <h3 class="text-xl font-semibold mb-2">TikTok Live</h3>
                    <p class="text-gray-600 mb-4">Únete a nuestras transmisiones en vivo</p>
                    <a href="https://www.tiktok.com/@graphicpizzeria" rel="noopener noreferrer" target="_blank" 
                       class="bg-black text-white px-6 py-2 rounded-lg hover:bg-gray-800 transition">
                        Ver en TikTok
                    </a>
                </div>
                <div class="bg-white rounded-lg shadow-lg p-6 text-center hover-lift slide-in-right">
                    <div class="live-indicator bg-vis-red text-white px-3 py-1 rounded-full text-sm mb-4 inline-block">
                        <i class="fas fa-circle text-xs mr-1" aria-hidden="true"></i> EN VIVO
                    </div>
                    <i class="fab fa-instagram text-4xl text-pink-600 mb-4 float" aria-label="Instagram"></i>
                    <h3 class="text-xl font-semibold mb-2">Instagram Live</h3>
                    <p class="text-gray-600 mb-4">Contenido exclusivo y tutoriales</p>
                    <a href="https://www.instagram.com/graphicpizzeria/" rel="noopener noreferrer" target="_blank" 
                       class="bg-gradient-to-r from-purple-500 to-pink-500 text-white px-6 py-2 rounded-lg hover:opacity-90 transition">
                        Ver en Instagram
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="servicios" class="py-16">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center mb-12 fade-in">Nuestros Servicios</h2>
            <div class="grid md:grid-cols-3 lg:grid-cols-4 gap-6">
                <div class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition text-center hover-lift scale-in">
                    <i class="fas fa-palette text-3xl text-vis-red mb-4 float" aria-label="Diseño Gráfico"></i>
                    <h3 class="font-semibold mb-2">Diseño Gráfico</h3>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition text-center hover-lift scale-in">
                    <i class="fas fa-code text-3xl text-vis-red mb-4 float" aria-label="Diseño Web"></i>
                    <h3 class="font-semibold mb-2">Diseño Web</h3>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition text-center hover-lift scale-in">
                    <i class="fas fa-book text-3xl text-vis-red mb-4 float" aria-label="Diseño Editorial"></i>
                    <h3 class="font-semibold mb-2">Diseño Editorial</h3>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition text-center hover-lift scale-in">
                    <i class="fas fa-chart-line text-3xl text-vis-red mb-4 float" aria-label="Marketing Digital"></i>
                    <h3 class="font-semibold mb-2">Marketing Digital</h3>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition text-center hover-lift scale-in">
                    <i class="fas fa-bullhorn text-3xl text-vis-red mb-4 float" aria-label="Publicidad"></i>
                    <h3 class="font-semibold mb-2">Publicidad</h3>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition text-center hover-lift scale-in">
                    <i class="fas fa-users text-3xl text-vis-red mb-4 float" aria-label="Community Manager"></i>
                    <h3 class="font-semibold mb-2">Community Manager</h3>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition text-center hover-lift scale-in">
                    <i class="fas fa-camera text-3xl text-vis-red mb-4 float" aria-label="Creación de Contenido"></i>
                    <h3 class="font-semibold mb-2">Creación de Contenido</h3>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition text-center hover-lift scale-in">
                    <i class="fas fa-video text-3xl text-vis-red mb-4 float" aria-label="Video Marketing"></i>
                    <h3 class="font-semibold mb-2">Video Marketing</h3>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition text-center hover-lift scale-in">
                    <i class="fas fa-graduation-cap text-3xl text-vis-red mb-4 float" aria-label="Curso"></i>
                    <h3 class="font-semibold mb-2">Curso</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portafolio" class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center mb-12 fade-in">Portafolio en Línea</h2>
            <div class="grid md:grid-cols-3 lg:grid-cols-6 gap-6 max-w-6xl mx-auto">
                <a href="https://www.behance.net/pizzeriagraficas" rel="noopener noreferrer" target="_blank" 
                   class="bg-white rounded-lg shadow-lg p-6 text-center hover:shadow-xl transition hover-lift scale-in" aria-label="Portafolio Behance">
                    <i class="fab fa-behance text-4xl text-blue-600 mb-4 float" aria-hidden="true"></i>
                    <h3 class="text-xl font-semibold mb-2">Behance</h3>
                    <p class="text-gray-600">Portafolio completo</p>
                </a>
                <a href="https://www.tiktok.com/@graphicpizzeria" rel="noopener noreferrer" target="_blank" 
                   class="bg-white rounded-lg shadow-lg p-6 text-center hover:shadow-xl transition hover-lift scale-in" aria-label="Portafolio TikTok">
                    <i class="fab fa-tiktok text-4xl text-black mb-4 float" aria-hidden="true"></i>
                    <h3 class="text-xl font-semibold mb-2">TikTok</h3>
                    <p class="text-gray-600">Contenido creativo</p>
                </a>
                <a href="https://www.instagram.com/graphicpizzeria/" rel="noopener noreferrer" target="_blank" 
                   class="bg-white rounded-lg shadow-lg p-6 text-center hover:shadow-xl transition hover-lift scale-in" aria-label="Portafolio Instagram">
                    <i class="fab fa-instagram text-4xl text-pink-600 mb-4 float" aria-hidden="true"></i>
                    <h3 class="text-xl font-semibold mb-2">Instagram</h3>
                    <p class="text-gray-600">Proceso creativo</p>
                </a>
                <a href="#" target="_blank" 
                   class="bg-white rounded-lg shadow-lg p-6 text-center hover:shadow-xl transition hover-lift scale-in" aria-label="Portafolio Facebook">
                    <i class="fab fa-facebook text-4xl text-blue-700 mb-4 float" aria-hidden="true"></i>
                    <h3 class="text-xl font-semibold mb-2">Facebook</h3>
                    <p class="text-gray-600">Comunidad activa</p>
                </a>
                <a href="#" target="_blank" 
                   class="bg-white rounded-lg shadow-lg p-6 text-center hover:shadow-xl transition hover-lift scale-in" aria-label="Portafolio YouTube">
                    <i class="fab fa-youtube text-4xl text-red-600 mb-4 float" aria-hidden="true"></i>
                    <h3 class="text-xl font-semibold mb-2">YouTube</h3>
                    <p class="text-gray-600">Tutoriales y tips</p>
                </a>
                <!-- THREADS -->
                <a href="https://www.threads.com/@graphicpizzeria" rel="noopener noreferrer" target="_blank" 
                   class="bg-white rounded-lg shadow-lg p-6 text-center hover:shadow-xl transition hover-lift scale-in" aria-label="Threads">
                    <i class="bi bi-threads text-4xl text-black mb-4 float"></i>
                    <h3 class="text-xl font-semibold mb-2">Threads</h3>
                    <p class="text-gray-600">Red social creativa</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Community Manager Packages -->
    <section class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center mb-12 fade-in">Paquetes Community Manager</h2>
            <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
                <!-- Paquete Básico -->
                <div class="bg-white rounded-lg shadow-lg p-8 text-center hover-lift scale-in">
                    <div class="bg-vis-red text-white px-4 py-2 rounded-full text-sm mb-6 inline-block">BÁSICO</div>
                    <h3 class="text-2xl font-bold mb-4">$150/mes</h3>
                    <ul class="text-left space-y-3 mb-8">
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>12 publicaciones mensuales</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Diseño de contenido</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Programación de posts</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Respuesta a comentarios</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Reporte mensual</li>
                    </ul>
                    <button class="w-full bg-vis-red text-white py-3 rounded-lg hover:bg-red-700 transition font-semibold">
                        Elegir Plan
                    </button>
                </div>
                <!-- Paquete Premium -->
                <div class="bg-white rounded-lg shadow-lg p-8 text-center hover-lift scale-in border-2 border-vis-red relative">
                    <div class="absolute -top-3 left-1/2 transform -translate-x-1/2 bg-vis-red text-white px-4 py-1 rounded-full text-sm">MÁS POPULAR</div>
                    <div class="bg-gradient-to-r from-vis-red to-red-700 text-white px-4 py-2 rounded-full text-sm mb-6 inline-block">PREMIUM</div>
                    <h3 class="text-2xl font-bold mb-4">$280/mes</h3>
                    <ul class="text-left space-y-3 mb-8">
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>20 publicaciones mensuales</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Diseño premium de contenido</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Stories diarios</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Gestión de comentarios y DM</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Análisis de competencia</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Reporte semanal</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>1 campaña publicitaria</li>
                    </ul>
                    <button class="w-full bg-vis-red text-white py-3 rounded-lg hover:bg-red-700 transition font-semibold glow">
                        Elegir Plan
                    </button>
                </div>
                <!-- Paquete Empresarial -->
                <div class="bg-white rounded-lg shadow-lg p-8 text-center hover-lift scale-in">
                    <div class="bg-vis-black text-white px-4 py-2 rounded-full text-sm mb-6 inline-block">EMPRESARIAL</div>
                    <h3 class="text-2xl font-bold mb-4">$450/mes</h3>
                    <ul class="text-left space-y-3 mb-8">
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>30 publicaciones mensuales</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Contenido multimedia premium</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Stories y Reels diarios</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Gestión completa de redes</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Estrategia de crecimiento</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Reportes en tiempo real</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>3 campañas publicitarias</li>
                        <li class="flex items-center"><i class="fas fa-check text-vis-red mr-3"></i>Consultoría personalizada</li>
                    </ul>
                    <button class="w-full bg-vis-black text-white py-3 rounded-lg hover:bg-gray-800 transition font-semibold">
                        Elegir Plan
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Client Success -->
    <section class="py-16">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center mb-12 fade-in">Cliente Satisfecho</h2>
            <div class="max-w-2xl mx-auto text-center">
                <div class="bg-white rounded-lg shadow-lg p-8 hover-lift slide-in-left">
                    <i class="fas fa-star text-vis-red text-2xl mb-4 float" aria-hidden="true"></i>
                    <h3 class="text-xl font-semibold mb-4">Tripsst World</h3>
                    <p class="text-gray-600 mb-6">Proyecto exitoso de branding y marketing digital</p>
                    <a href="https://www.instagram.com/tripsst.world" rel="noopener noreferrer" target="_blank" 
                       class="bg-vis-red text-white px-6 py-2 rounded-lg hover:bg-red-700 transition">
                        Ver Proyecto
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contacto" class="py-16 bg-vis-black text-white">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center mb-12 fade-in">Contacto</h2>
            <div class="grid md:grid-cols-2 gap-12 max-w-4xl mx-auto">
                <div class="slide-in-left">
                    <h3 class="text-xl font-semibold mb-6">Información de Contacto</h3>
                    <div class="space-y-4">
                        <div class="flex items-center">
                            <i class="fas fa-map-marker-alt text-vis-red mr-3 float" aria-hidden="true"></i>
                            <span>Valencia, Venezuela</span>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-envelope text-vis-red mr-3 float" aria-hidden="true"></i>
                            <a href="mailto:edgaryu23@gmail.com" class="hover:text-vis-red transition">edgaryu23@gmail.com</a>
                        </div>
                    </div>
                </div>
                <div class="slide-in-right">
                    <h3 class="text-xl font-semibold mb-6">Envíanos tu mensaje</h3>
                    <form class="space-y-4" action="mailto:edgaryu23@gmail.com" method="POST" enctype="text/plain">
                        <input type="text" name="nombre" placeholder="Tu nombre" class="w-full px-4 py-2 rounded text-black" required>
                        <input type="email" name="correo" placeholder="Tu correo" class="w-full px-4 py-2 rounded text-black" required>
                        <textarea name="mensaje" placeholder="Tu mensaje" class="w-full px-4 py-2 rounded text-black" rows="4" required></textarea>
                        <button type="submit" class="bg-vis-red text-white px-6 py-2 rounded hover:bg-red-700 transition">Enviar</button>
                    </form>
                </div>
            </div>
        </div>
    </section>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 text-center py-4">
        © 2025 Vis Solaris. Todos los derechos reservados.
    </footer>
    
    <!-- Menú móvil JS -->
    <script>
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuBtn.addEventListener('click', () => {
            if (mobileMenu.style.display === 'block') {
                mobileMenu.style.display = 'none';
            } else {
                mobileMenu.style.display = 'block';
            }
        });
    </script>
</body>
</html>