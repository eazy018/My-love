
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carta de Amor Vintage</title>
    <link href="https://fonts.googleapis.com/css2?family=Crimson+Pro:wght@400;600&family=Parisienne&display=swap" rel="stylesheet">
    <style>
        /* Estilos base */
        body {
            background-color: #f8f1e3;
            font-family: 'Crimson Pro', serif;
            line-height: 1.8;
            margin: 0;
            padding: 20px;
            color: #3d3d3d;
            min-height: 100vh;
            background-image: 
                url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADIAAAAyCAMAAAAp4XiDAAAAUVBMVEWFhYWDg4N3d3dtbW17e3t1dXWBgYGHh4d5eXlzc3OLi4ubm5uVlZWPj4+NjY19fX2JiYl/f39ra2uRkZGZmZlpaWmXl5dvb29xcXGTk5NnZ2c8TV1mAAAAG3RSTlNAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEAvEOwtAAAFVklEQVR4XpWWB67c2BUFb3g557T/hRo9/WUMZHlgr4Bg8Z4qQgQJlHI4A8SzFVrapvmTF9O7dmYRFZ60YiBhJRCgh1FYhiLAmdvX0CzTOpNE77ME0Zty/nWWzchDtiqrmQDeuv3powQ5ta2eN0FY0InkqDD73lT9c9lEzwUNqgFHs9VQce3TVClFCQrSTfOiYkVJQBmpbq2L6iZavPnAPcoU0dSw0SUTqz/GtrGuXfbyyBniKykOWQWGqwwMA7QiYAxi+IlPdqo+hYHnUt5ZPfnsHJyNiDtnpJyayNBkF6cWoYGAMY92U2hXHF/C1M8uP/ZtYdiuj26UdAdQQSXQErwSOMzt/XWRWAz5GuSBIkwG1H3FabJ2OsUOUhGC6tK4EMtJO0ttC6IBD3kM0ve0tJwMdSfjZo+EEISaeTr9P3wYrGjXqyC1krcKdhMpxEnt5JetoulscpyzhXN5FRpuPHvbeQaKxFAEB6EN+cYN6xD7RYGpXpNndMmZgM5Dcs3YSNFDHUo2LGfZuukSWyUYirJAdYbF3MfqEKmjM+I2EfhA94iG3L7uKrR+GdWD73ydlIB+6hgref1QTlmgmbM3/LeX5GI1Ux1RWpgxpLuZ2+I+IjzZ8wqE4nilvQdkUdfhzI5QDWy+kw5Wgg2pGpeEVeCCA7b85BO3F9DzxB3cdqvBzWcmzbyMiqhzuYqtHRVG2y4x+KOlnyqla8AoWWpuBoYRxzXrfCuILl6SfiWCbjxoZJUaCBj1CjH7GIaDbc9kqBY3W/Rgjda1iqQcOJu2WW+76pZC9QG7M00dffe9hNnseupFL53r8F7YHSwJWUKP2q+k7RdsxyOB11n0xtOvnW4irMMFNV4H0uqwS5ExsmP9AxbDTc9JwgneAT5vTiUSm1E7BSflSt3bfa1tv8Di3R8n3Af7MNWzs49hmauE2wP+ttrq+AsWpFG2awvsuOqbipWHgtuvuaAE+A1Z/7gC9hesnr+7wqCwG8c5yAg3AL1fm8T9AZtp/bbJGwl1pNrE7RuOX7PeMRUERVaPpEs+yqeoSmuOlokqw49pgomjLeh7icHNlG19yjsXXK1mL4tuHR8zK53wX/NrlvJLMhZieAAAAAElFTkSuQmCC'),
                linear-gradient(to bottom, rgba(248, 241, 227, 0.8), rgba(248, 241, 227, 0.8));
        }

        /* Corazones decorativos */
        .corazon-decorativo {
            position: fixed;
            color: #c44569;
            opacity: 0.15;
            animation: flotar 8s infinite linear;
            z-index: 0;
        }

        @keyframes flotar {
            0% { transform: translateY(0) rotate(0deg); }
            25% { transform: translateY(-20px) rotate(15deg); }
            50% { transform: translateY(0px) rotate(0deg); }
            75% { transform: translateY(20px) rotate(-15deg); }
            100% { transform: translateY(0) rotate(0deg); }
        }

        .corazon-decorativo:nth-child(1) { left: 10%; top: 20%; font-size: 40px; animation-delay: 0s; }
        .corazon-decorativo:nth-child(2) { right: 15%; top: 40%; font-size: 35px; animation-delay: 1s; }
        .corazon-decorativo:nth-child(3) { left: 25%; bottom: 30%; font-size: 50px; animation-delay: 2s; }
        .corazon-decorativo:nth-child(4) { right: 5%; bottom: 20%; font-size: 45px; animation-delay: 3s; }

        .contenedor {
            max-width: 800px;
            width: 90%;
            margin: 30px auto;
            padding: 40px;
            background: rgba(255, 250, 240, 0.9);
            border-radius: 3px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            border: 1px solid #e0d4c0;
            position: relative;
            z-index: 1;
        }

        .corazon-principal {
            color: #c44569;
            font-size: 50px;
            text-align: center;
            animation: latido 1.2s infinite;
            text-shadow: 0 0 15px rgba(196, 69, 105, 0.3);
            margin: 30px 0;
            position: relative;
            z-index: 2;
        }

        @keyframes latido {
            0% { transform: scale(1); }
            15% { transform: scale(1.3); }
            30% { transform: scale(0.9); }
            45% { transform: scale(1.2); }
            60% { transform: scale(1); }
            100% { transform: scale(1); }
        }

        h1 {
            color: #c44569;
            text-align: center;
            font-family: 'Parisienne', cursive;
            font-size: 2.8em;
            margin: 30px 0;
            letter-spacing: 2px;
        }

        .poema p {
            font-family: 'Crimson Pro', serif;
            color: #4a4a4a;
            font-size: 1.1em;
            line-height: 1.8;
            margin: 30px 0;
            position: relative;
            padding-bottom: 15px;
        }

        .poema p::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 1px;
            background: linear-gradient(90deg, transparent, #c44569, transparent);
        }

        .spotify-player {
            margin: 40px auto;
            width: 100%;
            max-width: 400px;
            border-radius: 5px;
            overflow: hidden;
            border: 1px solid #d8c4b5;
            filter: sepia(0.3) saturate(0.8);
        }

        /* (Estilos restantes se mantienen igual) */
    </style>
