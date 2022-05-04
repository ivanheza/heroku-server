# DESPLEGAR NUESTRO PROYECTO EN LA NUBE

Retomamos nuestro trabajo para implementar el proyecto en Heroku.
En el servidor local definir el PORT en .env

-  **npm run start:** inicializa el proyecto
-  **npm run dev:** inicializa en modo development

## - PORYECTO EN HEROKU

Se subió el codigo a heroku con la finalidad de utilizar el servidor desde heroku.

## Database

El proyecto esta programado para trabajar con MongoDB

-  MongoDB (mongoose)

*  Usuarios
*  Productos
*  Carts

#### PRODUCTOS "/api/productos"

-  GET " / " **Muestra todos los productos en la db productos.txt**
-  GET " /:idProducto " **Muestra el producto por ID**
-  POST " / " **Agrega un producto nuevo al archivo produtcos.txt**
-  PUT " /:idProducto " **Actualiza el producto solicitado por ID por el método PUT**
-  DELETE " /:idProducto " **Borra el producto con el ID selecicionado**

#### CARRITO "/api/carrito"

-  POST " / " **Agrega un carrito nuevo al archivo cartlist.txt**
-  DELETE " /:idcarrito " **Borra el carrito con el ID selecicionado**
-  GET " /:idcarrito/productos " **Muestra todos los productos dentro de un carrito con el ID solicitado**
-  POST " /:idcarrito/productos " **Agrega un producto específico al carrito con un ID específico**
-  DELETE " /:idcarrito/productos/:IDproducto " **Borra un producto específico(id) en el carrito con el ID selecicionado**

> > > > Importante > PARA LA PRUEBA DE ENDPOINTS POST, PUT Y DELETE SE UTILIZO POSTMAN

### Git Ignore

> > > node modules y archivos .DIR

### Dependencies

-  Para el servidor, manejo de rutas [Express JS](https://expressjs.com/es/ "Ver más")
-  Para el timestamp y fechas [Moment JS](https://momentjs.com/ "Ver más")
-  Para la asignación de IDs [uuid](https://www.npmjs.com/package/uuid "Ver más")
-  Se utilizo para la conexión a la instancia de MongoDB y realización de esquemas. [mongoose](https://mongoosejs.com/ "Ver más")
-  Se utilizó la dependencia de firebaseadmin para la configuración, conexión e implementacion de Cloud Firestore [firebase](https://www.npmjs.com/package/firebase-admin "Ver más")
-  Se utilizó la dependencia de dotenv para la implementacion y uso de variables de entorno .env [dotenv](https://www.npmjs.com/package/dotenv "Ver más")

#### Created by: **Ivan Hernández Preza**
