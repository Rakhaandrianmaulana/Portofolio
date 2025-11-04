<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README.md - Proyek Aurora (Gaya GitHub)</title>
    <!-- Memuat Tailwind CSS untuk styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Menggunakan font Inter untuk teks, dan JetBrains Mono untuk kode */
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&family=JetBrains+Mono:wght@400;700&display=swap');

        body {
            font-family: 'Inter', sans-serif;
            background-color: #010409; /* Warna latar belakang GitHub Dark */
            color: #C9D1D9; /* Warna teks utama */
            line-height: 1.6;
        }

        .container-readme {
            /* Meniru card konten utama di GitHub */
            background-color: #0D1117; 
            border: 1px solid #30363D;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
        }

        /* --- Styling Elemen Markdown --- */
        .md-content h1 { @apply text-3xl font-bold border-b border-gray-700 pb-3 mb-6 mt-6 text-white; }
        .md-content h2 { @apply text-2xl font-semibold border-b border-gray-700 pb-2 mb-4 mt-6 text-gray-200; }
        .md-content h3 { @apply text-xl font-semibold mb-3 mt-4 text-blue-400; }
        .md-content p { @apply mb-4; }
        
        .md-content ul, .md-content ol { @apply list-inside mb-4 pl-4 space-y-1; }
        .md-content ul { @apply list-disc; }
        .md-content ol { @apply list-decimal; }

        .md-content a { @apply text-blue-500 hover:text-blue-400 font-medium transition duration-150; }
        
        /* Inline Code */
        .md-content code {
            font-family: 'JetBrains Mono', monospace;
            @apply bg-[#30363D] text-[#56D4D9] px-1 py-0.5 rounded text-sm;
        }

        /* Code Block (Preformatted) */
        .md-content pre {
            font-family: 'JetBrains Mono', monospace;
            @apply bg-[#0D1117] border border-gray-700 p-4 rounded-lg overflow-x-auto text-sm shadow-inner mb-4;
        }
        /* Meniru Syntax Highlighting: Warna khusus untuk variabel/keyword JS */
        .md-content pre .keyword { color: #FF7B72; font-weight: bold; } /* Merah */
        .md-content pre .string { color: #A5D6FF; } /* Biru Muda */
        .md-content pre .comment { color: #8B949E; } /* Abu-abu */
        .md-content pre .variable { color: #FFA657; } /* Oranye */

        .md-content blockquote {
            @apply border-l-4 border-blue-500 pl-4 py-2 italic text-gray-400 bg-gray-800/50 rounded-r-md;
        }

        .md-content table {
            @apply w-full text-left border-collapse mb-4;
        }
        .md-content th, .md-content td {
            @apply border border-gray-700 p-3;
        }
        .md-content th {
            @apply bg-gray-800 font-semibold text-white;
        }
    </style>
</head>
<body class="p-4 sm:p-8">

    <!-- Kontainer Utama -->
    <div class="max-w-5xl mx-auto py-8 container-readme p-6 sm:p-10 rounded-xl">

        <!-- Header dan Badges -->
        <header class="mb-8 border-b border-gray-700 pb-4">
            <!-- Badges Realistis (gunakan gambar dari Shields.io) -->
            <div class="flex flex-wrap gap-2 mb-4">
                <img src="https://img.shields.io/github/last-commit/lanavyn/aurora-project?style=flat-square&color=3B82F6&label=Update" alt="Update Terakhir">
                <img src="https://img.shields.io/github/issues/lanavyn/aurora-project?style=flat-square&color=FFC107&label=Isu" alt="Total Isu">
                <img src="https://img.shields.io/badge/Lisensi-MIT-success?style=flat-square" alt="Lisensi MIT">
                <img src="https://img.shields.io/badge/Bahasa-JS%2FHMTL-E03C31?style=flat-square" alt="Bahasa Utama">
            </div>

            <h1 class="text-4xl font-extrabold text-white">
                Proyek AURORA 🌟
            </h1>
            <p class="text-lg text-gray-400 mt-2">
                Kerangka Kerja Statis Sederhana untuk Portofolio Minimalis (Single-File).
            </p>
        </header>

        <!-- Konten Markdown -->
        <article class="md-content">

            <blockquote>
                "Sederhana adalah kompleksitas yang diselesaikan. Proyek Aurora mewujudkan prinsip ini dengan menyediakan solusi portofolio yang ringkas dan sangat cepat."
            </blockquote>

            <!-- Daftar Isi Taktis -->
            <h2 id="toc">Daftar Isi</h2>
            <ul class="list-none space-y-0 text-blue-400">
                <li><a href="#pendahuluan">1. Pendahuluan</a></li>
                <li><a href="#fitur">2. Fitur Kunci</a></li>
                <li><a href="#instalasi">3. Instalasi & Setup</a></li>
                <li><a href="#konfigurasi">4. Konfigurasi Data</a></li>
                <li><a href="#kontribusi">5. Kontribusi</a></li>
            </ul>

            <!-- Bagian 1: Pendahuluan -->
            <h2 id="pendahuluan">1. Pendahuluan</h2>
            <p>
                Proyek Aurora adalah templat HTML/JavaScript satu file yang dirancang untuk kebutuhan portofolio ultra-ringan. Dengan meminimalkan dependensi, kami memastikan kecepatan loading yang optimal dan kemudahan penyebaran (deployment). Ini adalah solusi sempurna untuk menampilkan karya Anda dengan cepat dan elegan.
            </p>

            <!-- Bagian 2: Fitur -->
            <h2 id="fitur">2. Fitur Kunci ✨</h2>
            <ul>
                <li>**Single-File Build**: Semua logika, styling, dan markup dalam satu berkas HTML.</li>
                <li>**Zero Dependencies**: Hanya menggunakan Tailwind CSS CDN untuk styling modern.</li>
                <li>**Local Storage Database**: Menyimpan komentar dan rating secara lokal tanpa perlu server backend.</li>
                <li>**Desain Adaptif**: Sepenuhnya responsif, indah di perangkat mobile maupun desktop.</li>
            </ul>

            <!-- Bagian 3: Instalasi & Setup -->
            <h2 id="instalasi">3. Instalasi & Setup 🚀</h2>
            <p>Sangat mudah! Tidak perlu <code>npm install</code> atau <code>yarn start</code>.</p>
            <ol>
                <li>Kloning repositori ini (atau salin isi file ini).</li>
                <li>Buka file <code>index.html</code> di browser Anda.</li>
                <li>Mulai modifikasi data di variabel <code class="text-green-400">PORTFOLIO_DATA</code> di bagian `<script>`.</li>
            </ol>

            <h3>Contoh Blok Kode Realistis (JavaScript)</h3>
            <pre>
<span class="comment">// Pastikan untuk mengganti data ini dengan informasi pribadi Anda</span>
<span class="keyword">const</span> <span class="variable">PORTFOLIO_DATA</span> = {
    <span class="variable">name</span>: <span class="string">"LanaVyn Official"</span>,
    <span class="variable">age</span>: 15,
    <span class="variable">region</span>: <span class="string">"Secret Java, Indonesia"</span>,
};

<span class="keyword">function</span> calculateRating(comments) {
    <span class="keyword">if</span> (comments.<span class="variable">length</span> === 0) {
        <span class="keyword">return</span> 0;
    }
    <span class="comment">// Lakukan perhitungan rata-rata</span>
    <span class="keyword">return</span> totalRating / comments.<span class="variable">length</span>;
}</pre>

            <!-- Bagian 4: Konfigurasi Data -->
            <h2 id="konfigurasi">4. Konfigurasi Data 🛠️</h2>
            <p>Tabel di bawah menunjukkan lokasi data yang harus Anda edit:</p>
            <table>
                <thead>
                    <tr>
                        <th>Lokasi Data</th>
                        <th>Variabel</th>
                        <th>Tujuan</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>&lt;script&gt; section</td>
                        <td><code>PORTFOLIO_DATA</code></td>
                        <td>Semua informasi kontak dan profil.</td>
                    </tr>
                    <tr>
                        <td>&lt;style&gt; section</td>
                        <td><code>body</code> background</td>
                        <td>Mengubah skema warna gelap ke terang.</td>
                    </tr>
                </tbody>
            </table>

            <!-- Bagian 5: Kontribusi -->
            <h2 id="kontribusi">5. Kontribusi 🤝</h2>
            <p>Jika Anda menemukan bug atau memiliki ide baru, kami sangat menghargai kontribusi Anda! Silakan buat *Issue* baru atau kirim *Pull Request* ke repositori.</p>
            
            <p class="mt-8 text-center text-gray-500 text-sm">
                &copy; 2025 LanaVyn Official. Seluruh Hak Cipta Dilindungi.
            </p>

        </article>

    </div>
</body>
</html>
