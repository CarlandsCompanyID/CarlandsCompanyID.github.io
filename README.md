<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CarlandsCompanyID - Situs Resmi</title>
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap" rel="stylesheet">
    
    <!-- Custom CSS for animations and styling -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0a0a0a;
            color: #e5e5e5;
            overflow-x: hidden; /* Mencegah horizontal scroll */
        }
        .hero-gradient {
            background: radial-gradient(ellipse at top, #1a202c, #0a0a0a);
        }
        .header-scrolled {
            background-color: rgba(10, 10, 10, 0.8);
            backdrop-filter: blur(10px);
            border-bottom-width: 1px;
            border-bottom-color: #2d3748;
        }
        .reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
        }
        .reveal.visible {
            opacity: 1;
            transform: translateY(0);
        }
        .card {
            background-color: #171717;
            border: 1px solid #2d3748;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-8px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
        }
        .btn-secondary {
            background-color: #171717;
            border: 1px solid #4f46e5;
            color: #a5b4fc;
            transition: background-color 0.3s ease, color 0.3s ease;
        }
        .btn-secondary:hover {
             background-color: #4f46e5;
             color: #ffffff;
        }

        /* Styling untuk Running Text */
        .running-text-container {
            width: 100%; 
            background-color: #1e293b;
            color: #e5e5e5;
            padding: 12px 0;
            white-space: nowrap;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .running-text {
            display: inline-block;
            padding-left: 100%;
            animation: scrollText 40s linear infinite;
        }
        @keyframes scrollText {
            0% { transform: translateX(0%); }
            100% { transform: translateX(-100%); }
        }

        /* Styling untuk Partnership & Feedback Form */
        .themed-container {
            background-color: #171717;
            border: 1px solid #2d3748;
            border-radius: 12px;
            padding: 25px;
            width: 100%;
            margin: auto;
        }
        .themed-container h2 {
            text-align: center;
            color: #e5e5e5;
            border-bottom: 2px solid #2d3748;
            padding-bottom: 15px;
            margin-top: 0;
            letter-spacing: 1px;
            font-size: 1.25rem; /* Ukuran font disesuaikan */
            font-weight: 700;
        }
        @media (min-width: 768px) { /* md breakpoint */
             .themed-container h2 {
                font-size: 1.5rem;
             }
        }
        .partnership-list {
            list-style: none;
            padding: 0;
            margin: 20px 0 0 0;
        }
        .partner-slot {
            background-color: #2d3748;
            border: 1px solid #4a5568;
            padding: 15px;
            margin-bottom: 12px;
            border-radius: 8px;
            text-align: center;
            font-weight: 600;
            color: #a0aec0;
            transition: background-color 0.2s ease, transform 0.2s ease;
        }
        .partner-slot.filled {
            color: #e5e5e5;
            background-color: #4f46e5;
            border-color: #a5b4fc;
            font-weight: bold;
        }
        
        .feedback-form .form-group {
            margin-bottom: 20px;
        }
        .feedback-form label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            color: #a0aec0;
        }
        .feedback-form input, .feedback-form select, .feedback-form textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #4a5568;
            border-radius: 6px;
            font-size: 16px;
            box-sizing: border-box;
            background-color: #2d3748;
            color: #e5e5e5;
        }
         .feedback-form input::placeholder, .feedback-form textarea::placeholder {
            color: #718096;
        }
        .feedback-form textarea {
            resize: vertical;
            min-height: 120px;
        }
        .feedback-form button {
            width: 100%;
            padding: 15px;
            background-color: #4f46e5;
            border: none;
            border-radius: 6px;
            color: white;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.2s;
        }
        .feedback-form button:hover {
            background-color: #4338ca;
        }
        .feedback-form button:disabled {
            background-color: #3730a3;
            cursor: not-allowed;
        }
        #responseMessage {
            text-align: center;
            margin-top: 20px;
            font-weight: bold;
        }

        /* Social Media Link Styling */
        .social-link {
            background-color: #1e293b;
            border: 1px solid #334155;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 1rem;
            border-radius: 0.5rem;
            text-decoration: none;
            color: #cbd5e1;
            font-weight: 600;
            transition: all 0.2s ease-in-out;
        }
        .social-link:hover {
            background-color: #334155;
            color: #ffffff;
            transform: translateY(-2px);
            border-color: #4f46e5;
        }
        .social-link svg {
            width: 1.5rem;
            height: 1.5rem;
            margin-right: 0.75rem;
        }
    </style>
