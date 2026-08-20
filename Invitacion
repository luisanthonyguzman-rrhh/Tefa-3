<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Para Tefa ♡</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Baloo+2:wght@400;500;600;700;800&family=Pacifico&display=swap" rel="stylesheet">

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Baloo 2', cursive;
            background: #fff8f1;
            color: #302728;
            overflow-x: hidden;
        }

        /* =========================
           FONDO
        ========================= */

        body::before {
            content: "";
            position: fixed;
            inset: 0;
            background-image:
                radial-gradient(#f5a6b8 1px, transparent 1px),
                radial-gradient(#f5a6b8 1px, transparent 1px);
            background-size: 35px 35px;
            background-position: 0 0, 17px 17px;
            opacity: 0.08;
            pointer-events: none;
            z-index: -1;
        }

        /* =========================
           DECORACIÓN
        ========================= */

        .heart {
            position: absolute;
            color: #f06c87;
            animation: floating 3s ease-in-out infinite;
            user-select: none;
        }

        .heart.one {
            top: 120px;
            left: 7%;
            font-size: 35px;
        }

        .heart.two {
            top: 250px;
            right: 8%;
            font-size: 25px;
            animation-delay: 1s;
        }

        .heart.three {
            top: 550px;
            left: 10%;
            font-size: 28px;
            animation-delay: 1.5s;
        }

        .heart.four {
            top: 700px;
            right: 12%;
            font-size: 40px;
            animation-delay: .5s;
        }

        @keyframes floating {
            0%, 100% {
                transform: translateY(0) rotate(-5deg);
            }

            50% {
                transform: translateY(-12px) rotate(5deg);
            }
        }

        /* =========================
           HERO
        ========================= */

        .hero {
            min-height: 100vh;
            padding: 55px 20px 80px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            position: relative;
        }

        .top-decoration {
            font-size: 28px;
            letter-spacing: 10px;
            margin-bottom: 20px;
        }

        .small-text {
            color: #e86d88;
            font-size: 20px;
            font-weight: 700;
        }

        .name {
            font-family: 'Pacifico', cursive;
            font-size: clamp(55px, 12vw, 110px);
            color: #ec6682;
            line-height: 1;
            text-shadow: 4px 4px 0 #ffd5dd;
            margin: 5px 0 20px;
        }

        .question {
            max-width: 850px;
            font-size: clamp(30px, 5vw, 55px);
            line-height: 1.08;
            font-weight: 700;
        }

        .question strong {
            color: #ec6682;
            font-size: 1.2em;
        }

        .date {
            margin-top: 18px;
            font-size: 25px;
            color: #756365;
        }

        /* =========================
           FOTOS POLAROID
        ========================= */

        .polaroid {
            background: white;
            padding: 12px 12px 25px;
            box-shadow: 0 12px 30px rgba(80, 45, 45, .15);
            transition: .4s;
            position: relative;
        }

        .polaroid:hover {
            transform: rotate(0deg) scale(1.04) !important;
        }

        .polaroid img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }

        .polaroid::before {
            content: "";
            position: absolute;
            top: -13px;
            left: 50%;
            transform: translateX(-50%) rotate(-2deg);
            width: 90px;
            height: 25px;
            background: #f6b2bd;
            opacity: .8;
        }

        .photo-label {
            margin-top: 8px;
            font-size: 17px;
            color: #ec6682;
        }

        .hero-photos {
            width: min(900px, 100%);
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 50px;
            gap: 30px;
        }

        .hero-photos .polaroid {
            width: 240px;
            height: 285px;
        }

        .hero-photos .polaroid:first-child {
            transform: rotate(-6deg);
        }

        .hero-photos .polaroid:last-child {
            transform: rotate(6deg);
        }

        /* =========================
           GATO
        ========================= */

        .cat {
            font-size: 80px;
            animation: catBounce 2.5s ease-in-out infinite;
        }

        @keyframes catBounce {
            0%, 100% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(-15px);
            }
        }

        /* =========================
           RÍO
        ========================= */

        .river {
            position: relative;
            background: #83cfe7;
            padding: 80px 20px;
            overflow: hidden;
        }

        .river::before,
        .river::after {
            content: "";
            position: absolute;
            left: -5%;
            width: 110%;
            height: 80px;
            background: #fff8f1;
            border-radius: 50%;
        }

        .river::before {
            top: -45px;
        }

        .river::after {
            bottom: -55px;
        }

        .river-content {
            max-width: 1000px;
            margin: auto;
            position: relative;
            z-index: 2;
            text-align: center;
        }

        .river-title {
            font-size: clamp(35px, 6vw, 60px);
            color: white;
            text-shadow: 3px 3px rgba(55, 100, 120, .2);
        }

        .river-subtitle {
            color: #315766;
            font-size: 22px;
            margin-bottom: 35px;
        }

        .river-photo {
            max-width: 750px;
            height: 400px;
            margin: auto;
            transform: rotate(-1deg);
        }

        .river-photo img {
            border-radius: 3px;
        }

        .boat {
            font-size: 80px;
            position: absolute;
            right: 5%;
            bottom: 25px;
            animation: boat 4s ease-in-out infinite;
        }

        @keyframes boat {
            0%, 100% {
                transform: rotate(-4deg) translateY(0);
            }

            50% {
                transform: rotate(4deg) translateY(-10px);
            }
        }

        /* =========================
           IMAGINA ESTO
        ========================= */

        .section {
            padding: 100px 20px;
            max-width: 1100px;
            margin: auto;
        }

        .section-title {
            text-align: center;
            font-size: clamp(35px, 6vw, 55px);
            margin-bottom: 50px;
        }

        .section-title span {
            color: #ec6682;
        }

        .reasons {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
        }

        .reason {
            background: #fff;
            padding: 30px 20px;
            border-radius: 25px;
            text-align: center;
            box-shadow: 0 10px 25px rgba(80, 45, 45, .08);
            transition: .3s;
        }

        .reason:hover {
            transform: translateY(-8px);
        }

        .reason-icon {
            font-size: 50px;
            margin-bottom: 10px;
        }

        .reason h3 {
            color: #e96884;
            font-size: 22px;
            margin-bottom: 5px;
        }

        .reason p {
            color: #76686a;
            font-size: 17px;
        }

        /* =========================
           FOTO GATOS
        ========================= */

        .cat-section {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 60px;
            flex-wrap: wrap;
        }

        .cat-photo {
            width: 360px;
            height: 360px;
            transform: rotate(4deg);
        }

        .cat-message {
            max-width: 450px;
        }

        .cat-message h2 {
            font-size: 42px;
            color: #ec6682;
            margin-bottom: 15px;
        }

        .cat-message p {
            font-size: 21px;
            line-height: 1.5;
            color: #66585a;
        }

        /* =========================
           INVITACIÓN FINAL
        ========================= */

        .invitation {
            padding: 110px 20px;
            background: #ffe0e6;
            text-align: center;
            position: relative;
        }

        .invitation h2 {
            font-size: clamp(40px, 7vw, 65px);
            margin-bottom: 10px;
        }

        .invitation h2 span {
            color: #ec6682;
        }

        .invitation p {
            font-size: 23px;
            color: #69595c;
            margin-bottom: 35px;
        }

        .buttons {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        button {
            border: none;
            font-family: inherit;
            font-size: 22px;
            font-weight: 700;
            padding: 16px 32px;
            border-radius: 50px;
            cursor: pointer;
            transition: .3s;
        }

        .yes {
            background: #ed6b87;
            color: white;
            box-shadow: 0 8px 20px rgba(237, 107, 135, .3);
        }

        .yes:hover {
            transform: scale(1.08);
        }

        .think {
            background: white;
            color: #66585a;
        }

        .think:hover {
            transform: translateY(-3px);
        }

        /* =========================
           MENSAJE FINAL
        ========================= */

        #response {
            display: none;
            margin: 40px auto 0;
            max-width: 600px;
            background: white;
            border-radius: 30px;
            padding: 30px;
            box-shadow: 0 15px 35px rgba(80, 45, 45, .12);
            animation: appear .6s ease;
        }

        #response h3 {
            color: #ec6682;
            font-size: 35px;
        }

        #response p {
            font-size: 20px;
            margin: 10px 0 0;
        }

        @keyframes appear {
            from {
                opacity: 0;
                transform: translateY(20px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* =========================
           FOOTER
        ========================= */

        footer {
            background: #b98d65;
            color: white;
            text-align: center;
            padding: 25px;
            font-size: 18px;
        }

        /* =========================
           CORAZONES QUE CAEN
        ========================= */

        .falling-heart {
            position: fixed;
            top: -20px;
            font-size: 20px;
            pointer-events: none;
            animation: fall linear forwards;
            z-index: 999;
        }

        @keyframes fall {
            to {
                transform: translateY(110vh) rotate(360deg);
                opacity: 0;
            }
        }

        /* =========================
           RESPONSIVE
        ========================= */

        @media (max-width: 800px) {

            .hero {
                padding-top: 40px;
            }

            .hero-photos {
                flex-direction: column;
            }

            .hero-photos .polaroid {
                width: 250px;
            }

            .hero-photos .polaroid:last-child {
                margin-top: 20px;
            }

            .reasons {
                grid-template-columns: repeat(2, 1fr);
            }

            .boat {
                display: none;
            }

            .river-photo {
                height: 280px;
            }
        }

        @media (max-width: 500px) {

            .reasons {
                grid-template-columns: 1fr;
            }

            .question {
                font-size: 31px;
            }

            .name {
                font-size: 65px;
            }

            .cat {
                font-size: 60px;
            }

            .cat-photo {
                width: 300px;
                height: 300px;
            }

            .section {
                padding: 70px 20px;
            }
        }

    </style>
</head>

<body>

    <!-- DECORACIÓN -->
    <div class="heart one">♡</div>
    <div class="heart two">♥</div>
    <div class="heart three">♡</div>
    <div class="heart four">♥</div>


    <!-- =========================
         PORTADA
    ========================= -->

    <section class="hero">

        <div class="top-decoration">
            🐱 ♡ 🐱 ♡ 🐱
        </div>

        <div class="small-text">
            tengo una pequeña propuesta para ti...
        </div>

        <div class="name">
            Tefa ♡
        </div>

        <div class="question">

            ¿Quisieras ir a hacer

            <br>

            <strong>rafting</strong>

            <br>

            al río Chilina conmigo

            <br>

            el día sábado?

        </div>

        <div class="date">
            🌊 Una aventura, tú y yo 🌊
        </div>


        <div class="hero-photos">

            <!-- IMAGEN 1: FOTO DE TEFA
                 Archivo: img/tefa.jpg -->

            <div class="polaroid">

                <img
                    src="img/tefa.jpg"
                    alt="Foto de Tefa"
                    onerror="this.src='https://placehold.co/500x600/ffdce3/555?text=FOTO+DE+TEFA'"
                >

                <div class="photo-label">
                    ✨ Tefa ✨
                </div>

            </div>


            <div class="cat">
                🐱
            </div>


            <!-- IMAGEN 2: FOTO DE RAFTING
                 Archivo: img/rafting.jpg -->

            <div class="polaroid">

                <img
                    src="img/rafting.jpg"
                    alt="Rafting"
                    onerror="this.src='https://placehold.co/500x600/d5f3fa/555?text=RAFTING'"
                >

                <div class="photo-label">
                    🌊 aventura
                </div>

            </div>

        </div>

    </section>


    <!-- =========================
         RÍO CHILINA
    ========================= -->

    <section class="river">

        <div class="river-content">

            <div class="river-title">
                El plan 🌊
            </div>

            <div class="river-subtitle">
                Tú + yo + agua + un poquito de locura
            </div>


            <!-- IMAGEN 3: RÍO CHILINA
                 Archivo: img/rio-chilina.jpg -->

            <div class="polaroid river-photo">

                <img
                    src="img/rio-chilina.jpg"
                    alt="Río Chilina"
                    onerror="this.src='https://placehold.co/1200x600/b9e8f5/555?text=FOTO+DEL+RIO+CHILINA'"
                >

                <div class="photo-label">
                    📍 Río Chilina
                </div>

            </div>

        </div>

        <div class="boat">
            🛶
        </div>

    </section>


    <!-- =========================
         RAZONES
    ========================= -->

    <section class="section">

        <h2 class="section-title">
            Imagina esto... <span>♡</span>
        </h2>

        <div class="reasons">

            <div class="reason">

                <div class="reason-icon">
                    🛶
                </div>

                <h3>Aventura</h3>

                <p>
                    Algo diferente para salir de la rutina.
                </p>

            </div>


            <div class="reason">

                <div class="reason-icon">
                    📸
                </div>

                <h3>Recuerdos</h3>

                <p>
                    Fotos que probablemente nos darán risa después.
                </p>

            </div>


            <div class="reason">

                <div class="reason-icon">
                    😂
                </div>

                <h3>Risas</h3>

                <p>
                    Porque seguro alguno de los dos termina empapado.
                </p>

            </div>


            <div class="reason">

                <div class="reason-icon">
                    🐱
                </div>

                <h3>Buena compañía</h3>

                <p>
                    Y aparentemente los gatos ya aprobaron el plan.
                </p>

            </div>

        </div>

    </section>


    <!-- =========================
         SECCIÓN GATOS
    ========================= -->

    <section class="section">

        <div class="cat-section">


            <!-- IMAGEN 4: GATOS
                 Archivo: img/gatos.jpg -->

            <div class="polaroid cat-photo">

                <img
                    src="img/gatos.jpg"
                    alt="Gatitos"
                    onerror="this.src='https://placehold.co/600x600/ffe1e7/555?text=FOTO+DE+GATITOS'"
                >

                <div class="photo-label">
                    🐱 comité oficial de aprobación
                </div>

            </div>


            <div class="cat-message">

                <h2>
                    Una opinión importante...
                </h2>

                <p>
                    Consulté con los gatos y, después de una reunión
                    bastante seria, llegaron a la conclusión de que
                    deberías decir que sí.
                </p>

                <br>

                <p>
                    Yo también estoy de acuerdo con ellos. 🐱♡
                </p>

            </div>

        </div>

    </section>


    <!-- =========================
         FOTO DE USTEDES
    ========================= -->

    <section class="section" style="text-align:center;">

        <h2 class="section-title">
            Y si todo sale bien... <span>📸</span>
        </h2>


        <!-- IMAGEN 5: FOTO DE USTEDES
             Archivo: img/nosotros.jpg -->

        <div
            class="polaroid"
            style="
                max-width:650px;
                height:500px;
                margin:auto;
                transform:rotate(-2deg);
            "
        >

            <img
                src="img/nosotros.jpg"
                alt="Foto de nosotros"
                onerror="this.src='https://placehold.co/900x700/ffe5ea/555?text=AQUI+VA+UNA+FOTO+DE+NOSOTROS'"
            >

            <div class="photo-label">
                quizá esta sea nuestra próxima foto ♡
            </div>

        </div>

    </section>


    <!-- =========================
         PREGUNTA FINAL
    ========================= -->

    <section class="invitation">

        <div style="font-size:70px;">
            🐱 💗 🛶
        </div>

        <h2>
            Entonces, Tefa...
        </h2>

        <p>
            ¿Qué dices, te animas?
        </p>


        <div class="buttons">

            <button
                class="yes"
                onclick="sayYes()"
            >
                🐱 ¡Siii, vamos! ♡
            </button>


            <button
                class="think"
                onclick="sayThink()"
            >
                Déjame pensarlo 🙈
            </button>

        </div>


        <div id="response">

            <h3>
                SABÍA QUE DIRÍAS QUE SÍ 😭♡
            </h3>

            <p>
                Prometo llevar buena energía, ganas de pasarla bien
                y probablemente hacer el ridículo en algún momento.
            </p>

            <div style="font-size:50px; margin-top:15px;">
                🐱 🌊 🛶 💗
            </div>

        </div>

    </section>


    <!-- =========================
         FOOTER
    ========================= -->

    <footer>

        Hecho con ❤️ para Tefa 🐱

        <br>

        <small>
            PD: llevaré snacks y buena energía.
        </small>

    </footer>


    <!-- =========================
         JAVASCRIPT
    ========================= -->

    <script>

        function createHeart() {

            const heart = document.createElement("div");

            heart.classList.add("falling-heart");

            const hearts = ["♡", "♥", "💗", "🐱"];

            heart.innerHTML =
                hearts[Math.floor(Math.random() * hearts.length)];

            heart.style.left =
                Math.random() * 100 + "vw";

            heart.style.animationDuration =
                (3 + Math.random() * 4) + "s";

            heart.style.fontSize =
                (15 + Math.random() * 20) + "px";

            document.body.appendChild(heart);

            setTimeout(() => {
                heart.remove();
            }, 7000);
        }


        function sayYes() {

            const response =
                document.getElementById("response");

            response.style.display = "block";

            response.scrollIntoView({
                behavior: "smooth",
                block: "center"
            });


            // Lluvia de corazones
            for (let i = 0; i < 30; i++) {

                setTimeout(() => {
                    createHeart();
                }, i * 100);

            }

        }


        function sayThink() {

            const response =
                document.getElementById("response");

            response.style.display = "block";

            response.innerHTML = `

                <h3>
                    Está bien, Tefa 🙈♡
                </h3>

                <p>
                    Tómate tu tiempo...
                    pero los gatos y yo esperamos
                    que la respuesta sea sí. 🐱
                </p>

                <div style="font-size:50px; margin-top:15px;">
                    🐱 🥺 💗
                </div>

            `;

            response.scrollIntoView({
                behavior: "smooth",
                block: "center"
            });

        }


        // Corazones flotando ocasionalmente

        setInterval(() => {

            if (Math.random() > 0.5) {
                createHeart();
            }

        }, 1800);

    </script>

</body>
</html>
