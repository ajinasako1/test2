<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>猫の癒やし - 心を整えるひととき</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=M+PLUS+Rounded+1c:wght@300;500;700&display=swap');

        body {
            font-family: 'M PLUS Rounded+1c', sans-serif;
            background-color: #fff9f5;
            color: #5d4037;
        }

        .hero-gradient {
            background: linear-gradient(135deg, #ffeddb 0%, #ffd1ba 100%);
        }

        .cat-card:hover {
            transform: translateY(-5px);
            transition: all 0.3s ease;
        }

        .purr-animation {
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        .scroll-section {
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.6s ease-out;
        }

        .scroll-section.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav class="fixed w-full z-50 bg-white/80 backdrop-blur-md border-b border-orange-100">
        <div class="max-w-6xl mx-auto px-6 py-4 flex justify-between items-center">
            <div class="text-2xl font-bold text-orange-400 flex items-center gap-2">
                <i class="fas fa-cat"></i>
                <span>NekoRelief</span>
            </div>
            <div class="hidden md:flex gap-8 text-sm font-medium">
                <a href="#healing" class="hover:text-orange-400 transition">癒やしの秘密</a>
                <a href="#gallery" class="hover:text-orange-400 transition">ギャラリー</a>
                <a href="#benefits" class="hover:text-orange-400 transition">科学的効果</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="pt-32 pb-20 px-6 hero-gradient">
        <div class="max-w-4xl mx-auto text-center">
            <h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight">
                その「ゴロゴロ」が、<br><span class="text-orange-500">明日への活力になる。</span>
            </h1>
            <p class="text-lg md:text-xl mb-10 text-gray-600">
                忙しい毎日に、猫という名の休息を。ただ見つめるだけで、心はもっと軽くなる。
            </p>
            <div class="inline-block bg-white p-4 rounded-full shadow-lg purr-animation">
                <p class="text-orange-400 font-bold">画面越しに、深呼吸をどうぞ 🐾</p>
            </div>
        </div>
    </header>

    <!-- Healing Section -->
    <section id="healing" class="py-20 px-6 max-w-6xl mx-auto scroll-section">
        <div class="grid md:grid-cols-2 gap-12 items-center">
            <div>
                <img src="https://images.unsplash.com/photo-1514888286974-6c03e2ca1dba?auto=format&fit=crop&w=800&q=80" 
                     alt="[丸まって眠る猫]" 
                     class="rounded-3xl shadow-2xl"
                     onerror="this.src='https://via.placeholder.com/800x600?text=Sleeping+Cat'">
            </div>
            <div>
                <h2 class="text-3xl font-bold mb-6">なぜ、猫はこれほど愛おしいのか</h2>
                <p class="text-gray-600 leading-relaxed mb-6">
                    猫の丸み、柔らかい毛並み、そして無防備な寝顔。これらは私たちの脳に「守りたい」という本能的な感情を呼び起こし、ストレスホルモンであるコルチゾールの減少を助けます。
                </p>
                <ul class="space-y-4">
                    <li class="flex items-start gap-3">
                        <i class="fas fa-heart text-pink-400 mt-1"></i>
                        <span><strong>肉球の魔法:</strong> ぷにぷにとした感触は触覚を通じた癒やしを与えます。</span>
                    </li>
                    <li class="flex items-start gap-3">
                        <i class="fas fa-music text-blue-400 mt-1"></i>
                        <span><strong>ゴロゴロ音の周波数:</strong> 猫の喉を鳴らす音（20〜50ヘルツ）は、骨密度を高め、血圧を下げると言われています。</span>
                    </li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" class="py-20 bg-orange-50 px-6">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12">心ほどける、猫たちの日常</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Card 1 -->
                <div class="cat-card bg-white rounded-2xl overflow-hidden shadow-md">
                    <img src="https://images.unsplash.com/photo-1573865526739-10659fec78a5?auto=format&fit=crop&w=500&q=80" 
                         alt="[じっと見つめる猫]" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="font-bold mb-2">見つめるだけで。</h3>
                        <p class="text-sm text-gray-500">アイコンタクトは信頼と安心の証。あなたを優しく包み込みます。</p>
                    </div>
                </div>
                <!-- Card 2 -->
                <div class="cat-card bg-white rounded-2xl overflow-hidden shadow-md">
                    <img src="https://images.unsplash.com/photo-1548247416-ec66f4900b2e?auto=format&fit=crop&w=500&q=80" 
                         alt="[伸びをする猫]" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="font-bold mb-2">自由気ままに。</h3>
                        <p class="text-sm text-gray-500">「頑張りすぎなくていいよ」というメッセージを体現しています。</p>
                    </div>
                </div>
                <!-- Card 3 -->
                <div class="cat-card bg-white rounded-2xl overflow-hidden shadow-md">
                    <img src="https://images.unsplash.com/photo-1511497584788-876760111969?auto=format&fit=crop&w=500&q=80" 
                         alt="[一緒にくつろぐ猫]" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="font-bold mb-2">寄り添う温度。</h3>
                        <p class="text-sm text-gray-500">ただそこにいるだけで、孤独感は消え去っていきます。</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Scientific Benefits -->
    <section id="benefits" class="py-20 px-6 max-w-4xl mx-auto text-center scroll-section">
        <h2 class="text-3xl font-bold mb-10">科学が証明した猫のパワー</h2>
        <div class="grid md:grid-cols-3 gap-8">
            <div class="p-6 bg-white rounded-xl shadow-sm border border-orange-100">
                <div class="text-3xl text-orange-500 mb-4"><i class="fas fa-smile-beam"></i></div>
                <h4 class="font-bold mb-2">オキシトシン</h4>
                <p class="text-xs text-gray-500">「幸せホルモン」が増加し、幸福感が高まります。</p>
            </div>
            <div class="p-6 bg-white rounded-xl shadow-sm border border-orange-100">
                <div class="text-3xl text-orange-500 mb-4"><i class="fas fa-wind"></i></div>
                <h4 class="font-bold mb-2">血圧の安定</h4>
                <p class="text-xs text-gray-500">撫でることで副交感神経が優位になり、リラックス状態に。</p>
            </div>
            <div class="p-6 bg-white rounded-xl shadow-sm border border-orange-100">
                <div class="text-3xl text-orange-500 mb-4"><i class="fas fa-bed"></i></div>
                <h4 class="font-bold mb-2">安眠効果</h4>
                <p class="text-xs text-gray-500">寝る前に猫の動画を見るだけでも睡眠の質が改善されます。</p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12 px-6">
        <div class="max-w-6xl mx-auto flex flex-col md:flex-row justify-between items-center gap-6">
            <div class="text-xl font-bold flex items-center gap-2">
                <i class="fas fa-cat"></i> NekoRelief
            </div>
            <p class="text-gray-400 text-sm">© 2024 NekoRelief Project. 全ての猫たちに感謝を込めて。</p>
            <div class="flex gap-4">
                <a href="#" class="hover:text-orange-400 transition"><i class="fab fa-instagram text-xl"></i></a>
                <a href="#" class="hover:text-orange-400 transition"><i class="fab fa-twitter text-xl"></i></a>
            </div>
        </div>
    </footer>

    <script>
        // Simple Scroll Reveal Animation
        const observerOptions = {
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.scroll-section').forEach(section => {
            observer.observe(section);
        });

        // Smooth Scroll for Navigation
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
</html># test2
