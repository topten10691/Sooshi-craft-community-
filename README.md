<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SOOSHI CRAFT - Minecraft Roleplay</title>
    <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@300;400;600&family=VT323&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-orange: #FF7F50; 
            --secondary-gold: #F4C430; 
            --bg-color: #0f0f0f;       
            --text-color: #FFFFFF;     
            --card-bg: rgba(30, 30, 30, 0.9);        
        }
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Kanit', sans-serif; background-color: var(--bg-color); color: var(--text-color); line-height: 1.6; }
        h1, h2, h3 { font-family: 'VT323', monospace; text-transform: uppercase; }
        a { text-decoration: none; color: inherit; }

        /* Navbar */
        nav {
            display: flex; justify-content: space-between; align-items: center;
            padding: 15px 5%; background-color: rgba(0, 0, 0, 0.9);
            position: fixed; width: 100%; top: 0; z-index: 1000;
            border-bottom: 2px solid var(--primary-orange);
        }
        .nav-logo { font-size: 1.5rem; color: var(--primary-orange); font-family: 'VT323', monospace; }
        .btn-discord {
            background-color: #5865F2; color: white; padding: 8px 16px;
            border-radius: 5px; font-weight: bold; transition: 0.3s;
        }

        /* Hero Section with Background Image */
        .hero {
            height: 100vh; display: flex; flex-direction: column;
            justify-content: center; align-items: center; text-align: center;
            /* ใส่รูปภาพที่คุณเพิ่งส่งมาเป็นพื้นหลัง */
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.8)), 
                        url('https://i.postimg.cc/CL4t8Cs4/JPEG_20250108_171832_4760446089207986525.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            padding: 20px;
        }

        .hero-logo {
            width: 250px; max-width: 70%; height: auto; margin-bottom: 10px;
            animation: float 3s ease-in-out infinite;
            filter: drop-shadow(0 0 20px rgba(255, 127, 80, 0.5));
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
        }

        .hero h1 { font-size: clamp(3.5rem, 12vw, 6rem); color: var(--primary-orange); text-shadow: 4px 4px 0px #000; line-height: 1; }
        .hero p { font-size: 1.2rem; max-width: 700px; margin: 15px 0 30px 0; color: #eee; text-shadow: 1px 1px 5px #000; }
        
        .cta-button {
            background-color: var(--primary-orange); color: white;
            padding: 12px 35px; font-size: 1.8rem; border-radius: 50px;
            font-family: 'VT323', monospace; border: 3px solid var(--secondary-gold);
            transition: 0.3s; cursor: pointer; box-shadow: 0 5px 20px rgba(0,0,0,0.5);
        }
        .cta-button:hover { background-color: var(--secondary-gold); color: #000; transform: scale(1.1); }

        /* Content Section */
        .container { max-width: 1100px; margin: 0 auto; padding: 100px 20px; }
        .section-title { text-align: center; font-size: 3.5rem; margin-bottom: 50px; color: var(--secondary-gold); text-shadow: 2px 2px #000; }
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; }
        .card {
            background: var(--card-bg); padding: 40px; border-radius: 20px;
            text-align: center; border: 1px solid #444; transition: 0.3s;
            backdrop-filter: blur(5px);
        }
        .card:hover { border-color: var(--primary-orange); transform: translateY(-10px); background: rgba(50, 50, 50, 0.9); }
        .card h3 { font-size: 2.2rem; margin-bottom: 15px; color: var(--primary-orange); }

        footer { padding: 40px; text-align: center; background: #000; color: #777; border-top: 1px solid var(--primary-orange); }

        @media (max-width: 600px) {
            .hero h1 { font-size: 3rem; }
            .hero-logo { width: 180px; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="nav-logo">SOOSHI CRAFT</div>
        <a href="https://discord.gg/A9xX3tTCJ" target="_blank" class="btn-discord">DISCORD</a>
    </nav>

    <header class="hero">
        <img src="https://i.postimg.cc/3RxmG8f0/1000026330.png" alt="Sooshi Craft Logo" class="hero-logo">
        <h1>SOOSHI CRAFT</h1>
        <p>เปิดประสบการณ์การเล่น Minecraft Roleplay ในโลกที่คุณเลือกเป็นอะไรก็ได้ สังคมอบอุ่น กิจกรรมสนุก และระบบที่ลื่นไหล</p>
        <a href="https://discord.gg/A9xX3tTCJ" target="_blank" class="cta-button">เข้าสู่เซิร์ฟเวอร์</a>
    </header>

    <section class="container">
        <h2 class="section-title">SERVER INFO</h2>
        <div class="grid">
            <div class="card">
                <h3>🍣 THE ROLEPLAY</h3>
                <p>สร้างตัวละครในฝัน ทำอาชีพที่คุณรัก และผูกมิตรกับผู้เล่นคนอื่นๆ ในเมืองซูชิสุดหรรษา</p>
            </div>
            <div class="card">
                <h3>💰 ECONOMY</h3>
                <p>ระบบเงินตราและการค้าขายที่สมจริง สนับสนุนให้ผู้เล่นสร้างธุรกิจและเติบโตไปด้วยกัน</p>
            </div>
            <div class="card">
                <h3>🛠️ STABILITY</h3>
                <p>เซิร์ฟเวอร์เสถียร รองรับผู้เล่นได้จำนวนมาก พร้อมทีมงานดูแลและอัปเดตระบบสม่ำเสมอ</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2024-2026 SOOSHI CRAFT Community | ยินดีต้อนรับนักผจญภัยทุกคน</p>
    </footer>

</body>
</html>
