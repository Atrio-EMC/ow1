---
layout: blog
tittle: Sesiones online
---

|Fecha|Puntos a tratar|Ponente|
|:---:|----------|--------|
|7 de Octubre| 1,2,3 |José Domingo |
|14 de Octubre| 3,4,5,6,7,8,9,10,11 |José Domingo  |
|16 de Octubre| 11,12,13,14,15,16,17,18,19,20 | Alberto |
|19 de Octubre| 21,22,23,24,25,26,27,28 | José Domingo |
|21 de Octubre | 29,30,31,32,33,34,35,36,37,38,39,40 | José Domingo |
|26 de Octubre|  | Alberto |
|28 de Octubre| | José Domingo |
|4 de Noviembre|  | Alberto |
|9 de Noviembre|  | Alberto |
|11 de Noviembre|  | Alberto |

# Puntos

1. Presentación y explicación de los objetivos del curso, las secciones en que está dividido y que la dificultad irá creciendo poco a poco.
1. Contenidos: Introducción al Cloud Computing
1. Contenidos: Introducción a OpenStack
1. Contenidos: Introducción a StackOps Cirrusflex
1. Contenidos: Conceptos previos
1. Ejercicio: Trabajo con claves ssh
 * Explicación de cómo funciona la autentificación ssh con claves ssh
 * Crear un par de claves con frase de paso y utilizar ssh-add
 * Putty?
1. Ejercicio: Pasos previos
 * Exportar la clave pública a Cirrusflex
 * Crear una clave en Cirrusflex y guardar la clave privada
 * Introducción a los grupos de seguridad
 * Introducción a la gestión de IP flotantes
1. Ejercicio: Crear una instancia desde una imagen Linux y acceder desde fuera
 * Acceso con clave ssh, indicar que una vez que se ha accedido se pueden dar contraseñas a los usuarios y acceder con ellas, aunque es mejor acostumbrarse a utilizar claves RSA y aún mejor si tienen frase de paso.
 * Mientras hacemos la instancia Windows actualizamos los paquetes 
1. Ejercicio: Crear una instancia desde una imagen Windows y acceder desde fuera
1. Ejercicio: Instalación de Wordpress. Crear dos instancias, montar en una una BBDD y en la otra el servidor web. Abrir sólo el servidor web.
 * Utilizar dos grupos de seguridad, una para cada instancia y abrir sólo los puertos necesarios para cada uno.
 * Acceso a la instancia de BD desde la instancia del servidor web
