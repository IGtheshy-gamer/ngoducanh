<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ngô Đức Anh - Portfolio</title>
    <style>
        :root {
            --bg-color: #0f221b;
            --accent-gold: #e2b714;
            --text-light: #f4efe2;
            --card-bg: #183329;
        }
        body {
            margin: 0;
            padding: 0;
            background-color: var(--bg-color);
            color: var(--text-light);
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 8%;
        }
        .logo { font-weight: bold; font-size: 1.2rem; color: var(--accent-gold); }
        nav a { color: var(--text-light); margin-left: 20px; text-decoration: none; font-size: 0.9rem; }
        
        .container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            padding: 40px 8%;
            align-items: center;
        }
        .hero h1 { font-size: 3.5rem; margin: 10px 0; line-height: 1.1; }
        .hero p { line-height: 1.6; color: #b5c4bd; }
        .btn-gold {
            background-color: var(--accent-gold);
            color: #000;
            border: none;
            padding: 12px 24px;
            font-weight: bold;
            cursor: pointer;
            border-radius: 4px;
            margin-right: 15px;
        }
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin-top: 40px;
            border-top: 1px solid #23473a;
            padding-top: 20px;
        }
        .stat-box h3 { color: var(--accent-gold); margin: 0; font-size: 1.8rem; }
        .stat-box p { font-size: 0.8rem; margin: 5px 0 0 0; color: #8fa89d; }

        /* Monopoly Board CSS Layout */
        .board {
            width: 450px;
            height: 450px;
            border: 4px solid var(--accent-gold);
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            grid-template-rows: repeat(5, 1fr);
            gap: 2px;
            background-color: var(--accent-gold);
            margin: 0 auto;
        }
        .tile {
            background-color: #e2d7c5;
            color: #111;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            font-size: 0.7rem;
            font-weight: bold;
            text-align: center;
            padding: 5px;
        }
        .center-board {
            grid-column: 2 / 5;
            grid-row: 2 / 5;
            background-color: var(--bg-color);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            border: 2px solid var(--accent-gold);
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">🎴 ĐỨC ANH</div>
        <nav>
            <a href="#">Hồ sơ</a>
            <a href="#">Kinh tế học</a>
            <a href="#">Thiết kế</a>
            <a href="#">Dự án</a>
            <a href="#">Liên hệ</a>
        </nav>
    </header>

    <div class="container">
        <!-- Cột trái: Thông tin cá nhân -->
        <div class="hero">
            <span style="color: var(--accent-gold); font-size: 0.9rem;">MACROECONOMICS & CREATIVE DESIGN</span>
            <h1>NGÔ ĐỨC ANH</h1>
            <p>Đam mê nghiên cứu <b>Kinh tế vĩ mô</b> kết hợp tư duy thẩm mỹ trong <b>Thiết kế & Marketing</b>. Tạo dựng các mô hình phân tích chính xác và trải nghiệm thị giác ấn tượng.</p>
            <div style="margin-top: 30px;">
                <button class="btn-gold">Xem dự án</button>
                <button style="background: transparent; color: #fff; border: 1px solid #444; padding: 12px 24px; cursor: pointer;">Liên hệ</button>
            </div>
            <div class="stats-grid">
                <div class="stat-box">
                    <h3>3.8+</h3>
                    <p>GPA TÍCH LŨY</p>
                </div>
                <div class="stat-box">
                    <h3>MACRO</h3>
                    <p>NGHIÊN CỨU VĨ MÔ</p>
                </div>
                <div class="stat-box">
                    <h3>CANVA</h3>
                    <p>DESIGN PRO</p>
                </div>
            </div>
        </div>

        <!-- Cột phải: Bàn cờ Monopoly Mini -->
        <div class="board">
            <div class="tile">XUẤT PHÁT</div>
            <div class="tile">VĨ MÔ</div>
            <div class="tile">CANVA</div>
            <div class="tile">SPSS</div>
            <div class="tile">KHU TRÒ CHƠI</div>
            
            <div class="tile">DỰ ÁN APE</div>
            <div class="center-board">
                <h3 style="color: var(--accent-gold); margin: 5px;">DUC ANH & CO.</h3>
                <p style="font-size: 0.7rem; color: #aaa;">ĐI MỘT VÒNG BÀN CỜ</p>
                <button class="btn-gold" style="padding: 6px 12px; font-size: 0.8rem;" onclick="alert('🎲 Bạn quay trúng ô: Phân tích Kinh tế Vĩ mô!')">🎲 Tung xúc xắc</button>
            </div>
            <div class="tile">IELTS</div>
            
            <div class="tile">MARKETING</div>
            <div class="tile">POSTER G63</div>
            
            <div class="tile">NGHIÊN CỨU</div>
            <div class="tile">HỌC VẤN</div>
            
            <div class="tile">TRẠM TIẾP NƯỚC</div>
            <div class="tile">KỸ NĂNG</div>
            <div class="tile">BẢNG ĐIỂM</div>
            <div class="tile">LIÊN HỆ</div>
            <div class="tile">KẾT THÚC</div>
        </div>
    </div>
</body>
</html>
