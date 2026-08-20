<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Una propuesta para Tefa</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@500;600;700&display=swap" rel="stylesheet">

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
            font-family: 'DM Sans', sans-serif;
            background: #111614;
            color: #f5f1e8;
            overflow-x: hidden;
        }

        /* ================================
           VARIABLES
        ================================= */

        :root {
            --green: #173c35;
            --green-light: #28594e;
            --cream: #f5f1e8;
            --orange: #e68a55;
            --dark: #111614;
            --gray: #a9aaa4;
        }


        /* ================================
           HERO
        ================================= */

        .hero {
            min-height: 100vh;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 80px 25px;
            overflow: hidden;

            background:
                linear-gradient(
                    rgba(10, 18, 16, .78),
                    rgba(10, 18, 16, .88)
                ),
                url("img/rio-chilina.jpg");

            background-size: cover;
            background-position: center;
        }

        .hero-content {
            max-width: 900px;
            position: relative;
            z-index: 2;
        }

        .small-title {
            text-transform: uppercase;
            letter-spacing: 5px;
            font-size: 13px;
            color: #d4d1c7;
            margin-bottom: 25px;
        }

        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(60px, 11vw, 120px);
            line-height: .95;
            font-weight: 600;
            margin-bottom: 25px;
        }

        .hero h1 span {
            color: var(--orange);
            font-style: italic;
        }

        .hero-question {
            font-size: clamp(22px, 3vw, 34px);
            line-height: 1.4;
            color: #eeeae0;
        }

        .hero-question strong {
            color: white;
        }

        .hero-line {
            width: 70px;
            height: 2px;
            background: var(--orange);
            margin: 35px auto;
        }

        .hero-date {
            font-size: 16px;
            letter-spacing: 2px;
            color: #d1d1cb;
        }

        .scroll {
            position: absolute;
            bottom: 25px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 12px;
            letter-spacing: 3px;
            color: #aaa;
        }


        /* ================================
           INTRO
        ================================= */

        .intro {
            padding: 120px 25px;
            background: var(--cream);
            color: #1e2824;
        }

        .container {
            max-width: 1100px;
            margin: auto;
        }

        .intro-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 80px;
            align-items: center;
        }

        .intro-text h2 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(40px, 5vw, 65px);
            line-height: 1.05;
            margin-bottom: 25px;
        }

        .intro-text h2 span {
            color: var(--orange);
        }

        .intro-text p {
            font-size: 18px;
            line-height: 1.8;
            color: #5c625e;
            max-width: 500px;
        }

        .intro-photo {
            height: 520px;
            position: relative;
        }

        .intro-photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .photo-number {
            position: absolute;
            bottom: -15px;
            left: -15px;
            background: var(--orange);
            color: white;
            padding: 15px 20px;
            font-size: 13px;
            letter-spacing: 2px;
        }


        /* ================================
           RAFTING
        ================================= */

        .rafting-section {
            padding: 120px 25px;
            background: var(--green);
        }

        .section-header {
            text-align: center;
            max-width: 700px;
            margin: auto auto 60px;
        }

        .section-header small {
            text-transform: uppercase;
            letter-spacing: 4px;
            color: #aebdb8;
        }

        .section-header h2 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(42px, 6vw, 70px);
            margin: 15px 0;
        }

        .section-header p {
            color: #b7c3bf;
            font-size: 18px;
        }

        .large-photo {
            height: 550px;
            position: relative;
            overflow: hidden;
        }

        .large-photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform .8s ease;
        }

        .large-photo:hover img {
            transform: scale(1.04);
        }

        .photo-caption {
            position: absolute;
            left: 30px;
            bottom: 30px;
            background: rgba(10, 18, 16, .75);
            backdrop-filter: blur(8px);
            padding: 18px 25px;
            border-left: 3px solid var(--orange);
        }

        .photo-caption strong {
            display: block;
            font-size: 18px;
        }

        .photo-caption span {
            color: #c1c8c4;
            font-size: 14px;
        }


        /* ================================
           PLAN
        ================================= */

        .plan {
            padding: 120px 25px;
            background: #151b19;
        }

        .plan h2 {
            text-align: center;
            font-family: 'Playfair Display', serif;
            font-size: 55px;
            margin-bottom: 70px;
        }

        .plan-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .plan-card {
            border: 1px solid #303936;
            padding: 35px;
            transition: .3s;
        }

        .plan-card:hover {
            transform: translateY(-8px);
            border-color: var(--orange);
        }

        .plan-icon {
            font-size: 32px;
            margin-bottom: 25px;
        }

        .plan-card h3 {
            font-family: 'Playfair Display', serif;
            font-size: 26px;
            margin-bottom: 12px;
        }

        .plan-card p {
            color: #a9afac;
            line-height: 1.7;
        }


        /* ================================
           CHILINA
        ================================= */

        .chilina {
            padding: 120px 25px;
            background: var(--cream);
            color: #1d2824;
        }

        .chilina-grid {
            display: grid;
            grid-template-columns: 1.1fr .9fr;
            gap: 70px;
            align-items: center;
        }

        .chilina-photo {
            height: 550px;
        }

        .chilina-photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .chilina-text small {
            text-transform: uppercase;
            letter-spacing: 4px;
            color: #777c77;
        }

        .chilina-text h2 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(45px, 6vw, 70px);
            line-height: 1;
            margin: 20px 0 30px;
        }

        .chilina-text h2 span {
            color: var(--orange);
        }

        .chilina-text p {
            color: #646a66;
            line-height: 1.8;
            font-size: 18px;
        }


        /* ================================
           GATOS
        ================================= */

        .cats {
            padding: 100px 25px;
            background: #101513;
        }

        .cats-content {
            max-width: 800px;
            margin: auto;
            text-align: center;
        }

        .cats-symbol {
            font-size: 45px;
            margin-bottom: 20px;
            filter: grayscale(1);
        }

        .cats h2 {
            font-family: 'Playfair Display', serif;
            font-size: 45px;
            margin-bottom: 20px;
        }

        .cats p {
            color: #aeb5b1;
            font-size: 18px;
            line-height: 1.8;
        }

        .cats-photo {
            max-width: 700px;
            height: 380px;
            margin: 50px auto 0;
        }

        .cats-photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }


        /* ================================
           ÚLTIMA FOTO
        ================================= */

        .memory {
            padding: 120px 25px;
            background: var(--green-light);
        }

        .memory-container {
            max-width: 850px;
            margin: auto;
            text-align: center;
        }

        .memory h2 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(40px, 6vw, 65px);
            margin-bottom: 15px;
        }

        .memory p {
            color: #c0ccc8;
            font-size: 18px;
            margin-bottom: 50px;
        }

        .memory-photo {
            height: 520px;
        }

        .memory-photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }


        /* ================================
           FINAL
        ================================= */

        .final {
            min-height: 80vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 100px 25px;
            background:
                linear-gradient(
                    rgba(10, 15, 13, .90),
                    rgba(10, 15, 13, .95)
                ),
                url("img/rafting.jpg");

            background-size: cover;
            background-position: center;
        }

        .final-content {
            max-width: 800px;
        }

        .final small {
            text-transform: uppercase;
            letter-spacing: 4px;
            color: #b6bbb8;
        }

        .final h2 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(45px, 7vw, 75px);
            margin: 20px 0;
        }

        .final h2 span {
            color: var(--orange);
            font-style: italic;
        }

        .final p {
            font-size: 20px;
            color: #c4c8c5;
            margin-bottom: 40px;
        }


        /* ================================
           BOTONES
        ================================= */

        .buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        button {
            font-family: inherit;
            font-size: 16px;
            font-weight: 600;
            padding: 15px 30px;
            border-radius: 3px;
            cursor: pointer;
            transition: .3s;
        }

        .yes {
            background: var(--orange);
            border: 2px solid var(--orange);
            color: white;
        }

        .yes:hover {
            background: #d87342;
            transform: translateY(-3px);
        }

        .maybe {
            background: transparent;
            border: 2px solid #777d79;
            color: white;
        }

        .maybe:hover {
            border-color: white;
        }


        /* ================================
           RESPUESTA
        ================================= */

        #response {
            display: none;
            margin: 40px auto 0;
            max-width: 600px;
            padding: 30px;
            border: 1px solid #59645f;
            background: rgba(20, 30, 27, .9);
            animation: appear .5s ease;
        }

        #response h3 {
            font-family: 'Playfair Display', serif;
            color: var(--orange);
            font-size: 32px;
        }

        #response p {
            margin-top: 10px;
            color: #c4cbc7;
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


        /* ================================
           FOOTER
        ================================= */

        footer {
            background: #0b0e0d;
            text-align: center;
            padding: 30px;
            color: #777d79;
            font-size: 14px;
        }

        footer span {
            color: var(--orange);
        }


        /* ================================
           RESPONSIVE
        ================================= */

        @media (max-width: 800px) {

            .intro-grid,
            .chilina-grid {
                grid-template-columns: 1fr;
                gap: 45px;
            }

            .plan-grid {
                grid-template-columns: 1fr;
            }

            .intro-photo,
            .chilina-photo {
                height: 420px;
            }

            .large-photo {
                height: 400px;
            }

            .memory-photo {
                height: 400px;
            }
        }

        @media (max-width: 500px) {

            .hero h1 {
                font-size: 65px;
            }

            .hero-question {
                font-size: 21px;
            }

            .intro-photo,
            .chilina-photo {
                height: 350px;
            }

            .large-photo {
                height: 300px;
            }

            .cats-photo {
                height: 280px;
            }

            .memory-photo {
                height: 320px;
            }

            .plan h2 {
                font-size: 42px;
            }
        }

    </style>
