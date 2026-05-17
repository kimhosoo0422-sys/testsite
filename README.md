<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>외주 포트폴리오</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: "Pretendard", "Apple SD Gothic Neo", sans-serif;
    }

    body {
      color: #fff;
      background: #0f0f10;
      overflow-x: hidden;
      position: relative;
    }

    /* =========================
       FLOATING TECH IMAGES
    ========================== */

    .floating-icons {
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 1;
    }

    .floating-icons img {
      position: absolute;
      width: 140px;
      opacity: 0.12;
      filter: drop-shadow(0 0 20px rgba(255,255,255,0.08));
      animation: floatY 5s ease-in-out infinite;
    }

    /* 위 → 오른편 */
    .icon-css {
      top: 8%;
      right: 4%;
      animation-delay: 0s;
    }

    /* 중간 → 왼편 */
    .icon-java {
      top: 42%;
      left: 3%;
      animation-delay: 1s;
    }

    /* 아래 → 오른편 */
    .icon-html {
      bottom: 6%;
      right: 5%;
      animation-delay: 2s;
    }

    @keyframes floatY {
      0%,100% {
        transform: translateY(0px);
      }
      50% {
        transform: translateY(18px);
      }
    }

    /* =========================
       FADE ANIMATION
    ========================== */

    .fade-up {
      opacity: 0;
      transform: translateY(40px);
      animation: fadeUp 1s ease forwards;
    }

    .delay-1 {
      animation-delay: 0.2s;
    }

    .delay-2 {
      animation-delay: 0.5s;
    }

    .delay-3 {
      animation-delay: 0.8s;
    }

    .delay-4 {
      animation-delay: 1.1s;
    }

    @keyframes fadeUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* =========================
       HERO
    ========================== */

    .hero {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      background: radial-gradient(circle at top, #ff8a00, #1a1a1a 60%);
      padding: 20px;
      position: relative;
      z-index: 2;
    }

    .hero h1 {
      font-size: 46px;
      margin-bottom: 20px;
      letter-spacing: 1px;
    }

    .hero p {
      font-size: 18px;
      opacity: 0.9;
      max-width: 600px;
      line-height: 1.7;
    }

    .badge {
      margin-top: 20px;
      padding: 10px 18px;
      border: 1px solid rgba(255,255,255,0.3);
      border-radius: 30px;
      font-size: 14px;
      color: #fff;
      background: rgba(255, 138, 0, 0.15);
      backdrop-filter: blur(10px);
    }

    .scroll {
      position: absolute;
      bottom: 20px;
      font-size: 13px;
      opacity: 0.7;
      animation:
        floatText 2s infinite ease-in-out,
        fadeUp 1s ease forwards;
      animation-delay: 0s, 1.4s;
    }

    @keyframes floatText {
      0%,100% {
        transform: translateY(0);
      }
      50% {
        transform: translateY(8px);
      }
    }

    /* =========================
       SECTION
    ========================== */

    section {
      padding: 100px 20px;
      text-align: center;
      background: #141416;
      position: relative;
      z-index: 2;
    }

    .container {
      max-width: 900px;
      margin: auto;
    }

    h2 {
      font-size: 32px;
      margin-bottom: 20px;
      color: #ff8a00;
    }

    .desc {
      font-size: 17px;
      line-height: 1.9;
      opacity: 0.88;
    }

    /* =========================
       CONTACT
    ========================== */

    .contact {
      background: linear-gradient(135deg, #ff8a00, #d16627);
      color: #111;
    }

    .contact h2 {
      color: #111;
    }

    .card {
      background: rgba(255,255,255,0.2);
      padding: 25px;
      border-radius: 15px;
      backdrop-filter: blur(10px);
      margin-top: 20px;
      display: inline-block;
      min-width: 280px;

      opacity: 0;
      transform: translateY(40px);
      animation: fadeUp 1s ease forwards;
      animation-delay: 0.6s;
    }

    .card p {
      margin: 10px 0;
      font-weight: 500;
    }

    footer {
      padding: 20px;
      text-align: center;
      font-size: 13px;
      opacity: 0.7;
      background: #0f0f10;
      position: relative;
      z-index: 2;
    }

    a {
      color: inherit;
      text-decoration: none;
      font-weight: bold;
    }

    /* =========================
       MOBILE
    ========================== */

    @media (max-width: 768px) {

      .hero h1 {
        font-size: 34px;
      }

      .hero p {
        font-size: 16px;
      }

      .floating-icons img {
        width: 90px;
        opacity: 0.08;
      }

      .icon-css {
        top: 10%;
        right: -10px;
      }

      .icon-java {
        left: -10px;
      }

      .icon-html {
        right: -10px;
      }
    }

  </style>
</head>

<body>

  <!-- FLOATING ICONS -->
  <div class="floating-icons">

    <!-- CSS -->
    <img 
      src="css.png"
      alt="CSS"
      class="icon-css"
    />

    <!-- JAVA -->
    <img 
      src="java.png"
      alt="Java"
      class="icon-java"
    />

    <!-- HTML -->
    <img 
      src="html.png"
      alt="HTML"
      class="icon-html"
    />

  </div>

  <!-- HERO -->
  <div class="hero">

    <h1 class="fade-up">
      안녕하세요, 만나서 반갑습니다 :)
    </h1>

    <p class="fade-up delay-1">
      이 사이트는 외주 홍보용 포트폴리오 사이트입니다.<br/>
      깔끔하고 직관적인 디자인으로 당신의 프로젝트를 더 돋보이게 만듭니다.
    </p>


    <div class="scroll">
      ↓ 아래로 스크롤
    </div>

  </div>

  <!-- ABOUT -->
  <section>

    <div class="container">

      <h2 class="fade-up">
        소개
      </h2>

      <p class="desc fade-up delay-1">
        브랜드의 첫인상은 웹사이트에서 결정됩니다.<br/>
        저는 심플한 UI를 기반으로<br/>
        외주용 소규모 웹사이트, 랜딩페이지, 포트폴리오를 제작합니다.
      </p>

    </div>

  </section>

  <!-- CONTACT -->
  <section class="contact">

    <div class="container">

      <h2 class="fade-up">
        문의하기
      </h2>

      <div class="card">

        <p>📞 전화: 010-9570-8345</p>
        <p>📧 이메일: kimhosoo0422@gmail.com</p>
        <p>(왠만하면 전화로 부탁드립니다.)</p>
        <p>맡겨만 주세요!!</p>

      </div>

    </div>

  </section>

  <footer class="fade-up delay-1">
    © 2026 Portfolio Design. All rights reserved.
  </footer>

</body>
</html># testsite
