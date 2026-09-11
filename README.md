[Index.html](https://github.com/user-attachments/files/32115215/Index.html)
<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ekawati — Photographer & Videographer Portfolio</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Plus Jakarta Sans -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                    },
                    colors: {
                        pastel: {
                            bg: '#FDFBF7',        /* Cream soft background */
                            card: '#FFFDF9',      /* Pure soft white/cream */
                            peach: '#FFD1B3',     /* Soft Peach accent */
                            mint: '#C7E4DB',      /* Soft Mint accent */
                            lavender: '#E2D9F3',  /* Soft Lavender accent */
                            dark: '#2D3142',      /* Slate Dark text */
                            muted: '#7F8C8D',     /* Muted gray text */
                        }
                    }
                }
            }
        }
    </script>
    <style>
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #FDFBF7;
        }
        ::-webkit-scrollbar-thumb {
            background: #E2D9F3;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb-hover {
            background: #FFD1B3;
        }
        .pastel-shadow {
            box-shadow: 0 10px 30px -10px rgba(45, 49, 66, 0.08);
        }
        .hover-lift {
            transition: all 0.3s ease;
        }
        .hover-lift:hover {
            transform: translateY(-6px);
            box-shadow: 0 20px 40px -15px rgba(45, 49, 66, 0.12);
        }
    </style>
