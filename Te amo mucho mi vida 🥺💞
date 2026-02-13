<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Galaxia de Amor</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            background: linear-gradient(#0b001a, #2d004e);
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        /* Estrellas */
        .estrella {
            position: absolute;
            background: white;
            border-radius: 50%;
            animation: parpadear infinite alternate;
        }

        /* Corazones */
        .corazon {
            position: absolute;
            color: #ff4d94;
            font-size: 20px;
            animation: flotar infinite ease-in-out;
        }

        /* Título */
        .titulo {
            color: white;
            font-family: 'Arial', sans-serif;
            font-size: 2em;
            text-align: center;
            text-shadow: 0 0 15px #ff4d94, 0 0 30px #9900ff;
            z-index: 10;
        }

        /* Animaciones */
        @keyframes parpadear {
            from { opacity: 0.3; }
            to { opacity: 1; }
        }

        @keyframes flotar {
            from { transform: translateY(0) rotate(0deg); }
            to { transform: translateY(-30px) rotate(10deg); }
        }
    </style>
</head>
<body>
    <h1 class="titulo">Mi Galaxia de Amor</h1>

    <script>
        // Crear estrellas aleatorias
        function crearEstrellas(cantidad) {
            for (let i = 0; i < cantidad; i++) {
                const estrella = document.createElement('div');
                estrella.classList.add('estrella');
                
                const tamano = Math.random() * 3 + 1;
                const x = Math.random() * 100;
                const y = Math.random() * 100;
                const duracion = Math.random() * 3 + 2;

                estrella.style.width = `${tamano}px`;
                estrella.style.height = `${tamano}px`;
                estrella.style.left = `${x}%`;
                estrella.style.top = `${y}%`;
                estrella.style.animationDuration = `${duracion}s`;

                document.body.appendChild(estrella);
            }
        }

        // Crear corazones aleatorios
        function crearCorazones(cantidad) {
            for (let i = 0; i < cantidad; i++) {
                const corazon = document.createElement('div');
                corazon.classList.add('corazon');
                corazon.textContent = '❤️';
                
                const x = Math.random() * 100;
                const y = Math.random() * 100;
                const duracion = Math.random() * 8 + 5;
                const retraso = Math.random() * 5;

                corazon.style.left = `${x}%`;
                corazon.style.top = `${y}%`;
                corazon.style.animationDuration = `${duracion}s`;
                corazon.style.animationDelay = `${retraso}s`;

                document.body.appendChild(corazon);
            }
        }

        // Generar elementos
        crearEstrellas(200);
        crearCorazones(30);
    </script>
</body>
</html>
