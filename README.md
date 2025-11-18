# Resumen del sistema Agenda personal de citas
## Descripcion del caso

El sistema de Agenda personal de citas es una aplicación diseñada para apoyar al usuario en la organización de sus actividades diarias. Su finalidad es ofrecer una herramienta práctica que permita gestionar compromisos, ordenar el tiempo y evitar cruces entre horarios. Con esta agenda, el usuario puede llevar un control preciso de sus citas y recibir recordatorios que faciliten el cumplimiento de sus responsabilidades.



## Objetivos del sistema

Los objetivos del sistema se enfocan en garantizar que la aplicación cumpla su propósito principal: facilitar la gestión de citas de manera ordenada y eficiente. Para lograrlo, se establecen dos grupos de objetivos:

 Los objetivos del sistema: 
  
  * Lo que el sistema **"Debe hacer"** (RF)
     Corresponden a las acciones concretas que el usuario podrá realizar dentro del sistema. Estos objetivos se centran en ofrecer herramientas útiles para registrar, visualizar y administrar sus citas de forma sencilla.
  * Las **"caracteristicas"** que debe cumplir (RNF)
     Describen las cualidades y condiciones que el sistema debe cumplir para asegurar una experiencia estable, rápida y segura. Incluyen aspectos como rendimiento, compatibilidad, facilidad de uso y protección de la información.



## Requerimientos

### Requerimientos funcionales  (RF)
* **RF1 – Registro de nuevas citas con aviso anticipado:** El sistema debe permitir al usuario crear una cita y seleccionar cuánto tiempo antes desea recibir una alerta previa.
* **RF2 – Organización de citas mediante etiquetas:** El sistema debe permitir asignar etiquetas o categorías personalizables que faciliten la clasificación y búsqueda de las citas.
* **RF3 – Visualización del calendario en diferentes formatos:** El usuario debe poder consultar sus citas utilizando vistas de calendario como semanal o mensual para una mejor planificación.
* **RF4 – Generación de reportes en PDF:** El sistema debe ofrecer la opción de exportar las citas seleccionadas en un documento PDF según el intervalo de fechas elegido.



### Requerimientos no funcionales (RNF)
* **RNF1 – Funcionamiento en distintas plataformas:** La aplicación debe ser compatible tanto con dispositivos móviles como con equipos de escritorio sin perder funcionalidad.
* **RNF2 – Protección de la información almacenada:** El sistema debe mantener las citas resguardadas mediante un mecanismo de cifrado o seguridad básica que evite accesos no autorizados.
* **RNF3 – Eficiencia en la carga de información:** La aplicación debe mostrar la vista mensual del calendario en un tiempo inferior a 2 segundos, incluso cuando haya un número elevado de citas registradas.


## Casos de prueba (Sin tabla)

* **CP1**

 *Tipo: Unitario
 *Requerimiento: RF1
 *Datos: Usuario ingresa la fecha y la hora de la cita
 *Resutado esperado: La cita queda registrada y se programa un aviso previo
 *Resultado obtenido: La cita se creó correctamente y se configuró una alerta automática


* **CP3**

 *Tipo: Unitario
 *Requerimiento: RF2
 *Datos: Categoría ingresada: “Revisión médica"
 *Resutado esperado: La cita debe mostrarse con la etiqueta correspondiente a la categoría seleccionada
 *Resultado obtenido: La cita se visualiza con un color distintivo asignado a la categoría


* **CP4**

 *Tipo: Validacion
 *Requerimiento: RNF2
 *Datos: Usuario escribe sus credenciales (usuario y contraseña)
 *Resutado esperado: El sistema debe validar la información y permitir el acceso
 *Resultado obtenido: Las credenciales fueron aceptadas y se ingresó al sistema sin inconvenientes


* **CP5**

 *Tipo: Validacion
 *Requerimiento: RF5
 *Datos: El usuario selecciona un intervalo de fechas para exportar
 *Resutado esperado: Se debe generar un archivo PDF con las citas dentro del rango indicado
 *Resultado obtenido: Se generó correctamente un PDF con las citas seleccionadas



## Tipos de propuesta de mantenimiento 

* **Problema:** El sistema presenta fallos ocasionales al momento de sincronizar las citas entre dispositivos, lo que provoca que algunas actualizaciones no se reflejen correctamente.
 
 
  * **Tipo de Mantenimiento:** Mantenimiento correctivo
  * **Accion:** Revisar y reparar el módulo de sincronización, ajustando el manejo de datos en tiempo real y corrigiendo errores en la transferencia de información.
  * **Justificacion:** Es necesario solucionar estos fallos para evitar pérdidas de información y asegurar que las citas estén actualizadas en todos los dispositivos del usuario.


* **Problema:** La aplicación no ofrece opciones avanzadas de filtrado para buscar citas antiguas, lo que dificulta al usuario encontrar información específica rápidamente.
  

 
  * **Tipo de Mantenimiento:** Mantenimiento Perfectivo
  * **Accion:** Implementar nuevos filtros como búsqueda por palabra clave, categoría, estado de la cita y fecha exacta.
  * **Justificacion:** Estas mejoras incrementan la usabilidad y permiten acceder a la información de manera más eficiente, optimizando la experiencia del usuario.


## Reflexion sobre el control de versiones 

El control de versiones es una herramienta esencial para garantizar la evolución organizada del sistema. Permite conservar un registro completo de todos los cambios realizados, identificar mejoras, rastrear errores y restaurar versiones anteriores sin pérdida de información.

Publicar el proyecto en GitHub ofrece ventajas adicionales: respalda el código en un entorno seguro, facilita la colaboración, permite experimentar con nuevas funciones mediante ramas y asegura que cada actualización quede documentada de forma clara y accesible. Esta práctica ayuda a mantener la calidad del sistema y su crecimiento a largo plazo.

  
