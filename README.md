<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>후라이의 꿈 - 건강한 식품의 시작</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #fffacd;
            color: #333;
        }
        header {
            background-color: #ffe28c;
            color: #333;
            padding: 20px 0;
            text-align: center;
            position: relative;
        }
        header .logo h1 {
            font-size: 2.8rem;
            margin: 0;
            color: #ff8b07;
        }
        header .logo p {
            margin: 5px 0 0;
            font-size: 1.4rem;
            color: #ff8b07;
        }
        nav ul {
            list-style: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin: 0 10px;
        }
        nav ul li a {
            color: #333;
            text-decoration: none;
            font-weight: bold;
        }
        .login {
            position: absolute;
            top: 10px;
            right: 10px;
        }
       .login input {
            margin-right: 5px;
            padding: 5px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        .login button {
            background-color: #ffc107;
            color: white;
            border: none;
            padding: 5px 10px;
            border-radius: 5px;
            cursor: pointer;
        }
        main {
            padding: 20px;
        }
        section {
            margin-bottom: 40px;
        }
        #about {
            text-align: center;
        }
        #about img {
            width: 100%;
            max-width: 500px;
            margin: 20px 0;
            border-radius: 10px;
            box-shadow: 0 2px 6px rgba(0, 0, 0, 0.2);
        }
        #products {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            justify-items: center;
        }
        #products .product {
            border: 1px solid #ffe4b5;
            border-radius: 10px;
            background-color: #fff8dc;
            padding: 20px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        #products .product img {
            width: 100%;
            max-width: 200px;
            border-radius: 10px;
            margin-bottom: 10px;
        }
        .buy-button {
            background-color: #ffc107;
            color: white;
            font-size: 1rem;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
        }
        .buy-button:hover {
            background-color: #ffa000;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #ffc107;
            color: white;
        }
    </style>
    <script>
        function confirmPurchase(productName) {
            if (confirm(productName + "를 구매하시겠습니까?")) {
                alert("구매가 완료되었습니다!");
            } else {
                alert("구매가 취소되었습니다.");
            }
        }
    </script>
</head>
<body>
    <header>
        <div class="logo">
            <h1>🍳 후라이의 꿈 🍳</h1>
            <p>건강한 식품의 시작, 함께 해요!</p>
        </div>
        <nav>
            <ul>
                <li><a href="#about">후라이의 꿈을 소개합니다!</a></li>
                <li><a href="#products">제품 소개</a></li>
                <li><a href="#contact">문의하기</a></li>
            </ul>
        </nav>
        <div class="login">
            <input type="text" placeholder="ID" id="id">
            <input type="password" placeholder="Password" id="password">
            <button>로그인</button>
        </div>
    </header>
    <main>
        <section id="about">
            <hr>
            <h2>후라이의 꿈을 소개합니다!</h2>
            <img src="about_us.jpg" alt="회사 소개 이미지">
            <p><strong>후라이의 꿈</strong>은 2015년에 설립된 친환경 식품 회사로, 국내산 동물복지 계란을 중심으로 다양한 제품을 선보이고 있어요. <br>
            🌱 <strong>비전:</strong> 지속 가능한 농업과 건강한 식생활을 통한 행복한 사회를 만들어요!<br>
            🏆 <strong>성과:</strong> 지난 8년간 동물복지 인증을 유지하며 소비자 만족도 98%를 달성했답니다. ✨</p>
        </section>
        <section style="text-align: center;">
            <hr>
            <h2>제품 소개</h2>
        </section>
        <section id="products">
            <div class="product">
                <img src="egg1.jpg" alt="달빛닮은 동물복지 계란">
                <h3>달빛닮은 동물복지 계란</h3>
                <p>가격: 8,000원 (12개입)<br>항생제를 사용하지 않고 동물복지 기준을 준수하며 생산한 신선한 계란입니다.</p>
                <button class="buy-button" onclick="confirmPurchase('달빛닮은 동물복지 계란')">구매하기</button>
            </div>
            <div class="product">
                <img src="egg2.jpg" alt="달빛에 구운란">
                <h3>달빛에 구운란</h3>
                <p>가격: 10,000원 (10개입)<br>동물복지 계란으로 만들어진 맛있는 구운 계란. 간편하게 즐길 수 있는 건강 간식입니다.</p>
                <button class="buy-button" onclick="confirmPurchase('달빛에 구운란')">구매하기</button>
            </div>
            <div class="product">
                <img src="egg3.jpg" alt="특별한 오믈렛">
                <h3>특별한 오믈렛</h3>
                <p>가격: 12,000원 (5개입)<br>달걀의 부드러움을 살린 고급 오믈렛 제품으로, 프리미엄 재료만을 사용하여 만들었습니다.</p>
                <button class="buy-button" onclick="confirmPurchase('특별한 오믈렛')">구매하기</button>
            </div>
            <div class="product">
                <img src="egg4.jpg" alt="일본식 아지타마고">
                <h3>일본식 아지타마고</h3>
                <p>가격: 9,000원 (6개입)<br>국내산 동물복지 계란으로 만든 고소하고 부드러운 일본식 아지타마고입니다. 🍜🥚</p>
                <button class="buy-button" onclick="confirmPurchase('일본식 아지타마고')">구매하기</button>
            </div>
        </section>
        <section style="text-align: center;" id="contact">
            <hr>
            <h2>문의하기</h2>
            <form action="https://formsubmit.co/your-email" method="POST">
                <label for="name">이름:</label>
                <input type="text" id="name" name="name" required>
                <label for="email">이메일:</label>
                <input type="email" id="email" name="email" required>
                <label for="message">문의 내용:</label>
                <textarea id="message" name="message" rows="4" required></textarea>
                <button type="submit">보내기</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 후라이의 꿈. 모든 권리 보유. 💖</p>
    </footer>
</body>
</html>
