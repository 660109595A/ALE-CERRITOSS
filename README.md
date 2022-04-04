# ALE-CERRITOSS
PROYECTO INTEGRADOR 2

Definición de fuentes de datos a utilizar

El desarrollo de nuestro sistema utilizara seis tablas principales, las cuales nos ayudarán en
la función y el proceso para registrar usuarios, registrar productos o permitir el acceso a
usuarios asignado una contraseña cifrada; cada una de las tablas contara con registros como
usuario actualización y fecha actualización, los cuales beneficiaran al momento de efectuar
las auditorías internas.

Los principales tipos de datos utilizados en las tablas correspondientes son:

• Int: se utilizará inicialmente en los id de cada tabla, así como los registros que
requieran algún tipo de retorno numérico.
• Varchar: este tipo de datos nos proporcionara asignar nombre de usuarios, productos,
validar el tipo de navegador sobre el cual ingresan los usuarios o ser utilizado para
una parte fundamental del sistema, las cuales son el registro de las contraseñas
cifradas.
• Datetime: este tipo de dato nos retornara el día, el mes, el año y la hora incluyendo
minutos y segundos.
• Char: principalmente utilizado en datos de estado o impuesto agregado al producto a
comercializar

Diseño de tablas 

Procesos de extracción, transformación y carga de datos

Dado que la fuente de datos será la misma página web, con los datos que los usuarios
ingresen durante su proceso de registro, estos serán almacenados en la base de datos
elegida como nativa para la aplicación, que es MSSQL Server 2017 (como lo indicamos en
la etapa 1 del proyecto).
La carga de los datos la realizaremos mediante la integración de la base de datos con un
Business Intelligence que nos permita transformar y extraer los mismos:

• Integración: Proporcionamos los parámetros de la ubicación del servidor donde vive
la base de datos, que en este caso es el mismo en el que hostearemos el servicio
web, así como las credenciales correspondientes:

• Carga de datos: Procedemos con el mapeo de las tablas obtenidas desde la base
de datos, mismas que por el momento están vacías al no haber sido liberado el
servicio web y, por lo tanto, el único usuario registrado es el administrador:

• Extracción de datos: Como hemos comentado en el punto anterior, por el momento
no hay datos para extraer porque no se han realizado registros de usuarios, pero los
métodos que se utilizarán en la etapa 3 del proyecto son los siguientes:

Mecanismos e infraestructura para el almacenamiento y gestión de datos
Los mecanismos que utilizaremos, serán:
• Conexión nativa con la base de datos en tiempo real
• Importación manual de datos
• Importación programada de datos
15
• Almacenamiento en la unidad física del servidor donde se aloja la base de datos, con
opción a ser aumentado si es que el servidor es virtual, migrarse a una unidad de red,
equipo de storage o inclusive algún servicio de hosting como AWS o Microsoft Azure
• Procesamiento de datos mediante Business Intelligence (independientemente del
lugar donde se esté alojando la base de datos
• El Business Intelligence también tendrá la capacidad de aumentar sus recursos o ser
migrado a algún web service en la nube
La infraestructura necesaria es:
• Windows Server 2016 (evidentemente a 64 bits)
• Procesador Quadcore a 2.3 GHz o superior
• Memoria RAM de 16 GB
• Espacio libre en disco de 2 TB
• Comunicación mediante los puertos 995 para IMAPS y 465 para SMTPS. Lo anterior
es requerido para el envío de informes mediante correo electrónico con protocolos
seguros
Interfaz de usuario
La aplicación será desarrollada utilizando la base del lenguaje PHP, para esto la herramienta
de Visual Studio nos brindará la versatilidad en el diseño de la interfaz de usuario, la cual
integrará un login para acceder a la sección de productos.
Es importante que la empresa Bowen IT, tenga un registro actualizado de sus principales
clientes para que los datos le permitan a la organización parámetros en un dashboard de
visitas que el administrador podrá visualizar al iniciar su sesión.


https://drive.google.com/file/d/16FqJo-qYA4A8Vg9SzxrG0BP87FB2-cWy/view?usp=sharing
