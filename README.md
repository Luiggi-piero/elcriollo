## Proceso
1. Instalar herramientas de desarrollo: vsc, postman, node
2. Crear app Angular
    1. Crear una carpeta del proyecto
    2. Instalar @angular/cli
    3. Crear app frontend
3. Crear header
    1. Crear el componente
    2. Agregar html
    3. Agregar css
4. Lista de comidas
    1. Crear modelo de comida
    2. Crear data.ts
        1. Agregar ejemplos de comidas
    3. Agregar imagenes a assets
    4. Crear el servicio de comida
    5. Crear el componente home
        1. Agregar ts
        2. Agregar html
        3. Agregar css
5. Búsqueda
    1. Agregar metodo al servicio de comida
    2. Agregar ruta de búsqueda
    3. Mostrar el resultado de búsqueda en el componente home
    4. Crear el componente search
        1. Agregar al componente de inicio
        2. Agregar ts
        3. Agregar html
        4. Agregar css
6. Barra de etiquetas(tags) o categorías
    1. Crear el modelo de tag
    2. Agregar ejemplos de tag en data.ts
    3. Servicio Food
        1. Agregar método para obtener todos los tags
        2. Agregar método para todas las comidas relacionados a un tag
    4. Agregar ruta de tags
    5. Mostrar el tag resultante en el componente home
    6. Generar el componente Tags
        1. Agregar al componente home
        2. Agregar ts
        3. Agregar html
        4. Agregar css
7. Página de comida
    1. Agregrar método al servicio food
    2. Generar el componente de página de food
        1. Agregar ruta
        2. Agregar ts
        3. Agregar html
        4. Agregar css
8. Página del carrito de compras
    1. Crear modelo CartItem
    2. Crear modelo Cart
    3. Generar el servicio Cart
    4. Añadir el botón agregar al carro en la página de comida
    5. Generar el componente Cart Page
        1. Agregar ruta
        2. Agregar ts
        3. Agregar html
        4. Agregar css
9. No encontrado
    1. Generar compoenente
        1. Agregar ts
        2. Agregar html
        3. Agregar css
    2. Agregar a las páginas
        1. A la página home
        2. A la página Food
        3. A la página Cart
10. Conectarse al backend
    1. Crear la carpeta backend
    2. npm init -y (inicializa npm en el backend)
    3. npm install typescript
    4. crear tsconfig.json
    5. crear .gitignore
    6. Copiar data.ts a backend/src
    7. npm install express cors
    8. Crear server.ts
        1. install @types
        2. Agregar apis
    9. npm install nodemon ts-node --save-dev
    10. Agregar urs.ts al frontend
    11. Agregar HttpClient module
    12. Actualizar el servicio Food
11. Página de login
    1. Generar componente
        1. Agregar ruta
        2. Agregar ts
        3. Agregar html
            1. Importar Reactive forms module
        4. Agregar css
    2. Agregar api de login
        1. Usar json
        2. Agregar jsonwebtoken
        3. Probar en Postman
    3. Crear servicio User
        1. Generar modelo user
        2. Agregar User Subject
        3. Agregar el método login
            1. Agregar urls de user
            2. Generar IUserLogin interface
            3. Agregar ngx-toastr
                1. Import modulo
                2. Import BrowserAnimationsModule
                3. Agregar estilos en angular.json
            4. Agregar al header
        4. Agregar método local storage
        5. Agregar el método logout
            1. Agregar al header
12. Crear componentes para la página login
    1. Contenedor del input
    2. Validación del input
    3. Text Input
    4. Default button
13. Conectar la api de login a MongoDB Atlas
    1. Mover Apis a routers (enrutadores)
    2. Crear MongoDB Atlas
    3. Crear el archivo .env
    4. Instalar
        1. mongoose
        2. dotenv
        3. bcryptjs: proteger las contraseñas almacenadas en una base de datos
        4. express-async-handler: Manejo de errores en funciones asincronas
    5. Conectar a MongoDB Atlas
    6. Usar MongoDB Atlas en lugar del archivo data.ts en apis 
14. Registrar usuario
    1. Agregar api de registro
    2. Agregar método en el servicio
    3. Agregar ruta de la página del registro
    4. Agregar componente de registro
15. Loading
    1. Agregar imagen
    2. Agregar componente
    3. Agregar servicio
    4. Agregar interceptor
16. Página checkout
    1. Crear modelo Order
    2. Crear el componente checkout page
        1. Agregar ruta
    3. Agregar usuario al servicio de usuario
    4. Agregar carro al servicio del carro de compras
    5. Crear componente de lista de articulos de pedido
    6. Agregar mapa en la página de checkout
        1. Agregar el paquete leaflet para mapas interactivos => npm install leaflet
            1. Agregar el tipo @types/leaflet => npm install --save-dev @types/leaflet
            2. Agregar css en angular.json
        2. Agregar AddressLatLng al modelo de Order
        3. Crear el componente Map
            1. Agregar a la página checkout
            2. Agregar ts
                1. Cambiar el selector app-map a map
            3. Agregar html
            4. Agregar css
        2. Agregar auth guard

    7. Guardar Order
        1. Agregar modelo Order en backend
        2. Agregar el status order de tipo enum
        3. Agregar middleware Auth
        4. Agregar Router de order  
            1. Agregar la api create
        5. Agregar urls de order a url.ts
        6. Agregar el servicio order
            1. Agregar el método crear
        7. Agregar el interceptor Auth
17. Página payment
    1. Crear el componente
    2. Agregar api getOrderForCurrentUser
    3. Agregar método al servicio order
    4. Conectar el servicio con el componente
    5. Hacer que el componente del map sea solo de lectura
18. Agregar Paypal
    1. Crear el componente
        1. Agregar a la página payment
    2. Obtener el id del cliente paypal
    3. Agregar Paypal js al index.html
    4. Configurar el botón paypal
    5. Agregar la api Pay al router de order
    6. Obtener una cuenta de zona segura de paypal
19. Página Order Track
    1. Crear el componente
        1. Agregar las rutas
    2. Agregar api
        1. Agregar a urls.ts
    3. Agregar el método al servicio order
    4. Agregar html
    5. Agregar css
<!-- Activar backend -->
<!-- ir a la carpeta backend y ejecutar npm start -->
<!-- cd backend -->

<!-- Activar frontend -->
<!-- ir a la carpeta frontend y ejecutar ng serve -o -->
<!-- cd frontend -->