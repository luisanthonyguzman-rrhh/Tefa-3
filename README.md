


<html lang="es">

<head>

    <meta charset="UTF-8">

    <meta
        name="viewport"
        content="width=device-width, initial-scale=1.0, viewport-fit=cover"
    >

    <meta
        name="theme-color"
        content="#111614"
    >

    <title>Una propuesta para Tefa</title>


    <!-- FUENTES -->

    <link rel="preconnect" href="https://fonts.googleapis.com">

    <link
        rel="preconnect"
        href="https://fonts.gstatic.com"
        crossorigin
    >

    <link
        href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@500;600;700&display=swap"
        rel="stylesheet"
    >


    <style>

        /* =====================================================
           CONFIGURACIÓN GENERAL
        ===================================================== */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }


        html {
            width: 100%;
            min-height: 100%;
            scroll-behavior: smooth;
        }


        body {

            width: 100%;
            min-height: 100%;

            margin: 0;

            font-family: "DM Sans", sans-serif;

            background: #111614;

            color: #f5f1e8;

            overflow-x: hidden;

            -webkit-text-size-adjust: 100%;
            text-size-adjust: 100%;
        }


        img {

            display: block;

            width: 100%;

            max-width: 100%;

            height: auto;
        }


        button {

            -webkit-tap-highlight-color: transparent;

            touch-action: manipulation;
        }


        :root {

            --dark: #111614;

            --dark2: #151b19;

            --green: #173c35;

            --green2: #28594e;

            --cream: #f5f1e8;

            --orange: #e68a55;

            --gray: #a9aaa4;

            --white: #ffffff;
        }



        /* =====================================================
           CONTENEDOR
        ===================================================== */

        .container {

            width: min(1100px, calc(100% - 40px));

            margin-left: auto;
            margin-right: auto;
        }



        /* =====================================================
           PORTADA
        ===================================================== */

        .hero {

            width: 100%;

            min-height: 100vh;
            min-height: 100svh;

            position: relative;

            display: flex;

            align-items: center;

            justify-content: center;

            text-align: center;

            padding:
                max(40px, env(safe-area-inset-top))
                20px
                max(70px, env(safe-area-inset-bottom))
                20px;

            overflow: hidden;

            background:

                linear-gradient(
                    rgba(8, 14, 12, 0.78),
                    rgba(8, 14, 12, 0.90)
                ),

                url("img/rio-chilina.jpg");

            background-size: cover;

            background-position: center;
        }


        .hero-content {

            width: 100%;

            max-width: 900px;

            margin: auto;

            position: relative;

            z-index: 2;
        }


        .small-title {

            text-transform: uppercase;

            letter-spacing: 4px;

            font-size: 12px;

            line-height: 1.5;

            color: #d4d1c7;

            margin-bottom: 25px;
        }


        .hero h1 {

            font-family: "Playfair Display", serif;

            font-size: clamp(
                62px,
                15vw,
                120px
            );

            line-height: 0.95;

            font-weight: 600;

            margin-bottom: 28px;
        }


        .hero h1 span {

            color: var(--orange);

            font-style: italic;
        }


        .hero-question {

            width: 100%;

            max-width: 780px;

            margin: auto;

            font-size: clamp(
                21px,
                4vw,
                34px
            );

            line-height: 1.45;

            color: #eeeae0;
        }


        .hero-question strong {

            color: #ffffff;

            font-weight: 700;
        }


        .hero-line {

            width: 65px;

            height: 2px;

            background: var(--orange);

            margin: 30px auto;
        }


        .hero-date {

            font-size: 12px;

            letter-spacing: 2px;

            line-height: 1.6;

            color: #c7c9c4;
        }


        .scroll {

            position: absolute;

            bottom: max(
                20px,
                env(safe-area-inset-bottom)
            );

            left: 50%;

            transform: translateX(-50%);

            font-size: 10px;

            letter-spacing: 3px;

            color: #aaa;

            white-space: nowrap;
        }



        /* =====================================================
           INTRO
        ===================================================== */

        .intro {

            width: 100%;

            padding: 90px 0;

            background: var(--cream);

            color: #1e2824;
        }


        .intro-grid {

            display: grid;

            grid-template-columns:
                minmax(0, 1fr)
                minmax(0, 1fr);

            gap: 60px;

            align-items: center;
        }


        .intro-text {

            min-width: 0;
        }


        .intro-text h2 {

            font-family: "Playfair Display", serif;

            font-size: clamp(
                40px,
                6vw,
                65px
            );

            line-height: 1.05;

            margin-bottom: 25px;
        }


        .intro-text h2 span {

            color: var(--orange);
        }


        .intro-text p {

            max-width: 520px;

            font-size: 18px;

            line-height: 1.8;

            color: #5c625e;
        }


        .intro-photo {

            width: 100%;

            aspect-ratio: 4 / 5;

            max-height: 620px;

            position: relative;

            overflow: hidden;
        }


        .intro-photo img {

            width: 100%;
            height: 100%;

            object-fit: cover;
        }


        .photo-number {

            position: absolute;

            left: 0;

            bottom: 0;

            background: var(--orange);

            color: white;

            padding: 12px 16px;

            font-size: 11px;

            letter-spacing: 2px;
        }



        /* =====================================================
           RAFTING
        ===================================================== */

        .rafting-section {

            width: 100%;

            padding: 90px 0;

            background: var(--green);
        }


        .section-header {

            text-align: center;

            width: 100%;

            max-width: 700px;

            margin: 0 auto 50px;
        }


        .section-header small {

            text-transform: uppercase;

            letter-spacing: 4px;

            color: #aebdb8;

            font-size: 11px;
        }


        .section-header h2 {

            font-family: "Playfair Display", serif;

            font-size: clamp(
                42px,
                7vw,
                70px
            );

            line-height: 1.05;

            margin: 15px 0;
        }


        .section-header p {

            color: #b7c3bf;

            font-size: 17px;

            line-height: 1.6;
        }


        .large-photo {

            width: 100%;

            height: min(
                65vh,
                550px
            );

            min-height: 300px;

            position: relative;

            overflow: hidden;
        }


        .large-photo img {

            width: 100%;
            height: 100%;

            object-fit: cover;

            transition: transform .7s ease;
        }


        .large-photo:hover img {

            transform: scale(1.03);
        }


        .photo-caption {

            position: absolute;

            left: 20px;

            right: 20px;

            bottom: 20px;

            background: rgba(
                10,
                18,
                16,
                .78
            );

            padding: 15px 18px;

            border-left: 3px solid var(--orange);

            backdrop-filter: blur(7px);

            -webkit-backdrop-filter: blur(7px);
        }


        .photo-caption strong {

            display: block;

            font-size: 16px;

            line-height: 1.4;
        }


        .photo-caption span {

            display: block;

            color: #c1c8c4;

            font-size: 13px;

            margin-top: 3px;
        }



        /* =====================================================
           PLAN
        ===================================================== */

        .plan {

            width: 100%;

            padding: 90px 0;

            background: var(--dark2);
        }


        .plan h2 {

            text-align: center;

            font-family: "Playfair Display", serif;

            font-size: clamp(
                42px,
                7vw,
                60px
            );

            margin-bottom: 55px;
        }


        .plan-grid {

            display: grid;

            grid-template-columns:
                repeat(3, minmax(0, 1fr));

            gap: 20px;
        }


        .plan-card {

            min-width: 0;

            border: 1px solid #303936;

            padding: 30px;

            transition:
                transform .3s ease,
                border-color .3s ease;
        }


        .plan-card:hover {

            transform: translateY(-6px);

            border-color: var(--orange);
        }


        .plan-icon {

            font-size: 28px;

            margin-bottom: 20px;
        }


        .plan-card h3 {

            font-family: "Playfair Display", serif;

            font-size: 25px;

            margin-bottom: 10px;
        }


        .plan-card p {

            color: #a9afac;

            line-height: 1.7;

            font-size: 15px;
        }



        /* =====================================================
           CHILINA
        ===================================================== */

        .chilina {

            width: 100%;

            padding: 90px 0;

            background: var(--cream);

            color: #1d2824;
        }


        .chilina-grid {

            display: grid;

            grid-template-columns:
                minmax(0, 1.1fr)
                minmax(0, .9fr);

            gap: 60px;

            align-items: center;
        }


        .chilina-photo {

            width: 100%;

            aspect-ratio: 4 / 5;

            max-height: 600px;

            overflow: hidden;
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

            font-size: 11px;
        }


        .chilina-text h2 {

            font-family: "Playfair Display", serif;

            font-size: clamp(
                45px,
                7vw,
                70px
            );

            line-height: 1;

            margin: 20px 0 30px;
        }


        .chilina-text h2 span {

            color: var(--orange);
        }


        .chilina-text p {

            color: #646a66;

            line-height: 1.8;

            font-size: 17px;
        }



        /* =====================================================
           FOTO DE USTEDES
        ===================================================== */

        .memory {

            width: 100%;

            padding: 90px 0;

            background: var(--green2);
        }


        .memory-container {

            width: 100%;

            max-width: 850px;

            margin: auto;

            text-align: center;
        }


        .memory h2 {

            font-family: "Playfair Display", serif;

            font-size: clamp(
                42px,
                7vw,
                65px
            );

            margin-bottom: 10px;
        }


        .memory p {

            color: #c0ccc8;

            font-size: 17px;

            margin-bottom: 40px;
        }


        .memory-photo {

            width: 100%;

            aspect-ratio: 16 / 10;

            max-height: 550px;

            overflow: hidden;
        }


        .memory-photo img {

            width: 100%;
            height: 100%;

            object-fit: cover;
        }



        /* =====================================================
           FINAL
        ===================================================== */

        .final {

            width: 100%;

            min-height: 80vh;
            min-height: 80svh;

            display: flex;

            align-items: center;

            justify-content: center;

            text-align: center;

            padding:
                90px 20px
                max(90px, env(safe-area-inset-bottom))
                20px;

            background:

                linear-gradient(
                    rgba(10, 15, 13, .88),
                    rgba(10, 15, 13, .95)
                ),

                url("img/rafting.jpg");

            background-size: cover;

            background-position: center;
        }


        .final-content {

            width: 100%;

            max-width: 800px;

            margin: auto;
        }


        .final small {

            text-transform: uppercase;

            letter-spacing: 4px;

            color: #b6bbb8;

            font-size: 11px;
        }


        .final h2 {

            font-family: "Playfair Display", serif;

            font-size: clamp(
                45px,
                8vw,
                75px
            );

            line-height: 1.05;

            margin: 20px 0;
        }


        .final h2 span {

            color: var(--orange);

            font-style: italic;
        }


        .final p {

            font-size: 18px;

            line-height: 1.6;

            color: #c4c8c5;

            margin-bottom: 35px;
        }



        /* =====================================================
           BOTONES
        ===================================================== */

        .buttons {

            width: 100%;

            display: flex;

            justify-content: center;

            align-items: center;

            gap: 12px;

            flex-wrap: wrap;
        }


        button {

            min-height: 52px;

            padding: 14px 28px;

            border-radius: 4px;

            font-family: "DM Sans", sans-serif;

            font-size: 15px;

            font-weight: 600;

            cursor: pointer;

            transition:
                transform .25s ease,
                background .25s ease,
                border-color .25s ease;

            -webkit-appearance: none;

            appearance: none;
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



        /* =====================================================
           RESPUESTA
        ===================================================== */

        #response {

            display: none;

            width: 100%;

            max-width: 600px;

            margin: 35px auto 0;

            padding: 25px;

            border: 1px solid #59645f;

            background: rgba(
                20,
                30,
                27,
                .95
            );

            animation: appear .5s ease;
        }


        #response h3 {

            font-family: "Playfair Display", serif;

            color: var(--orange);

            font-size: clamp(
                28px,
                6vw,
                35px
            );
        }


        #response p {

            margin-top: 10px;

            color: #c4cbc7;

            line-height: 1.6;
        }


        @keyframes appear {

            from {

                opacity: 0;

                transform: translateY(15px);
            }

            to {

                opacity: 1;

                transform: translateY(0);
            }
        }



        /* =====================================================
           FOOTER
        ===================================================== */

        footer {

            width: 100%;

            background: #0b0e0d;

            text-align: center;

            padding:
                25px
                20px
                max(25px, env(safe-area-inset-bottom));

            color: #777d79;

            font-size: 13px;
        }


        footer span {

            color: var(--orange);
        }



        /* =====================================================
           TABLET
        ===================================================== */

        @media (max-width: 850px) {

            .intro-grid {

                grid-template-columns: 1fr;

                gap: 45px;
            }


            .intro-text {

                text-align: center;
            }


            .intro-text p {

                margin-left: auto;

                margin-right: auto;
            }


            .intro-photo {

                width: min(
                    100%,
                    600px
                );

                margin: auto;
            }


            .chilina-grid {

                grid-template-columns: 1fr;

                gap: 45px;
            }


            .chilina-text {

                text-align: center;
            }


            .chilina-photo {

                width: min(
                    100%,
                    650px
                );

                margin: auto;
            }


            .plan-grid {

                grid-template-columns: 1fr;
            }


            .plan-card {

                text-align: center;
            }


            .large-photo {

                height: 420px;
            }
        }



        /* =====================================================
           CELULAR
        ===================================================== */

        @media (max-width: 600px) {

            .container {

                width: calc(100% - 30px);
            }


            .hero {

                padding-left: 15px;

                padding-right: 15px;
            }


            .small-title {

                font-size: 10px;

                letter-spacing: 3px;

                margin-bottom: 20px;
            }


            .hero h1 {

                font-size: clamp(
                    60px,
                    19vw,
                    85px
                );

                margin-bottom: 25px;
            }


            .hero-question {

                font-size: clamp(
                    20px,
                    5.5vw,
                    26px
                );

                line-height: 1.45;
            }


            .hero-line {

                margin: 25px auto;
            }


            .hero-date {

                font-size: 10px;

                letter-spacing: 1.5px;
            }


            .intro,
            .rafting-section,
            .plan,
            .chilina,
            .memory {

                padding-top: 70px;

                padding-bottom: 70px;
            }


            .intro-text h2 {

                font-size: 42px;
            }


            .intro-text p,
            .chilina-text p {

                font-size: 16px;

                line-height: 1.75;
            }


            .intro-photo {

                aspect-ratio: 4 / 5;

                max-height: 480px;
            }


            .section-header {

                margin-bottom: 35px;
            }


            .section-header h2 {

                font-size: 42px;
            }


            .section-header p {

                font-size: 16px;
            }


            .large-photo {

                height: 65vw;

                min-height: 250px;

                max-height: 380px;
            }


            .photo-caption {

                left: 12px;

                right: 12px;

                bottom: 12px;

                padding: 12px 14px;
            }


            .photo-caption strong {

                font-size: 14px;
            }


            .photo-caption span {

                font-size: 12px;
            }


            .plan h2 {

                font-size: 42px;

                margin-bottom: 40px;
            }


            .plan-card {

                padding: 25px 20px;
            }


            .plan-card h3 {

                font-size: 23px;
            }


            .chilina-photo {

                aspect-ratio: 4 / 5;

                max-height: 480px;
            }


            .chilina-text h2 {

                font-size: 48px;
            }


            .memory h2 {

                font-size: 45px;
            }


            .memory p {

                font-size: 16px;
            }


            .memory-photo {

                aspect-ratio: 4 / 3;
            }


            .final {

                min-height: 90vh;

                min-height: 90svh;

                padding-left: 15px;

                padding-right: 15px;
            }


            .final h2 {

                font-size: 48px;
            }


            .final p {

                font-size: 17px;
            }


            .buttons {

                flex-direction: column;

                width: 100%;

                max-width: 320px;

                margin-left: auto;

                margin-right: auto;
            }


            button {

                width: 100%;

                min-height: 54px;

                font-size: 16px;
            }


            #response {

                padding: 22px 18px;
            }

        }



        /* =====================================================
           CELULARES MUY PEQUEÑOS
        ===================================================== */

        @media (max-width: 380px) {

            .hero h1 {

                font-size: 58px;
            }


            .hero-question {

                font-size: 19px;
            }


            .hero-date {

                font-size: 9px;
            }


            .intro-text h2 {

                font-size: 37px;
            }


            .section-header h2 {

                font-size: 36px;
            }


            .final h2 {

                font-size: 42px;
            }

        }



        /* =====================================================
           CELULAR HORIZONTAL
        ===================================================== */

        @media (
            max-height: 500px
        ) and (
            orientation: landscape
        ) {

            .hero {

                min-height: 100svh;

                padding-top: 30px;

                padding-bottom: 50px;
            }


            .hero h1 {

                font-size: 55px;

                margin-bottom: 15px;
            }


            .hero-question {

                font-size: 18px;
            }


            .hero-line {

                margin: 15px auto;
            }


            .hero-date {

                font-size: 9px;
            }


            .scroll {

                display: none;
            }

        }

    </style>

