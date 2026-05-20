free_fire_techniques.html

html_code = '''<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تقنيات فري فاير</title>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Tajawal', sans-serif;
            background: #000;
            color: #fff;
            overflow-x: hidden;
        }
        
        /* Hero Section with Red Sun */
        .hero {
            position: relative;
            min-height: 100vh;
            background: linear-gradient(180deg, #0a0000 0%, #1a0000 30%, #2d0000 60%, #0d0000 100%);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
            padding-top: 60px;
            overflow: hidden;
        }
        
        /* Animated Stars */
        .stars {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        
        .star {
            position: absolute;
            width: 2px;
            height: 2px;
            background: #fff;
            border-radius: 50%;
            animation: twinkle 2s infinite;
        }
        
        @keyframes twinkle {
            0%, 100% { opacity: 0.3; }
            50% { opacity: 1; }
        }
        
        /* Red Sun */
        .sun-container {
            position: relative;
            width: 300px;
            height: 300px;
            margin: 40px auto;
        }
        
        .sun {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 200px;
            height: 200px;
            background: radial-gradient(circle, #000 30%, #1a0000 50%, #330000 70%, #ff0000 100%);
            border-radius: 50%;
            box-shadow: 
                0 0 60px 20px rgba(255, 0, 0, 0.6),
                0 0 120px 40px rgba(255, 0, 0, 0.3),
                0 0 200px 60px rgba(255, 0, 0, 0.1);
        }
        
        .sun-rays {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 280px;
            height: 280px;
            border-radius: 50%;
            background: conic-gradient(
                from 0deg,
                transparent 0deg,
                rgba(255, 0, 0, 0.1) 10deg,
                transparent 20deg,
                rgba(255, 0, 0, 0.15) 30deg,
                transparent 40deg,
                rgba(255, 0, 0, 0.1) 50deg,
                transparent 60deg,
                rgba(255, 0, 0, 0.2) 70deg,
                transparent 80deg,
                rgba(255, 0, 0, 0.1) 90deg,
                transparent 100deg,
                rgba(255, 0, 0, 0.15) 110deg,
                transparent 120deg,
                rgba(255, 0, 0, 0.1) 130deg,
                transparent 140deg,
                rgba(255, 0, 0, 0.2) 150deg,
                transparent 160deg,
                rgba(255, 0, 0, 0.1) 170deg,
                transparent 180deg,
                rgba(255, 0, 0, 0.15) 190deg,
                transparent 200deg,
                rgba(255, 0, 0, 0.1) 210deg,
                transparent 220deg,
                rgba(255, 0, 0, 0.2) 230deg,
                transparent 240deg,
                rgba(255, 0, 0, 0.1) 250deg,
                transparent 260deg,
                rgba(255, 0, 0, 0.15) 270deg,
                transparent 280deg,
                rgba(255, 0, 0, 0.1) 290deg,
                transparent 300deg,
                rgba(255, 0, 0, 0.2) 310deg,
                transparent 320deg,
                rgba(255, 0, 0, 0.1) 330deg,
                transparent 340deg,
                rgba(255, 0, 0, 0.15) 350deg,
                transparent 360deg
            );
            animation: rotate 20s linear infinite;
        }
        
        @keyframes rotate {
            from { transform: translate(-50%, -50%) rotate(0deg); }
            to { transform: translate(-50%, -50%) rotate(360deg); }
        }
        
        /* Title */
        .title {
            font-size: 3.5rem;
            font-weight: 900;
            text-align: center;
            background: linear-gradient(135deg, #ff6b35 0%, #ff0000 50%, #ff6b35 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-shadow: 0 0 30px rgba(255, 0, 0, 0.5);
            margin-bottom: 20px;
            position: relative;
            z-index: 10;
            letter-spacing: 2px;
        }
        
        /* Red Clouds */
        .clouds-bottom {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 200px;
            background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 1440 320'%3E%3Cpath fill='%234a0000' fill-opacity='0.8' d='M0,224L48,213.3C96,203,192,181,288,181.3C384,181,480,203,576,224C672,245,768,267,864,261.3C960,256,1056,224,1152,208C1248,192,1344,192,1392,192L1440,192L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z'%3E%3C/path%3E%3Cpath fill='%23660000' fill-opacity='0.6' d='M0,256L48,245.3C96,235,192,213,288,213.3C384,213,480,235,576,250.7C672,267,768,277,864,266.7C960,256,1056,224,1152,218.7C1248,213,1344,235,1392,245.3L1440,256L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z'%3E%3C/path%3E%3C/svg%3E") no-repeat bottom;
            background-size: cover;
        }
        
        /* Player Card Section */
        .player-section {
            background: linear-gradient(180deg, #0d0000 0%, #1a0000 50%, #0a0000 100%);
            padding: 60px 20px;
            position: relative;
        }
        
        .player-card {
            max-width: 600px;
            margin: 0 auto;
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.1) 0%, rgba(255, 255, 255, 0.05) 100%);
            backdrop-filter: blur(10px);
            border: 2px solid rgba(255, 0, 0, 0.3);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 
                0 0 30px rgba(255, 0, 0, 0.2),
                inset 0 0 30px rgba(255, 0, 0, 0.05);
            position: relative;
            overflow: hidden;
        }
        
        .player-card::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(45deg, #ff0000, #ff6b35, #ff0000);
            border-radius: 20px;
            opacity: 0.3;
            z-index: -1;
        }
        
        .card-header {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 15px;
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 2px solid rgba(255, 0, 0, 0.3);
        }
        
        .card-title {
            font-size: 1.8rem;
            font-weight: 700;
            color: #fff;
            text-shadow: 0 0 10px rgba(255, 0, 0, 0.5);
        }
        
        .atom-icon {
            font-size: 2rem;
            animation: spin 10s linear infinite;
        }
        
        @keyframes spin {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        .card-content {
            display: flex;
            gap: 30px;
            align-items: flex-start;
        }
        
        .character-img {
            width: 150px;
            height: 200px;
            object-fit: cover;
            border-radius: 15px;
            border: 3px solid rgba(255, 0, 0, 0.5);
            box-shadow: 0 0 20px rgba(255, 0, 0, 0.3);
        }
        
        .player-info {
            flex: 1;
        }
        
        .avatar-container {
            display: flex;
            justify-content: flex-end;
            margin-bottom: 20px;
        }
        
        .avatar {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            border: 3px solid rgba(255, 107, 53, 0.8);
            object-fit: cover;
            box-shadow: 0 0 15px rgba(255, 107, 53, 0.4);
        }
        
        .info-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 0;
            border-bottom: 1px solid rgba(255, 0, 0, 0.2);
        }
        
        .info-label {
            color: #ff6b35;
            font-weight: 700;
            font-size: 1.1rem;
        }
        
        .info-value {
            color: #fff;
            font-weight: 700;
            font-size: 1.1rem;
        }
        
        .freefire-logo {
            width: 120px;
            margin-top: 20px;
            filter: drop-shadow(0 0 10px rgba(255, 0, 0, 0.5));
        }
        
        .card-footer {
            margin-top: 20px;
            padding-top: 15px;
            border-top: 2px solid rgba(255, 0, 0, 0.3);
            text-align: center;
            color: #aaa;
            font-size: 0.9rem;
            line-height: 1.6;
        }
        
        .warning-icon {
            color: #ff0000;
            font-size: 1.2rem;
        }
        
        /* Responsive */
        @media (max-width: 600px) {
            .title {
                font-size: 2.5rem;
            }
            
            .card-content {
                flex-direction: column;
                align-items: center;
            }
            
            .character-img {
                width: 120px;
                height: 160px;
            }
            
            .player-info {
                width: 100%;
            }
        }
        
        /* Glow Animation */
        .glow-text {
            animation: glow 2s ease-in-out infinite alternate;
        }
        
        @keyframes glow {
            from { text-shadow: 0 0 10px rgba(255, 0, 0, 0.5); }
            to { text-shadow: 0 0 20px rgba(255, 0, 0, 0.8), 0 0 30px rgba(255, 107, 53, 0.5); }
        }
    </style>
</head>
<body>
    <!-- Hero Section -->
    <section class="hero">
        <div class="stars" id="stars"></div>
        
        <h1 class="title glow-text">تقنيات فري فاير</h1>
        
        <div class="sun-container">
            <div class="sun-rays"></div>
            <div class="sun"></div>
        </div>
        
        <div class="clouds-bottom"></div>
    </section>
    
    <!-- Player Card Section -->
    <section class="player-section">
        <div class="player-card">
            <div class="card-header">
                <span class="atom-icon">⚛</span>
                <h2 class="card-title">رخصة فري فاير</h2>
            </div>
            
            <div class="card-content">
                <img src="CHARACTER_IMAGE_URL" alt="شخصية فري فاير" class="character-img" id="characterImg">
                
                <div class="player-info">
                    <div class="avatar-container">
                        <img src="AVATAR_IMAGE_URL" alt="الصورة الشخصية" class="avatar" id="avatarImg">
                    </div>
                    
                    <div class="info-row">
                        <span class="info-label">الاسم:</span>
                        <span class="info-value">الفاعوري</span>
                    </div>
                    
                    <div class="info-row">
                        <span class="info-label">المنطقة:</span>
                        <span class="info-value">سوري_حمص</span>
                    </div>
                    
                    <div class="info-row">
                        <span class="info-label">اسم اللاعب:</span>
                        <span class="info-value">ابو خالد</span>
                    </div>
                    
                    <div class="info-row">
                        <span class="info-label">الوزن:</span>
                        <span class="info-value">56</span>
                    </div>
                    
                    <div class="info-row">
                        <span class="info-label">الطول:</span>
                        <span class="info-value">156</span>
                    </div>
                    
                    <img src="FREE_FIRE_LOGO_URL" alt="Free Fire" class="freefire-logo" id="logoImg">
                </div>
            </div>
            
            <div class="card-footer">
                <span class="warning-icon">☢</span>
                الرجاء عدم الاقتراب او التعرض لصاحب البطاقة<br>
                يمكنه الدفاع عن نفسه ضد اكثر من شخص
            </div>
        </div>
    </section>
    
    <script>
        // Generate random stars
        const starsContainer = document.getElementById('stars');
        for (let i = 0; i < 100; i++) {
            const star = document.createElement('div');
            star.className = 'star';
            star.style.left = Math.random() * 100 + '%';
            star.style.top = Math.random() * 100 + '%';
            star.style.animationDelay = Math.random() * 2 + 's';
            star.style.width = Math.random() * 3 + 1 + 'px';
            star.style.height = star.style.width;
            starsContainer.appendChild(star);
        }
        
        // Image error handling - show placeholders if images fail to load
        const placeholderChar = 'data:image/svg+xml,%3Csvg xmlns=\'http://www.w3.org/2000/svg\' width=\'150\' height=\'200\'%3E%3Crect fill=\'%23333\' width=\'150\' height=\'200\'/%3E%3Ctext fill=\'%23ff6b35\' font-family=\'Arial\' font-size=\'14\' x=\'50%25\' y=\'50%25\' text-anchor=\'middle\'%3Eشخصية%3C/text%3E%3C/svg%3E';
        
        const placeholderAvatar = 'data:image/svg+xml,%3Csvg xmlns=\'http://www.w3.org/2000/svg\' width=\'80\' height=\'80\'%3E%3Ccircle fill=\'%23333\' cx=\'40\' cy=\'40\' r=\'40\'/%3E%3Ctext fill=\'%23ff6b35\' font-family=\'Arial\' font-size=\'12\' x=\'50%25\' y=\'50%25\' text-anchor=\'middle\'%3Eصورة%3C/text%3E%3C/svg%3E';
        
        const placeholderLogo = 'data:image/svg+xml,%3Csvg xmlns=\'http://www.w3.org/2000/svg\' width=\'120\' height=\'40\'%3E%3Crect fill=\'%23333\' width=\'120\' height=\'40\'/%3E%3Ctext fill=\'%23ff6b35\' font-family=\'Arial\' font-weight=\'bold\' font-size=\'16\' x=\'50%25\' y=\'50%25\' text-anchor=\'middle\'%3EFREE FIRE%3C/text%3E%3C/svg%3E';
        
        document.getElementById('characterImg').onerror = function() {
            this.src = placeholderChar;
        };
        
        document.getElementById('avatarImg').onerror = function() {
            this.src = placeholderAvatar;
        };
        
        document.getElementById('logoImg').onerror = function() {
            this.src = placeholderLogo;
        };
    </script>
</body>
</html>'''

# Save the HTML file
with open('/mnt/agents/output/free_fire_techniques.html', 'w', encoding='utf-8') as f:
    f.write(html_code)

print("✅ تم إنشاء الموقع بنجاح!")
print("📁 الملف محفوظ في: /mnt/agents/output/free_fire_techniques.html")