1. Ejercicio: Operaciones sobre la instancia
1. Ejercicio: Levantar una instancia en jupiter para enseñar Horizon y utilizarla luego para ver OpenStack por dentro
1. Contenidos: Administración de imágenes.[http://docs.openstack.org/image-guide/content/ch_preface.html](http://docs.openstack.org/image-guide/content/ch_preface.html)
 * Explicar lo que es una imagen
 * Dónde se pueden obtener
 * Implicaciones de utilizarlas desde un punto de vista de seguridad
1. Ejercicio: Subir una imagen de Debian Jessie stable
1. Hacer un despliegue de un cluster CoreOS: [https://www.stackops.com/en/coreos-openstack/](https://www.stackops.com/en/coreos-openstack/)
1. OpenStack por dentro 1: Proceso de instanciación con KVM/Qemu
 * Hipervisores disponibles - ![https://blog.xenproject.org/wp-content/uploads/2015/05/NovaCILoopMay2015.png](https://blog.xenproject.org/wp-content/uploads/2015/05/NovaCILoopMay2015.png)
 * Imágenes base
 * Planificador
 * Discos de las instancias
 * Definición de las instancias en un nodo (virsh)
 * OpenStack metadata
1. Ejercicio: 
 * Lanzar una instancia con la imagen de debian jessie
1. Ejercicio: Instantáneas
 * Explicación de lo que es una instantánea y los tipos que hay
 * Instalar alguna aplicación más en la instancia de jessie
 * Actualizar
 * Crear una instantánea de la instancia de debian jessie
 * Crear una o varias nuevas instancias a partir de la instantánea con otro sabor
1. Ejercicio: Modificar el control de acceso de una instantánea dando acceso a todos los proyectos del curso
1. Contenidos: Conceptos previos de volúmenes
1. Redimensión
 * Explicar lo que es la redimensión (escalado vertical) y explicar por qué no se reduce el sistema de ficheros
 * Ejercicio: Redimensionar una instancia (escalado vertical) hacia arriba y hacia abajo
 * Explicar que al utilizar un sabor más pequeño el disco no se reduce
1. Ejercicio: Copias de seguridad (instantáneas programadas)
1. Ejercicio: Rescate de instancias
 * Borrar el archivo authorized_keys, no podemos acceder a la instancia.
 * Recuperar la instancia y crear un nuevo fichero authorized_keys
1. Ejercicio: Crear un volumen y asociación a una instancia
 * Formateo y particionado en XFS. Instalar xfsprogs
 * Formateo y particionado en NTFS
 * Desasociar el volumen NTFS y asociarlo a una instancia windows
 * Desasociar el volumen XFS y asociarlo a una instancia linux
1. Ejercicio: Puntos de montaje permanentes y montaje en el arranque definiendo el fstab
1. Ejercicio: Crear una instancia con el sistema raiz en un volumen
 * Terminar la instancia e instanciar una nueva
1. Ejercicio: Crear una nueva imagen desde un volumen con sistema operativo
1. Ejercicio: Instalación de owncloud
1. Contenidos: Conceptos previos de redes
1. Ejercicio: Estudiar la configuración de la red por defecto de nuestro proyecto
 * Ver la red y subred definidas
 * Ver el router que tiene nuestro proyecto
 * Ver los puertos
1. Ejercicio 1 de red: dos redes privadas con dos routers:
 * Creación de dos redes internas y sus subredes
 * Creación de dos routers conectandos a la red externa
 * Creación de dos instancias en cada una de lass redes
 * Asignación de ip flotantes
 * Comprobación de que no hay conectividad entre las instancias usando las ip fijas.
1. Ejercicio: Eliminación de la infraestructura de red creada

1. Ejercicio 2 de red: dos redes privadas conectadas a un sólo router.
1. Ejercicio: Instalador de un DNS local

1. Contenido: Concepto previo de CLI
1. Ejercicio: Instalación de los clientes
1. Ejercicio: Gestión de instancias con nova
1. Ejercicio: Gestión de volúmenes con nova y cinder
1. Ejercicio: Gestión de redes con neutron
1. Ejercicio: Gestión de imágenes con glance
1. Contenidos: Cinder por dentro:
 * [Cinder support matrix](https://wiki.openstack.org/wiki/CinderSupportMatrix)
 * Funcionamiento de LVM + iSCSI
1. Contenido: Introducción a la virtualización de redes
1. Contenidos: Neutron por dentro
<hr/>
####Sesión 7
1. Ejercicio: Ejercicio avanzado con redes: Dos redes internas conectar por un router intermedio
 * Creación de la red y el router
 * Añadir una nueva interfaz al router
 * Añadir las rutas de encaminamiento
 * Creación de instancias en las redes
 * Asignación de IP flotante a la segunda instancia
 * Accediendo a la segunda instancia
 * Añadir reglas de encaminamiento al router
1. Ejercicio: Utilizar una máquina Linux como router
1. Ejercicio: Instancias con varias interfaces de red
1. Ejercicio: Balanceador de carga
 * Explicar lo que es un balanceador de carga y la implementación en OpenStack
1. Ejercicio: Creación de un servidor VPN
1. Balanceador con CLI
1. Conceptos: Almacenamiento de objetos
1. Ejercicio: Almacenamiento privado
1. Ejercicio: Almacenamiento público 
<hr/>
####Sesión 8

<hr/>
####Sesión 9
1. Aprovisionamiento automático vs orquestación
 * Configurar automáticamente una instancia: ansible, puppet, chef, ...
 * Montar automáticamente un escenario (aprovisionamiento): heat, shell, ansible, puppet, ...
 * Gestionar un escenario dinámico y configurar cada nodo (orquestación)
1. Ejercicios:
 * Creación de un entorno con bash paso a paso
 * Mostrar el ejemplo demo.sh
 * Mostrar el demo-inv.sh
1. Ejercicios:
 * Python
1. Ejercicio de ansible
1. Repaso de OpenStack. Arquitectura
1. Uso de OpenStack
1. Modos de instalación