</head>


<body>


<!-- ==========================================
     PORTADA
=========================================== -->

<section class="hero">

    <div class="hero-content">

        <div class="small-title">
            una propuesta para ti
        </div>

        <h1>
            Tefa<span>.</span>
        </h1>

        <div class="hero-question">

            ¿Quisieras ir a hacer

            <strong>rafting</strong>

            al río Chilina conmigo

            el día sábado?

        </div>

        <div class="hero-line"></div>

        <div class="hero-date">
            UNA AVENTURA · UNA TARDE · TÚ Y YO
        </div>

    </div>

    <div class="scroll">
        ↓ DESLIZA
    </div>

</section>



<!-- ==========================================
     INTRO + FOTO TEFA
=========================================== -->

<section class="intro">

    <div class="container">

        <div class="intro-grid">

            <div class="intro-text">

                <h2>
                    Tengo una idea
                    <span>un poco diferente.</span>
                </h2>

                <p>

                    Pensé que podríamos hacer algo distinto
                    este sábado.

                    Nada demasiado complicado.

                    Solo una buena aventura, un lugar bonito
                    y alguien con quien valga la pena compartirla.

                </p>

            </div>


            <!--
            ======================================
            IMAGEN 1 — TEFA

            Pon aquí:
            img/tefa.jpg

            NO necesitas cambiar el nombre.
            ======================================
            -->

            <div class="intro-photo">

                <img
                    src="img/tefa.jpg"
                    alt="Tefa"
                >

                <div class="photo-number">
                    01 / TEFA
                </div>

            </div>

        </div>

    </div>