</head>
<body>
    <!-- Corazones flotantes -->
    <div class="corazon-decorativo">♥</div>
    <div class="corazon-decorativo">♥</div>
    <div class="corazon-decorativo">♥</div>
    <div class="corazon-decorativo">♥</div>

    <div class="contenedor">
        <div class="flores">✉️ ❤️ ✉️</div>
        <div class="corazon-principal">♥</div>
        
        <h1>Para Mi Princesa</h1>
        
        <p class="fecha">8 de Marzo, 2025</p>
        
        <p>Mi Reyna,</p>

        <div class="poema">
            <p>
                "En tus ojos quiero ver historias de nosotros más románticas que las letras de Murder o Gonzalo.<br>
                En cada mirada me vuelves loco y tienes el poder de mirar y yo perderme,<br>
                y en esos labios que me muerden, siento mi realidad vuela<br>
                y el tiempo se rinde ante la intensidad de lo que somos.
            </p>

            <div class="flores">~ * ~</div>

            <p>
                Nuestros átomos vagaron por el universo,<br>
                fueron polvo de estrellas y parte de mundos desconocidos,<br>
                solo para encontrarse en este instante perfecto.
            </p>

            <div class="flores">~ * ~</div>

            <p>
                Si ya nos veíamos y no nos atrevimos a hablarnos,<br>
                me hace pensar que quizás antes fuimos una sola estrella,<br>
                separada por el tiempo, esperando volver a brillar juntos.
            </p>
        </div>

        <div class="spotify-player">
            <iframe 
                src="https://open.spotify.com/embed/track/1MKsphr9WmAkAGameksHDu?si=pQuLI3ogQ4m-RKsLVRQbUA" 
                width="100%" 
                height="152" 
                frameborder="0" 
                allowfullscreen="" 
                allow="encrypted-media" 
                loading="lazy">
            </iframe>
        </div>

        <ul>
            <li>Que tu sonrisa es mi mejor regalo</li>
            <li>Que tus abrazos son mi lugar favorito</li>
            <li>Que cada día a tu lado es una bendición</li>
        </ul>
        
        <p class="firma">
            Con todo mi corazón,<br>
            <span style="font-family: 'Parisienne', cursive; font-size: 1.3em;">Eazy</span>
        </p>
        
        <div class="flores">✉️ ❤️ ✉️</div>
    </div>
</body>
</html>