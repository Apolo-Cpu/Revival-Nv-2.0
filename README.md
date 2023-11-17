# Revival-Nv-2.0 By:
![Nexus azul](https://github.com/Apolo-Cpu/Revival-Nv-2.0/assets/131043287/5292bca0-c31a-4684-9677-e68bb6230ad2)

Lo que encontrarás aquí es un conjunto de varias versiones de un mismo programa. Sin embargo, las versiones más recomendadas para su uso son las 1.7 y 1.8. Las diferencias más notables entre ellas se centran principalmente en el diseño de la interfaz. Hemos procurado no realizar cambios significativos en su funcionamiento para permitir la creación de versiones personalizadas. A continuación, basaré la explicación en la versión 1.8.

# Revival 1.8:
**Inicio de Sesion**

![image](https://github.com/Apolo-Cpu/Revival-Nv-2.0/assets/131043287/2fcf5577-531d-4543-b019-081891d484b1)
El proyecto incluye un sistema de inicio de sesión basado en el nombre de usuario, el tipo de usuario y la contraseña. La verificación de estos datos se realiza utilizando información incorporada en el código del formulario. Si decides implementar una validación adicional, ten en cuenta que el resto del programa ajusta sus opciones según los nombres y tipos de usuario proporcionados durante el inicio de sesión. Se sugiere considerar esto cuidadosamente para mantener la coherencia en el funcionamiento del programa.

# Pendulo Invertido
**Idea de Funcionamiento**

**Importante**
La idea principal es lograr que el sistema se mantenga por sí mismo una vez se hayan encontrado los valores ideales. Es importante destacar que los valores ideales pueden variar entre diferentes casos, por lo que se sugiere comenzar colocando todos los valores en cero e ir ajustándolos hasta encontrar estabilidad.

En mi experiencia, recomendaría iniciar variando los valores de Kp. Una vez que hayas identificado un rango en el que te sientas cómodo, es decir, donde el sistema oscile en un punto deseado, puedes comenzar a modular Kd. Ajusta este valor hasta lograr cambios relativamente rápidos.

Determinar el valor de Ki puede ser más desafiante. En algunos proyectos, se deja en cero, pero se sugiere encontrar este valor por cuenta propia. Cada variable cumple una función específica en este proyecto, o al menos así es como lo he entendido:

* **Kp:** Actúa en el presente para aplicar una corrección proporcional al error actual, como intentar corregir la posición de un péndulo en el instante presente.

* **Kd:** Se encarga de prever y contrarrestar el comportamiento futuro del sistema al analizar la tasa de cambio del error. En el ejemplo del péndulo, Kd se aplicaría para anticipar el movimiento futuro del péndulo analizando la velocidad con la que está cambiando la posición.

* **Ki:** Corrige acumulativamente el error pasado en el sistema. Tomando el ejemplo del péndulo, Ki se aplicaría para aprender de los errores acumulados en el pasado y realizar correcciones más suaves y a largo plazo, amortiguando las oscilaciones.

![pendulo_invertido_funcionando1](https://github.com/Apolo-Cpu/Revival-Nv-2.0/assets/131043287/ae12c2d0-28a5-4848-9c0d-b28570c3ebd1)


![image](https://github.com/Apolo-Cpu/Revival-Nv-2.0/assets/131043287/12160930-b688-4535-bc95-492c8d57592c)

El robot es capaz de funcionar de manera autónoma e independiente, sin depender de conexiones externas o controladores adicionales para realizar sus tareas. Puede mantener el equilibrio del péndulo y ejecutar sus funciones sin la necesidad constante de intervención externa.

![image](https://github.com/Apolo-Cpu/Revival-Nv-2.0/assets/131043287/6348a38d-31ae-4bda-870e-e405297ff0f7)

Variables identificadas y lectura entre estas

![image](https://github.com/Apolo-Cpu/Revival-Nv-2.0/assets/131043287/085aa4a4-c37d-4ddd-8e2d-9e9142eac367)




# Posibles Preguntas ¿?

* ¿Que es esto?

Este proyecto es un programa desarrollado en visual studio .net de nombre clave  "Revival Nv" que Permite a distintos tipos de usuarios ejercer control sobre  funciones y variables específicas para el control y monitoreo de un robot tipo Pendulo Invertido

* ¿Robot tipo Pendulo invertido?

Un robot de péndulo invertido es como un carrito con una vara vertical en la parte superior y un péndulo en el extremo. La tarea del robot es mantener esa vara en posición vertical, incluso cuando el carrito se mueve. Este tipo de robots son utilizados para aprender sobre cómo controlar sistemas y mantener el equilibrio

* ¿Que puedo hacer con este programa?

En resumen este proyecto nos permite:

1. Conectarnos a un esp32 por medio de bluetooth
2. Visualisar en forma de grafica un registro de los ultimos 10/20 grados registrados por el sensor
3. Cambiar las constantes correspondientes a Kp, Ki y Kd para realizar un ajuste rápido sin necesidad de modificar el código en Arduino.
4. Dar órdenes de movimiento manual, como moverse hacia adelante o girar en un sentido.
5. Examinar la respuesta del sistema, incluyendo valores proporcional, integral, derivativo y PID, representados en gráficas.

   
* No puedo compilar el programa, ¿qué puedo hacer?

1. Verifica las bibliotecas que tienes tanto en Arduino como en Visual Studio .NET.
2. Las versiones que he subido a este repositorio y de las que estoy seguro que deberían funcionar en cualquier equipo son la 1.7 y la 1.8, sin embargo, te recomiendo revisar el archivo llamado 'Version Actualizacion.txt' para descartar posibles fallos por nuevas implementaciones o cambios.

* "No logro establecer la conexión Bluetooth. ¿Qué debo hacer?

1. Verifica el nombre de tu dispositivo.
2. Asegúrate de tener los controladores de Bluetooth actualizados
3. Revisa a qué puerto se está conectando el dispositivo. En mi caso, al interactuar con una ESP y Windows, deberías ver dos puertos COM (por ejemplo, COM4 y COM5). En algunas ocasiones, la conexión puede ser más estable en uno de los dos puertos.
4. Confirma que el equipo esté correctamente vinculado al dispositivo. Si tienes problemas a pesar de la vinculación, te sugiero desinstalar el dispositivo desde el 'Administrador de dispositivos', desvincularlo y luego volver a vincularlo a través del menú de Bluetooth en el dispositivo."
