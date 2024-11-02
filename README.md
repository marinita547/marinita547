- <!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> pidenos ya</title>
    <link rel="stylesheet" href="styles.css">
    <style>


    </style>
</head>

<body>
    <header>
        <h1>ALMUERZOS Y TIPICOS MARGARITA</h1>
        <p>
        <h3></h3>
        </p>
        <img src="Logo Parrilla Argentina Circular Marrón y Negro.jpg" alt="Descripción de la imagen" class="imagen-redonda" class="imagen-izquierda"
            class="led-border">
    </header>
    <nav>
        <ul>
        
            <li><a href="contacto2.html">Contactos</a></li>
            <li><a href="chat.html" > seyi</a></li>


        </ul>

    </nav>

    <style>
        .producto {
            margin-bottom: 10px;
        }
    </style>
    </head>
    
    <body>
        <h1>Buscador de Productos de Comida</h1>
    
        <div id="search">
            <h2>Encuentra lo que mas te guste</h2>
            <input type="text" placeholder="Busca por nombre o tipo de comida...">
            <button>Buscar</button>
            <button>
        <script>

            // Elementos del DOM
            const buscador = document.getElementById('buscador');
            const resultados = document.getElementById('resultados');

            // Función para mostrar los productos filtrados
            function mostrarResultados(filtro) {
                resultados.innerHTML = ''; // Limpiar resultados anteriores
                const productosFiltrados = productos.filter(producto =>
                    producto.nombre.toLowerCase().includes(filtro.toLowerCase()) ||
                    producto.descripcion.toLowerCase().includes(filtro.toLowerCase())
                );

                if (productosFiltrados.length > 0) {
                    productosFiltrados.forEach(producto => {
                        const divProducto = document.createElement('div');
                        divProducto.classList.add('producto');
                        divProducto.innerHTML = `<strong>${producto.nombre}</strong>: ${producto.descripcion}`;
                        resultados.appendChild(divProducto);
                    });
                } else {
                    resultados.innerHTML = '<p>No se encontraron productos.</p>';
                }
            }

            // A Milton le gustan los niños JAJA
            buscador.addEventListener('input', (e) => {
                const filtro = e.target.value;
                mostrarResultados(filtro);
            });

            // HECTOR no se baña
            mostrarResultados('');
        </script>
    </body>
    
    </html>
    
    </div>
    
            </script>
        

        </button>
        <section id="contact">
            <h2>Contacto</h2>
            <form action="#">
                <label for="name">Nombre:</label>
                <input type="text" id="name" name="name">
                <label for="email">Correo:</label>
                <input type="email" id="email" name="email">
                <button type="submit">Enviar</button>
            </form>
            <head><h2>GRACIASPOR PREFERIRNOS: <br> lo que tu gustes aqui te lo preparamos tenemos 16 años de estar laborando puedes dejarnos tu nombre para tener tu registroy te preparamos la comida que tu gustes <br> la autenticidad de nuestros alimentos es lo que nos identifica  aqui abajo te dejamos algunos de nuestros productos  ¡DISFRUTA! <br> ATT:Margarita </h2></head>
   
        </div>
    <section id="categories">
        <div class="category">
            <img src="almuerzo 1.jpeg" alt="" width="60%" height="70%">
            <h3>fajitas de carne</h3>
            
            <button onclick="mostrarAlerta()">Añadir </button>
            
            <script>
                function mostrarAlerta() {
                    alert("Añadido al carrito");
                }
            </script>
        </div>
        <div class="category">
            <img src="almuerzo2.jpg" alt="" width="60%" height="70%">
            <h3>carne a la plancha</h3>
            <button onclick="mostrarAlerta()">Añadir </button>
            
            <script>
                function mostrarAlerta() {
                    alert("Añadido al carrito");
                }
            </script>
        </div>
        <div class="category">
            <img src="almuerzo 3.jpg" alt="" width="60%" height="70%">
            <h3> sopa de patas</h3>
            <button onclick="mostrarAlerta()">Añadir </button>
            
            <script>
                function mostrarAlerta() {
                    alert("Añadido al carrito");
                }
            </script>
        </div>
    </section>
    <section id="products">
        <div class="product">
            <img src="tipico 1.jpg" alt="" width="60%" height="70%">
            <h3>pastelitos de masa</h3>
            <button onclick="mostrarAlerta()">Añadir</button>
            
            <script>
                function mostrarAlerta() {
                    alert("Añadido al carrito");
                }
            </script>

        </div>
        <div class="product">
            <img src="tipico 2.webp" alt="" width="60%" height="70%%">
            <h3> yuca con chicharron</h3>
            <button onclick="mostrarAlerta()">Añadir </button>
            
            <script>
                function mostrarAlerta() {
                    alert("Añadido al carrito");
                }
            </script>
        </div>
        <div class="product">
            <img src="tipico 3.jpg" alt="" width="60%" height="70%">
            <h3>tamalitos de elote</h3>
            <button onclick="mostrarAlerta()">Añadir </button>
            
            <script>
                function mostrarAlerta() {
                    alert("Añadido al carrito");
                }
            </script>
            
        </div>

    </section>
    <footer>
        
    </footer>
</body>

</html>
    
    </section>
    

    <footer>
        <h3>©2024 Almuerzos y tipicos Margarita-gracias por preferirnos-derechos reservados</h3>
    </footer>

    <script src="scripts.js"></script>
