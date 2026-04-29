# MARZO

## Semana 2 - 6 de marzo

Durante esta semana añadí la lógica para bloquear vehículos cuando se inicia un parte, y cambiar su estado cuando se pausa o se finaliza. Esto era importante para evitar conflictos y tener un control más realista del uso de los vehículos.

También implementé el sistema de bajas programadas. Para esto tuve que crear una nueva tabla específica que facilitara el cambio de estados y permitiera mostrar las bajas en una tabla de forma clara.

Además, desarrollé una función asíncrona que, a una hora concreta, crea automáticamente el parte asociado a la baja y la marca como procesada. Fue una tarea interesante porque implicaba automatizar procesos dentro del sistema.

---

## Semana 9 - 13 de marzo

Esta semana creé un usuario de prueba para la parte de inventarios, con el objetivo de poder hacer pruebas y entender mejor cómo funciona todo antes de implementarlo.

Durante estas pruebas me di cuenta de que la información de Sage relacionada con la empresa de prueba no se estaba traspasando correctamente. Por eso, revisé los scripts y los modifiqué para que también tuvieran en cuenta esta empresa.

Además, también resolví algunas incidencias que surgieron en RHP.

---

## Semana 16 - 20 de marzo

Durante esta semana seguí investigando el funcionamiento del sistema en la parte de inventario y artículos. Me centré en cómo se gestionan los consumos, y detecté un problema: al hacer un consumo, el stock del artículo volvía a su valor inicial al cabo de un rato.

Para solucionarlo, tuve que revisar varios scripts hasta encontrar cuál estaba fallando. Finalmente conseguí arreglarlo, y además este proceso me ayudó a entender mejor cómo funcionan internamente estos scripts, lo que me será útil para futuras tareas.

También implementé todo lo relacionado con la imputación de artículos en los partes y empecé a estructurar las tablas y controladores necesarios para el sistema de inventarios.

---

## Semana 23 - 27 de marzo

Esta semana terminé la sección de inventarios, completando su funcionalidad principal.

También añadí una mejora visual para resaltar los partes de tipo “serie X” que tienen albarán asociado, facilitando su identificación.

Por otro lado, estuve investigando cómo funcionan los partes precerrados y acabé implementando esta funcionalidad en el sistema.

En la parte de base de datos, añadí modificaciones en funciones de SQL Server para trabajar con una empresa específica (3001) y con una nueva base de datos del programa, con el objetivo de hacer las pruebas finales.

Durante estas pruebas surgieron algunos problemas, ya que en la nueva base de datos algunas tablas no tenían autoincremento en los ID. Esto se había hecho así para facilitar la migración de datos, ya que muchas tablas dependen de otros ID.

Finalmente, volví a crear las tablas con autoincremento para poder trabajar correctamente.

Por último, intenté publicar la aplicación en el IIS de la empresa, pero no fue posible porque no soporta la versión de .NET con la que está desarrollado el programa.
