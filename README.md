<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تهنئة عيد الفطر المبارك | المهندس إياد جمال</title>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #D4AF37;
            --dark-blue: #0A2463;
            --light-gold: #F5D7A1;
            --cream: #FFF5E0;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Tajawal', sans-serif;
            background-color: var(--dark-blue);
            color: var(--cream);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow: hidden;
            position: relative;
        }
        
        /* تأثيرات الخلفية الإسلامية */
        .islamic-pattern {
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: 
                radial-gradient(circle, var(--gold) 1px, transparent 1px),
                radial-gradient(circle, var(--gold) 1px, transparent 1px);
            background-size: 50px 50px;
            background-position: 0 0, 25px 25px;
            opacity: 0.1;
            z-index: 0;
        }
        
        .card-container {
            position: relative;
            z-index: 10;
            perspective: 1000px;
            width: 90%;
            max-width: 600px;
        }
        
        .card {
            background: linear-gradient(145deg, rgba(10, 36, 99, 0.9), rgba(10, 36, 99, 0.7));
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5),
                        0 0 0 2px var(--gold),
                        0 0 0 6px rgba(212, 175, 55, 0.3);
            transform-style: preserve-3d;
            transition: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            position: relative;
            overflow: hidden;
            backdrop-filter: blur(5px);
        }
        
        .card:hover {
            transform: translateY(-10px) rotateX(5deg);
            box-shadow: 0 30px 70px rgba(0, 0, 0, 0.6),
                        0 0 0 2px var(--gold),
                        0 0 0 10px rgba(212, 175, 55, 0.3);
        }
        
        .card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(
                to bottom right,
                transparent 45%,
                rgba(212, 175, 55, 0.1) 50%,
                transparent 55%
            );
            transform: rotate(30deg);
            animation: shine 5s infinite;
        }
        
        @keyframes shine {
            0% { transform: translateX(-100%) rotate(30deg); }
            100% { transform: translateX(100%) rotate(30deg); }
        }
        
        h1 {
            color: var(--gold);
            font-size: 2.8rem;
            margin-bottom: 30px;
            text-align: center;
            position: relative;
            text-shadow: 0 2px 10px rgba(212, 175, 55, 0.5);
        }
        
        h1::after {
            content: '';
            display: block;
            width: 100px;
            height: 3px;
            background: linear-gradient(to right, transparent, var(--gold), transparent);
            margin: 15px auto;
        }
        
        .name {
            font-size: 2rem;
            text-align: center;
            margin: 25px 0;
            background: linear-gradient(to right, var(--light-gold), var(--gold));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
            position: relative;
            display: inline-block;
            padding: 0 20px;
        }
        
        .name::before,
        .name::after {
            content: '✻';
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            color: var(--gold);
            font-size: 1.5rem;
        }
        
        .name::before {
            left: -10px;
        }
        
        .name::after {
            right: -10px;
        }
        
        p {
            font-size: 1.3rem;
            line-height: 1.8;
            margin: 20px 0;
            text-align: center;
        }
        
        .decoration {
            position: absolute;
            font-size: 2rem;
            color: rgba(212, 175, 55, 0.3);
            z-index: -1;
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(10deg); }
        }
        
        .mosque-icon {
            font-size: 4rem;
            margin: 30px 0;
            color: var(--gold);
            text-align: center;
            animation: pulse 2s infinite alternate;
        }
        
        @keyframes pulse {
            from { transform: scale(1); opacity: 0.8; }
            to { transform: scale(1.1); opacity: 1; }
        }
        
        .gold-border {
            border: 1px solid var(--gold);
            border-radius: 10px;
            padding: 20px;
            margin: 30px 0;
            position: relative;
        }
        
        .gold-border::before {
            content: '';
            position: absolute;
            top: -5px;
            left: -5px;
            right: -5px;
            bottom: -5px;
            border: 1px solid var(--gold);
            border-radius: 12px;
            pointer-events: none;
            opacity: 0.5;
        }
        
        .footer {
            margin-top: 30px;
            font-size: 0.9rem;
            text-align: center;
            color: var(--light-gold);
        }
        
        /* تأثيرات النجوم */
        .star {
            position: absolute;
            background-color: var(--gold);
            clip-path: polygon(50% 0%, 61% 35%, 98% 35%, 68% 57%, 79% 91%, 50% 70%, 21% 91%, 32% 57%, 2% 35%, 39% 35%);
            animation: twinkle var(--duration) infinite ease-in-out;
            opacity: 0;
        }
        
        @keyframes twinkle {
            0%, 100% { opacity: 0; transform: scale(0.5); }
            50% { opacity: 1; transform: scale(1); }
        }
        
        /* زر الموسيقى */
        .music-btn {
            background: linear-gradient(to right, var(--dark-blue), var(--gold));
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 50px;
            margin: 20px auto;
            display: block;
            cursor: pointer;
            font-weight: bold;
            font-size: 1rem;
            transition: all 0.3s;
            box-shadow: 0 4px 15px rgba(212, 175, 55, 0.4);
            position: relative;
            overflow: hidden;
        }
        
        .music-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(212, 175, 55, 0.6);
        }
        
        .music-btn::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to right, rgba(255,255,255,0.1), rgba(255,255,255,0));
            transform: translateX(-100%);
            transition: transform 0.4s ease;
        }
        
        .music-btn:hover::after {
            transform: translateX(100%);
        }
        
        /* هلال متحرك */
        .moon {
            position: absolute;
            font-size: 3rem;
            color: var(--gold);
            animation: orbit 20s linear infinite;
            z-index: -1;
        }
        
        @keyframes orbit {
            from { transform: rotate(0deg) translateX(150px) rotate(0deg); }
            to { transform: rotate(360deg) translateX(150px) rotate(-360deg); }
        }
    </style>
