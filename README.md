```html
<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>整体院LP</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:
    "Helvetica Neue",
    "Yu Gothic",
    sans-serif;

    color:#333;
    background:#ffffff;
    line-height:1.8;
}

/* =========================
   共通
========================= */

section{
    padding:100px 20px;
}

.container{
    width:100%;
    max-width:1100px;
    margin:auto;
}

h2{
    text-align:center;
    font-size:36px;
    margin-bottom:60px;
    color:#2a7fba;
    letter-spacing:0.05em;
}

.btn{
    display:inline-block;
    background:#2a7fba;
    color:#fff;
    text-decoration:none;
    padding:18px 38px;
    border-radius:999px;
    font-weight:bold;
    transition:0.3s;
    box-shadow:0 10px 30px rgba(0,0,0,0.12);
}

.btn:hover{
    transform:translateY(-3px);
    opacity:0.9;
}

/* =========================
   ファーストビュー
========================= */

.hero{
    position:relative;
    min-height:100vh;

    background:
    linear-gradient(
        rgba(0,0,0,0.35),
        rgba(0,0,0,0.35)
    ),
    url("https://images.unsplash.com/photo-1519823551278-64ac92734fb1?q=80&w=1600&auto=format&fit=crop");

    background-size:cover;
    background-position:center;

    display:flex;
    align-items:center;
    justify-content:center;

    text-align:center;
    color:#fff;
    padding:20px;
}

.hero-content{
    max-width:800px;
}

.hero-sub{
    font-size:18px;
    letter-spacing:0.1em;
    margin-bottom:20px;
}

.hero h1{
    font-size:58px;
    line-height:1.4;
    margin-bottom:30px;
    font-weight:700;
}

.hero-text{
    font-size:18px;
    margin-bottom:40px;
    opacity:0.95;
}

/* =========================
   悩み
========================= */

.problem{
    background:#f7fbff;
}

.problem-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(240px,1fr));
    gap:25px;
}

.problem-card{
    background:#fff;
    padding:35px;
    border-radius:20px;
    box-shadow:0 10px 30px rgba(0,0,0,0.05);
}

.problem-card h3{
    margin-bottom:15px;
    color:#2a7fba;
}

/* =========================
   選ばれる理由
========================= */

.reason-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:30px;
}

.reason-card{
    background:#fff;
    border-radius:20px;
    padding:40px;
    box-shadow:0 10px 30px rgba(0,0,0,0.06);
    transition:0.3s;
}

.reason-card:hover{
    transform:translateY(-6px);
}

.reason-card h3{
    margin-bottom:18px;
    color:#2a7fba;
    font-size:22px;
}

/* =========================
   メニュー
========================= */

.menu{
    background:#f7fbff;
}

.menu-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:30px;
}

.menu-card{
    background:#fff;
    border-radius:20px;
    padding:40px;
    text-align:center;
    box-shadow:0 10px 30px rgba(0,0,0,0.06);
}

.price{
    font-size:32px;
    color:#2a7fba;
    font-weight:bold;
    margin:20px 0;
}

/* =========================
   お客様の声
========================= */

.voice-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:30px;
}

.voice-card{
    background:#fff;
    border-radius:20px;
    padding:35px;
    box-shadow:0 10px 30px rgba(0,0,0,0.06);
    position:relative;
}

.voice-card::before{
    content:"“";
    position:absolute;
    top:10px;
    left:20px;
    font-size:80px;
    color:#d9ecfa;
}

.voice-card h3{
    margin-bottom:15px;
    color:#2a7fba;
    position:relative;
}

/* =========================
   院長紹介
========================= */

.profile{
    background:#f7fbff;
}

.profile-wrap{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:50px;
    align-items:center;
}

.profile img{
    width:100%;
    border-radius:20px;
    object-fit:cover;
    box-shadow:0 10px 30px rgba(0,0,0,0.1);
}

.profile-text h3{
    font-size:32px;
    margin-bottom:20px;
    color:#2a7fba;
}

/* =========================
   アクセス
========================= */

.access{
    text-align:center;
}

.access-box{
    background:#fff;
    max-width:700px;
    margin:auto;
    padding:50px;
    border-radius:20px;
    box-shadow:0 10px 30px rgba(0,0,0,0.06);
}

.access-box p{
    margin-bottom:15px;
}

/* =========================
   CTA
========================= */

.cta{
    background:
    linear-gradient(
        rgba(42,127,186,0.92),
        rgba(42,127,186,0.92)
    ),
    url("https://images.unsplash.com/photo-1506744038136-46273834b3fb?q=80&w=1600&auto=format&fit=crop");

    background-size:cover;
    background-position:center;

    color:#fff;
    text-align:center;
}

.cta h2{
    color:#fff;
}

.cta p{
    margin-bottom:40px;
    font-size:18px;
}

.cta .btn{
    background:#fff;
    color:#2a7fba;
}

/* =========================
   フッター
========================= */

footer{
    background:#1e2b36;
    color:#fff;
    text-align:center;
    padding:30px 20px;
    font-size:14px;
}

/* =========================
   スマホ
========================= */

@media(max-width:768px){

    section{
        padding:70px 20px;
    }

    .hero h1{
        font-size:38px;
    }

    h2{
        font-size:28px;
    }

    .profile-wrap{
        grid-template-columns:1fr;
    }

}
</style>
</head>

<body>

<!-- ファーストビュー -->
<header class="hero">
    <div class="hero-content">

        <p class="hero-sub">
            完全予約制 / 国家資格者対応
        </p>

        <h1>
            肩こり・腰痛を<br>
            根本から改善
        </h1>

        <p class="hero-text">
            あなたの身体に寄り添う、
            やさしい整体院。
            落ち着いた空間で、
            心と身体を整えます。
        </p>

        <a href="#" class="btn">
            初回限定 3,000円で予約する
        </a>

    </div>
</header>

<!-- 悩み -->
<section class="problem">

    <div class="container">

        <h2>こんなお悩みありませんか？</h2>

        <div class="problem-grid">

            <div class="problem-card">
                <h3>肩こりがつらい</h3>
                <p>
                    デスクワークやスマホ疲れで
                    首・肩が重い。
                </p>
            </div>

            <div class="problem-card">
                <h3>腰痛を繰り返す</h3>
                <p>
                    一時的によくなっても
                    すぐ再発してしまう。
                </p>
            </div>

            <div class="problem-card">
                <h3>疲れが抜けない</h3>
                <p>
                    身体が重く、
                    毎日スッキリしない。
                </p>
            </div>

        </div>

    </div>

</section>

<!-- 選ばれる理由 -->
<section>

    <div class="container">

        <h2>選ばれる理由</h2>

        <div class="reason-grid">

            <div class="reason-card">
                <h3>国家資格者による施術</h3>
                <p>
                    身体の状態を丁寧に確認し、
                    無理のない施術を行います。
                </p>
            </div>

            <div class="reason-card">
                <h3>根本改善を目指す</h3>
                <p>
                    その場しのぎではなく、
                    原因へアプローチします。
                </p>
            </div>

            <div class="reason-card">
                <h3>完全予約制</h3>
                <p>
                    落ち着いた空間で
                    ゆったり施術を受けられます。
                </p>
            </div>

        </div>

    </div>

</section>

<!-- メニュー -->
<section class="menu">

    <div class="container">

        <h2>施術メニュー</h2>

        <div class="menu-grid">

            <div class="menu-card">
                <h3>整体コース</h3>
                <div class="price">¥6,000</div>
                <p>
                    身体の歪みを整え、
                    痛みを改善します。
                </p>
            </div>

            <div class="menu-card">
                <h3>骨盤調整</h3>
                <div class="price">¥3,500</div>
                <p>
                    産後の骨盤ケアにも
                    おすすめです。
                </p>
            </div>

            <div class="menu-card">
                <h3>全身メンテナンス</h3>
                <div class="price">¥8,500</div>
                <p>
                    疲労回復・姿勢改善に。
                </p>
            </div>

        </div>

    </div>

</section>

<!-- お客様の声 -->
<section>

    <div class="container">

        <h2>お客様の声</h2>

        <div class="voice-grid">

            <div class="voice-card">
                <h3>肩こりが軽くなりました！</h3>
                <p>
                    デスクワークでつらかった肩こりが
                    改善しました。
                    院内も落ち着いていて安心できます。
                </p>
            </div>

            <div class="voice-card">
                <h3>丁寧で安心できました</h3>
                <p>
                    初めての整体でしたが、
                    説明が丁寧でリラックスして
                    受けられました。
                </p>
            </div>

        </div>

    </div>

</section>

<!-- 院長紹介 -->
<section class="profile">

    <div class="container">

        <h2>院長紹介</h2>

        <div class="profile-wrap">

            <img
            src="https://images.unsplash.com/photo-1612349317150-e413f6a5b16d?q=80&w=1200&auto=format&fit=crop"
            alt="院長">

            <div class="profile-text">

                <h3>院長 山田 太郎</h3>

                <p>
                    整体歴10年。
                    「一人ひとりの身体に合わせた施術」
                    を大切にしています。
                </p>

                <br>

                <p>
                    身体だけでなく、
                    心まで軽くなるような空間づくりを
                    心がけています。
                </p>

            </div>

        </div>

    </div>

</section>

<!-- アクセス -->
<section class="access">

    <div class="container">

        <h2>アクセス</h2>

        <div class="access-box">

            <p>愛知県〇〇市〇〇町1-2-3</p>
            <p>〇〇駅から徒歩5分</p>
            <p>営業時間 10:00〜20:00</p>
            <p>定休日 水曜日</p>
            <p>駐車場あり</p>

        </div>

    </div>

</section>

<!-- CTA -->
<section class="cta">

    <div class="container">

        <h2>まずはお気軽にご相談ください</h2>

        <p>
            初回限定価格で
            ご予約受付中です。
        </p>

        <a href="#" class="btn">
            24時間予約はこちら
        </a>

    </div>

</section>

<footer>
    © 2026 整体院サンプルLP
</footer>

</body>
</html>
```
