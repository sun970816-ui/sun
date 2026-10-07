<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Los Angeles Dodgers | 道奇球員介紹</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, "Microsoft JhengHei", sans-serif;
            background: #f4f7fb;
            color: #222;
        }

        /* 導覽列 */
        nav {
            background: #005A9C;
            height: 70px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0 8%;
            color: white;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav .logo {
            font-size: 24px;
            font-weight: bold;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 30px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 16px;
            transition: 0.3s;
        }

        nav ul li a:hover {
            color: #FFD700;
        }

        /* 首頁 */
        .hero {
            min-height: 550px;
            background: linear-gradient(
                rgba(0, 40, 90, 0.75),
                rgba(0, 40, 90, 0.75)
            ),
            url("https://images.unsplash.com/photo-1566577739112-5180d4bf9390")
            center/cover;

            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            padding: 30px;
        }

        .hero h1 {
            font-size: 60px;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 22px;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            background: #EF3E42;
            color: white;
            padding: 14px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            transform: scale(1.05);
            background: #d92f34;
        }

        /* 區塊 */
        section {
            padding: 70px 8%;
        }

        section h2 {
            text-align: center;
            color: #005A9C;
            font-size: 36px;
            margin-bottom: 40px;
        }

        /* 球隊介紹 */
        .about {
            max-width: 900px;
            margin: auto;
            text-align: center;
            line-height: 1.9;
            font-size: 18px;
        }

        /* 球員卡片 */
        .players {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
            max-width: 1200px;
            margin: auto;
        }

        .card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.12);
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 30px rgba(0,0,0,0.2);
        }

        .card img {
            width: 100%;
            height: 280px;
            object-fit: cover;
        }

        .card-content {
            padding: 25px;
        }

        .card h3 {
            color: #005A9C;
            font-size: 25px;
            margin-bottom: 10px;
        }

        .card p {
            line-height: 1.8;
            color: #555;
        }

        .number {
            display: inline-block;
            background: #005A9C;
            color: white;
            padding: 5px 12px;
            border-radius: 20px;
            margin-bottom: 10px;
        }

        /* 球隊資訊 */
        .stats {
            background: #005A9C;
            color: white;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            text-align: center;
            gap: 20px;
        }

        .stat h3 {
            font-size: 40px;
            margin-bottom: 10px;
        }

        .stat p {
            font-size: 18px;
        }

        /* Footer */
        footer {
            background: #002D62;
            color: white;
            text-align: center;
            padding: 30px;
        }

        /* 手機版 */
        @media (max-width: 900px) {
            .players {
                grid-template-columns: repeat(2, 1fr);
            }

            .hero h1 {
                font-size: 45px;
            }
        }

        @media (max-width: 600px) {
            nav {
                padding: 0 5%;
            }

            nav ul {
                gap: 10px;
            }

            nav ul li a {
                font-size: 13px;
            }

            .hero h1 {
                font-size: 35px;
            }

            .hero p {
                font-size: 17px;
            }

            .players {
                grid-template-columns: 1fr;
            }

            .stats {
                grid-template-columns: 1fr;
            }

            section {
                padding: 50px 5%;
            }
        }
    </style>
</head>

<body>

    <!-- 導覽列 -->
    <nav>
        <div class="logo">⚾ DODGERS</div>

        <ul>
            <li><a href="#home">首頁</a></li>
            <li><a href="#about">球隊介紹</a></li>
            <li><a href="#players">球員</a></li>
            <li><a href="#stats">資訊</a></li>
        </ul>
    </nav>


    <!-- 首頁 -->
    <section class="hero" id="home">
        <div>
            <h1>LOS ANGELES DODGERS</h1>

            <p>
                Welcome to the Dodgers
            </p>

            <a href="#players" class="btn">
                查看球員
            </a>
        </div>
    </section>


    <!-- 球隊介紹 -->
    <section id="about">

        <h2>球隊介紹</h2>

        <div class="about">

            <p>
                洛杉磯道奇隊（Los Angeles Dodgers）是美國職業棒球大聯盟
                MLB 的一支球隊，隸屬於國家聯盟西區。
            </p>

            <br>

            <p>
                道奇隊成立於 1883 年，歷史悠久，曾經在布魯克林發展，
                後來於 1958 年搬遷至洛杉磯。
            </p>

            <br>

            <p>
                道奇隊以優秀的投手、強大的打擊陣容以及悠久的棒球文化聞名，
                是 MLB 最具代表性的球隊之一。
            </p>

        </div>

    </section>


    <!-- 球員 -->
    <section id="players">

        <h2>明星球員</h2>

        <div class="players">

            <!-- 大谷翔平 -->
            <div class="card">

                <img
                    src="https://img.mlbstatic.com/mlb-photos/image/upload/w_600,q_auto/v1/people/660271/action/vertical/current"
                    alt="Shohei Ohtani"
                >

                <div class="card-content">

                    <span class="number">#17</span>

                    <h3>大谷翔平</h3>

                    <p>
                        <strong>位置：</strong>投手 / 指定打擊
                    </p>

                    <p>
                        日本出生的二刀流球星，
                        以強大的打擊能力與投球能力聞名。
                    </p>

                </div>

            </div>


            <!-- Freddie Freeman -->
            <div class="card">

                <img
                    src="https://img.mlbstatic.com/mlb-photos/image/upload/w_600,q_auto/v1/people/518692/action/vertical/current"
                    alt="Freddie Freeman"
                >

                <div class="card-content">

                    <span class="number">#5</span>

                    <h3>Freddie Freeman</h3>

                    <p>
                        <strong>位置：</strong>一壘手
                    </p>

                    <p>
                        左打的一壘手，
                        擁有優秀的打擊能力與豐富的大聯盟經驗。
                    </p>

                </div>

            </div>


            <!-- Mookie Betts -->
            <div class="card">

                <img
                    src="https://img.mlbstatic.com/mlb-photos/image/upload/w_600,q_auto/v1/people/605141/action/vertical/current"
                    alt="Mookie Betts"
                >

                <div class="card-content">

                    <span class="number">#50</span>

                    <h3>Mookie Betts</h3>

                    <p>
                        <strong>位置：</strong>內野手 / 外野手
                    </p>

                    <p>
                        全能型球員，兼具優秀的打擊、
                        守備與跑壘能力。
                    </p>

                </div>

            </div>

        </div>

    </section>


    <!-- 球隊資訊 -->
    <section id="stats" class="stats">

        <div class="stat">

            <h3>1883</h3>

            <p>球隊成立</p>

        </div>

        <div class="stat">

            <h3>1958</h3>

            <p>搬遷至洛杉磯</p>

        </div>

        <div class="stat">

            <h3>MLB</h3>

            <p>美國職業棒球大聯盟</p>

        </div>

    </section>


    <!-- Footer -->
    <footer>

        <p>
            © 2026 Los Angeles Dodgers Fan Website
        </p>

        <p>
            This website is created for educational purposes.
        </p>

    </footer>

</body>
</html>
