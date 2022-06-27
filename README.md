# RECURSOS DE COMPUTO EN AZURE
## SESIÓN 4 PRÁCTICA 2
En esta práctica aprenderemos a crar una máquina virtual y abrir una máquina virtual dentro de otra.

**Requisitos**
* Iniciar sesión en el portal de Azure
* Crear dos máquinas virtuales

------------------------------------------

### ¿Cómo crear una máquina virtual en Azure?
Para crear una máquina virtual en Azure, nos dirigimos a nuestro portal Azure y en la primera ventana nos mostrara la opción "Máquinas Virtuales" o en el apartado de busqueda podemos escribir 
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/1portalazure.png)

Damos clic en "+ crear" y seleccionamos la opción "Maquina virtual de Azure"
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/2crear.png)

Crearemos un nuevo recurso para esta práctica que se llame "sesion4"
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/3crearrecurso.png)

En el apartado detalles de instancia, llenaremos los siguientes rubros:
* Nombre de máquina virtual: elegimos como queremos que se llame nuestra máquina virtual
* Región: elegimos donde queremos que se hospede nuestra máquina virtual

![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/4instancias.png)

Mientras que en el apartado de cuentas del administrador creamos un nuevo usuario con su contraseña. De igual corroboramos que en el rubro para seleccionar el puerto de entrada tenga seleccionado "RDP"
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/5admin.png)

El apartado de redes y todo los demás los dejamos igual. 

Ahora nos dirigimos a  "Revisar y crear" y damos clic en el botón "Crear" 
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/7crear.png) 

Y esperamos a que se cree la implementación.
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/8secreo.png)

-------------------------------

### Creación de nuestra segunda máquina virtual 
Para crear nuestra segunda máquina virtual vamos a seguir los mismos pasos que en el apartado anterior, inclusive vamos a elegir el mismos grupo de recursos que creamos anteriormente. Lo único que va a cambiar seria el nombre de la máquina virtual y posiblemente la región. 
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/9otramaquina.png)

Una vez completados los datos básicos y haber dejado todo lo demás igual. Nos dirigimos al apartado "Revisar y Crear" y damos clic en el botón "Crear"
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/12otracreada.png)

Y esperamos a que termine la implementación.
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/13listorecurso.png)

**Nota**
Si entramos a nuestro grupo de recursos llamado "sesion4" podemos visualizar todos los recursos que se nos crearon aparte de las máquinas virtuales.
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/14datos.png)

---------------------------------------------

### Conexión entre máquinas virtuales
Para seguir con nuestra conexión entre máquinas, es necesario entrar a nuestra primera máquina virtual al apartado de "Conectar" damos clic en la opción "RDP"
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/15conectar.png)

Damos clci en el botón "Descargar archivo RDP"
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/16rdp.png)

Nos dirigimos al "explorador de archivos" en nuestro equipo de computo, luego "descargas" --> "abrir con" -->Conexión a Escritorio remoto
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/17conexion.png)

* Posteriormente nos pedira que le demos clic en continuar, puede que tarde un poco en conectar, ya que, depende de la región que hayamos elegido. 
* Una vez establecida la conexión, nos pedira que iniciemos sesión, los datos serán aquellos que establecimos en la creación de nuestra máquina virtual.
* Si los datos son correctos nuestra máquina virtual iniciara. 
Realizamos ping a nuestra segunda virtual de manera local. 
* Si se logra correctamente el ping se procede a conectar a la segunda virtual por escritorio remoto.

**¡Listo hemos logrados conectar dos máquinas virtuales, una dentro de otra!** 
![](https://github.com/JohannaJBalderas/S4-practica2/blob/main/images/maquinasobremaquina.png)
