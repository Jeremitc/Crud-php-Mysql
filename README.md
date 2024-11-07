# CRUD PHP-MySQL

Este proyecto implementa una aplicación web básica que permite realizar operaciones CRUD (Crear, Leer, Actualizar y Eliminar) sobre una base de datos MySQL utilizando PHP.

## Características

- **Interfaz de usuario intuitiva**: Diseñada para facilitar la gestión de registros en la base de datos.
- **Operaciones CRUD completas**: Permite crear, leer, actualizar y eliminar registros de manera eficiente.
- **Conexión segura a la base de datos**: Utiliza prácticas recomendadas para interactuar con MySQL.

## Requisitos previos

Antes de ejecutar este proyecto, asegúrese de tener instalados los siguientes componentes:

- **Servidor web**: Apache o similar.
- **PHP**: Versión 7.0 o superior.
- **MySQL**: Servidor de base de datos MySQL.

Se recomienda utilizar [XAMPP](https://www.apachefriends.org/index.html) para simplificar la instalación y configuración de Apache, PHP y MySQL en entornos locales.

## Instalación y configuración

1. **Clonar el repositorio**:

   ```bash
   git clone https://github.com/Jeremitc/Crud-php-Mysql.git
   ```

2. **Configurar la base de datos**:

   - Crear una base de datos en MySQL llamada `php_mysql_crud`.
   - Importar el archivo `database/script.sql` para crear la tabla necesaria.

3. **Configurar la conexión a la base de datos**:

   - En el archivo `db.php`, asegúrese de que las credenciales de conexión coincidan con su configuración local:

     ```php
     $conn = mysqli_connect(
         'localhost',
         'root',
         '',
         'php_mysql_crud'
     );
     ```

4. **Iniciar el servidor**:

   - Coloque los archivos del proyecto en el directorio raíz de su servidor web (por ejemplo, `htdocs` en XAMPP).
   - Acceda a la aplicación mediante `http://localhost/Crud-php-Mysql/` en su navegador.

## Uso de la aplicación

- **Crear un nuevo registro**: Complete el formulario en la página principal y haga clic en "Guardar".
- **Leer registros**: Los registros existentes se muestran en una tabla en la página principal.
- **Actualizar un registro**: Haga clic en "Editar" junto al registro que desea modificar, realice los cambios y guarde.
- **Eliminar un registro**: Haga clic en "Eliminar" junto al registro que desea eliminar.

## Estructura del proyecto

- `index.php`: Página principal que muestra y gestiona los registros.
- `db.php`: Archivo de conexión a la base de datos.
- `save_task.php`: Procesa la creación de nuevos registros.
- `edit.php`: Formulario para editar registros existentes.
- `delete_task.php`: Procesa la eliminación de registros.
- `includes/`: Directorio que contiene archivos auxiliares, como encabezados y pies de página.
- `database/script.sql`: Script SQL para crear la tabla necesaria en la base de datos.

## Contribuciones

Las contribuciones son bienvenidas. Si desea mejorar este proyecto, por favor:

1. Haga un fork del repositorio.
2. Cree una nueva rama (`git checkout -b feature/nueva-funcionalidad`).
3. Realice sus cambios y haga commit (`git commit -am 'Añadir nueva funcionalidad'`).
4. Haga push a la rama (`git push origin feature/nueva-funcionalidad`).
5. Cree un Pull Request.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulte el archivo `LICENSE` para más detalles.

---

Este proyecto es una excelente demostración de habilidades en desarrollo web full stack, mostrando competencia en PHP, MySQL y la creación de aplicaciones CRUD funcionales.
