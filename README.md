# Revival-Nv-2.0 By:
![Nexus azul](https://github.com/Apolo-Cpu/Revival-Nv-2.0/assets/131043287/5292bca0-c31a-4684-9677-e68bb6230ad2)

Lo que encontrarás aqui es un recopilatorio  de varias versiones de un mismo programa, mas sin embargo las mas recomendadas para su uso son las versiones 1.7 y 1.8, sus diferencias mas radicales serian  el diseño de la interfaz, intentamos no tocar nada respecto a su funcionamiento por si deseas realizar tu propia version/adaptacion, mas sin embargo voy a basar la explicacion por medio de la 1.8

# Posibles Preguntas ¿?

* ¿Que es esto?

Este proyecto es un programa desarrollado en visual studio .net de nombre clave  "Revival Nv" que Permite a distintos tipos de usuarios ejercer control sobre  funciones y variables específicas para el control y monitoreo de un robot tipo Pendulo Invertido

* ¿Robot tipo Pendulo invertido?

Un robot de péndulo invertido es como un carrito con una vara vertical en la parte superior y un péndulo en el extremo. La tarea del robot es mantener esa vara en posición vertical, incluso cuando el carrito se mueve. Este tipo de robots son utilizados para aprender sobre cómo controlar sistemas y mantener el equilibrio

* ¿Que puedo hacer con este programa?

En resumen este proyecto nos permite:

1. Conectarnos a un esp32 por medio de bluetooth
2. Visualisar en forma de grafica un registro de los ultimos 10/20 grados registrados por el sensor
3. Cambiar las Constantes correspondientes a Kp, Ki, & Kd para realizar un ajuste rapido sin pasar por el codigo en arduino
4. Dar orden de movimiento manual (moverse hacia adelante, girar en un sentido)
5. Examinar la respuesta del sistema (valores proporcional, integral, derivativo y PID) en forma de graficas

   
* ¿No me compila el programa, que puedo hacer?

1. Revisa que librerias tienes tanto en arduino como en visual studio .net
2. Las versiones que he subido a este recopilatorio de las que estoy seguro deberian funcionar en cualquier equipo son las 1.7 y 1.8 o final, mas sin embargo recomiendo revises el apartado llamado Version Actualizacion.txt para descartar fallos por nueva implemtacion y/o cambio





# Revival 1.8:
**Inicio de Sesion**

![image](https://github.com/Apolo-Cpu/Revival-Nv-2.0/assets/131043287/2fcf5577-531d-4543-b019-081891d484b1)
el proyecto tiene un inicio de sesion que se basa en nombre de usuario, tipo de usuario y contraseña, dicha validacion de datos está hecha con datos que se encuentran en el mismo codigo del formulario, si deseas añadir una validacion puedes hacerlo, pero ten en cuenta que el resto del programa habilita opciones por medio de dichos nombres/tipo de usuario, te recomiendo tenerlo presente

// Para una mejor comprension de que se hace en cada version, revisar archivo "Version Actualizacion.txt"

// A partir de la version 1.8 se realizan cambios visuales, si deseas netamente la version mas estable puedes utilizar la 1.7 y realizar tus adecuaciones, mas sin embargo recomendamos ver las notas en "Version Actualizacion.txt"

**Nombre del Proyecto: Revival Nv - Robot Móvil de Péndulo Invertido**


//......................................................................................................................................................................................................................................//

**Características Destacadas:**

**Control Preciso:** El corazón de este robot es un sistema de control PID digital que garantiza un equilibrio constante. Utiliza datos proporcionados por un sensor de velocidad angular y un microcontrolador Esp32 para lograr un movimiento estable y preciso.

**Interfaz Gráfica de Usuario (GUI):** Revival Nv presenta una interfaz gráfica de usuario desarrollada en Visual Studio .NET. Esto permite a los operadores monitorear y controlar el robot de manera intuitiva. La interfaz proporciona información en tiempo real y opciones de ajuste de parámetros.
**
Comunicación Inalámbrica:** Gracias a su capacidad de comunicación inalámbrica, este robot puede transmitir datos de manera eficiente entre la interfaz gráfica y el prototipo por medio de Bluetooth. Esto facilita un control ágil y la supervisión constante del estado del robot.

//......................................................................................................................................................................................................................................//


**Contribuciones Bienvenidas:**
El proyecto Revival Nv en GitHub está abierto a la colaboración de la comunidad.
Si tienes ideas para mejoras, correcciones o características adicionales, no dudes en descargarlo y usarlo de base para tu proyecto. Estamos aquí para apoyarnos mutuamente en la creación de soluciones tecnológicas innovadoras.

//......................................................................................................................................................................................................................................//

**Cómo Contribuir:**
**Descargar el Código:** Puedes comenzar descargando el código fuente de Revival Nv desde este repositorio.

**Realizar Modificaciones:** Una vez que tengas el código, siéntete libre de realizar modificaciones y mejoras de acuerdo a tus objetivos o requisitos específicos.

**Colaborar:** Si consideras que tus modificaciones pueden ser valiosas para otros usuarios, puedes colaborar con la comunidad compartiendo tus cambios a través de solicitudes de extracción (pull requests).

**Reportar Problemas:** Si encuentras problemas o errores en el proyecto, puedes reportarlos a través de las solicitudes de problemas (issues) en este repositorio.

**Documentación:** Contribuir a la documentación del proyecto también es una forma valiosa de apoyar. Puedes mejorar la documentación existente o crear nuevas guías y tutoriales.
