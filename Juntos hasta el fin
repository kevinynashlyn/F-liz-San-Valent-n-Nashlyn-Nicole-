<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nashlyn, Mi Princesa</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-image: url('https://i.imgur.com/wr5kzC5.jpeg'); /* Imagen de fondo */
            background-size: cover;
            background-position: center;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            padding: 0 20px;
            overflow: hidden;
        }

        #message {
            font-size: 3em;
            margin: 20px 0;
            color: #ffb6c1;
            text-shadow: 0 0 8px rgba(255, 182, 193, 0.9), 0 0 10px rgba(255, 182, 193, 0.9);
        }

        #btnSi, #btnNo {
            padding: 20px 40px;
            font-size: 2em;
            margin: 10px;
            border: none;
            border-radius: 15px;
            cursor: pointer;
            transition: all 0.3s ease;
            position: relative;
        }

        #btnSi {
            background-color: #d6336c;
            color: white;
        }

        #btnNo {
            background-color: #ff758c;
            color: white;
        }

        .hidden {
            display: none;
        }

        #nuevaPantalla {
            display: none;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            text-align: center;
            padding: 20px;
        }

        #nuevaPantalla h1, #nuevaPantalla p {
            color: #00bfff;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7), 0 0 15px rgba(0, 191, 255, 1); /* Mejor contraste */
            font-size: 2.5em;
            font-weight: bold; /* Hace el texto más claro */
        }

        .btn-container {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

    </style>
</head>
<body>
    <!-- Primera pantalla -->
    <div id="pantallaInicial">
        <div id="message">Nashlyn, Mi Princesa, ¿Quieres ser mi San Valentín? ❤️✨</div>
        <div class="btn-container">
            <button id="btnSi">Sí</button>
            <button id="btnNo">No</button>
        </div>
    </div>

    <!-- Segunda pantalla (oculta inicialmente) -->
    <div id="nuevaPantalla" class="hidden">
        <h1>¡Sabía que dirías que sí! ❤️✨</h1>
        <p>Por eso te amo muchísimo</p>
        <p>Eres el amor de mi vida ❤️✨</p>
        <p>Eres la mejor novia del mundo ❤️✨</p>
        <p>30.08.24❤️✨ Juntos Hasta El Fin ❤️✨</p>
    </div>

    <script>
        let noCount = 0;
        const btnSi = document.getElementById('btnSi');
        const btnNo = document.getElementById('btnNo');
        const message = document.getElementById('message');
        const pantallaInicial = document.getElementById('pantallaInicial');
        const nuevaPantalla = document.getElementById('nuevaPantalla');

        // Lista de respuestas personalizadas para el "No"
        const respuestasNo = [
            "¿De verdad dices que no? 🥺",
            "No puede ser... dime que sí 🥹",
            "¿Me estás haciendo sufrir a propósito? 😢",
            "Si dices que no, mi corazón se rompe 💔",
            "¡No acepto un no como respuesta! 😤",
            "Dime que es una broma, por favor 🥺",
            "¿Cómo puedes decirme que no? 😭",
            "Si sigues diciendo que no, voy a llorar 😞",
            "Te amo tanto, no me hagas esto 🥺",
            "Dime que sí, por favor 😭",
            "Si dices que no, te voy a llenar de besos hasta que digas que sí 😘",
            "Nooo, no me hagas esto 🥺💔",
            "Si sigues diciendo que no, me voy a derretir de tristeza 🫠",
            "Voy a contar hasta tres y dirás que sí 😏",
            "No juegues con mi corazón así 😖",
            "Cada vez que dices no, mi amor por ti se multiplica ❤️",
            "Voy a seguir insistiendo hasta que digas que sí 😘",
            "Te haré reír tanto que dirás que sí sin darte cuenta 😆",
            "No puedo imaginar mi San Valentín sin ti 😞",
            "Eres el amor de mi vida, dime que sí 💕"
        ];

        // Reducir tamaño y hacer desaparecer el botón "No", y hacer crecer el "Sí"
        btnNo.addEventListener('click', () => {
            if (noCount < respuestasNo.length) { // Asegura que se elijan respuestas dentro del límite
                message.innerHTML = respuestasNo[noCount];
                let scaleSizeNo = 1 - noCount * 0.05; // Reduce el tamaño del botón "No"
                let scaleSizeSi = 1 + noCount * 0.05; // Aumenta el tamaño del botón "Sí"
                btnNo.style.transform = `scale(${scaleSizeNo})`; // Cambia el tamaño del botón "No"
                btnSi.style.transform = `scale(${scaleSizeSi})`; // Cambia el tamaño del botón "Sí"
                noCount++;
            } else {
                btnNo.style.display = 'none'; // Elimina el botón "No" después de que se acaben las respuestas
            }
        });

        // Muestra la segunda pantalla cuando se presiona "Sí"
        btnSi.addEventListener('click', () => {
            pantallaInicial.style.display = 'none'; // Ocultar la pantalla inicial
            nuevaPantalla.style.display = 'flex'; // Mostrar la nueva pantalla

            // Agregar las frases personalizadas al nuevo contenedor
            nuevaPantalla.innerHTML = `
                <h1>¡Sabía que dirías que sí! ❤️✨</h1>
                <p>Por eso te amo muchísimo</p>
                <p>Eres el amor de mi vida ❤️✨</p>
                <p>Eres la mejor novia del mundo ❤️✨</p>
                <p>30.08.24❤️✨ Juntos Hasta El Fin ❤️✨</p>
            `;
        });
    </script>

</body>
</html>
