<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>โปรไฟล์นักศึกษา | อริย์ธัช นาดวง (โนอาห์)</title>
    <!-- นำเข้า Google Fonts ภาษาไทย (สารบัญ/สุขุมวิทสไตล์ผ่านฟอนต์อเนกประสงค์ 'Noto Sans Thai' และ 'Kanit') -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@300;400;500;600&family=Noto+Sans+Thai:wght@300;400;500;600&display=swap" rel="stylesheet">
    <!-- นำเข้า FontAwesome สำหรับไอคอน Social Links -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --primary-color: #0f172a; /* Slate 900 */
            --secondary-color: #0d9488; /* Teal 600 */
            --secondary-hover: #0f766e; /* Teal 700 */
            --bg-color: #f8fafc; /* Slate 50 */
            --card-bg: #ffffff;
            --text-main: #334155; /* Slate 700 */
            --text-muted: #64748b; /* Slate 500 */
            --border-radius: 16px;
            --transition: all 0.3s ease;
            --shadow: 0 4px 6px -1px rgb(0 0 0 / 0.05), 0 2px 4px -2px rgb(0 0 0 / 0.05);
            --shadow-lg: 0 10px 15px -3px rgb(0 0 0 / 0.05), 0 4px 6px -4px rgb(0 0 0 / 0.05);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Noto Sans Thai', 'Kanit', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            padding: 40px 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            gap: 24px;
        }

        /* 1. Profile Grid Section */
        .profile-grid {
            display: grid;
            grid-template-columns: 1.5fr 1fr;
            gap: 24px;
        }

        @media (max-width: 768px) {
            .profile-grid {
                grid-template-columns: 1fr;
            }
        }

        .profile-info-card, .profile-photo-card, .social-links-card, .video-link-card {
            background: var(--card-bg);
            border-radius: var(--border-radius);
            padding: 32px;
            box-shadow: var(--shadow);
            border: 1px solid #e2e8f0;
            transition: var(--transition);
        }

        .profile-info-card:hover, .social-links-card:hover, .video-link-card:hover {
            box-shadow: var(--shadow-lg);
            transform: translateY(-2px);
        }

        h3 {
            color: var(--primary-color);
            font-size: 1.4rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 8px;
            font-family: 'Kanit', sans-serif;
            font-weight: 500;
        }

        h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 40px;
            height: 3px;
            background-color: var(--secondary-color);
            border-radius: 2px;
        }

        .profile-info-card p {
            margin-bottom: 12px;
            font-size: 1rem;
        }

        .profile-info-card p strong {
            color: var(--primary-color);
            font-weight: 500;
        }

        .profile-photo-card {
            padding: 0;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 250px;
        }

        .profile-photo-card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }

        .profile-photo-card:hover img {
            transform: scale(1.03);
        }

        /* 2. Profile Stats Section */
        .profile-stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 16px;
        }

        @media (max-width: 576px) {
            .profile-stats {
                grid-template-columns: 1fr;
            }
        }

        .profile-stat-card {
            background: linear-gradient(135deg, var(--primary-color), #1e293b);
            color: #ffffff;
            padding: 24px;
            border-radius: var(--border-radius);
            text-align: center;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        .profile-stat-card strong {
            display: block;
            font-size: 2rem;
            color: var(--secondary-color);
            font-family: 'Kanit', sans-serif;
            margin-bottom: 4px;
        }

        .profile-stat-card span {
            font-size: 0.95rem;
            color: #cbd5e1;
        }

        /* 3. Profile Quote Section */
        .profile-quote {
            background: linear-gradient(to right, #f0fdfa, #ccfbf1);
            border-left: 5px solid var(--secondary-color);
            padding: 24px 32px;
            border-radius: 4px var(--border-radius) var(--border-radius) 4px;
            box-shadow: var(--shadow);
        }

        .profile-quote p {
            font-size: 1.15rem;
            font-style: italic;
            color: #0f766e;
            font-weight: 500;
            text-align: center;
        }

        /* 4. About Highlights Section */
        .about-highlights {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        @media (max-width: 768px) {
            .about-highlights {
                grid-template-columns: 1fr;
            }
        }

        .about-highlights > div {
            background: var(--card-bg);
            border-radius: var(--border-radius);
            padding: 24px;
            box-shadow: var(--shadow);
            border-top: 4px solid var(--secondary-color);
        }

        .about-highlights h3 {
            font-size: 1.2rem;
            margin-bottom: 12px;
        }

        .about-highlights p {
            font-size: 0.95rem;
            color: var(--text-main);
            text-align: justify;
        }

        /* 5. Social Links Section */
        .social-links {
            display: flex;
            gap: 16px;
            flex-wrap: wrap;
            margin-top: 16px;
        }

        .social-links a {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            text-decoration: none;
            color: var(--text-main);
            padding: 10px 20px;
            border-radius: 30px;
            background-color: #f1f5f9;
            font-size: 0.95rem;
            font-weight: 500;
            transition: var(--transition);
            border: 1px solid #e2e8f0;
        }

        .social-links a:hover {
            background-color: var(--primary-color);
            color: #ffffff;
            border-color: var(--primary-color);
        }

        /* 6. Video Link Card Section */
        .video-link-card p {
            margin-bottom: 20px;
            color: var(--text-muted);
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            padding: 12px 28px;
            font-weight: 500;
            border-radius: 30px;
            transition: var(--transition);
            cursor: pointer;
            font-family: 'Kanit', sans-serif;
        }

        .btn-secondary {
            background-color: var(--secondary-color);
            color: #ffffff;
            box-shadow: 0 4px 10px rgb(13 148 136 / 0.3);
        }

        .btn-secondary:hover {
            background-color: var(--secondary-hover);
            box-shadow: 0 6px 14px rgb(13 148 136 / 0.4);
            transform: translateY(-1px);
        }
    </style>
</head>
<body>

    <div class="container">
        
        <!-- ข้อมูลพื้นฐานและรูปภาพ -->
        <div class="profile-grid">
            <div class="profile-info-card">
                <h3>ข้อมูลพื้นฐาน</h3>
                <p><strong>ชื่อ-นามสกุล:</strong> อริย์ธัช นาดวง</p>
                <p><strong>ชื่อเล่น:</strong> โนอาห์</p>
                <p><strong>สาขาวิชา:</strong> สาขาวิชาเทคโนโลยีดิจิทัลและสารสนเทศ หลักสูตรระดับปริญญาตรี (วท.บ.) ของสถาบันการจัดการปัญญาภิวัฒน์ (PIM) คณะวิศวกรรมศาสตร์ PIM</p>
                <p><strong>กลุ่มเรียน:</strong> DIT</p>
            </div>

            <div class="profile-photo-card">
                <img src="https://images.unsplash.com/photo-1516321497487-e288fb19713f?auto=format&fit=crop&w=900&q=80" alt="Person working on digital technology and web design">
            </div>
        </div>

        <!-- สถิติและความตั้งใจ -->
        <div class="profile-stats">
            <div class="profile-stat-card">
                <strong>100%</strong>
                <span>ความตั้งใจในการเรียนรู้</span>
            </div>
            <div class="profile-stat-card">
                <strong>3</strong>
                <span>มิติของความสนใจ</span>
            </div>
            <div class="profile-stat-card">
                <strong>24/7</strong>
                <span>พยายามพัฒนาตัวเอง</span>
            </div>
        </div>

        <!-- คำคม/คติพจน์ -->
        <div class="profile-quote">
            <p>“การเรียนรู้ไม่ใช่แค่เพื่อเก่งขึ้น แต่เพื่อสร้างความสามารถที่ใช้สร้างอนาคตได้จริง”</p>
        </div>

        <!-- ไฮไลท์การเรียนและความคาดหวัง -->
        <div class="about-highlights">
            <div>
                <h3>เหตุผลที่อยากเรียน</h3>
                <p>อยากเรียนรู้และหาประสบการณ์ใหม่ ๆ ในโลกดิจิทัล เพราะเชื่อว่าความรู้ด้านเทคโนโลยีจะช่วยให้สามารถต่อยอดตนเองและสร้างโอกาสในอนาคตได้</p>
            </div>
            <div>
                <h3>ความคาดหวังต่อวิชานี้</h3>
                <p>หวังว่าเรียนนี้จะช่วยให้เข้าใจหลักการสร้างเว็บและพัฒนาเว็บไซต์ได้ดีขึ้น เพื่อใช้ต่อยอดในการสร้างผลงานและนำไปใช้ในการทำงานในอนาคตที่บริษัท</p>
            </div>
            <div>
                <h3>จุดอ่อน</h3>
                <p>ไม่ค่อยเก่งเรื่องภาษาเท่าไหร่ แต่พยายามฝึกฝนและเรียนรู้อยู่เสมอ เพื่อพัฒนาให้ดีขึ้นในทุก ๆ วัน</p>
            </div>
        </div>

        <!-- ลิงก์ช่องทางโซเชียลมีเดีย -->
        <div class="social-links-card">
            <h3>Social Links</h3>
            <div class="social-links">
                <a href="https://www.facebook.com/avenjerr" target="_blank" rel="noopener noreferrer"><i class="fa-brands fa-facebook" style="color: #1877f2;"></i> Facebook</a>
                <a href="https://line.me/ti/p/~noah_soki" target="_blank" rel="noopener noreferrer"><i class="fa-brands fa-line" style="color: #06c755;"></i> Line</a>
                <a href="mailto:nomasoad@gmail.com"><i class="fa-solid fa-envelope" style="color: #ea4335;"></i> Gmail</a>
            </div>
        </div>

        <!-- การ์ดลิงก์วิดีโอภายนอก -->
        <div class="video-link-card">
            <h3>เรียนรู้ HTML จาก YouTube</h3>
            <p>ตัวอย่างคลิปสั้น ๆ สำหรับเริ่มต้นเรียน HTML แบบเข้าใจง่าย</p>
            <a href="https://www.youtube.com/watch?v=UB1O30fR-EE" target="_blank" rel="noopener noreferrer" class="btn btn-secondary"><i class="fa-brands fa-youtube" style="margin-right: 8px;"></i>ดูคลิป HTML</a>
        </div>

    </div>

</body>
</html>