</head>


<body>


    <!-- =====================================================
         PORTADA
    ====================================================== -->

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



    <!-- =====================================================
         INTRO
    ====================================================== -->

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
                IMAGEN 1

                ARCHIVO:
                img/tefa.jpg
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



    <!-- =====================================================
         RAFTING
    ====================================================== -->

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

                    Porque una salida diferente
                    siempre se recuerda un poco más.

                </p>

            </div>



            <!--
            IMAGEN 2

            ARCHIVO:
            img/rafting.jpg
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



    <!-- =====================================================
         PLAN
    ====================================================== -->

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



    <!-- =====================================================
         RÍO CHILINA
    ====================================================== -->

    <section class="chilina">

        <div class="container">

            <div class="chilina-grid">


                <!--
                IMAGEN 3

                ARCHIVO:
                img/rio-chilina.jpg
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



    <!-- =====================================================
         FOTO DE USTEDES
    ====================================================== -->

    <section class="memory">

        <div class="container">

            <div class="memory-container">


                <h2>
                    Y quizá...
                </h2>


                <p>
                    esta podría ser nuestra próxima foto juntos.
                </p>



                <!--
                IMAGEN 4

                ARCHIVO:
                img/nosotros.jpg
                -->

                <div class="memory-photo">

                    <img
                        src="img/nosotros.jpg"
                        alt="Nosotros"
                    >

                </div>


            </div>

        </div>

    </section>



    <!-- =====================================================
         PREGUNTA FINAL
    ====================================================== -->

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
                    type="button"
                    class="yes"
                    id="yesButton"
                >
                    Sí, vamos.
                </button>


                <button
                    type="button"
                    class="maybe"
                    id="maybeButton"
                >
                    Déjame pensarlo.
                </button>


            </div>


            <!--
            ESTE ESPACIO SE LLENA
            AUTOMÁTICAMENTE AL PRESIONAR
            UNO DE LOS BOTONES.
            -->

            <div id="response"></div>


        </div>

    </section>



    <!-- =====================================================
         FOOTER
    ====================================================== -->

    <footer>

        Hecho especialmente para
        <span>Tefa</span>.

    </footer>



    <!-- =====================================================
         JAVASCRIPT
         LOS BOTONES FUNCIONAN DESDE AQUÍ
    ====================================================== -->

    <script>

        document.addEventListener(
            "DOMContentLoaded",
            function () {


                const yesButton =
                    document.getElementById("yesButton");


                const maybeButton =
                    document.getElementById("maybeButton");


                const response =
                    document.getElementById("response");



                /* =========================================
                   BOTÓN "SÍ, VAMOS"
                ========================================= */

                yesButton.addEventListener(
                    "click",
                    function () {

                        response.style.display = "block";

                        response.innerHTML = `

                            <h3>
                                Entonces tenemos un plan.
                            </h3>

                            <p>
                                Me alegra que hayas dicho que sí.
                                Ahora solo falta preparar todo
                                para el sábado. 🌊
                            </p>

                        `;


                        setTimeout(
                            function () {

                                response.scrollIntoView({
                                    behavior: "smooth",
                                    block: "center"
                                });

                            },
                            100
                        );

                    }
                );



                /* =========================================
                   BOTÓN "DÉJAME PENSARLO"
                ========================================= */

                maybeButton.addEventListener(
                    "click",
                    function () {

                        response.style.display = "block";

                        response.innerHTML = `

                            <h3>
                                Está bien...
                            </h3>

                            <p>
                                Piénsalo con calma.
                                Aunque espero que al final
                                te animes a ir conmigo. 🌊
                            </p>

                        `;


                        setTimeout(
                            function () {

                                response.scrollIntoView({
                                    behavior: "smooth",
                                    block: "center"
                                });

                            },
                            100
                        );

                    }
                );


            }
        );

    </script>


</body>

</html>