</section>



<!-- ==========================================
     RAFTING
=========================================== -->

<section class="rafting-section">

    <div class="container">

        <div class="section-header">

            <small>
                LA AVENTURA
            </small>

            <h2>
                Un poco de adrenalina.
            </h2>

            <p>
                Porque una salida diferente siempre
                se recuerda un poco más.
            </p>

        </div>


        <!--
        ======================================
        IMAGEN 2 — RAFTING

        Pon aquí:
        img/rafting.jpg
        ======================================
        -->

        <div class="large-photo">

            <img
                src="img/rafting.jpg"
                alt="Rafting"
            >

            <div class="photo-caption">

                <strong>
                    Río, aventura y buena compañía.
                </strong>

                <span>
                    El plan empieza aquí.
                </span>

            </div>

        </div>

    </div>

</section>



<!-- ==========================================
     EL PLAN
=========================================== -->

<section class="plan">

    <div class="container">

        <h2>
            El plan.
        </h2>

        <div class="plan-grid">

            <div class="plan-card">

                <div class="plan-icon">
                    🌊
                </div>

                <h3>
                    Río Chilina
                </h3>

                <p>
                    Un lugar diferente para desconectarnos
                    un rato de todo.
                </p>

            </div>


            <div class="plan-card">

                <div class="plan-icon">
                    🛶
                </div>

                <h3>
                    Rafting
                </h3>

                <p>
                    Una experiencia nueva que seguramente
                    nos dará alguna buena historia.
                </p>

            </div>


            <div class="plan-card">

                <div class="plan-icon">
                    📸
                </div>

                <h3>
                    Recuerdos
                </h3>

                <p>
                    Fotos, risas y probablemente alguna
                    foto en la que salgamos completamente empapados.
                </p>

            </div>

        </div>

    </div>

