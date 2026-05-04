# ABRIL

# Abril 2026

## Semana 7 - 10 de abril

Durante esta semana me encargaron hacer una versión reducida del programa de taller en PHP, enfocada a los perfiles de conductor e inventario.

La idea era que se pudiera usar desde tablets que no están conectadas por cable a la red del ayuntamiento, por lo que no pueden acceder directamente ni al programa principal ni a la base de datos.

Para solucionarlo, tuve que copiar las tablas necesarias a una base de datos MySQL y desarrollar esta versión en PHP. Además, también era necesario crear un sistema que permitiera traspasar los datos desde MySQL a SQL Server, para que todo quedara sincronizado con el sistema principal.

---

## Semana 13 - 17 de abril

Esta semana terminé el programa de sincronización (SINCRO), que permite traspasar información entre ambos sistemas.

Gracias a esto, ahora se pueden sincronizar los partes, sus estados (iniciar, pausar, finalizar, etc.) y los artículos inventariados entre la versión en PHP y el programa principal.

También ajusté la duración de la sesión tanto en la aplicación en C# como en la versión en PHP. En el caso de PHP, debido a la configuración del servidor, tuve que hacer un script que refresca la página automáticamente cada 5 minutos para mantener la sesión activa.

---

## Semana 20 - 24 de abril

Durante esta semana añadí un CRUD de zonas en la web de contenedores. Ahora se pueden dibujar zonas en el mapa, asignarles un nombre y, al pasar el ratón por encima, se muestra ese nombre.

Esto facilita bastante identificar si los contenedores están en su sitio correcto.

También estuve revisando un error en la app de trabajadores relacionado con la subida de fotos de justificantes a RHP, pero después de investigarlo vimos que todo funcionaba correctamente y no había ningún problema real.

---

## Semana 27 - 30 de abril

Esta semana seguimos haciendo pruebas del programa de taller, sobre todo en la parte de traspaso de datos tanto entre sistemas como hacia Sage.

Detectamos que algunos datos no se estaban enviando correctamente a Sage. Esto ocurría porque antes de llegar a Sage, los datos pasan por una tabla intermedia en otra base de datos. El problema era que la base original del BIIT utiliza IDs altos (20000+), mientras que en las nuevas tablas los IDs empezaban desde valores bajos, lo que generaba conflictos en esa tabla intermedia.

Este problema debería solucionarse cuando se haga la migración completa y los IDs sigan la numeración original.

Además, hice un pequeño programa en una Raspberry Pi para el comedor: cuando se enciende la televisión, automáticamente selecciona el HDMI de la Raspberry y abre un navegador en modo kiosco con un carrusel de imágenes. Fue una tarea más diferente pero interesante.