</head>
<body class="antialiased">

    <!-- Header / Navbar -->
    <header id="header" class="fixed top-0 left-0 right-0 z-50 transition-all duration-300">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8 flex justify-between items-center">
            <a href="#" class="text-xl font-bold text-white">CarlandsCompanyID</a>
            
            <nav class="hidden md:flex space-x-6 lg:space-x-8">
                <a href="#beranda" class="text-gray-300 hover:text-white transition-colors duration-300">Beranda</a>
                <a href="#misi" class="text-gray-300 hover:text-white transition-colors duration-300">Misi</a>
                <a href="#layanan" class="text-gray-300 hover:text-white transition-colors duration-300">Layanan</a>
                <a href="#gabung" class="text-gray-300 hover:text-white transition-colors duration-300">Gabung</a>
                <a href="#info" class="text-gray-300 hover:text-white transition-colors duration-300">Info</a>
                <a href="#media-sosial" class="text-gray-300 hover:text-white transition-colors duration-300">Media Sosial</a>
            </nav>

            <button id="mobile-menu-button" class="md:hidden text-white focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
            </button>
        </div>
        
        <div id="mobile-menu" class="hidden md:hidden bg-gray-900">
            <a href="#beranda" class="block py-3 px-6 text-gray-300 hover:bg-gray-800">Beranda</a>
            <a href="#misi" class="block py-3 px-6 text-gray-300 hover:bg-gray-800">Misi</a>
            <a href="#layanan" class="block py-3 px-6 text-gray-300 hover:bg-gray-800">Layanan</a>
            <a href="#gabung" class="block py-3 px-6 text-gray-300 hover:bg-gray-800">Gabung</a>
            <a href="#info" class="block py-3 px-6 text-gray-300 hover:bg-gray-800">Info Lain</a>
            <a href="#media-sosial" class="block py-3 px-6 text-gray-300 hover:bg-gray-800">Media Sosial</a>
        </div>
    </header>

    <main>
        <!-- Section 1: Beranda (Hero Section) -->
        <section id="beranda" class="min-h-screen flex items-center justify-center hero-gradient px-4">
            <div class="container mx-auto text-center">
                <div class="reveal">
                    <h1 class="text-4xl sm:text-5xl lg:text-7xl font-extrabold text-white leading-tight mb-4">
                        👋👋 Selamat datang!
                    </h1>
                    <p class="text-lg md:text-xl text-gray-300 max-w-4xl mx-auto">
                        Selamat datang di situs resmi kami. Semoga hari Anda menyenangkan dan penuh produktivitas.
                    </p>
                    <div class="mt-8 text-gray-400 text-sm tracking-widest uppercase">
                        Dibawakan oleh CarlandsCompanyID
                    </div>
                    <div class="mt-2 text-indigo-300 text-lg font-semibold">
                        Inovasi • Teknologi • Kreativitas
                    </div>
                </div>
            </div>
        </section>

        <!-- Running Text Section -->
        <section class="running-text-container">
            <div class="running-text">
                Selamat Datang di CarlandsCompanyID! Hai, Sobat Carlanders! 👋 Terima kasih sudah bergabung bersama kami... • CarlandsCompanyID Situs Resmi • Selamat datang di situs resmi kami. Semoga hari Anda menyenangkan dan penuh produktivitas. • Dibawakan oleh CarlandsCompanyID: Inovasi, Teknologi, Kreativitas...
            </div>
        </section>

        <!-- Section 2: Pendaftaran -->
        <section id="pendaftaran" class="py-16 sm:py-20 md:py-24 bg-gray-900">
             <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl">
                <div class="reveal card p-6 sm:p-8 md:p-12 text-center max-w-4xl mx-auto">
                    <h2 class="text-xl sm:text-2xl md:text-3xl font-bold text-white mb-3">📝 Pendaftaran Akun Pencoblosan</h2>
                    <p class="text-red-400 font-bold text-lg mb-6">[CLOSE CLOTER 1]</p>
                    <p class="text-gray-300 mb-8">Pendaftaran untuk kloter pertama saat ini telah ditutup. Nantikan informasi selanjutnya untuk pembukaan kloter berikutnya. Terima kasih atas antusiasme Anda!</p>
                    <a href="https://forms.gle/croHjnC3FR4rZpbSA" target="_blank" rel="noopener noreferrer" class="btn-secondary font-bold py-3 px-8 rounded-full text-lg inline-block cursor-not-allowed opacity-60">
                        Kunjungi Halaman Pendaftaran
                    </a>
                </div>
            </div>
        </section>

        <!-- Section 3: Misi Kami -->
        <section id="misi" class="py-16 sm:py-20 md:py-24">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl">
                <div class="reveal text-center mb-12 md:mb-16">
                    <h2 class="text-3xl sm:text-4xl font-bold text-white">🎯 Misi Kami</h2>
                    <div class="w-24 h-1 bg-indigo-500 mx-auto mt-4"></div>
                </div>
                <div class="reveal max-w-5xl mx-auto">
                    <p class="text-gray-300 text-center text-base sm:text-lg">Mengembangkan game berkualitas tinggi dengan cerita, gameplay, dan fitur yang orisinal serta menarik bagi berbagai kalangan. Mendukung kreativitas dan talenta lokal dalam industri game melalui kolaborasi, pelatihan, dan pengembangan tim internal. Membangun komunitas game yang inklusif dan sehat, di mana pemain merasa dihargai, aman, dan memiliki ruang untuk berekspresi. Menggunakan teknologi terbaru untuk menciptakan pengalaman bermain yang responsif, realistis, dan inovatif. Mewujudkan pertumbuhan berkelanjutan baik dari sisi produk maupun kontribusi terhadap industri kreatif di Indonesia.</p>
                </div>
            </div>
        </section>

        <!-- Section 4: Apa yang Kami Tawarkan -->
        <section id="layanan" class="py-16 sm:py-20 md:py-24 bg-black bg-opacity-20">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl">
                <div class="reveal text-center mb-12 md:mb-16">
                    <h2 class="text-3xl sm:text-4xl font-bold text-white">🚀 Apa yang Kami Tawarkan</h2>
                    <div class="w-24 h-1 bg-indigo-500 mx-auto mt-4"></div>
                </div>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                    <div class="reveal card rounded-lg p-8 text-center">
                        <div class="text-5xl mb-4">🌟</div>
                        <h3 class="text-xl font-bold text-white mb-2">Pengembangan Game & Roleplay Server</h3>
                    </div>
                    <div class="reveal card rounded-lg p-8 text-center">
                        <div class="text-5xl mb-4">💼</div>
                        <h3 class="text-xl font-bold text-white mb-2">Layanan Digital & Kreatif</h3>
                    </div>
                    <div class="reveal card rounded-lg p-8 text-center sm:col-span-2 lg:col-span-1">
                         <div class="text-5xl mb-4">🛠️</div>
                        <h3 class="text-xl font-bold text-white mb-2">Inovasi Teknologi Masa Depan</h3>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Section 5: Bergabunglah Bersama Kami -->
        <section id="gabung" class="py-16 sm:py-20 md:py-24">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl">
                 <div class="reveal text-center mb-12 md:mb-16">
                    <h2 class="text-3xl sm:text-4xl font-bold text-white">🤝 Bergabunglah Bersama Kami</h2>
                    <div class="w-24 h-1 bg-indigo-500 mx-auto mt-4"></div>
                </div>
                <div class="reveal max-w-4xl mx-auto bg-gray-900 rounded-lg p-6 sm:p-8 md:p-12 text-center border border-gray-700">
                    <h3 class="text-2xl sm:text-3xl font-bold text-indigo-400 mb-4">🎮 Gabung Bersama CarlandsCompanyID! 🚀</h3>
                    <p class="text-gray-300 mb-6">Apakah kamu punya semangat untuk menciptakan dunia game yang seru, inovatif, dan penuh tantangan? Di CarlandsCompanyID, kami bukan hanya membuat game — kami membangun pengalaman, komunitas, dan masa depan industri game Indonesia!</p>
                    <h4 class="text-xl font-semibold text-white mt-8 mb-4">✨ Mengapa bergabung dengan kami?</h4>
                    <ul class="text-gray-300 space-y-2 inline-block text-left mb-8">
                        <li class="flex items-center"><svg class="w-5 h-5 mr-2 text-green-400 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>Lingkungan kreatif dan kolaboratif</li>
                        <li class="flex items-center"><svg class="w-5 h-5 mr-2 text-green-400 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>Proyek game yang seru dan penuh potensi</li>
                        <li class="flex items-center"><svg class="w-5 h-5 mr-2 text-green-400 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>Kesempatan berkembang bersama tim profesional</li>
                        <li class="flex items-center"><svg class="w-5 h-5 mr-2 text-green-400 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>Dukungan penuh untuk ide dan inovasi kamu</li>
                    </ul>
                    <p class="text-gray-300 mb-6">💡Baik kamu developer, desainer, storyteller, content creator, atau gamers yang ingin berkarya — ini saatnya kamu ambil peran!</p>
                    <p class="text-white font-semibold mb-2">📩 Yuk, kirim portofolio atau kenalan dulu dengan tim kami!</p>
                    <p class="text-gray-400">Temukan info lengkap di [website/link komunitas]<br>Atau DM kami langsung di [Instagram/Discord/WhatsApp]</p>
                    <p class="text-indigo-400 font-bold mt-8">#CarlandsCompanyID #GameDeveloperIndonesia #JoinUs #Carlandsantipungli</p>
                </div>
            </div>
        </section>

        <!-- Section 6: Info Lainnya (Partnership & Feedback) -->
        <section id="info" class="py-16 sm:py-20 md:py-24 bg-black bg-opacity-20">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl">
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 lg:gap-12">
                    <!-- Partnership Column -->
                    <div class="reveal">
                         <div class="themed-container h-full">
                            <h2>CARLANDSCOMPANYID PARTNERSHIP</h2>
                            <ul class="partnership-list">
                                <li class="partner-slot filled">RSLP OFFICIAL</li>
                                <li class="partner-slot filled">NKRP</li>
                                <li class="partner-slot">[ SLOT KOSONG ]</li>
                                <li class="partner-slot">[ SLOT KOSONG ]</li>
                                <li class="partner-slot">[ SLOT KOSONG ]</li>
                                <li class="partner-slot">[ SLOT KOSONG ]</li>
                                <li class="partner-slot">[ SLOT KOSONG ]</li>
                                <li class="partner-slot">[ SLOT KOSONG ]</li>
                            </ul>
                        </div>
                    </div>
                    <!-- Feedback Form Column -->
                    <div class="reveal">
                        <div class="themed-container feedback-form h-full">
                            <h2>Formulir Masukan</h2>
                            <form id="feedbackForm" class="mt-6">
                                <div class="form-group">
                                    <label for="nama">Nama Anda (Opsional)</label>
                                    <input type="text" id="nama" name="nama" placeholder="Contoh: Budi">
                                </div>
                                <div class="form-group">
                                    <label for="tipe">Jenis Masukan</label>
                                    <select id="tipe" name="tipe" required>
                                        <option value="Saran" data-color="3447003">💡 Saran</option>
                                        <option value="Saran" data-color="3447003"> 🤝 Kerjasama</option>
                                        <option value="Kritik" data-color="16705372">⚠️ Kritik</option>
                                        <option value="Laporan Bug" data-color="15548997">⚠️ Laporan Bug</option>
                                        <option value="Kritik" data-color="16705372">⚠️ Laporan orang mencurigakan</option>
                                        <option value="Kritik" data-color="16705372">⚠️ Laporan Penipu</option>
                                        <option value="Laporan Bug" data-color="15548997">⚠️ Laporan Pelanggaran Grup whatsapp / discord</option>
                                    </select>
                                </div>
                                <div class="form-group">
                                    <label for="pesan">Pesan Anda</label>
                                    <textarea id="pesan" name="pesan" placeholder="Tuliskan detail pesan Anda di sini..." required></textarea>
                                </div>
                                <button type="submit" id="submitButton">Kirim Masukan</button>
                            </form>
                            <div id="responseMessage"></div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Section 7: Media Sosial -->
        <section id="media-sosial" class="py-16 sm:py-20 md:py-24">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl">
                <div class="reveal text-center mb-12 md:mb-16">
                    <h2 class="text-3xl sm:text-4xl font-bold text-white">Ikuti Kami</h2>
                    <div class="w-24 h-1 bg-indigo-500 mx-auto mt-4"></div>
                    <p class="text-gray-400 mt-4 max-w-2xl mx-auto">Terhubung dengan kami melalui media sosial untuk mendapatkan info terbaru, pengumuman, dan menjadi bagian dari komunitas kami.</p>
                </div>
                <div class="reveal grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 max-w-4xl mx-auto">
                    <!-- YouTube -->
                    <a href="https://www.youtube.com/@carlandsid" target="_blank" rel="noopener noreferrer" class="social-link">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24"><path d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"/></svg>
                        <span>YouTube</span>
                    </a>
                    <!-- TikTok -->
                    <a href="https://www.tiktok.com/@carlandscompanyid/" target="_blank" rel="noopener noreferrer" class="social-link">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24"><path d="M12.525.02c1.31-.02 2.61-.01 3.91-.02.08 1.53.63 3.09 1.75 4.17 1.12 1.11 2.7 1.62 4.24 1.79v4.03c-1.44-.05-2.89-.35-4.2-.97-.01-1.58-.01-3.18-.01-4.75-.26.03-.53.05-.78.08v6.2c0 2.51-1.34 4.84-3.57 6.14-2.23 1.3-4.99 1.1-7.15-.4-2.16-1.5-3.57-3.8-3.57-6.29v-2.89c.7.43 1.5.68 2.29.68.81 0 1.59-.27 2.29-.76v-6.5h3.91z"/></svg>
                        <span>TikTok</span>
                    </a>
                    <!-- Instagram -->
                    <a href="https://www.instagram.com/carlandscompanyid/" target="_blank" rel="noopener noreferrer" class="social-link">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.85s-.011 3.584-.069 4.85c-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07s-3.584-.012-4.85-.07c-3.252-.148-4.771-1.691-4.919-4.919-.058-1.265-.069-1.645-.069-4.85s.011-3.584.069-4.85c.149-3.225 1.664-4.771 4.919-4.919 1.266-.057 1.644-.069 4.85-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948s.014 3.667.072 4.947c.2 4.359 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072s3.667-.014 4.947-.072c4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.947s-.014-3.667-.072-4.947c-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.689-.073-4.948-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.162 6.162 6.162 6.162-2.759 6.162-6.162-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4s1.791-4 4-4 4 1.79 4 4-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44 1.441-.645 1.441-1.44-.645-1.44-1.441-1.44z"/></svg>
                        <span>Instagram</span>
                    </a>
                    <!-- WhatsApp 1 -->
                    <a href="https://chat.whatsapp.com/Gmc3109bU4j1jy4pRPEgMc" target="_blank" rel="noopener noreferrer" class="social-link">
                       <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946.003-6.556 5.338-11.891 11.893-11.891 3.181.001 6.167 1.24 8.413 3.488 2.245 2.248 3.481 5.236 3.48 8.414-.003 6.557-5.338 11.892-11.894 11.892-1.99-.001-3.951-.5-5.688-1.448l-6.305 1.654zm6.597-3.807c1.676.995 3.276 1.591 5.392 1.592 5.448 0 9.886-4.434 9.889-9.885.002-5.462-4.415-9.89-9.881-9.892-5.452 0-9.887 4.434-9.889 9.884-.001 2.225.651 4.315 1.847 6.062l-1.011 3.697 3.824-1.004zm6.278-6.002c-.312-.157-1.84-1.04-2.126-1.164s-.495-.157-.704.157c-.208.312-.799.987-.98 1.164-.182.176-.364.195-.663.039-.3-.156-1.432-.533-2.723-1.684-1.002-.88-1.67-1.97-1.869-2.314s-.208-.51-.01-1.002c.176-.438.396-.723.595-.967.2-.245.3-.408.457-.682.157-.274.078-.518-.04-.675-.117-.157-.704-1.684-.96-2.292-.255-.607-.523-.523-.704-.534-.182-.01-.364-.01-.546-.01s-.486.078-.732.39c-.246.312-.951 1.164-1.187 2.152-.237.988-.237 1.943.04 2.199.277.255.986 1.152 2.25 2.136 1.261.984 2.275 1.549 2.772 1.819.5.27 1.164.237 1.684.156.52-.08 1.84-.75 2.106-1.464.265-.715.265-1.33.187-1.464s-.157-.237-.312-.39z"/></svg>
                        <span>Grup WhatsApp</span>
                    </a>
                    <!-- WhatsApp 2 -->
                    <a href="https://chat.whatsapp.com/EoyF4WTKUHB1feKjRdowss" target="_blank" rel="noopener noreferrer" class="social-link">
                         <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2C6.486 2 2 6.486 2 12s4.486 10 10 10c1.465 0 2.865-.327 4.144-.928l.192.115c.983.585 2.029.985 3.12 1.166l-.286-1.713c.4-.64.71-1.341.92-2.083l.115-.192C21.673 14.865 22 13.465 22 12c0-5.514-4.486-10-10-10zm0 18c-4.411 0-8-3.589-8-8s3.589-8 8-8 8 3.589 8 8-3.589 8-8 8z"/><path d="M15.293 14.707a.999.999 0 00-1.414 0L12 16.586l-1.879-1.879a.999.999 0 10-1.414 1.414L10.586 18l-1.879 1.879a.999.999 0 101.414 1.414L12 19.414l1.879 1.879a.999.999 0 101.414-1.414L13.414 18l1.879-1.879a.999.999 0 000-1.414zM8 7h8v2H8zM8 11h8v2H8z"/></svg>
                        <span>Komunitas WhatsApp</span>
                    </a>
                    <!-- Email -->
                    <a href="mailto:carlandscompanyid@gmail.com" class="social-link">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24"><path d="M20 4H4c-1.103 0-2 .897-2 2v12c0 1.103.897 2 2 2h16c1.103 0 2-.897 2-2V6c0-1.103-.897-2-2-2zm0 2v.511l-8 6.223-8-6.223V6h16zM4 18V9.044l7.386 5.763a.998.998 0 001.228 0L20 9.044V18H4z"/></svg>
                        <span>Email</span>
                    </a>
                </div>
            </div>
        </section>

    </main>
    
    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8 py-8 text-center text-gray-400">
            <div class="max-w-3xl mx-auto bg-yellow-900 bg-opacity-20 border border-yellow-700 rounded-lg p-4 mb-8 flex items-start sm:items-center justify-center space-x-3">
                <svg class="w-8 h-8 sm:w-6 sm:h-6 text-yellow-400 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z"></path></svg>
                <p class="text-yellow-200 text-sm text-left sm:text-center"><strong>Peringatan:</strong> Ini adalah situs resmi milik CarlandsCompanyID. Situs selain ini adalah tidak resmi atau palsu.</p>
            </div>
            <p>&copy; 2025 CarlandsCompanyID. Semua Hak Dilindungi.</p>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Function to handle header scroll effect
            const header = document.getElementById('header');
            window.addEventListener('scroll', function() {
                if (window.scrollY > 50) {
                    header.classList.add('header-scrolled');
                } else {
                    header.classList.remove('header-scrolled');
                }
            });

            // Function to handle mobile menu
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuButton.addEventListener('click', function() {
                mobileMenu.classList.toggle('hidden');
            });
            const mobileLinks = Array.from(mobileMenu.getElementsByTagName('a'));
            mobileLinks.forEach(link => {
                link.addEventListener('click', () => {
                     mobileMenu.classList.add('hidden');
                });
            });

            // Function for reveal-on-scroll animation
            const revealElements = document.querySelectorAll('.reveal');
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                        observer.unobserve(entry.target);
                    }
                });
            }, { threshold: 0.1 });
            revealElements.forEach(el => observer.observe(el));
            
            // --- Feedback Form Logic ---
            const webhookURL = "https://discord.com/api/webhooks/1384002247180157088/nrIjsVyhN9eEPPOz1Qt8XZS70Sn72PjzjP_fhr8vFPKBVqDS4B0lcofKwsZ2dK-F9z-P"; // URL Webhook Anda
            const form = document.getElementById('feedbackForm');
            const submitButton = document.getElementById('submitButton');
            const responseMessage = document.getElementById('responseMessage');

            form.addEventListener('submit', function(e) {
                e.preventDefault();

                if (webhookURL.includes("GANTI_DENGAN_URL")) {
                    responseMessage.innerText = '❌ Harap masukkan URL Webhook yang valid di dalam kode.';
                    responseMessage.style.color = '#f87171'; // red-400
                    return;
                }

                submitButton.disabled = true;
                submitButton.innerText = 'Mengirim...';

                const namaPengirim = document.getElementById('nama').value || 'Anonim';
                const tipeSelect = document.getElementById('tipe');
                const tipeMasukan = tipeSelect.value;
                const pesanMasukan = document.getElementById('pesan').value;
                const selectedOption = tipeSelect.options[tipeSelect.selectedIndex];
                const embedColor = selectedOption.getAttribute('data-color');

                const payload = {
                    username: "AnomaliJualanAgama",
                    avatar_url: "https://i.imgur.com/4M34hi2.png",
                    embeds: [{
                        title: `Masukan Baru: ${tipeMasukan}`,
                        color: parseInt(embedColor),
                        fields: [
                            { name: "👤 Pengirim", value: namaPengirim, inline: true },
                            { name: "🏷️ Tipe", value: tipeMasukan, inline: true },
                            { name: "✉️ Pesan", value: pesanMasukan }
                        ],
                        footer: { text: `Dikirim pada` },
                        timestamp: new Date().toISOString()
                    }]
                };

                fetch(webhookURL, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                })
                .then(response => {
                    if (response.ok) {
                        responseMessage.innerText = '✅ Terima kasih! Masukan Anda telah berhasil dikirim.';
                        responseMessage.style.color = '#4ade80'; // green-400
                        form.reset();
                    } else {
                        responseMessage.innerText = `❌ Gagal mengirim. Discord merespon dengan status: ${response.status}`;
                        responseMessage.style.color = '#f87171'; // red-400
                    }
                })
                .catch(error => {
                    console.error('Error:', error);
                    responseMessage.innerText = '❌ Terjadi kesalahan jaringan. Periksa koneksi Anda.';
                    responseMessage.style.color = '#f87171'; // red-400
                })
                .finally(() => {
                    submitButton.disabled = false;
                    submitButton.innerText = 'Kirim Masukan';
                });
            });
        });
    </script>
</body>
</html>