</head>
<body class="bg-pastel-bg text-pastel-dark font-sans antialiased selection:bg-pastel-peach selection:text-pastel-dark">

    <nav class="fixed top-0 left-0 right-0 z-50 bg-pastel-bg/80 backdrop-blur-md border-b border-pastel-lavender/30 transition-all duration-300" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <div class="flex items-center space-x-3">
                    <a href="#home" class="text-xl font-bold tracking-tight bg-gradient-to-r from-pastel-dark to-slate-600 bg-clip-text text-transparent">
                        EKAWATI <span class="text-xs uppercase tracking-widest px-2 py-0.5 rounded-full bg-pastel-mint text-pastel-dark ml-1 font-semibold">Visuals</span>
                    </a>
                </div>
                <!-- Desktop Navigation Links -->
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="text-pastel-dark hover:text-pastel-muted font-medium transition-colors text-sm">Beranda</a>
                    <a href="#photography" class="text-pastel-dark hover:text-pastel-muted font-medium transition-colors text-sm">Fotografi</a>
                    <a href="#videography" class="text-pastel-dark hover:text-pastel-muted font-medium transition-colors text-sm">Videografi</a>
                    <a href="#about" class="text-pastel-dark hover:text-pastel-muted font-medium transition-colors text-sm">Tentang</a>
                    <button onclick="openUploadModal()" class="px-4 py-2 rounded-full bg-pastel-peach text-pastel-dark hover:bg-orange-200 font-medium text-xs shadow-sm transition-all flex items-center space-x-1.5">
                        <i class="fa-solid fa-plus-circle"></i>
                        <span>Upload Karya</span>
                    </button>
                    <a href="#contact" class="px-5 py-2.5 rounded-full bg-pastel-dark text-pastel-bg hover:bg-slate-800 font-medium text-sm shadow-md transition-all">Hubungi Saya</a>
                </div>
                <!-- Mobile Menu Button -->
                <div class="md:hidden flex items-center space-x-2">
                    <button onclick="openUploadModal()" class="px-3 py-1.5 rounded-full bg-pastel-peach text-pastel-dark font-medium text-xs">
                        <i class="fa-solid fa-plus"></i> Upload
                    </button>
                    <button id="mobile-menu-btn" class="text-pastel-dark p-2 focus:outline-none">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile Dropdown Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-pastel-card border-t border-pastel-lavender/30 px-6 pt-4 pb-6 space-y-3 shadow-lg">
            <a href="#home" class="block text-pastel-dark py-2 font-medium mobile-link">Beranda</a>
            <a href="#photography" class="block text-pastel-dark py-2 font-medium mobile-link">Fotografi</a>
            <a href="#videography" class="block text-pastel-dark py-2 font-medium mobile-link">Videografi</a>
            <a href="#about" class="block text-pastel-dark py-2 font-medium mobile-link">Tentang</a>
            <a href="#contact" class="block text-center py-3 rounded-full bg-pastel-dark text-pastel-bg font-medium mobile-link">Hubungi Saya</a>
        </div>
    </nav>

    <section id="home" class="min-h-screen flex items-center justify-center relative overflow-hidden pt-24 pb-16">
        <!-- Soft pastel decorative background blur blobs -->
        <div class="absolute top-1/4 left-10 w-96 h-96 bg-pastel-peach/30 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute bottom-10 right-10 w-96 h-96 bg-pastel-mint/30 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute top-1/2 right-1/4 w-80 h-80 bg-pastel-lavender/40 rounded-full blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 w-full text-center">
            <div class="inline-flex items-center space-x-2 px-4 py-1.5 rounded-full bg-pastel-card border border-pastel-lavender/50 text-pastel-dark text-xs sm:text-sm font-semibold mb-6 shadow-sm">
                <span class="w-2 h-2 rounded-full bg-pastel-peach animate-pulse"></span>
                <span>Photographer & Videographer — Bandung, Indonesia</span>
            </div>
            
            <h1 class="text-4xl sm:text-7xl font-extrabold tracking-tight text-pastel-dark leading-tight max-w-4xl mx-auto">
                Mengabadikan Cerita Melalui <span class="bg-gradient-to-r from-orange-400 via-pink-400 to-indigo-400 bg-clip-text text-transparent">Lensa Estetik</span>
            </h1>

            <p class="mt-6 text-lg sm:text-xl text-pastel-muted max-w-2xl mx-auto font-normal leading-relaxed">
                Halo, saya Ekawati. Menghadirkan karya fotografi dan videografi lengkap
                (portrait pribadi, dokumentasi pernikahan, fotografi fashion, produk apparel, anak, art story & kuliner).
            </p>

            <div class="mt-10 flex flex-col sm:flex-row items-center justify-center gap-4">
                <a href="#photography" class="w-full sm:w-auto px-8 py-4 rounded-full bg-pastel-dark text-pastel-bg font-semibold hover:bg-slate-800 transition-all shadow-lg flex items-center justify-center space-x-2">
                    <span>Lihat Portofolio Foto</span>
                    <i class="fa-solid fa-arrow-down text-xs"></i>
                </a>
                <a href="#videography" class="w-full sm:w-auto px-8 py-4 rounded-full bg-pastel-card border border-pastel-lavender text-pastel-dark font-semibold hover:bg-pastel-lavender/20 transition-all flex items-center justify-center space-x-2">
                    <i class="fa-solid fa-video text-orange-400 mr-1"></i>
                    <span>Lihat Portofolio Video</span>
                </a>
            </div>

            <!-- Social badges quick link (Instagram & WhatsApp) -->
            <div class="mt-12 flex items-center justify-center space-x-4">
                <a href="https://instagram.com/ekaaaaaw__" target="_blank" class="w-11 h-11 rounded-full bg-pastel-card border border-pastel-lavender/60 flex items-center justify-center text-pastel-dark hover:bg-pastel-peach/40 transition-colors shadow-sm"><i class="fa-brands fa-instagram"></i></a>
                <a href="https://wa.me/6283876352793" target="_blank" class="w-11 h-11 rounded-full bg-pastel-card border border-pastel-lavender/60 flex items-center justify-center text-pastel-dark hover:bg-pastel-mint/40 transition-colors shadow-sm"><i class="fa-brands fa-whatsapp"></i></a>
            </div>
        </div>
    </section>

    <section id="photography" class="py-24 relative bg-pastel-card/50 border-t border-pastel-lavender/20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-14 space-y-3">
                <span class="text-xs font-bold tracking-widest text-pastel-muted uppercase px-3 py-1 rounded-full bg-pastel-peach/30">GALERI FOTOGRAFI</span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-pastel-dark">Koleksi Lengkap Karya Visual</h2>
                <p class="text-pastel-muted text-sm sm:text-base">Koleksi lengkap berbagai kategori proyek fotografi untuk e-commerce dan sosial media.</p>
            </div>

            <!-- Filter Categories Button Group Fixed Clean Layout with no text wrap breaking -->
            <div class="flex flex-wrap justify-center items-center gap-2.5 sm:gap-3 mb-12 max-w-5xl mx-auto px-2">
                <button class="filter-btn active px-4 py-2.5 rounded-full text-xs sm:text-sm font-semibold transition-all bg-pastel-dark text-pastel-bg shadow-sm whitespace-nowrap" data-filter="all">Semua Foto</button>
                <button class="filter-btn px-4 py-2.5 rounded-full text-xs sm:text-sm font-semibold transition-all bg-pastel-card border border-pastel-lavender text-pastel-dark hover:bg-pastel-peach/30 whitespace-nowrap" data-filter="fashion">Muslimah Wear</button>
                <button class="filter-btn px-4 py-2.5 rounded-full text-xs sm:text-sm font-semibold transition-all bg-pastel-card border border-pastel-lavender text-pastel-dark hover:bg-pastel-peach/30 whitespace-nowrap" data-filter="apparel">Foto Produk Apparel</button>
                <button class="filter-btn px-4 py-2.5 rounded-full text-xs sm:text-sm font-semibold transition-all bg-pastel-card border border-pastel-lavender text-pastel-dark hover:bg-pastel-peach/30 whitespace-nowrap" data-filter="product">Foto Produk</button>
                <button class="filter-btn px-4 py-2.5 rounded-full text-xs sm:text-sm font-semibold transition-all bg-pastel-card border border-pastel-lavender text-pastel-dark hover:bg-pastel-peach/30 whitespace-nowrap" data-filter="kids">Produk Pakaian Anak</button>
                <button class="filter-btn px-4 py-2.5 rounded-full text-xs sm:text-sm font-semibold transition-all bg-pastel-card border border-pastel-lavender text-pastel-dark hover:bg-pastel-peach/30 whitespace-nowrap" data-filter="food">Home Cooked</button>
                <button class="filter-btn px-4 py-2.5 rounded-full text-xs sm:text-sm font-semibold transition-all bg-pastel-card border border-pastel-lavender text-pastel-dark hover:bg-pastel-peach/30 whitespace-nowrap" data-filter="art">Art & Story</button>
                <button class="filter-btn px-4 py-2.5 rounded-full text-xs sm:text-sm font-semibold transition-all bg-pastel-card border border-pastel-lavender text-pastel-dark hover:bg-pastel-peach/30 whitespace-nowrap" data-filter="documentation">Documentation</button>
            </div>

            <!-- Gallery Grid (Multiple items per category) -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8" id="gallery-grid">
                
                <!-- Muslimah Wear 1 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="fashion" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?auto=format&fit=crop&w=800&q=80" alt="Muslimah Wear 1" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pastel-mint/60 text-pastel-dark">Muslimah Wear</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Graceful Muslimah Wear I</h3>
                        <p class="text-xs text-pastel-muted mt-1">Pelengkap e-commerce dan konten media sosial dengan kesan elegan.</p>
                    </div>
                </div>

                <!-- Muslimah Wear 2 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="fashion" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1490481651871-ab68de25d43d?auto=format&fit=crop&w=800&q=80" alt="Muslimah Wear 2" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pastel-mint/60 text-pastel-dark">Muslimah Wear</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Graceful Muslimah Wear II</h3>
                        <p class="text-xs text-pastel-muted mt-1">Gaya busana muslimah modis dengan pencahayaan natural.</p>
                    </div>
                </div>

                <!-- Foto Produk Apparel 1 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="apparel" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1445205170230-053b83016050?auto=format&fit=crop&w=800&q=80" alt="Foto Produk Apparel 1" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-amber-100 text-amber-800">Foto Produk Apparel</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Katalog Produk Pakaian & Apparel</h3>
                        <p class="text-xs text-pastel-muted mt-1">Menampilkan detail bahan, tekstur, dan potongan busana secara profesional.</p>
                    </div>
                </div>

                <!-- Foto Produk Apparel 2 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="apparel" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1523381210434-271e8be1f52b?auto=format&fit=crop&w=800&q=80" alt="Foto Produk Apparel 2" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-amber-100 text-amber-800">Foto Produk Apparel</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Modern Apparel Lookbook</h3>
                        <p class="text-xs text-pastel-muted mt-1">Menonjolkan detail jahitan dan gaya pakaian modern untuk e-commerce.</p>
                    </div>
                </div>

                <!-- Foto Produk (Kategori Baru) -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="product" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?auto=format&fit=crop&w=800&q=80" alt="Foto Produk 1" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-orange-100 text-orange-800">Foto Produk</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Commercial Gadget & Lifestyle Product</h3>
                        <p class="text-xs text-pastel-muted mt-1">Foto produk komersial dengan pencahayaan studio yang bersih dan berfokus pada daya tarik estetika barang.</p>
                    </div>
                </div>

                <!-- Foto Produk 2 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="product" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?auto=format&fit=crop&w=800&q=80" alt="Foto Produk 2" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-orange-100 text-orange-800">Foto Produk</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Minimalist Watch & Accessories</h3>
                        <p class="text-xs text-pastel-muted mt-1">Menampilkan detail kemewahan produk dengan komposisi penataan benda yang rapi.</p>
                    </div>
                </div>

                <!-- Produk Pakaian Anak 1 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="kids" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1522771930-78848d9293e8?auto=format&fit=crop&w=800&q=80" alt="Produk Pakaian Anak 1" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pink-100 text-pink-800">Produk Pakaian Anak</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Katalog Fashion Anak Ceria I</h3>
                        <p class="text-xs text-pastel-muted mt-1">Fotografi produk pakaian anak dengan sentuhan warna cerah dan hangat.</p>
                    </div>
                </div>

                <!-- Produk Pakaian Anak 2 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="kids" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1503944583220-74979e2d44c7?auto=format&fit=crop&w=800&q=80" alt="Produk Pakaian Anak 2" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pink-100 text-pink-800">Produk Pakaian Anak</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Katalog Fashion Anak Ceria II</h3>
                        <p class="text-xs text-pastel-muted mt-1">Koleksi baju anak yang nyaman dengan latar estetik.</p>
                    </div>
                </div>

                <!-- Home Cooked 1 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="food" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1546069901-ba9599a7e63c?auto=format&fit=crop&w=800&q=80" alt="Home Cooked 1" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pastel-peach/40 text-pastel-dark">Home Cooked</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Masakan Rumahan Autentik I</h3>
                        <p class="text-xs text-pastel-muted mt-1">Sajian masakan rumahan lezat dan menggugah selera.</p>
                    </div>
                </div>

                <!-- Home Cooked 2 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="food" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1555939594-58d7cb561ad1?auto=format&fit=crop&w=800&q=80" alt="Home Cooked 2" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pastel-peach/40 text-pastel-dark">Home Cooked</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Masakan Rumahan Autentik II</h3>
                        <p class="text-xs text-pastel-muted mt-1">Dokumentasi kuliner tradisional rumahan penuh cita rasa.</p>
                    </div>
                </div>

                <!-- Art & Story Photography 1 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="art" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1518709268805-4e9042af9f23?auto=format&fit=crop&w=800&q=80" alt="Art & Story Photography 1" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pastel-lavender text-pastel-dark">Art Photography</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Visual Narasi & Seni Estetik I</h3>
                        <p class="text-xs text-pastel-muted mt-1">Fotografi konseptual yang menyampaikan cerita mendalam.</p>
                    </div>
                </div>

                <!-- Art & Story Photography 2 -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="art" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?auto=format&fit=crop&w=800&q=80" alt="Art & Story Photography 2" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pastel-lavender text-pastel-dark">Art Photography</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Visual Narasi & Seni Estetik II</h3>
                        <p class="text-xs text-pastel-muted mt-1">Eksplorasi visual lanskap dan seni bercerita melalui bidikan kamera.</p>
                    </div>
                </div>

                <!-- Documentation 1 (Wedding) -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="documentation" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=800&q=80" alt="Wedding Documentation" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pastel-lavender text-pastel-dark">Documentation</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Wedding Documentation I</h3>
                        <p class="text-xs text-pastel-muted mt-1">Mengabadikan momen sakral pernikahan dengan sentuhan hangat.</p>
                    </div>
                </div>

                <!-- Documentation 2 (Wedding) -->
                <div class="gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm" data-category="documentation" onclick="openModal(this)">
                    <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1511285560929-80b456fea0bc?auto=format&fit=crop&w=800&q=80" alt="Wedding Moments" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                        </div>
                    </div>
                    <div class="p-5">
                        <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pastel-lavender text-pastel-dark">Documentation</span>
                        <h3 class="text-lg font-bold text-pastel-dark mt-2">Wedding Documentation II</h3>
                        <p class="text-xs text-pastel-muted mt-1">Momen bahagia resepsi dan akad nikah penuh kehangatan.</p>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <section id="videography" class="py-24 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-14 space-y-3">
                <span class="text-xs font-bold tracking-widest text-pastel-muted uppercase px-3 py-1 rounded-full bg-pastel-mint/40">VIDEOGRAFI</span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-pastel-dark">Karya Video</h2>
                <p class="text-pastel-muted text-sm sm:text-base">Konten review produk dan lookbook yang berfokus menunjukkan detail secara jelas dan estetis.</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-10" id="video-grid">
                
                <!-- Video Slot 1 -->
                <div class="bg-pastel-card rounded-3xl overflow-hidden border border-pastel-lavender/40 shadow-sm p-6 space-y-4">
                    <div class="flex items-center justify-between">
                        <span class="px-3 py-1 rounded-full text-xs font-semibold bg-pastel-mint/60 text-pastel-dark">Muslimah Wear Content</span>
                        <span class="text-xs text-pastel-muted italic">Local Video File (.mp4)</span>
                    </div>
                    <div class="aspect-video rounded-2xl overflow-hidden bg-slate-900 relative flex items-center justify-center border border-pastel-lavender/30 shadow-inner">
                        <video class="w-full h-full object-cover" controls preload="metadata" poster="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?auto=format&fit=crop&w=800&q=80">
                            <source src="https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerBlazes.mp4" type="video/mp4">
                            Browser Anda tidak mendukung tag video.
                        </video>
                    </div>
                    <div>
                        <h3 class="text-xl font-bold text-pastel-dark">Muslimah Wear Lookbook Cinematic</h3>
                        <p class="text-sm text-pastel-muted mt-1">Konten review produk yang berfokus menunjukkan detail secara jelas dan estetis.</p>
                    </div>
                </div>

                <!-- Video Slot 2 -->
                <div class="bg-pastel-card rounded-3xl overflow-hidden border border-pastel-lavender/40 shadow-sm p-6 space-y-4">
                    <div class="flex items-center justify-between">
                        <span class="px-3 py-1 rounded-full text-xs font-semibold bg-pastel-mint/60 text-pastel-dark">Muslimah Wear Content</span>
                        <span class="text-xs text-pastel-muted italic">Local Video File (.mp4)</span>
                    </div>
                    <div class="aspect-video rounded-2xl overflow-hidden bg-slate-900 relative flex items-center justify-center border border-pastel-lavender/30 shadow-inner">
                        <video class="w-full h-full object-cover" controls preload="metadata" poster="https://images.unsplash.com/photo-1490481651871-ab68de25d43d?auto=format&fit=crop&w=800&q=80">
                            <source src="https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerEscapes.mp4" type="video/mp4">
                            Browser Anda tidak mendukung tag video.
                        </video>
                    </div>
                    <div>
                        <h3 class="text-xl font-bold text-pastel-dark">Modest Fashion Styling & Detail Review</h3>
                        <p class="text-sm text-pastel-muted mt-1">Konten review produk yang berfokus menunjukkan detail secara jelas dan estetis.</p>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- ABOUT SECTION -->
    <section id="about" class="py-24 relative bg-pastel-card/50 border-t border-pastel-lavender/20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <div class="lg:col-span-5">
                    <div class="aspect-[4/5] rounded-3xl overflow-hidden border border-pastel-lavender/50 shadow-md relative bg-pastel-lavender/20">
                        <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=800&q=80" alt="Eka Wati Portrait" class="w-full h-full object-cover">
                    </div>
                </div>
                <div class="lg:col-span-7 space-y-6">
                    <span class="text-xs font-bold tracking-widest text-pastel-muted uppercase px-3 py-1 rounded-full bg-pastel-lavender/40">TENTANG SAYA</span>
                    <h2 class="text-3xl sm:text-4xl font-extrabold text-pastel-dark">Halo, Saya Eka Wati</h2>
                    <p class="text-pastel-muted leading-relaxed">
                        Seorang fotografer dan videografer profesional berbasis di Bandung, Indonesia. Saya memiliki minat besar dalam menangkap estetika visual yang bersih, hangat, dan bernyawa.
                    </p>
                    <p class="text-pastel-muted leading-relaxed">
                        Karya-karya saya difokuskan untuk membantu brand, UMKM, dan kreator konten untuk menghadirkan visual terbaik sebagai pelengkap e-commerce, katalog produk apparel, hingga konten media sosial yang menarik perhatian audiens.
                    </p>
                    <div class="grid grid-cols-2 gap-4 pt-4">
                        <div class="p-4 rounded-2xl bg-pastel-card border border-pastel-lavender/40">
                            <h4 class="font-bold text-pastel-dark text-lg">Spesialisasi</h4>
                            <p class="text-xs text-pastel-muted mt-1">Fotografi Produk, Apparel, Muslimah Wear, Kuliner & Videografi.</p>
                        </div>
                        <div class="p-4 rounded-2xl bg-pastel-card border border-pastel-lavender/40">
                            <h4 class="font-bold text-pastel-dark text-lg">Lokasi</h4>
                            <p class="text-xs text-pastel-muted mt-1">Bandung & Siap Luar Kota.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CONTACT SECTION -->
    <section id="contact" class="py-24 relative">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="bg-pastel-card rounded-3xl p-8 sm:p-12 border border-pastel-lavender/50 shadow-sm text-center space-y-6">
                <span class="text-xs font-bold tracking-widest text-pastel-muted uppercase px-3 py-1 rounded-full bg-pastel-peach/40">MARI BEKERJASAMA</span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-pastel-dark">Hubungi Saya</h2>
                <p class="text-pastel-muted max-w-lg mx-auto text-sm sm:text-base">
                    Punya proyek fotografi atau videografi untuk brand atau 
                    e-commerce Anda? Diskusikan kebutuhan Anda sekarang!
                </p>
                <div class="flex flex-wrap justify-center gap-4 pt-4">
                    <a href="https://wa.me/6283876352793" target="_blank" class="px-8 py-3.5 rounded-full bg-emerald-600 text-white font-semibold hover:bg-emerald-700 transition-all shadow-md flex items-center space-x-2">
                        <i class="fa-brands fa-whatsapp text-lg"></i>
                        <span>WhatsApp (Chat)</span>
                    </a>
                    <a href="https://instagram.com/ekaaaaaw__" target="_blank" class="px-8 py-3.5 rounded-full bg-gradient-to-r from-amber-500 via-pink-500 to-purple-600 text-white font-semibold hover:opacity-95 transition-all shadow-md flex items-center space-x-2">
                        <i class="fa-brands fa-instagram text-lg"></i>
                        <span>Instagram DM</span>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <footer class="py-12 bg-pastel-card border-t border-pastel-lavender/30 text-center text-xs text-pastel-muted">
        <p>&copy; 2026 Eka Wati. All rights reserved. Designed with Pastel Aesthetics.</p>
    </footer>

    <!-- Full Image Modal -->
    <div id="imageModal" class="fixed inset-0 z-50 bg-black/80 backdrop-blur-sm hidden items-center justify-center p-4" onclick="closeModal()">
        <div class="relative max-w-4xl w-full max-h-[90vh] flex items-center justify-center" onclick="event.stopPropagation()">
            <button onclick="closeModal()" class="absolute -top-12 right-0 text-white text-2xl p-2 hover:text-pastel-peach transition-colors focus:outline-none">
                <i class="fa-solid fa-xmark"></i>
            </button>
            <img id="modalImg" src="" alt="Enlarged Photo" class="max-w-full max-h-[85vh] object-contain rounded-2xl shadow-2xl">
        </div>
    </div>

    <!-- Upload Modal -->
    <div id="uploadModal" class="fixed inset-0 z-50 bg-black/70 backdrop-blur-sm hidden items-center justify-center p-4">
        <div class="bg-pastel-card rounded-3xl max-w-md w-full p-6 sm:p-8 border border-pastel-lavender shadow-2xl relative space-y-6">
            <div class="flex items-center justify-between">
                <h3 class="text-xl font-bold text-pastel-dark flex items-center space-x-2">
                    <i class="fa-solid fa-cloud-arrow-up text-orange-400"></i>
                    <span>Upload Karya Baru</span>
                </h3>
                <button onclick="closeUploadModal()" class="text-pastel-muted hover:text-pastel-dark text-xl"><i class="fa-solid fa-xmark"></i></button>
            </div>
            
            <form id="uploadForm" onsubmit="handleUpload(event)" class="space-y-4">
                <div>
                    <label class="block text-xs font-semibold text-pastel-dark uppercase mb-1">Tipe Media</label>
                    <select id="mediaType" onchange="toggleMediaType()" class="w-full px-4 py-2.5 rounded-xl border border-pastel-lavender/60 bg-pastel-bg text-sm text-pastel-dark focus:outline-none">
                        <option value="photo">Foto (Galeri)</option>
                        <option value="video">Video (Videografi)</option>
                    </select>
                </div>

                <div id="categoryGroup">
                    <label class="block text-xs font-semibold text-pastel-dark uppercase mb-1">Kategori Foto</label>
                    <select id="photoCategory" class="w-full px-4 py-2.5 rounded-xl border border-pastel-lavender/60 bg-pastel-bg text-sm text-pastel-dark focus:outline-none">
                        <option value="fashion">Muslimah Wear</option>
                        <option value="apparel">Foto Produk Apparel</option>
                        <option value="product">Foto Produk</option>
                        <option value="kids">Produk Pakaian Anak</option>
                        <option value="food">Home Cooked</option>
                        <option value="art">Art & Story</option>
                        <option value="documentation">Documentation</option>
                    </select>
                </div>

                <div>
                    <label class="block text-xs font-semibold text-pastel-dark uppercase mb-1">Judul Karya</label>
                    <input type="text" id="mediaTitle" required placeholder="Contoh: Koleksi Terbaru Lebaran" class="w-full px-4 py-2.5 rounded-xl border border-pastel-lavender/60 bg-pastel-bg text-sm text-pastel-dark focus:outline-none">
                </div>

                <div>
                    <label class="block text-xs font-semibold text-pastel-dark uppercase mb-1">Deskripsi Singkat</label>
                    <input type="text" id="mediaDesc" required placeholder="Contoh: Detail bahan dan warna pastel lembut." class="w-full px-4 py-2.5 rounded-xl border border-pastel-lavender/60 bg-pastel-bg text-sm text-pastel-dark focus:outline-none">
                </div>

                <div>
                    <label class="block text-xs font-semibold text-pastel-dark uppercase mb-1">Pilih File dari Komputer</label>
                    <input type="file" id="mediaFile" accept="image/*,video/*" required class="w-full text-xs text-pastel-muted file:mr-4 file:py-2 file:px-4 file:rounded-full file:border-0 file:text-xs file:font-semibold file:bg-pastel-peach file:text-pastel-dark hover:file:bg-orange-200">
                </div>

                <button type="submit" class="w-full py-3.5 rounded-full bg-pastel-dark text-pastel-bg font-semibold hover:bg-slate-800 transition-all shadow-md text-sm">
                    Tambahkan ke Website
                </button>
            </form>
        </div>
    </div>

    <script>
        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Close mobile menu on link click
        document.querySelectorAll('.mobile-link').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // Filter Gallery Logic
        const filterBtns = document.querySelectorAll('.filter-btn');
        
        function applyFilter(filterValue) {
            filterBtns.forEach(b => {
                if(b.getAttribute('data-filter') === filterValue) {
                    b.classList.add('active', 'bg-pastel-dark', 'text-pastel-bg', 'shadow-sm');
                    b.classList.remove('bg-pastel-card', 'border', 'border-pastel-lavender', 'text-pastel-dark');
                } else {
                    b.classList.remove('active', 'bg-pastel-dark', 'text-pastel-bg', 'shadow-sm');
                    b.classList.add('bg-pastel-card', 'border', 'border-pastel-lavender', 'text-pastel-dark');
                }
            });

            const galleryItems = document.querySelectorAll('.gallery-item');
            galleryItems.forEach(item => {
                if (filterValue === 'all' || item.getAttribute('data-category') === filterValue) {
                    item.style.display = 'block';
                } else {
                    item.style.display = 'none';
                }
            });
        }

        filterBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                applyFilter(btn.getAttribute('data-filter'));
            });
        });

        // Modal Logic
        function openModal(element) {
            const img = element.querySelector('img');
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImg');
            modalImg.src = img.src;
            modal.classList.remove('hidden');
            modal.classList.add('flex');
            document.body.style.overflow = 'hidden';
        }

        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
            document.body.style.overflow = 'auto';
        }

        // Upload Modal Logic
        function openUploadModal() {
            document.getElementById('uploadModal').classList.remove('hidden');
            document.getElementById('uploadModal').classList.add('flex');
            document.body.style.overflow = 'hidden';
        }

        function closeUploadModal() {
            document.getElementById('uploadModal').classList.add('hidden');
            document.getElementById('uploadModal').classList.remove('flex');
            document.body.style.overflow = 'auto';
        }

        function toggleMediaType() {
            const type = document.getElementById('mediaType').value;
            const categoryGroup = document.getElementById('categoryGroup');
            if(type === 'video') {
                categoryGroup.style.display = 'none';
            } else {
                categoryGroup.style.display = 'block';
            }
        }

        // Handle Custom Upload from Local File
        function handleUpload(event) {
            event.preventDefault();
            const mediaType = document.getElementById('mediaType').value;
            const title = document.getElementById('mediaTitle').value;
            const desc = document.getElementById('mediaDesc').value;
            const fileInput = document.getElementById('mediaFile');

            if(fileInput.files && fileInput.files[0]) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    const fileUrl = e.target.result;

                    if(mediaType === 'photo') {
                        const category = document.getElementById('photoCategory').value;
                        const categoryNames = {
                            'fashion': 'Muslimah Wear',
                            'apparel': 'Foto Produk Apparel',
                            'product': 'Foto Produk',
                            'kids': 'Produk Pakaian Anak',
                            'food': 'Home Cooked',
                            'art': 'Art & Story',
                            'documentation': 'Documentation'
                        };
                        const catName = categoryNames[category] || 'Karya Foto';

                        const grid = document.getElementById('gallery-grid');
                        const newItem = document.createElement('div');
                        newItem.className = 'gallery-item group cursor-pointer hover-lift bg-pastel-card rounded-2xl overflow-hidden border border-pastel-lavender/40 shadow-sm';
                        newItem.setAttribute('data-category', category);
                        newItem.setAttribute('onclick', 'openModal(this)');
                        newItem.innerHTML = `
                            <div class="aspect-[4/3] overflow-hidden relative bg-pastel-lavender/20">
                                <img src="${fileUrl}" alt="${title}" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                                <div class="absolute inset-0 bg-pastel-dark/30 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                                    <span class="px-4 py-2 rounded-full bg-pastel-card text-pastel-dark text-xs font-bold shadow-lg"><i class="fa-solid fa-magnifying-glass-plus mr-2"></i>Perbesar Foto</span>
                                </div>
                            </div>
                            <div class="p-5">
                                <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-pastel-mint/60 text-pastel-dark">${catName}</span>
                                <h3 class="text-lg font-bold text-pastel-dark mt-2">${title}</h3>
                                <p class="text-xs text-pastel-muted mt-1">${desc}</p>
                            </div>
                        `;
                        grid.prepend(newItem);
                        applyFilter(category);
                    } else {
                        const videoGrid = document.getElementById('video-grid');
                        const newVideo = document.createElement('div');
                        newVideo.className = 'bg-pastel-card rounded-3xl overflow-hidden border border-pastel-lavender/40 shadow-sm p-6 space-y-4';
                        newVideo.innerHTML = `
                            <div class="flex items-center justify-between">
                                <span class="px-3 py-1 rounded-full text-xs font-semibold bg-pastel-mint/60 text-pastel-dark">Uploaded Video</span>
                                <span class="text-xs text-pastel-muted italic">Local Video File (.mp4)</span>
                            </div>
                            <div class="aspect-video rounded-2xl overflow-hidden bg-slate-900 relative flex items-center justify-center border border-pastel-lavender/30 shadow-inner">
                                <video class="w-full h-full object-cover" controls preload="metadata">
                                    <source src="${fileUrl}" type="video/mp4">
                                    Browser Anda tidak mendukung tag video.
                                </video>
                            </div>
                            <div>
                                <h3 class="text-xl font-bold text-pastel-dark">${title}</h3>
                                <p class="text-sm text-pastel-muted mt-1">${desc}</p>
                            </div>
                        `;
                        videoGrid.prepend(newVideo);
                    }

                    closeUploadModal();
                    document.getElementById('uploadForm').reset();
                };
                reader.readAsDataURL(fileInput.files[0]);
            }
        }
    </script>
</body>
</html>
