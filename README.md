
![logo](https://www.ochobitshacenunbyte.com/wp-content/uploads/2016/10/Puppet-image-mini.jpg)



<center> 

**FACULTAD DE INGENIERÍA**

**PROGRAMA:**

INGENIERÍA DE SISTEMAS

**ASIGNATURA:**

SISTEMAS DISTRIBUIDOS

**9no SEMESTRE**

**DOCENTE:**

RONALD CUELLO MEZA

**INTEGRANTES:**


MARIN HOYOS RICARDO

MAY ALEMAN JASON

TUIRAN CONEO SANTIAGO

VILLAMIZAR MUNIVES DIEGO


**CARTAGENA/BOLÍVAR
2022** </center>


# **Puppet** 
Puppet puede administrar numerosos servidores, especificar la infraestructura como código y hacer cumplir la configuración del sistema. Y hay mucho más.

Puppet es una herramienta fantástica de DevOps para administrar una gran cantidad de servidores.

Los administradores de sistemas solían ejecutar los servidores usando scripts de shell. Todavía se usa, aunque el enfoque es ineficiente. Incluso el administrador de sistemas más capacitado está demasiado preocupado por modificar los scripts de cientos o miles de servidores y configuraciones de sistemas que cambian continuamente.

![logo](https://upload.wikimedia.org/wikipedia/commons/3/34/140228puppetrunExampleManuallyInvokedPackageUpdate.png)

Al automatizar la configuración del servidor, la instalación del programa y la administración del sistema, las aplicaciones DevOps pueden superar este problema. Puppet es una de las aplicaciones más importantes.

Según la encuesta de tendencias DevOps de RightScale de 2016, Puppet y Chef son los programas DevOps más utilizados. Puppet es utilizado por el 42 % de las empresas que utilizan enfoques DevOps, seguido de cerca por Chef (37 %).


Puppet es una herramienta de implementación y gestión de configuración de software de código abierto. Por lo general, se usa en Linux y Windows para mover simultáneamente los hilos en diferentes servidores de aplicaciones. Sin embargo, Puppet se puede usar en una variedad de sistemas, incluidos los mainframes de IBM, los enrutadores de Cisco y los servidores de Mac OS.

||Informacion General       |
|-------------|-------------|
| Autor       | Puppet Labs |
| Lanzamiento | 2005        |
| programado  | Ruby        |
| Sitio web oficial  | [Puppet.com](https://puppet.com/)       |
| Repositorio de codigo  | [codigo](https://github.com/puppetlabs/puppet)         |


Por ejemplo, no tienes que indicar a Puppet que necesitas que en esa máquina esté Maven, y por ser una máquina Linux  el comando para instalar Maven es X. Solo tienes indicar que necesitas que Maven esté instalado, y Puppet mirará bajo qué sistema operativo está ejecutándose y actuará en consecuencia.
Aquí tienes un ejemplo en el que indicamos a Puppet que queremos tener instalada la versión 3.0.4-2 del paquete de Maven:

![logo](https://www.javiergarzas.com/wp-content/uploads/2014/05/site-300x89.png)


## **Operación de Puppet**

Puppet le permite especificar el software y la configuración que requiere un sistema y luego conservar ese estado después de la configuración inicial.

Para definir los parámetros de configuración para un entorno o una infraestructura determinados, utiliza un lenguaje específico de dominio (DSL) declarativo comparable a Ruby. Puppet aprende acerca de un sistema usando Facter, una utilidad que se carga cuando instala el paquete de software de Puppet. Consulte Uso de Facter para recopilar información del sistema.

Puppet máster es el sistema que maneja información de configuración crítica para todos los nodos bajo su control a través de manifiestos. Echa un vistazo a los manifiestos de marionetas.

El maestro controla los nodos que tienen Puppet instalado y ejecutan el agente de Puppet, que es un demonio. El agente envía la información de configuración que obtiene sobre un nodo al maestro de Puppet. El Puppet máster luego crea un catálogo dependiendo de la configuración del nodo. Esa información es utilizada por cada nodo para aplicar las actualizaciones de configuración necesarias a sí mismo.

Puppet opera en un modo de extracción, con agentes que sondean al maestro a intervalos regulares para recibir configuraciones específicas del sitio y del nodo. La aplicación del agente Puppet a menudo se ejecuta como un servicio en segundo plano en nodos controlados en este sistema. Se pueden encontrar más detalles en Descripción general de la arquitectura de Puppet.

![logo](https://static.packt-cdn.com/products/9781783981427/graphics/1427OS_02_03.jpg)


## **¿Qué es exactamente Puppet en DevOps?**

Puppet es una herramienta de gestión de sistemas que ayuda en la automatización y centralización de la gestión de la configuración. También se utiliza para implementar software. Viene en versiones comerciales y de código abierto.

Ayuda en la administración de la configuración del servidor, las implementaciones del servidor y la orquestación de numerosas aplicaciones en toda la vasta infraestructura de la organización.

Suponga que tiene 100 servidores que deben mantenerse, administrarse y configurarse manualmente. Puppet hace lo siguiente:

*  Puppet nos permite hacer configuraciones separadas para cada host
*  Supervisa continuamente el servidor en busca de configuraciones y, si las configuraciones se modifican, cambia automáticamente a una configuración predefinida en los hosts.
*  Tiene control sobre mucha infraestructura para que las configuraciones centralizadas se efectúen en cada una de las infraestructuras
*  También se utiliza como herramienta de implementación automática para todas las aplicaciones en los servidores. 
*  Implementa Infraestructura como Código, las políticas y configuraciones se escriben como código.



Puppet define los atributos de configuración para la infraestructura o el entorno especializado utilizando el lenguaje específico de dominio (DSL) declarativo. Busca información sobre los sistemas utilizando un programa llamado facter. Para gobernar y administrar los nodos con información de configuración, el puppet máster utiliza un método conocido como manifiestos. Este tambien controla los nodos, que no son más que servidores o infraestructura con un agente de Puppet o aplicación instalada.

Hay 5 pasos, en los que la infraestructura es administrada y controlada por Puppet Máster y Puppet Agents,

1. El nodo que ejecuta los agentes puppets mandan solicitud a el maestro y utilizan la información de extracción. Usando los hechos, el nodo recopila información sobre sí mismo.
2. El agente envía estos detalles al puppet.
3. El puppet crea un catálogo que describe cómo se debe configurar el nodo.
4. El catálogo es enviado al agente por el maestro.
5. El agente se configura y se comunica con el maestro.