</section>



<!-- ==========================================
     RÍO CHILINA
=========================================== -->

<section class="chilina">

    <div class="container">

        <div class="chilina-grid">


            <!--
            ======================================
            IMAGEN 3 — RÍO CHILINA

            Pon aquí:
            img/rio-chilina.jpg
            ======================================
            -->

            <div class="chilina-photo">

                <img
                    src="img/rio-chilina.jpg"
                    alt="Río Chilina"
                >

            </div>


            <div class="chilina-text">

                <small>
                    DESTINO
                </small>

                <h2>
                    Río
                    <span>Chilina.</span>
                </h2>

                <p>

                    Creo que podría ser un buen lugar
                    para pasar el sábado.

                    Un poco de aventura, salir de la rutina
                    y simplemente pasarla bien.

                    Y sí, también prometo intentar no hacer
                    alguna tontería en el río.

                </p>

            </div>

        </div>

    </div>

</section>



<!-- ==========================================
     GATOS
=========================================== -->

<section class="cats">

    <div class="cats-content">

        <div class="cats-symbol">
            🐈
        </div>

        <h2>
            Hay una pequeña condición.
        </h2>

        <p>

            Los gatos tienen que aprobar oficialmente
            nuestra salida.

            Por suerte, parece que ya están de acuerdo.

        </p>


        <!--
        ======================================
        IMAGEN 4 — GATOS

        Pon aquí:
        img/gatos.jpg

        Puede ser una foto de gatos que te guste.
        ======================================
        -->

        <div class="cats-photo">

            <img
                src="img/gatos.jpg"
                alt="Gatos"
            >

        </div>

    </div>

</section>



<!-- ==========================================
     FOTO DE USTEDES
=========================================== -->

<section class="memory">

    <div class="memory-container">

        <h2>
            Y quizá...
        </h2>

        <p>
            esta podría ser nuestra próxima foto juntos.
        </p>


        <!--
        ======================================
        IMAGEN 5 — USTEDES

        Pon aquí:
        img/nosotros.jpg

        Si todavía no tienes una foto de ustedes,
        puedes dejar esta imagen para después.
        ======================================
        -->

        <div class="memory-photo">

            <img
                src="img/nosotros.jpg"
                alt="Nosotros"
            >

        </div>

    </div>

</section>



<!-- ==========================================
     PREGUNTA FINAL
=========================================== -->

<section class="final">

    <div class="final-content">

        <small>
            Y ahora sí...
        </small>

        <h2>
            Tefa,
            <span>¿te animas?</span>
        </h2>

        <p>
            Prometo que será un buen sábado.
        </p>


        <div class="buttons">

            <button
                class="yes"
                onclick="sayYes()"
            >
                Sí, vamos.
            </button>

            <button
                class="maybe"
                onclick="sayMaybe()"
            >
                Déjame pensarlo.
            </button>

        </div>


        <div id="response">

            <h3>
                Entonces tenemos un plan.
            </h3>

            <p>
                Me alegra que hayas dicho que sí.
                Ahora solo falta preparar todo para el sábado. 🌊
            </p>

        </div>

    </div>

</section>



<!-- ==========================================
     FOOTER
=========================================== -->

<footer>

    Hecho especialmente para <span>Tefa</span>.

</footer>



<script>

    function sayYes() {

        const response =
            document.getElementById("response");

        response.style.display = "block";

        response.innerHTML = `

            <h3>
                Entonces tenemos un plan.
            </h3>

            <p>
                Me alegra que hayas dicho que sí.
                Ahora solo falta preparar todo para el sábado. 🌊
            </p>

        `;

        response.scrollIntoView({
            behavior: "smooth",
            block: "center"
        });

    }


    function sayMaybe() {

        const response =
            document.getElementById("response");

        response.style.display = "block";

        response.innerHTML = `

            <h3>
                Está bien.
            </h3>

            <p>
                Piénsalo con calma...
                aunque espero que los gatos terminen
                convenciéndote. 🐈
            </p>

        `;

        response.scrollIntoView({
            behavior: "smooth",
            block: "center"
        });

    }

</script>


</body>
</html>
