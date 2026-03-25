# Boutique-
Mi pequeño emprendimiento
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lumina Boutique | Moda Minimalista</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;600&family=Playfair+Display:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
    <style>
        :root {
            --pastel-pink: #fce4ec;
            --pastel-blue: #e3f2fd;
            --pastel-mint: #e8f5e9;
            --pastel-lavender: #f3e5f5;
            --soft-text: #4a4a4a;
        }
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            color: var(--soft-text);
            background-color: #ffffff;
        }
        .serif { font-family: 'Playfair Display', serif; }
        .bg-pastel-gradient {
            background: linear-gradient(135deg, var(--pastel-pink) 0%, var(--pastel-lavender) 100%);
        }
        .product-card:hover .product-image {
            transform: scale(1.05);
        }
        .transition-all { transition: all 0.4s ease; }
    </style>
</head>
<body class="overflow-x-hidden">

    <!-- Navegación -->
    <nav class="fixed w-full z-50 bg-white/80 backdrop-blur-md border-b border-gray-100">
        <div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
            <h1 class="serif text-2xl font-bold tracking-tight">LUMINA</h1>
            <div class="hidden md:flex space-x-10 text-sm font-medium uppercase tracking-widest">
                <a href="#" class="hover:text-pink-400 transition-colors">Nueva Colección</a>
                <a href="#" class="hover:text-pink-400 transition-colors">Mujer</a>
                <a href="#" class="hover:text-pink-400 transition-colors">Accesorios</a>
                <a href="#" class="hover:text-pink-400 transition-colors">Nosotros</a>
            </div>
            <div class="flex items-center space-x-5">
                <button class="p-2 hover:bg-gray-50 rounded-full transition-all">
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
                </button>
                <button class="p-2 hover:bg-gray-50 rounded-full transition-all relative">
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M6 2L3 6v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V6l-3-4Z"></path><line x1="3" y1="6" x2="21" y2="6"></line><path d="M16 10a4 4 0 0 1-8 0"></path></svg>
                    <span class="absolute top-0 right-0 bg-pink-200 text-[10px] w-4 h-4 flex items-center justify-center rounded-full">2</span>
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative h-screen flex items-center pt-20 overflow-hidden">
        <div class="absolute inset-0 bg-pastel-gradient opacity-40"></div>
        <div class="max-w-7xl mx-auto px-6 w-full grid md:grid-cols-2 gap-12 items-center relative z-10">
            <div>
                <span class="inline-block px-4 py-1 bg-white rounded-full text-xs font-semibold tracking-widest uppercase mb-6 shadow-sm text-pink-400">Temporada Primavera</span>
                <h2 class="serif text-6xl md:text-8xl mb-8 leading-tight">Suavidad <br><span class="italic text-pink-300">en cada hilo.</span></h2>
                <p class="text-lg text-gray-500 mb-10 max-w-md leading-relaxed">Descubre nuestra nueva línea de básicos esenciales diseñados con textiles orgánicos y una paleta de colores que calma el alma.</p>
                <div class="flex space-x-4">
                    <a href="#shop" class="bg-gray-900 text-white px-10 py-4 rounded-full text-sm font-semibold hover:bg-gray-800 transition-all shadow-lg hover:shadow-xl">Comprar ahora</a>
                    <a href="#" class="bg-white text-gray-900 px-10 py-4 rounded-full text-sm font-semibold border border-gray-100 hover:border-gray-200 transition-all shadow-sm">Explorar</a>
                </div>
            </div>
            <div class="hidden md:block relative">
                <div class="w-full h-[600px] rounded-[40px] overflow-hidden shadow-2xl rotate-2">
                    <img src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?auto=format&fit=crop&q=80&w=1000" alt="Modelo con ropa pastel" class="w-full h-full object-cover">
                </div>
                <!-- Floating Element -->
                <div class="absolute -bottom-10 -left-10 bg-white p-6 rounded-2xl shadow-xl flex items-center space-x-4 -rotate-3 border border-pink-50">
                    <div class="w-12 h-12 bg-pink-100 rounded-full flex items-center justify-center text-pink-400">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m5 11 4-7"/><path d="m19 11-4-7"/><path d="M2 11h20"/><path d="m3.5 11 1.6 7.4a2 2 0 0 0 2 1.6h9.8a2 2 0 0 0 2-1.6l1.7-7.4"/><path d="M9 11v1"/><path d="M15 11v1"/></svg>
                    </div>
                    <div>
                        <p class="text-xs text-gray-400 uppercase font-bold">Hecho en México</p>
                        <p class="text-sm font-bold">100% Algodón</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Productos Destacados -->
    <section id="shop" class="py-24 bg-white">
        <div class="max-w-7xl mx-auto px-6">
            <div class="flex justify-between items-end mb-16">
                <div>
                    <h3 class="serif text-4xl mb-2">Favoritos del Mes</h3>
                    <p class="text-gray-400">Piezas seleccionadas para elevar tu estilo diario.</p>
                </div>
                <a href="#" class="text-sm font-bold border-b-2 border-pink-200 pb-1 hover:border-pink-400 transition-all">Ver todo</a>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-12">
                <!-- Producto 1 -->
                <div class="product-card group cursor-pointer">
                    <div class="aspect-[3/4] rounded-3xl overflow-hidden bg-gray-50 mb-6 relative">
                        <img src="https://images.unsplash.com/photo-1583743814966-8936f5b7be1a?auto=format&fit=crop&q=80&w=800" alt="Sudadera Menta" class="product-image w-full h-full object-cover transition-all duration-700">
                        <div class="absolute top-4 right-4">
                            <button class="bg-white/90 backdrop-blur p-2 rounded-full shadow-sm opacity-0 group-hover:opacity-100 transition-all">
                                <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 14c1.49-1.46 3-3.21 3-5.5A5.5 5.5 0 0 0 16.5 3c-1.76 0-3 .5-4.5 2-1.5-1.5-2.74-2-4.5-2A5.5 5.5 0 0 0 2 8.5c0 2.3 1.5 4.05 3 5.5l7 7Z"/></svg>
                            </button>
                        </div>
                        <div class="absolute bottom-4 left-4 right-4 translate-y-12 group-hover:translate-y-0 transition-all duration-500">
                            <button class="w-full bg-white text-gray-900 py-3 rounded-xl text-xs font-bold shadow-lg">Añadir al Carrito</button>
                        </div>
                    </div>
                    <div class="flex justify-between items-start">
                        <div>
                            <h4 class="text-lg font-medium mb-1">Cárdigan "Serenity"</h4>
                            <p class="text-sm text-gray-400">Verde Menta Pastel</p>
                        </div>
                        <span class="font-semibold text-pink-400">$850.00</span>
                    </div>
                </div>

                <!-- Producto 2 -->
                <div class="product-card group cursor-pointer">
                    <div class="aspect-[3/4] rounded-3xl overflow-hidden bg-gray-50 mb-6 relative">
                        <img src="https://images.unsplash.com/photo-1591047139829-d91aecb6caea?auto=format&fit=crop&q=80&w=800" alt="Chaqueta Lavanda" class="product-image w-full h-full object-cover transition-all duration-700">
                        <div class="absolute bottom-4 left-4 right-4 translate-y-12 group-hover:translate-y-0 transition-all duration-500">
                            <button class="w-full bg-white text-gray-900 py-3 rounded-xl text-xs font-bold shadow-lg">Añadir al Carrito</button>
                        </div>
                    </div>
                    <div class="flex justify-between items-start">
                        <div>
                            <h4 class="text-lg font-medium mb-1">Blusa Silky Rose</h4>
                            <p class="text-sm text-gray-400">Rosa Palo</p>
                        </div>
                        <span class="font-semibold text-pink-400">$620.00</span>
                    </div>
                </div>

                <!-- Producto 3 -->
                <div class="product-card group cursor-pointer">
                    <div class="aspect-[3/4] rounded-3xl overflow-hidden bg-gray-50 mb-6 relative">
                        <div class="absolute top-4 left-4 z-10">
                            <span class="bg-pink-100 text-pink-500 text-[10px] font-bold px-3 py-1 rounded-full uppercase tracking-widest">Agotándose</span>
                        </div>
                        <img src="https://images.unsplash.com/photo-1576566588028-4147f3842f27?auto=format&fit=crop&q=80&w=800" alt="Accesorios" class="product-image w-full h-full object-cover transition-all duration-700">
                        <div class="absolute bottom-4 left-4 right-4 translate-y-12 group-hover:translate-y-0 transition-all duration-500">
                            <button class="w-full bg-white text-gray-900 py-3 rounded-xl text-xs font-bold shadow-lg">Añadir al Carrito</button>
                        </div>
                    </div>
                    <div class="flex justify-between items-start">
                        <div>
                            <h4 class="text-lg font-medium mb-1">Pantalón "Cloud"</h4>
                            <p class="text-sm text-gray-400">Azul Cielo</p>
                        </div>
                        <span class="font-semibold text-pink-400">$1,100.00</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Categoría Visual -->
    <section class="py-20 bg-pink-50/30">
        <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-2 gap-8 h-[500px]">
            <div class="bg-pastel-blue rounded-[40px] p-12 flex flex-col justify-end group cursor-pointer overflow-hidden relative">
                <div class="absolute inset-0 group-hover:scale-105 transition-all duration-700 opacity-20">
                     <img src="https://images.unsplash.com/photo-1543163521-1bf539c55dd2?auto=format&fit=crop&q=80&w=800" alt="Calzado" class="w-full h-full object-cover">
                </div>
                <div class="relative z-10">
                    <h5 class="serif text-3xl mb-2">Accesorios</h5>
                    <p class="text-sm mb-6 text-gray-600">Completa tu look minimalista.</p>
                    <button class="bg-white/80 backdrop-blur px-6 py-2 rounded-full text-xs font-bold uppercase tracking-wider hover:bg-white transition-all">Ver más</button>
                </div>
            </div>
            <div class="bg-pastel-mint rounded-[40px] p-12 flex flex-col justify-end group cursor-pointer overflow-hidden relative">
                <div class="absolute inset-0 group-hover:scale-105 transition-all duration-700 opacity-20">
                     <img src="https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&q=80&w=800" alt="Moda" class="w-full h-full object-cover">
                </div>
                <div class="relative z-10">
                    <h5 class="serif text-3xl mb-2">Nueva Colección</h5>
                    <p class="text-sm mb-6 text-gray-600">Recién llegados de temporada.</p>
                    <button class="bg-white/80 backdrop-blur px-6 py-2 rounded-full text-xs font-bold uppercase tracking-wider hover:bg-white transition-all">Descubrir</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-white pt-24 pb-12 border-t border-gray-100">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid md:grid-cols-4 gap-12 mb-16">
                <div class="col-span-1 md:col-span-1">
                    <h2 class="serif text-2xl font-bold mb-6">LUMINA</h2>
                    <p class="text-sm text-gray-400 leading-relaxed">Creando moda consciente y estética minimalista desde 2024. Calidad sobre cantidad.</p>
                </div>
                <div>
                    <h6 class="text-xs font-bold uppercase tracking-widest mb-6">Tienda</h6>
                    <ul class="text-sm text-gray-500 space-y-4">
                        <li><a href="#" class="hover:text-pink-300 transition-colors">Todo el catálogo</a></li>
                        <li><a href="#" class="hover:text-pink-300 transition-colors">Best Sellers</a></li>
                        <li><a href="#" class="hover:text-pink-300 transition-colors">Ofertas</a></li>
                    </ul>
                </div>
                <div>
                    <h6 class="text-xs font-bold uppercase tracking-widest mb-6">Ayuda</h6>
                    <ul class="text-sm text-gray-500 space-y-4">
                        <li><a href="#" class="hover:text-pink-300 transition-colors">Envíos</a></li>
                        <li><a href="#" class="hover:text-pink-300 transition-colors">Devoluciones</a></li>
                        <li><a href="#" class="hover:text-pink-300 transition-colors">Contacto</a></li>
                    </ul>
                </div>
                <div>
                    <h6 class="text-xs font-bold uppercase tracking-widest mb-6">Newsletter</h6>
                    <p class="text-sm text-gray-400 mb-6">Recibe un 10% en tu primera compra.</p>
                    <div class="flex">
                        <input type="email" placeholder="Tu email" class="bg-gray-50 border-none px-4 py-3 rounded-l-xl text-sm w-full focus:ring-1 focus:ring-pink-200 outline-none">
                        <button class="bg-pink-100 text-pink-500 px-4 py-3 rounded-r-xl">
                            <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 18 6-6-6-6"/></svg>
                        </button>
                    </div>
                </div>
            </div>
            <div class="pt-12 border-t border-gray-50 flex flex-col md:row justify-between items-center text-[10px] text-gray-400 font-bold uppercase tracking-widest">
                <p>© 2024 Lumina Boutique. Todos los derechos reservados.</p>
                <div class="flex space-x-6 mt-4 md:mt-0">
                    <a href="#" class="hover:text-pink-300 transition-colors">Instagram</a>
                    <a href="#" class="hover:text-pink-300 transition-colors">Pinterest</a>
                    <a href="#" class="hover:text-pink-300 transition-colors">TikTok</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scroll sencillo
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>

