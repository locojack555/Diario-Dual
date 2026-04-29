# ENERO

## Semana 5 - 9 de enero

Durante esta semana hice mejoras en la gestión de usuarios. Añadí la opción de habilitar y deshabilitar usuarios, cambiando la forma en la que se guardaba en la base de datos.

Antes se hacía creando una fila con clave igual al id del usuario y valor "deshabilitado", lo cual no era muy práctico. Yo lo mejoré añadiendo una nueva columna donde 0 significa habilitado y 1 deshabilitado, haciendo el sistema más simple y eficiente.

Además, añadí una nueva funcionalidad en RHP relacionada con las vacaciones: ahora las vacaciones no disfrutadas del año anterior pasan al año actual y se pueden utilizar hasta el 15 de enero. Esto implicó tocar lógica del sistema y entender bien cómo se gestionan estos datos.

---

## Semana 12 - 16 de enero

Esta semana terminé la funcionalidad de las vacaciones en RHP, asegurándome de que funcionara correctamente en todos los casos.

También seguí estudiando la base de datos del programa de taller para prepararme para el desarrollo, y estuve resolviendo algunas incidencias que iban saliendo en el día a día.

---

## Semana 19 - 23 de enero

Durante esta semana estuve a la espera de que mi tutor copiara las tablas principales necesarias para empezar a desarrollar la lógica del programa de taller.

Mientras tanto, seguí revisando la estructura de la base de datos y preparando ideas de cómo organizar el desarrollo cuando ya tuviera todo listo.

---

## Semana 26 - 30 de enero

Esta semana ya tuve disponibles las tablas necesarias para empezar a trabajar, aunque estaban vacías porque el programa de taller actual sigue en uso y sus datos se actualizan constantemente.

Por este motivo, empecé a desarrollar los CRUDs basándome en la estructura de la base de datos original. Además, implementé un sistema de login funcional con gestión de perfiles y empresa, lo que permitió empezar a tener una base más sólida del programa.
