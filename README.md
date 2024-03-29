Proyecto Final
-----------------------

1. Crear Script a partir de documento de Test Cases y la coleccion de postman facilitada en la carpeta [material](https://github.com/angeleliseo/perf1/tree/main/material) de este repositorio.
* Nota: Usar mecanismo de grabacion por jmeter proxy o creacion manual del script (Sampler por sampler)
2. Crear un ThreadGroup por Test Case.
3. Aplicar las mejores practicas en uso de Naming Conventions, Creacion de transacciones, uso de assertions, Parametrizacion y Correlacion.
4. Utilizar el UltimateThreadGroup plugin para configurar un escenario de LoadTest, con un steady state de 30 minutos y obtener un baseline de la aplicacion para una carga de:
	- 24 TPM (transacciones por minuto) para GET /people
	- 12 TPM para POST /people
	- 12 TPM para GET /people/{person_id}
	- 12 TPM para DELETE /people/{person_id}
	- 8 TPM para PATCH /people/{person_id}
* Nota: Se debera de dejar un ThinkTime (Timer) al final de cada transaccion para emular de forma mas realista el comportamiento humano. 
5. Utilizar el UltimateThreadGroup plugin para configurar un escenario de Estress que ayude a entender la escalabilidad de la aplicacion. Usando como punto de partida su Baseline de su ejecucion anterior e incrementar a 2X, 3X y 4X, con periodos de steady state de 10 minutos.
6. Usar Listeners de Active Threads, Response Time, Transactions per second y HTTP codes per second y tomar evidencias durante la ejecucion de carga (1x) usando el GUI de JMeter (imagenes o screenshots)
7. El escenario de Estress debera de ser ejecutado en modo consola (tomar evidencias en capturas de pantalla)
8. Generar un reporte HTML de la prueba de estres usando el archivo *.jtl obtenido de la ejecucion en consola.
### **Entregables que se revisaran:**
* Script Funcional con mejores practicas configurado para prueba de carga
* Script Funcional con mejores practicas configurado para prueba de estres
* Calculo de carga para escenario de carga y de estres.
* Capturas de pantalla durante la ejecucion de prueba de carga usando los Listeners mencionados en el proyecto final.
* Capturas de la ejecucion modo consola
* Archivo resultante de la ejecucion por linea de comandos *.jtl
* Reporte en formato HTML (en zip)


**Nota**: Actualizacion. No sera necesario incluir la parte de monitoreo del lado del servidor con Grafana o NMon para la entrega del proyecto final.

**Fecha limite de entrega: 24 de Noviembre 11:59PM**
