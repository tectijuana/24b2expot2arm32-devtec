

# 1. Introducción a ARM32 y el entorno de desarrollo


![image](https://github.com/tectijuana/24b2expot2arm32-devtec/assets/158236387/83eb166e-dd3a-4b64-8071-6ead5fbae68b)




------

<pre>

	<p align=center>

Tecnológico Nacional de México
Instituto Tecnológico de Tijuana

Departamento de Sistemas y Computación
Ingeniería en Sistemas Computacionales

Semestre:
Febrero - Junio 2022

Materia:
Lenguajes de interfaz

Docente:
M.C. Rene Solis Reyes 

Unidad:
1

Título del trabajo:
Introducción a ARM32 y el entorno de desarrollo

Estudiante:
Juan Flores Fernandez
ROSY SALAZAR
Saul Perez
Adrian Valdes Cansino
Angel Gabriel Quiñones Agramon

	</p>

</pre>

<pre>

	<p align=center>
		Historia de ARM

	<p align=left>


ARM, que significa "Advanced RISC Machine", es una arquitectura de procesador desarrollada por ARM Holdings.
La historia de ARM se remonta a la década de 1980, cuando Acorn Computers Ltd. buscaba un diseño de CPU para su nueva computadora, 
el Acorn Archimedes. En lugar de desarrollar su propia arquitectura, Acorn se asoció con VLSI Technology
y fundó ARM Ltd. en 1990 para desarrollar una arquitectura de bajo consumo y alto rendimiento.

		
En la imagen de a continuacion muestra la evolución de los microprocesadores desde 1971 hasta 2001. 
Se pueden observar varios cambios importantes a lo largo de las generaciones:
		
Aumento del número de transistores: Más transistores significan mayor velocidad, potencia y eficiencia.

Reducción del tamaño: Los dispositivos electrónicos son más pequeños y portátiles.

Aumento de la velocidad de reloj: Las tareas se ejecutan más rápido.

Nuevos conjuntos de instrucciones: Mayor capacidad para ejecutar tareas.

Arquitectura multi-núcleo: Mayor eficiencia y potencia.

Integración de otros componentes: Mayor eficiencia y compacidad.

Otros cambios: Introducción de la arquitectura x86, desarrollo de procesadores de 16 bits y 32 bits, aparición de nuevos competidores.

	</pre>
![image](https://github.com/tectijuana/24b2expot2arm32-devtec/assets/158236387/b4a69915-d551-4133-95fe-4d34652827f0)



<pre>
	<p align=center>
		Arquitectura

	<p align=left>

	Se realiza manipulación manual de pila
	Solo hay 25 tipos de instrucciones básicas
	Cada instrucción tiene sus propias condiciones con registros

	Ventajas.

		Son mas baratos en comparacion a otros procesadores.
		Mas eficientes energeticamente.
		Funciona mas rapido porque realiza una operacion a la vez

		
	Desventajas

		Windows no esta bien optimizado porque no es compatible binariamente con x86
		La velocidad y banda ancha de la memoria son limitados por las frecuencias de reloj del procesador
		Es mas complicado de debugear por la secuencia de instrucciones
		El desempeño depende totalmente de la ejecucion, asi que si el usuario no lo ejecuta correctamente
		puede tomar mucho tiempo para trabajar correctamente
		

</pre>

</pre>

<pre>
	<p align=left>
	Configuración del entorno de desarrollo en Raspberry Pi.
	<p align=center>
	1. Actualizar el sistema operativo
	<p align=left>
	Es importante comenzar actualizando el sistema operativo de tu Raspberry Pi a la última versión. 
	Esto te asegurará tener las últimas correcciones de errores y seguridad, 
	así como las últimas versiones de las herramientas de desarrollo.

	Codigo:
		sudo apt update
		sudo apt upgrade

	<p align=center>
	2. Instalar herramientas de desarrollo
	<p align=left>
	A continuación, instalar las herramientas de desarrollo esenciales, 
	como el compilador GCC para ARM, el comando make y el depurador GDB.

	Codigo:
		sudo apt install gcc-arm-linux-gnueabihf
		sudo apt install make
		sudo apt install gdb

	<p align=center>
	3. Configurar el entorno de desarrollo
	<p align=left>
	Ahora se podra configurar el entorno de desarrollo.
	
	3.1. Configurar el path

	Edita el archivo ~/.bashrc y agrega la siguiente línea al final:
		export PATH=$PATH:$HOME/bin
	Esto te permitirá ejecutar comandos desde tu directorio personal sin tener que escribir la ruta completa.

	3.2. Configurar el editor de código.

	Elige un editor de código que te guste, como nano, vim o Visual Studio Code. 
	Si usas nano, puedes configurarlo para que resalte la sintaxis del código C/C++ 
	agregando la siguiente línea al archivo ~/.nanorc:
		set syntax=c
</pre>	
	
