# examen-especial

Instalar symphony 
Instalar xampp
Instalar composer
Instalar git
abrir cmd y cambiar directorio al del proyecto (originalmente se instalo en la ruta C:/xampp/htdocs/test)
abrir xampp e iniciar apache y mysql
Iniciar servidor con
symfony server:start
(de iniciar) se puede proseguir con la instalacion desde otro cmd
la direccion es 127.0.0.1:8000
console make:entity NOTA:LA BASE DE DATOS DEL PROYECTO SE NOMBRO test, favor de respetar el nombre para no tener conflictos(aqui se crearan los datos de la base de datos)
se utilizo nombre, edad, ocupacion (edad es int, los otros dos string)
NOTA: AL CREAR LA BASE DE DATOS, SE PUEDE ARRANCAR EL REPOSITORIO, SE RECOMIENDA ACTUALIZAR LA PAGINA DE NUEVO
DE APARECER LA TABLA, LOS OTROS DATOS DE LA INSTALACION POSTERIOR A ESTA NOTA, YA NO SERAN NECESARIOS, 
composer req orm
composer req maker
composer req twig
dentro del proyecto, en el archivo .env configurar la url de la base de datos de la siguiente manera
DATABASE_URL="mysql://root@127.0.0.1:3307/test?serverVersion=8&charset=utf8mb4" (su puerto puede ser el 3306, en mi caso no lo fue)
console make:controller
Maincontroller
symfony server:start (si conecta, configuramos bien el puerto de la base de datos) 
console make:entity (aqui se crearan los datos de la base de datos)
se utilizo nombre edad ocupacion (edad es int, los otros dos string)
php bin/console make:migration
php bin/console doctrine:migrations:migrate
composer require form validator
php bin/console make:form 
symfony server:start
