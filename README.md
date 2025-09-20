<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>4 frands - أربعة أصدقاء</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Cairo', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
            direction: rtl;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .header {
            text-align: center;
            margin-bottom: 40px;
            color: white;
        }
        
        .header h1 {
            font-size: 3rem;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            animation: bounce 2s infinite;
        }
        
        .header p {
            font-size: 1.2rem;
            opacity: 0.9;
        }
        
        .friends-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }
        
        .friend-card {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            transform: translateY(0);
            transition: all 0.3s ease;
            border: 3px solid transparent;
            background-clip: padding-box;
        }
        
        .friend-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
            border-color: #667eea;
        }
        
        .friend-card.soualimen {
            background: linear-gradient(135deg, #ffeaa7, #fdcb6e);
        }
        
        .friend-card.eya {
            background: linear-gradient(135deg, #2d3436, #636e72);
            color: white;
        }
        
        .friend-card.youssef {
            background: linear-gradient(135deg, #74b9ff, #0984e3);
            color: white;
        }
        
        .friend-card.dali {
            background: linear-gradient(135deg, #fd79a8, #e84393);
            color: white;
        }
        
        .friend-name {
            font-size: 2rem;
            font-weight: 700;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }
        
        .friend-traits {
            list-style: none;
            margin-bottom: 30px;
        }
        
        .friend-traits li {
            font-size: 1.1rem;
            margin-bottom: 10px;
            padding: 8px 15px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 50px;
            display: inline-block;
            margin: 5px;
            backdrop-filter: blur(10px);
        }
        
        .instagram-btn {
            background: linear-gradient(45deg, #833ab4, #fd1d1d, #fcb045);
            color: white;
            padding: 12px 30px;
            border: none;
            border-radius: 50px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            text-decoration: none;
            display: inline-block;
            transition: all 0.3s ease;
            text-align: center;
        }
        
        .instagram-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(131, 58, 180, 0.4);
        }
        
        .footer {
            text-align: center;
            color: white;
            font-size: 1.1rem;
            margin-top: 40px;
        }
        
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0);
            }
            40% {
                transform: translateY(-10px);
            }
            60% {
                transform: translateY(-5px);
            }
        }
        
        @media (max-width: 768px) {
            .header h1 {
                font-size: 2rem;
            }
            
            .friends-grid {
                grid-template-columns: 1fr;
                gap: 20px;
            }
            
            .friend-card {
                padding: 20px;
            }
            
            body {
                padding: 10px;
            }
        }
        
        .emoji-float {
            position: fixed;
            font-size: 2rem;
            animation: float 6s ease-in-out infinite;
            pointer-events: none;
            opacity: 0.7;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
        }
        
        .emoji-1 { top: 10%; left: 10%; animation-delay: 0s; }
        .emoji-2 { top: 20%; right: 15%; animation-delay: 1s; }
        .emoji-3 { bottom: 30%; left: 20%; animation-delay: 2s; }
        .emoji-4 { bottom: 10%; right: 10%; animation-delay: 3s; }
    </style>
</head>
<body>
    <div class="emoji-float emoji-1">🤣</div>
    <div class="emoji-float emoji-2">❤️</div>
    <div class="emoji-float emoji-3">🥲</div>
    <div class="emoji-float emoji-4">😑</div>
    
    <div class="container">
        <header class="header">
            <h1>4 friends ❤️ 🎉</h1>
            <p> my best friend ❤️ 🌟</p>
        </header>
        
        <div class="friends-grid">
            <!-- بطاقة سليمان -->
            <div class="friend-card soualimen">
                <div class="friend-name">
                    <span>soualimen</span>
                    <span>⚡</span>
                </div>
                <ul class="friend-traits">
                    <li>الذكي صاحب الموقع 🤓</li>
                    <li>وخبير البهامة 🤦</li>
                </ul>
                <a href="https://www.instagram.com/soulaimen_999?igsh=MWNuMXRqeHJ1bWRtbQ==" 
                   target="_blank" class="instagram-btn">
                     Instagram 📸
                </a>
            </div>
            
            <!-- بطاقة إيا -->
            <div class="friend-card eya">
                <div class="friend-name">
                    <span>eya</span>
                    <span>🖤</span>
                </div>
                <ul class="friend-traits">
                    <li>قصيرة 🐈</li>
                    <li>لسنها طويل 👅</li>
                    <li>وتحب BTS 🥔</li>
                </ul>
                <a href="https://www.instagram.com/9.svxn?igsh=MXBveDVuajg1aGR3Mw==" 
                   target="_blank" class="instagram-btn">
                     Instagram 📸
                </a>
            </div>
            
            <!-- بطاقة يوسف -->
            <div class="friend-card youssef">
                <div class="friend-name">
                    <span>Youssef</span>
                    <span>💫</span>
                </div>
                <ul class="friend-traits">
                    <li>طويل 🗼</li>
                    <li>بهيم 🤣</li>
                    <li>وديما مدبرم 😑</li>
                </ul>
                <a href="https://www.instagram.com/ysf_____333?igsh=MTN3dnhrNGx3ZWZnbQ==" 
                   target="_blank" class="instagram-btn">
                     Instagram 📸
                </a>
            </div>
            
            <!-- بطاقة دالي -->
            <div class="friend-card dali">
                <div class="friend-name">
                    <span>Dali</span>
                    <span>🎉</span>
                </div>
                <ul class="friend-traits">
                    <li>قصير 🐈</li>
                    <li>بهيم مع البنات 🫏</li>
                    <li>وميتحركش من بلاصتو 🧱</li>
                </ul>
                <a href="https://www.instagram.com/mohamedali_isaoui?igsh=anZkd3NiZmhpODE=" 
                   target="_blank" class="instagram-btn">
                    Instagram 📸
                </a>
            </div>
        </div>
        
        <footer class="footer">
            <p>my best friends ❤️ 2025</p>
        </footer>
    </div>
    
    <script>
        // إضافة تأثيرات تفاعلية
        document.addEventListener('DOMContentLoaded', function() {
            const cards = document.querySelectorAll('.friend-card');
            
            cards.forEach(card => {
                card.addEventListener('mouseenter', function() {
                    this.style.transform = 'translateY(-15px) scale(1.02)';
                });
                
                card.addEventListener('mouseleave', function() {
                    this.style.transform = 'translateY(0) scale(1)';
                });
            });
            
            // تأثير النقر على الأزرار
            const buttons = document.querySelectorAll('.instagram-btn');
            buttons.forEach(btn => {
                btn.addEventListener('click', function(e) {
                    this.style.transform = 'scale(0.95)';
                    setTimeout(() => {
                        this.style.transform = 'scale(1.05)';
                    }, 150);
                });
            });
        });
        
        // إضافة إيموجيات عشوائية
        function createRandomEmoji() {
            const emojis = ['🤣', '🤓', '😑', '❤️', '🥲', '🎉', '⚡', '🖤', '💫'];
            const emoji = document.createElement('div');
            emoji.innerHTML = emojis[Math.floor(Math.random() * emojis.length)];
            emoji.className = 'emoji-float';
            emoji.style.left = Math.random() * 100 + '%';
            emoji.style.top = Math.random() * 100 + '%';
            emoji.style.animationDuration = (Math.random() * 3 + 3) + 's';
            
            document.body.appendChild(emoji);
            
            setTimeout(() => {
                emoji.remove();
            }, 6000);
        }
        
        // إنشاء إيموجي عشوائي كل 3 ثوان
        setInterval(createRandomEmoji, 3000);
    </script>
</body>
</html>