</head>
<body>
    <!-- نمط إسلامي للخلفية -->
    <div class="islamic-pattern"></div>
    
    <!-- تأثير النجوم -->
    <div id="stars-container"></div>
    
    <!-- هلالان متحركان -->
    <div class="moon" style="top: 20%; left: 10%;">🌙</div>
    <div class="moon" style="bottom: 20%; right: 10%;">🌙</div>
    
    <!-- زخارف إسلامية -->
    <div class="decoration" style="top: 10%; right: 15%;">ﷲ</div>
    <div class="decoration" style="bottom: 15%; left: 20%;">ﷺ</div>
    <div class="decoration" style="top: 30%; left: 5%;">✽</div>
    <div class="decoration" style="bottom: 40%; right: 5%;">✿</div>
    
    <div class="card-container">
        <div class="card">
            <h1>عيد فطر مبارك</h1>
            
            <div class="mosque-icon">🕌</div>
            
            <div class="gold-border">
                <div class="name">المهندس إياد جمال</div>
            </div>
            
            <p>كل عام وأنت بخير، تقبل الله منا ومنك صالح الأعمال</p>
            <p>وجعل أيامكم فرحًا وسرورًا وبركة</p>
            <p>🎉 عيدكم مبارك 🎊</p>
            
            <button class="music-btn" onclick="toggleMusic()">🎵 تشغيل موسيقى العيد</button>
            <audio id="eid-music" loop>
                <source src="https://audio-previews.elements.envatousercontent.com/files/459718666/preview.mp3" type="audio/mpeg">
                (يمكنك استبدال الرابط بأغنية من اختيارك)
            </audio>
            
            <div class="footer">
                تهنئة من القلب بمناسبة عيد الفطر المبارك
            </div>
        </div>
    </div>

    <script>
        // إنشاء النجوم المتلألئة
        function createStars() {
            const container = document.getElementById('stars-container');
            const starCount = 30;
            
            for (let i = 0; i < starCount; i++) {
                const star = document.createElement('div');
                star.className = 'star';
                star.style.left = Math.random() * 100 + 'vw';
                star.style.top = Math.random() * 100 + 'vh';
                star.style.width = (Math.random() * 10 + 5) + 'px';
                star.style.height = star.style.width;
                star.style.setProperty('--duration', (Math.random() * 3 + 2) + 's');
                star.style.animationDelay = Math.random() * 5 + 's';
                container.appendChild(star);
            }
        }
        
        // تشغيل/إيقاف الموسيقى
        function toggleMusic() {
            const music = document.getElementById('eid-music');
            const btn = document.querySelector('.music-btn');
            
            if (music.paused) {
                music.play();
                btn.innerHTML = '⏸ إيقاف الموسيقى';
            } else {
                music.pause();
                btn.innerHTML = '🎵 تشغيل موسيقى العيد';
            }
        }
        
        // تأثيرات ثلاثية الأبعاد للبطاقة
        document.querySelector('.card-container').addEventListener('mousemove', (e) => {
            const xAxis = (window.innerWidth / 2 - e.pageX) / 25;
            const yAxis = (window.innerHeight / 2 - e.pageY) / 25;
            document.querySelector('.card').style.transform = `rotateY(${xAxis}deg) rotateX(${yAxis}deg)`;
        });
        
        // إعادة البطاقة إلى وضعها الطبيعي عند مغادرة الماوس
        document.querySelector('.card-container').addEventListener('mouseleave', () => {
            document.querySelector('.card').style.transform = 'rotateY(0deg) rotateX(0deg)';
        });
        
        // تشغيل التأثيرات عند تحميل الصفحة
        window.onload = function() {
            createStars();
        };
    </script>
</body>
</html>
