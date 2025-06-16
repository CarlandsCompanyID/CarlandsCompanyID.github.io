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
            width: 100%; /* Lebar akan diatur oleh grid parent */
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
                <a href="#kontak" class="text-gray-300 hover:text-white transition-colors duration-300">Kontak</a>
                <a href="#info" class="text-gray-300 hover:text-white transition-colors duration-300">Info</a>
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
            <a href="#kontak" class="block py-3 px-6 text-gray-300 hover:bg-gray-800">Kontak</a>
            <a href="#info" class="block py-3 px-6 text-gray-300 hover:bg-gray-800">Info Lain</a>
        </div>
    </header>

    <main>
        <!-- Section 1: Beranda (Hero Section) -->
        <section id="beranda" class="min-h-screen flex items-center justify-center hero-gradient px-4">
            <div class="container mx-auto text-center">
                <div class="reveal">
                    <!-- Responsive Font Size -->
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

        <!-- Section 6: Kontak -->
        <section id="kontak" class="py-16 sm:py-20 md:py-24 bg-black bg-opacity-20">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl">
                <div class="reveal text-center mb-12 md:mb-16">
                    <h2 class="text-3xl sm:text-4xl font-bold text-white">Kontak Kami</h2>
                     <div class="w-24 h-1 bg-indigo-500 mx-auto mt-4"></div>
                </div>
                <div class="reveal max-w-2xl mx-auto text-center">
                    <p class="text-gray-300 mb-8">Hai, butuh bantuan atau ingin bekerja sama dengan CarlandsCompanyID? Kami menunggu kabar darimu! Jangan ragu untuk mengirimkan pertanyaan, saran, atau sekadar menyapa. Kami akan membalas secepat mungkin!</p>
                    <div class="bg-gray-800 border border-gray-700 rounded-lg p-6 inline-block">
                        <p class="text-gray-400">Email Utama:</p>
                        <a href="mailto:carlandscompanyid@gmail.com" class="text-xl text-indigo-300 hover:text-indigo-200 break-all">carlandscompanyid@gmail.com</a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Section 7: Info Lainnya (Partnership & Feedback) -->
        <section id="info" class="py-16 sm:py-20 md:py-24">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl">
                <!-- Responsive Grid: 1 kolom di mobile, 2 kolom di tablet/desktop -->
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 lg:gap-12">
                    <!-- Partnership Column -->
                    <div class="reveal">
                         <div class="themed-container h-full">
                            <h2>CARLANDSCOMPANYID PARTNERSHIP</h2>
                            <ul class="partnership-list">
                                <li class="partner-slot filled">RSLP OFFICIAL</li>
                                <li class="partner-slot">[ SLOT KOSONG ]</li>
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
                                        <option value="Kritik" data-color="16705372">⚠️ Kritik</option>
                                        <option value="Laporan Bug" data-color="15548997">🐞 Laporan Bug</option>
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
                    username: "Feedback Bot",
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
```
<!--Start of Tawk.to Script-->
<script type="text/javascript">
var Tawk_API=Tawk_API||{}, Tawk_LoadStart=new Date();
(function(){
var s1=document.createElement("script"),s0=document.getElementsByTagName("script")[0];
s1.async=true;
s1.src='https://embed.tawk.to/684cd03b47f3b9190b9ffeb1/1itm0qqrh';
s1.charset='UTF-8';
s1.setAttribute('crossorigin','*');
s0.parentNode.insertBefore(s1,s0);
})();
</script>
<!--End of Tawk.to Script-->
