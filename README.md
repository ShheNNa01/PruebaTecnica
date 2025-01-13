# Prueba Técnica
Entregable para la empresa JUJU

Descripción
Este repositorio contiene una aplicación para gestionar una librería, que incluye endpoints documentados en Swagger para realizar pruebas funcionales.

Proceso de inicio de la aplicación

Descargar y preparar el proyecto
1. Clonar o descargar el repositorio desde GitHub.
2. Extraer el archivo ZIP en la ubicación de tu preferencia.
   
Configurar la base de datos
1. Abrir SQL Server Management Studio (SSMS).
2. Crear un nuevo query.
3. Copiar y pegar el contenido del archivo SQL SCRIPT DB.sql en el nuevo query (archivo en la carpeta extraida).
4. Ejecutar el script seleccionando, seleccionando todo el código (Ctrl + A) y presionando F5.
5. Confirmar que se haya creado correctamente la base de datos Libros.
   
Abrir el proyecto en Visual Studio Code (VS Code)
1. Abrir una terminal en la carpeta del proyecto:
2. Navegar a la carpeta del proyecto.
3. Escribir cmd en la barra de direcciones y presionar Enter.
4. En la consola, escribir: code .
   
Configurar la cadena de conexión
1. En VS Code, ir a la carpeta config y abrir el archivo db.js.
2. Verificar que el valor Database=Libros esté configurado correctamente. Este es como se muestra anteriormente.

Instalar dependencias y ejecutar el proyecto
1. Abrir una terminal (Ctrl + Ñ) dentro de VS Code.
2. Ejecutar el comando: npm install.
3. Una vez instaladas las dependencias, ejecutar la aplicación con F5.
4. Confirmar que la aplicación esté corriendo en el puerto 3000 y mostrar la URL en la consola (http://localhost:3000).
   
Acceder a Swagger
1. Abrir el navegador y visitar: http://localhost:3000/api-docs/.
2. Proceso para ejecutar pruebas
3. Registro de usuario
4. Ir al endpoint POST /api/users/register.
5. Hacer clic en el botón Try Out.
6. Completar los datos necesarios o utilizar los valores por defecto.
7. Hacer clic en Execute para registrar un nuevo usuario.

Inicio de sesión
1. Ir al endpoint POST /api/users/login.
2. Hacer clic en el botón Try Out.
3. Introducir las credenciales utilizadas en el registro.
4. Hacer clic en Execute.
5 Copiar el token generado en la respuesta (valor del campo "token").

Autenticación
1. En el menú de Swagger, localizar el candado junto al endpoint que deseas probar.
2. Hacer clic en el candado y pegar el token copiado en el campo correspondiente.
3. Autorizar la autenticación para realizar pruebas en los demás endpoints

Listo en este punto estaria todo perfecto para proceder con los EndPoints de la libreria.
