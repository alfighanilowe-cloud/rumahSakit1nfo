<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sistem Informasi Rumah Sakit Sehat Sejahtera</title>
    <!-- Menggunakan Tailwind CSS dari CDN untuk styling instan -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Google -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <!-- Icon Library -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <style>
        body { font-family: 'Poppins', sans-serif; }
        .hero-bg {
            background-image: linear-gradient(rgba(0, 128, 128, 0.8), rgba(0, 128, 128, 0.6)), url('https://images.unsplash.com/photo-1519494026892-80bbd2d6fd0d?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">

    <!-- NAVBAR -->
    <nav class="bg-white shadow-md fixed w-full z-50">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-teal-600 flex items-center gap-2">
                <i class="fa-solid fa-hospital"></i> RS. Sehat Sejahtera
            </a>
            
            <div class="hidden md:flex space-x-8 font-medium">
                <a href="#beranda" class="hover:text-teal-600 transition">Beranda</a>
                <a href="#layanan" class="hover:text-teal-600 transition">Layanan</a>
                <a href="#dokter" class="hover:text-teal-600 transition">Jadwal Dokter</a>
                <a href="#kontak" class="hover:text-teal-600 transition">Kontak</a>
            </div>

            <div class="flex items-center space-x-4">
                <button onclick="openModal()" class="bg-teal-600 text-white px-5 py-2 rounded-full hover:bg-teal-700 transition shadow-lg">
                    Login Sistem
                </button>
            </div>
        </div>
    </nav>

    <!-- HERO SECTION -->
    <section id="beranda" class="hero-bg h-screen flex items-center justify-center text-center text-white px-6">
        <div class="max-w-3xl animate-fade-in-up">
            <h1 class="text-4xl md:text-6xl font-bold mb-6">Pelayanan Kesehatan Terpadu & Digital</h1>
            <p class="text-xl mb-8 text-gray-100">Solusi Sistem Informasi Manajemen Rumah Sakit yang terintegrasi, cepat, dan akurat untuk pasien dan tenaga medis.</p>
            <div class="flex flex-col md:flex-row gap-4 justify-center">
                <a href="#layanan" class="bg-white text-teal-600 px-8 py-3 rounded-full font-bold hover:bg-gray-100 transition shadow-lg">Lihat Layanan</a>
                <button onclick="alert('Fitur Pendaftaran Online akan aktif setelah backend terhubung.')" class="border-2 border-white text-white px-8 py-3 rounded-full font-bold hover:bg-white hover:text-teal-600 transition">Daftar Online</button>
            </div>
        </div>
    </section>

    <!-- STATISTIK / FITUR UTAMA -->
    <section class="container mx-auto px-6 -mt-20 relative z-10">
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
            <!-- Card 1 -->
            <div class="bg-white p-8 rounded-xl shadow-xl border-t-4 border-teal-500 hover:-translate-y-2 transition duration-300">
                <div class="text-teal-600 text-4xl mb-4"><i class="fa-solid fa-user-doctor"></i></div>
                <h3 class="text-xl font-bold mb-2">Cari Dokter</h3>
                <p class="text-gray-500">Temukan dokter spesialis sesuai kebutuhan Anda dengan jadwal yang fleksibel.</p>
            </div>
            <!-- Card 2 -->
            <div class="bg-white p-8 rounded-xl shadow-xl border-t-4 border-blue-500 hover:-translate-y-2 transition duration-300">
                <div class="text-blue-500 text-4xl mb-4"><i class="fa-solid fa-calendar-check"></i></div>
                <h3 class="text-xl font-bold mb-2">Booking Online</h3>
                <p class="text-gray-500">Hindari antrian panjang dengan mendaftar rawat jalan secara online.</p>
            </div>
            <!-- Card 3 -->
            <div class="bg-white p-8 rounded-xl shadow-xl border-t-4 border-red-500 hover:-translate-y-2 transition duration-300">
                <div class="text-red-500 text-4xl mb-4"><i class="fa-solid fa-truck-medical"></i></div>
                <h3 class="text-xl font-bold mb-2">IGD 24 Jam</h3>
                <p class="text-gray-500">Pelayanan gawat darurat siap siaga 24/7 dengan armada ambulans lengkap.</p>
            </div>
        </div>
    </section>

    <!-- LAYANAN SECTION -->
    <section id="layanan" class="py-20 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-800">Layanan Unggulan</h2>
                <div class="h-1 w-20 bg-teal-600 mx-auto mt-2"></div>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <!-- Service Item -->
                <div class="bg-white p-6 rounded-lg shadow hover:shadow-lg transition text-center">
                    <img src="https://img.icons8.com/fluency/96/null/stethoscope.png" alt="Poli Umum" class="mx-auto mb-4 w-16">
                    <h4 class="font-bold text-lg">Poli Umum</h4>
                </div>
                <div class="bg-white p-6 rounded-lg shadow hover:shadow-lg transition text-center">
                    <img src="https://img.icons8.com/fluency/96/null/dental-braces.png" alt="Poli Gigi" class="mx-auto mb-4 w-16">
                    <h4 class="font-bold text-lg">Poli Gigi</h4>
                </div>
                <div class="bg-white p-6 rounded-lg shadow hover:shadow-lg transition text-center">
                    <img src="https://img.icons8.com/fluency/96/null/baby-calendar.png" alt="Poli Anak" class="mx-auto mb-4 w-16">
                    <h4 class="font-bold text-lg">Poli Anak</h4>
                </div>
                <div class="bg-white p-6 rounded-lg shadow hover:shadow-lg transition text-center">
                    <img src="https://img.icons8.com/fluency/96/null/microscope.png" alt="Laboratorium" class="mx-auto mb-4 w-16">
                    <h4 class="font-bold text-lg">Laboratorium</h4>
                </div>
            </div>
        </div>
    </section>

    <!-- DASHBOARD PREVIEW (MOCKUP) -->
    <section class="py-20 bg-white">
        <div class="container mx-auto px-6 flex flex-col md:flex-row items-center gap-12">
            <div class="md:w-1/2">
                <img src="https://cdn.dribbble.com/users/1615584/screenshots/15710176/media/0d750058b857703358055c65f2479e03.jpg?compress=1&resize=800x600" alt="Dashboard SIRS" class="rounded-xl shadow-2xl">
            </div>
            <div class="md:w-1/2">
                <span class="text-teal-600 font-bold tracking-wider uppercase text-sm">Dashboard Admin</span>
                <h2 class="text-3xl font-bold mt-2 mb-4">Kelola Data Pasien dengan Mudah</h2>
                <p class="text-gray-600 mb-6 leading-relaxed">Sistem Informasi Rumah Sakit kami dilengkapi dengan dashboard admin yang user-friendly untuk mengelola rekam medis elektronik (RME), stok obat, jadwal dokter, dan tagihan pasien secara real-time.</p>
                <ul class="space-y-3">
                    <li class="flex items-center text-gray-700"><i class="fa-solid fa-check text-teal-500 mr-3"></i> Integrasi BPJS (V-Claim)</li>
                    <li class="flex items-center text-gray-700"><i class="fa-solid fa-check text-teal-500 mr-3"></i> Laporan Keuangan Otomatis</li>
                    <li class="flex items-center text-gray-700"><i class="fa-solid fa-check text-teal-500 mr-3"></i> Manajemen Apotek & Gudang</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-gray-900 text-white py-10">
        <div class="container mx-auto px-6 grid grid-cols-1 md:grid-cols-3 gap-8">
            <div>
                <h3 class="text-xl font-bold mb-4">RS. Sehat Sejahtera</h3>
                <p class="text-gray-400 text-sm">Memberikan pelayanan kesehatan terbaik dengan dukungan teknologi informasi terkini.</p>
            </div>
            <div>
                <h3 class="text-xl font-bold mb-4">Kontak Kami</h3>
                <ul class="text-gray-400 text-sm space-y-2">
                    <li><i class="fa-solid fa-location-dot mr-2"></i> Jl. Kesehatan No. 123, Jakarta</li>
                    <li><i class="fa-solid fa-phone mr-2"></i> (021) 555-0123</li>
                    <li><i class="fa-solid fa-envelope mr-2"></i> info@rs-sehat.com</li>
                </ul>
            </div>
            <div>
                <h3 class="text-xl font-bold mb-4">Jam Operasional</h3>
                <p class="text-gray-400 text-sm">IGD: 24 Jam</p>
                <p class="text-gray-400 text-sm">Poli: Senin - Sabtu (08:00 - 16:00)</p>
            </div>
        </div>
        <div class="text-center text-gray-600 text-sm mt-10 pt-4 border-t border-gray-800">
            &copy; 2023 Sistem Informasi Rumah Sakit. All rights reserved.
        </div>
    </footer>

    <!-- LOGIN MODAL -->
    <div id="loginModal" class="fixed inset-0 bg-black bg-opacity-50 hidden z-50 flex items-center justify-center backdrop-blur-sm">
        <div class="bg-white p-8 rounded-lg shadow-2xl w-96 transform transition-all scale-100">
            <div class="flex justify-between items-center mb-6">
                <h2 class="text-2xl font-bold text-gray-800">Login SIRS</h2>
                <button onclick="closeModal()" class="text-gray-400 hover:text-red-500"><i class="fa-solid fa-times text-xl"></i></button>
            </div>
            <form onsubmit="event.preventDefault(); alert('Ini hanya demo frontend. Backend belum terhubung.');">
                <div class="mb-4">
                    <label class="block text-gray-700 text-sm font-bold mb-2">Username / NIP</label>
                    <input type="text" class="w-full px-3 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-teal-500" placeholder="admin">
                </div>
                <div class="mb-6">
                    <label class="block text-gray-700 text-sm font-bold mb-2">Password</label>
                    <input type="password" class="w-full px-3 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-teal-500" placeholder="••••••">
                </div>
                <button type="submit" class="w-full bg-teal-600 text-white py-2 rounded-lg font-bold hover:bg-teal-700 transition">Masuk</button>
            </form>
        </div>
    </div>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        // Modal Logic
        function openModal() {
            const modal = document.getElementById('loginModal');
            modal.classList.remove('hidden');
        }

        function closeModal() {
            const modal = document.getElementById('loginModal');
            modal.classList.add('hidden');
        }

        // Close modal when clicking outside
        window.onclick = function(event) {
            const modal = document.getElementById('loginModal');
            if (event.target == modal) {
                closeModal();
            }
        }
    </script>
</body>
</html>
