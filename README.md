<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README.md Web Terbaik</title>
    <!-- Memuat Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&family=JetBrains+Mono:wght@400;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0F172A; /* Slate 900 - Latar belakang gelap */
            color: #E2E8F0; /* Slate 200 - Warna teks utama */
            line-height: 1.6;
        }
        /* Styling untuk konten (meniru Markdown) */
        .markdown-body h1 { @apply text-4xl font-extrabold border-b border-blue-500/50 pb-3 mb-6 mt-8 text-white; }
        .markdown-body h2 { @apply text-2xl font-bold border-b border-gray-600 pb-2 mb-4 mt-6 text-slate-200; }
        .markdown-body h3 { @apply text-xl font-semibold mb-3 mt-4 text-blue-300; }
        .markdown-body p { @apply mb-4; }
        .markdown-body ul, .markdown-body ol { @apply list-inside mb-4 pl-4 space-y-2; }
        .markdown-body ul { @apply list-disc; }
        .markdown-body ol { @apply list-decimal; }
        .markdown-body a { @apply text-blue-400 hover:text-blue-300 underline transition duration-200; }
        .markdown-body code {
            font-family: 'JetBrains Mono', monospace;
            @apply bg-slate-700/50 text-yellow-300 px-1 py-0.5 rounded text-sm;
        }
        .markdown-body pre {
            font-family: 'JetBrains Mono', monospace;
            @apply bg-slate-800 p-4 rounded-lg overflow-x-auto shadow-lg text-green-300 text-sm;
        }
        .badge {
            @apply inline-flex items-center px-3 py-1 text-xs font-medium rounded-full;
        }
    </style>
</head>
<body class="p-4 sm:p-8">

    <!-- Container Utama: Maksimal 800px lebar, terpusat -->
    <div class="max-w-4xl mx-auto py-10 card p-6 sm:p-10 rounded-2xl shadow-2xl bg-slate-900 border border-slate-700">

        <!-- Header / Judul Proyek -->
        <header class="text-center mb-10">
            <div class="space-x-2 mb-4">
                <span class="badge bg-green-500/20 text-green-400">Versi 1.0.0</span>
                <span class="badge bg-purple-500/20 text-purple-400">Lisensi MIT</span>
                <span class="badge bg-yellow-500/20 text-yellow-400">Status: Aktif</span>
            </div>
            <h1 class="text-6xl font-black text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-indigo-500 mb-2">
                PROJECT KODE-NAMA: ARGON
            </h1>
            <p class="text-xl text-slate-400 italic">Solusi Inovatif untuk Manajemen Portofolio Digital.</p>
        </header>
        
        <!-- Badge / Status Proyek -->
        <div class="flex flex-wrap justify-center gap-3 mb-10">
            <!-- Contoh Badge Fiktif -->
            <img src="https://img.shields.io/github/stars/user/repo?style=flat&color=4C1D95&label=Stars" alt="GitHub Stars">
            <img src="https://img.shields.io/github/last-commit/user/repo?style=flat&color=3B82F6" alt="Last Commit">
            <img src="https://img.shields.io/badge/Dibuat%20dengan-HTML%2FJS-red?style=flat" alt="Made With HTML/JS">
        </div>

        <!-- Konten README ala Markdown -->
        <article class="markdown-body">
            
            <!-- Deskripsi Singkat -->
            <p class="text-lg text-slate-300">
                **Project Argon** adalah kerangka kerja (framework) minimalis yang dirancang untuk memfasilitasi pembangunan portofolio web tunggal yang sangat cepat dan ringan. Fokus utamanya adalah pada kecepatan loading, responsivitas, dan kemudahan deployment (penyebaran). Ini adalah jawaban untuk kebutuhan dokumentasi yang ringkas dan efektif.
            </p>

            <!-- Daftar Isi -->
            <h2>Daftar Isi</h2>
            <ul>
                <li><a href="#instalasi">Instalasi Cepat</a></li>
                <li><a href="#fitur-unggul">Fitur Unggulan</a></li>
                <li><a href="#penggunaan">Panduan Penggunaan</a></li>
                <li><a href="#kontribusi">Kontribusi dan Dukungan</a></li>
            </ul>

            <!-- Instalasi -->
            <h2 id="instalasi">🚀 Instalasi Cepat</h2>
            <p>Untuk menjalankan proyek ini secara lokal, ikuti langkah-langkah sederhana di bawah ini. Tidak diperlukan instalasi Node.js atau paket manager!</p>
            
            <h3>1. Kloning Repositori</h3>
            <pre><code>git clone https://github.com/lanavyn/argon.git
cd argon</code></pre>

            <h3>2. Jalankan File</h3>
            <p>Buka file <code>index.html</code> (atau <code>readme_web.html</code> ini) langsung di browser pilihan Anda (Chrome/Firefox). Selesai!</p>

            <!-- Fitur Unggulan -->
            <h2 id="fitur-unggul">✨ Fitur Unggulan</h2>
            <ul class="list-disc">
                <li>**Desain Single-File**: Semua kode (HTML, CSS, JS) berada dalam satu file untuk portabilitas maksimum.</li>
                <li>**Full Responsive**: Tampilan optimal di semua ukuran perangkat (Mobile, Tablet, Desktop).</li>
                <li>**Minimal Dependencies**: Hanya menggunakan Tailwind CSS CDN untuk styling.</li>
                <li>**Skrip Ringan**: JavaScript murni yang fokus pada performa.</li>
            </ul>

            <!-- Penggunaan -->
            <h2 id="penggunaan">🛠️ Panduan Penggunaan</h2>
            
            <h3>Struktur Data</h3>
            <p>Semua data portofolio utama disimpan dalam objek JavaScript <code>PORTFOLIO_DATA</code> untuk kemudahan modifikasi. Anda hanya perlu mengedit bagian ini.</p>
            <pre><code>const PORTFOLIO_DATA = {
    name: "LanaVyn Official",
    age: 15,
    favoriteColor: "Blue",
    // ... data lainnya
};</code></pre>

            <h3>Kustomisasi Warna</h3>
            <p>Untuk mengubah tema warna utama dari Biru ke Merah, cukup ganti semua instance <code>blue-400</code> menjadi <code>red-400</code> dalam tag <code>&lt;style&gt;</code> di bagian head.</p>
            
            <!-- Kontribusi -->
            <h2 id="kontribusi">🤝 Kontribusi dan Dukungan</h2>
            <p>Kontribusi Anda sangat kami hargai! Jika Anda memiliki saran, laporkan <a href="#">issue</a>, atau kirimkan <a href="#">pull request</a>.</p>
            
            <p class="text-sm italic text-slate-500 mt-8">Dibuat dengan semangat oleh LanaVyn Official.</p>
        </article>
        
        <!-- Footer / Lisensi -->
        <footer class="text-center mt-12 pt-6 border-t border-slate-700/50">
            <p class="text-xs text-slate-500">
                &copy; 2025 Project Argon. Dirilis di bawah <a href="#" class="text-blue-400 hover:text-blue-300">Lisensi MIT</a>.
            </p>
        </footer>

    </div>
</body>
</html>