</body>
</html>
document.querySelector('form').addEventListener('submit', function (event) {
    event.preventDefault();
    const name = document.querySelector('#name').value;
    const email = document.querySelector('#email').value;

    if (name === '' || email === '') {
        alert('Por favor, rellena todos los campos.');
    } else {
        alert(`Gracias por preferirnos, ${name}!`);
    }
});
    function buscarTexto() {
        
        let input = document.getElementById("search-input").value.toLowerCase();
    let contenido = document.getElementById("contenido");
    let paragraphs = contenido.getElementsByTagName("p");

   
    for (let paragraph of paragraphs) {
        paragraph.innerHTML = paragraph.innerHTML.replace(/<span class="highlight">|<\/span>/g, "");
            }

    
    for (let paragraph of paragraphs) {
        let texto = paragraph.innerText.toLowerCase();
    if (texto.includes(input)) {
        let regex = new RegExp(input, "gi");
    paragraph.innerHTML = paragraph.innerHTML.replace(regex, `<span class="highlight">${input}</span>`);
                }
            }
        }
     
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>pidenos ya</title>
    <link rel="stylesheet" href="styles.css">
</head>

<body>
    <header>
        <h1>AlMUERZOS Y TIPICOS MARGARITA</h1>
        <div class="contenido">
            <img src="Logo Parrilla Argentina Circular Marrón y Negro.jpg" alt="Descripción de la imagen" class="imagen-redonda" class="imagen-izquierda">
            <p>
            <h3> </h3>
            </p>

            <nav>


                </style>
                </head>

                <body>

                    <ul>
                
                        <li><a href="paginafinal.html">principal</a></li>

                    </ul>
            </nav>
    </header>


    <title>Tarjeta de Presentación</title>
    <style>

    </style>
    </head>

    <body>

    
      <div class="tarjeta">
       

            
            <div class="contenido">
                <h2>Florinda Margarita Gonzalez corado</h2>
                <p>dueña del negocio </p>
                <p>ALMUERZOS Y TIPICOS MARGARITA </p>

                <!-- Enlace a perfil o contacto -->
                <a href="https://wa.me/50370534220">Contactar</a>
            </div>
        </div>

        <div class="tarjeta">
            
            <div class="contenido">
                <h2>Marina Margarita Tobar Gonzalez</h2>
                <p>GERENTE </p>
                <p>ALMUERZO Y TIPICOS MARGARITA</p>

                <!-- Enlace a perfil o contacto -->
                <a href="https://wa.me/50370534220">Contactar</a>
            </div>
        </div>
        <footer>
            <p>
            <h3>&copy;2024 Almuerzos y tipicos Margarita-gracias por preferirnos-derechos reservados</h3>
            </p>
        </footer>
    </body>

</html>
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chatbot de Comedor</title>
    <link rel="stylesheet" href="styles.css">
<body>
<header>
    <h1>AlMUERZOS Y TIPICOS MARGARITA</h1>
    <div class="contenido">
        <img src="Logo Parrilla Argentina Circular Marrón y Negro.jpg" alt="Descripción de la imagen"
            class="imagen-redonda" class="imagen-izquierda">
        <p>
        <h3> </h3>
        <nav>
            <ul>
        
                <li><a href="paginafinal.html">principal</a></li>
                
        
        
            </ul>
        
        </nav>
        <body>
            
        </body>
    <style>
        body {
            font-family: Arial, sans-serif;
        }

        #chatbot {
            width: 300px;
            border: 1px solid #3f3f3f;
            padding: 10px;
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #fffab2;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
        }

        #messages {
            height: 200px;
            overflow-y: auto;
            margin-bottom: 10px;
            border: 1px solid #ddd;
            padding: 5px;
        }

        .message {
            margin: 5px 0;
        }

        .user {
            text-align: right;
            color: blue;
        }

        .bot {
            text-align: left;
            color: green;
        }

        #userInput {
            width: 100%;
            padding: 5px;
            box-sizing: border-box;
        }
    </style>
</head>

<body>

    <div id="chatbot">
        <div id="messages"></div>
        <input type="text" id="userInput" placeholder="Escribe tu pregunta..." autocomplete="off">
    </div>

    <script src="chat.js"></script>
</body>

</html>
document.addEventListener("DOMContentLoaded", function () {
    const messages = document.getElementById("messages");
    const userInput = document.getElementById("userInput");

    const respuestas = {
        "horario": "Nuestro horario de atención es de lunes a viernes de 9:00 a 20:00.",
        "reservar": "Puedes hacer una reserva llamando a nuestro número o directamente desde nuestra página web.",
        "menú": "Contamos con un menú variado de platos locales e internacionales. Puedes ver el menú completo en la sección 'Menú' de nuestra página.",
        "platos recomendados": "¡Te recomendamos todos nuestros platillos pero este domingo  3 te tendremos sopa de gallina y sopa de patas ven prueba comparte y disfruta !.",
        "ubicación": "Nos encontramos en ciudad pacifico, en la calle principal.",
        "gracias": "¡Gracias a ti! Estoy aquí para ayudarte.",
        "default": "Lo siento, no entiendo tu pregunta. Por favor intenta preguntar algo más específico sobre el comedor."
    };

    function agregarMensaje(texto, clase) {
        const mensaje = document.createElement("div");
        mensaje.className = `message ${clase}`;
        mensaje.textContent = texto;
        messages.appendChild(mensaje);
        messages.scrollTop = messages.scrollHeight; // Hector no se baña
    }

    function procesarEntrada(input) {
        input = input.toLowerCase();
        let respuesta = respuestas["default"];

        for (let clave in respuestas) {
            if (input.includes(clave)) {
                respuesta = respuestas[clave];
                break;
            }
        }

        return respuesta;
    }

    userInput.addEventListener("keypress", function (e) {
        if (e.key === "Enter" && userInput.value.trim() !== "") {
            const input = userInput.value.trim();
            agregarMensaje(input, "user");

            const respuesta = procesarEntrada(input);
            setTimeout(() => agregarMensaje(respuesta, "bot"), 500);

            userInput.value = "";
        }
    });
});

<!---
marinita547/marinita547 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
